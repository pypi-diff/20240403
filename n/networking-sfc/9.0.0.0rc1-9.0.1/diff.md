# Comparing `tmp/networking-sfc-9.0.0.0rc1.tar.gz` & `tmp/networking-sfc-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/networking-sfc-9.0.0.0rc1.tar", last modified: Wed Sep 25 08:53:24 2019, max compression
+gzip compressed data, was "dist/networking-sfc-9.0.1.tar", last modified: Mon Feb  1 15:31:57 2021, max compression
```

## Comparing `networking-sfc-9.0.0.0rc1.tar` & `networking-sfc-9.0.1.tar`

### file list

```diff
@@ -1,336 +1,336 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5940 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/PKG-INFO
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/etc/oslo-config-generator/networking-sfc.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/etc/oslo-policy-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/etc/oslo-policy-generator/policy.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/etc/README.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/setup.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3472 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/user/usage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1087 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2796 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/user/command_extensions.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2294 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/install/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/install/install.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/contribution.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5754 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/ovs_symmetric_port_chain.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7428 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/sfc_port_chain_tap.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32478 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4506 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/sfc_non_transparent_sf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8254 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/sfc_proxy_port_correlation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1815 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11269 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/ovs_driver_and_agent_workflow.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30233 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/ietf_sfc_encapsulation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12498 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/sfc_ovn_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3860 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/alembic_migration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11302 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/contributor/system_design_and_workflow.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/configuration/policy-sample.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/configuration/policy.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/source/configuration/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/configuration/samples/networking-sfc.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/configuration/networking-sfc.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pairs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pairs/port-pair-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pairs/port-pair-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pairs/port-pair-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pairs/port-pair-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pairs/port-pair-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pairs/port-pair-create-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pair-groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pair-groups/port-pair-group-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pair-groups/port-pair-group-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pair-groups/port-pair-group-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pair-groups/port-pair-group-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pair-groups/port-pair-group-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-port-pair-groups/port-pair-group-create-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-create-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-create-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-classifiers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-classifiers/flow-classifier-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-classifiers/flow-classifier-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-classifiers/flow-classifier-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-classifiers/flow-classifier-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-classifiers/flow-classifier-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-classifiers/flow-classifier-list-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3551 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/zuul.d/jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/zuul.d/projects.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/bindep.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/CONTRIBUTING.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42471 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/sfc_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/README
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/models/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/models/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/models/head.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/newton/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/06382790fb2c_fix_foreign_constraints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3616 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/010308b06b49_rename_tenant_to_project.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/queens/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/d6fb381b65f2_tap_enabled_attribute_port_pair_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3077 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/53ed5bec6cff_add_service_graph_api_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/a3ad63aa834f_extra_attributes_for_pathnode.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/ocata/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/b3adaf631bab__add_fwd_path_and_in_mac_column.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/6185f1633a3d_add_correlation_as_pp_detail.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/CONTRACT_HEAD
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/contract/48072cb59133_initial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4903 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/5a475fc853e6_ovs_data_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/24fc7241aa5_initial.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/d1002a1f97f6_update_flow_classifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2005 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/fa75d46a7f11_add_port_pair_group_params.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/9768e6a66c9_flowclassifier_data_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4888 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/c3e178d4a985_sfc_data_model.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/pike/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/8329e9be2d8a_modify_value_column_size_in_port_pair_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/61832141fb82_add_ppg_n_tuple_mapping_column.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/start_networking_sfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/EXPAND_HEAD
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3647 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14161 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/db/flowclassifier_db.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4725 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/cli/port_pair.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8711 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/cli/port_pair_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5826 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/cli/port_chain.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7619 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/cli/flow_classifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/db/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/db/test_models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/sfc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/sfc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/sfc/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/sfc/agent/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/sfc/agent/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1138 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/sfc/agent/extensions/test_ovs_agent_sfc_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/sfc/agent/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2531 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   130999 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/db/test_sfc_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64608 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/db/test_flowclassifier_db.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6848 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/test_port_pair.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8139 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/test_flow_classifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7938 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/test_port_pair_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12900 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/test_port_chain.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7373 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/test_servicegraph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36166 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/test_sfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34678 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/test_flowclassifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5188 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/test_tap.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4821 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/test_driver_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/drivers/ovs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/drivers/ovs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4142 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/drivers/ovs/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14236 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/test_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3056 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/common/test_ovs_ext_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9514 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/test_driver_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/drivers/ovs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/drivers/ovs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   340304 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/drivers/ovs/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2192 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/extensions/test_sfc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/extensions/openvswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/extensions/openvswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   186320 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/extensions/openvswitch/test_sfc_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46431 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/test_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5466 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10923 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/extensions/flowclassifier.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7365 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/extensions/servicegraph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/extensions/tap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18616 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/extensions/sfc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1817 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/policies/port_pair.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1895 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/policies/port_pair_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/policies/port_chain.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1895 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/policies/flow_classifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1869 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/policies/service_graph.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5620 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/driver_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/common/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/ovs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/ovs/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/ovs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1274 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/dummy/dummy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/dummy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4807 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7796 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/driver_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4281 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/ovs_ext_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3173 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14421 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81506 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3035 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/rpc_topics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1571 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2383 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/dummy/dummy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/dummy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13892 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7044 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/extensions/sfc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/extensions/openvswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/extensions/openvswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39436 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/extensions/openvswitch/sfc_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/networking_sfc/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/playbooks/multinode-scenario-pre-run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7737 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4409 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/api-ref/source/sfc-port-pair-groups.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4372 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/api-ref/source/sfc-port-pairs.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6072 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/api-ref/source/sfc-classifiers.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4648 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/api-ref/source/sfc-chains.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3766 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/api-ref/source/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/notes/networking-sfc-0151b67501c641ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/notes/service-graphs-4a1e54f6bbbfe805.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/notes/mpls-correlation-c36070eba63b9f87.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/notes/unique-correlation-in-ppg-96d803a244425f66.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/notes/sfc-tap-port-pair-db6b2f3d29520c9b.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9187 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/stein.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3120 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/.pylintrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/devstack/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/devstack/settings
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3660 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4688 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/MANIFEST.in
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5940 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12309 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1628 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/tools/check_unit_test_structure.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      196 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/tools/clean.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2817 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19554 2019-09-25 08:53:24.000000 networking-sfc-9.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2019-09-25 08:52:38.000000 networking-sfc-9.0.0.0rc1/HACKING.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.149097 networking-sfc-9.0.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3120 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3660 2021-02-01 15:31:56.000000 networking-sfc-9.0.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19821 2021-02-01 15:31:56.000000 networking-sfc-9.0.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5935 2021-02-01 15:31:57.149097 networking-sfc-9.0.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.105097 networking-sfc-9.0.1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.117097 networking-sfc-9.0.1/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7737 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3766 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/api-ref/source/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4648 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/api-ref/source/sfc-chains.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6072 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/api-ref/source/sfc-classifiers.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4409 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/api-ref/source/sfc-port-pair-groups.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4372 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/api-ref/source/sfc-port-pairs.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.117097 networking-sfc-9.0.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/devstack/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.105097 networking-sfc-9.0.1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.105097 networking-sfc-9.0.1/doc/api_samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.117097 networking-sfc-9.0.1/doc/api_samples/sfc-chains/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-update-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.117097 networking-sfc-9.0.1/doc/api_samples/sfc-classifiers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-classifiers/flow-classifier-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-classifiers/flow-classifier-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-classifiers/flow-classifier-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-classifiers/flow-classifier-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-classifiers/flow-classifier-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-classifiers/flow-classifier-update-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.117097 networking-sfc-9.0.1/doc/api_samples/sfc-port-pair-groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pair-groups/port-pair-group-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pair-groups/port-pair-group-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pair-groups/port-pair-group-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pair-groups/port-pair-group-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pair-groups/port-pair-group-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pair-groups/port-pair-group-update-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.121097 networking-sfc-9.0.1/doc/api_samples/sfc-port-pairs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pairs/port-pair-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pairs/port-pair-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pairs/port-pair-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pairs/port-pair-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pairs/port-pair-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-port-pairs/port-pair-update-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.121097 networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-update-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.121097 networking-sfc-9.0.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.121097 networking-sfc-9.0.1/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/_static/.placeholder
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3472 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.121097 networking-sfc-9.0.1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/configuration/networking-sfc.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/configuration/policy-sample.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/configuration/policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.121097 networking-sfc-9.0.1/doc/source/configuration/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/configuration/samples/networking-sfc.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.121097 networking-sfc-9.0.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3860 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/alembic_migration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32478 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/contribution.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30233 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/ietf_sfc_encapsulation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1815 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11269 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/ovs_driver_and_agent_workflow.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5754 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/ovs_symmetric_port_chain.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4506 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/sfc_non_transparent_sf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12498 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/sfc_ovn_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7428 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/sfc_port_chain_tap.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8254 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/sfc_proxy_port_correlation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11302 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/contributor/system_design_and_workflow.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.125097 networking-sfc-9.0.1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2294 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/install/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/install/install.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.125097 networking-sfc-9.0.1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2796 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/user/command_extensions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1087 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.125097 networking-sfc-9.0.1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/etc/README.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.125097 networking-sfc-9.0.1/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/etc/oslo-config-generator/networking-sfc.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.125097 networking-sfc-9.0.1/etc/oslo-policy-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/etc/oslo-policy-generator/policy.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2851 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.125097 networking-sfc-9.0.1/networking_sfc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.125097 networking-sfc-9.0.1/networking_sfc/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7619 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/cli/flow_classifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5826 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/cli/port_chain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4725 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/cli/port_pair.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8711 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/cli/port_pair_group.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.125097 networking-sfc-9.0.1/networking_sfc/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14161 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/flowclassifier_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3647 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/CONTRACT_HEAD
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/EXPAND_HEAD
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.109097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/contract/48072cb59133_initial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/24fc7241aa5_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4903 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/5a475fc853e6_ovs_data_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2860 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/9768e6a66c9_flowclassifier_data_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4888 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/c3e178d4a985_sfc_data_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/d1002a1f97f6_update_flow_classifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2005 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/fa75d46a7f11_add_port_pair_group_params.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.109097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/newton/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3616 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/010308b06b49_rename_tenant_to_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/06382790fb2c_fix_foreign_constraints.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.109097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/ocata/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/6185f1633a3d_add_correlation_as_pp_detail.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/b3adaf631bab__add_fwd_path_and_in_mac_column.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.109097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/pike/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/61832141fb82_add_ppg_n_tuple_mapping_column.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/8329e9be2d8a_modify_value_column_size_in_port_pair_.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.109097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/queens/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3077 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/53ed5bec6cff_add_service_graph_api_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/a3ad63aa834f_extra_attributes_for_pathnode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/d6fb381b65f2_tap_enabled_attribute_port_pair_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/start_networking_sfc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.129097 networking-sfc-9.0.1/networking_sfc/db/migration/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/migration/models/head.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42471 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/db/sfc_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10923 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/extensions/flowclassifier.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7365 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/extensions/servicegraph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18616 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/extensions/sfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/extensions/tap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1895 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/policies/flow_classifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/policies/port_chain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1817 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/policies/port_pair.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1895 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/policies/port_pair_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1869 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/policies/service_graph.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/common/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5620 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/driver_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/dummy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1274 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/dummy/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/ovs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/ovs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/ovs/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4807 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/flowclassifier/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/sfc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/sfc/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/agent/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/sfc/agent/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/agent/extensions/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.133097 networking-sfc-9.0.1/networking_sfc/services/sfc/agent/extensions/openvswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/agent/extensions/openvswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39436 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/agent/extensions/openvswitch/sfc_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7044 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/agent/extensions/sfc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/services/sfc/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3173 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/common/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4281 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/common/ovs_ext_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7796 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/driver_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/dummy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2383 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/dummy/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1571 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14421 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81506 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3035 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/rpc_topics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13892 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/services/sfc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5466 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/tests/functional/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/db/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/db/test_models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/tests/functional/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/tests/functional/services/sfc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/services/sfc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/tests/functional/services/sfc/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/services/sfc/agent/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/tests/functional/services/sfc/agent/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/services/sfc/agent/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1138 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/services/sfc/agent/extensions/test_ovs_agent_sfc_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2721 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/functional/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.137097 networking-sfc-9.0.1/networking_sfc/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8139 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/cli/test_flow_classifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12900 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/cli/test_port_chain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6848 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/cli/test_port_pair.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7938 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/cli/test_port_pair_group.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64608 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/db/test_flowclassifier_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   130999 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/db/test_sfc_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34678 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/test_flowclassifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7373 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/test_servicegraph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36166 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/test_sfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5188 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/test_tap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/drivers/ovs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/drivers/ovs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4142 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/drivers/ovs/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4821 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/test_driver_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14236 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.141097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/extensions/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.145097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/extensions/openvswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/extensions/openvswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   186320 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/extensions/openvswitch/test_sfc_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2192 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/extensions/test_sfc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.145097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3056 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/common/test_ovs_ext_lib.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.145097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.145097 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/drivers/ovs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/drivers/ovs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   340304 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/drivers/ovs/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9514 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/test_driver_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46431 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/test_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/networking_sfc/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.125097 networking-sfc-9.0.1/networking_sfc.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5935 2021-02-01 15:31:57.000000 networking-sfc-9.0.1/networking_sfc.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12309 2021-02-01 15:31:57.000000 networking-sfc-9.0.1/networking_sfc.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 15:31:57.000000 networking-sfc-9.0.1/networking_sfc.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2021-02-01 15:31:57.000000 networking-sfc-9.0.1/networking_sfc.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 15:31:57.000000 networking-sfc-9.0.1/networking_sfc.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-02-01 15:31:57.000000 networking-sfc-9.0.1/networking_sfc.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2021-02-01 15:31:57.000000 networking-sfc-9.0.1/networking_sfc.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-02-01 15:31:57.000000 networking-sfc-9.0.1/networking_sfc.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.145097 networking-sfc-9.0.1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/playbooks/multinode-scenario-pre-run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.113097 networking-sfc-9.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.145097 networking-sfc-9.0.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/notes/mpls-correlation-c36070eba63b9f87.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/notes/networking-sfc-0151b67501c641ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/notes/service-graphs-4a1e54f6bbbfe805.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/notes/sfc-tap-port-pair-db6b2f3d29520c9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/notes/unique-correlation-in-ppg-96d803a244425f66.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.145097 networking-sfc-9.0.1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.145097 networking-sfc-9.0.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9187 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2021-02-01 15:31:57.149097 networking-sfc-9.0.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.145097 networking-sfc-9.0.1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1628 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/tools/check_unit_test_structure.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      196 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/tools/clean.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4687 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 15:31:57.149097 networking-sfc-9.0.1/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3563 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/zuul.d/jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-02-01 15:31:03.000000 networking-sfc-9.0.1/zuul.d/projects.yaml
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `networking-sfc-9.0.0.0rc1/PKG-INFO` & `networking-sfc-9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: networking-sfc
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: API's and implementations to support Service Function Chaining in Neutron.
 Home-page: https://docs.openstack.org/networking-sfc/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ============================================================
         Service Function Chaining Extension for OpenStack Networking
```

### Comparing `networking-sfc-9.0.0.0rc1/etc/README.txt` & `networking-sfc-9.0.1/etc/README.txt`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/setup.py` & `networking-sfc-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/LICENSE` & `networking-sfc-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/setup.cfg` & `networking-sfc-9.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/conf.py` & `networking-sfc-9.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/user/usage.rst` & `networking-sfc-9.0.1/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/user/index.rst` & `networking-sfc-9.0.1/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/user/command_extensions.rst` & `networking-sfc-9.0.1/doc/source/user/command_extensions.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/index.rst` & `networking-sfc-9.0.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/install/index.rst` & `networking-sfc-9.0.1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/install/configuration.rst` & `networking-sfc-9.0.1/doc/source/install/configuration.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/install/install.rst` & `networking-sfc-9.0.1/doc/source/install/install.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/contribution.rst` & `networking-sfc-9.0.1/doc/source/contributor/contribution.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/ovs_symmetric_port_chain.rst` & `networking-sfc-9.0.1/doc/source/contributor/ovs_symmetric_port_chain.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/sfc_port_chain_tap.rst` & `networking-sfc-9.0.1/doc/source/contributor/sfc_port_chain_tap.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/api.rst` & `networking-sfc-9.0.1/doc/source/contributor/api.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/sfc_non_transparent_sf.rst` & `networking-sfc-9.0.1/doc/source/contributor/sfc_non_transparent_sf.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/sfc_proxy_port_correlation.rst` & `networking-sfc-9.0.1/doc/source/contributor/sfc_proxy_port_correlation.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/index.rst` & `networking-sfc-9.0.1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/ovs_driver_and_agent_workflow.rst` & `networking-sfc-9.0.1/doc/source/contributor/ovs_driver_and_agent_workflow.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/ietf_sfc_encapsulation.rst` & `networking-sfc-9.0.1/doc/source/contributor/ietf_sfc_encapsulation.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/sfc_ovn_driver.rst` & `networking-sfc-9.0.1/doc/source/contributor/sfc_ovn_driver.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/alembic_migration.rst` & `networking-sfc-9.0.1/doc/source/contributor/alembic_migration.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/contributor/system_design_and_workflow.rst` & `networking-sfc-9.0.1/doc/source/contributor/system_design_and_workflow.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/configuration/policy-sample.rst` & `networking-sfc-9.0.1/doc/source/configuration/policy-sample.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/source/configuration/index.rst` & `networking-sfc-9.0.1/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-create-req.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-create-req.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-list-resp.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-list-resp.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-get-resp.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-create-resp.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-update-resp.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-update-resp.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-service-graphs/service-graph-create-resp.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-service-graphs/service-graph-get-resp.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-list-resp.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-list-resp.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-update-resp.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-create-resp.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-update-req.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-get-resp.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-get-resp.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-update-req.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-chains/port-chain-create-resp.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-chains/port-chain-update-resp.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/doc/api_samples/sfc-classifiers/flow-classifier-list-resp.json` & `networking-sfc-9.0.1/doc/api_samples/sfc-classifiers/flow-classifier-list-resp.json`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/zuul.d/jobs.yaml` & `networking-sfc-9.0.1/zuul.d/jobs.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     name: networking-sfc-functional
     parent: neutron-functional
     vars:
         project_name: networking-sfc
 
 - job:
     name: networking-sfc-tempest
-    parent: neutron-tempest-plugin-sfc
+    parent: neutron-tempest-plugin-sfc-train
     files: ^.*$
     irrelevant-files:
       - ^(test-|)requirements.txt$
       - ^setup.cfg$
 
 - job:
     name: networking-sfc-tempest-multinode
@@ -102,8 +102,8 @@
             $NEUTRON_L3_CONF:
               agent:
                 availability_zone: nova
 
 - job:
     name: networking-sfc-tempest-periodic
     parent: networking-sfc-tempest
-    branches: master
+    branches: stable/train
```

### Comparing `networking-sfc-9.0.0.0rc1/CONTRIBUTING.rst` & `networking-sfc-9.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/_i18n.py` & `networking-sfc-9.0.1/networking_sfc/_i18n.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/version.py` & `networking-sfc-9.0.1/networking_sfc/version.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/__init__.py` & `networking-sfc-9.0.1/networking_sfc/__init__.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/sfc_db.py` & `networking-sfc-9.0.1/networking_sfc/db/sfc_db.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/models/head.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/models/head.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/script.py.mako` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/06382790fb2c_fix_foreign_constraints.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/06382790fb2c_fix_foreign_constraints.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/010308b06b49_rename_tenant_to_project.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/newton/contract/010308b06b49_rename_tenant_to_project.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/d6fb381b65f2_tap_enabled_attribute_port_pair_group.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/d6fb381b65f2_tap_enabled_attribute_port_pair_group.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/53ed5bec6cff_add_service_graph_api_resource.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/53ed5bec6cff_add_service_graph_api_resource.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/a3ad63aa834f_extra_attributes_for_pathnode.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/queens/expand/a3ad63aa834f_extra_attributes_for_pathnode.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/b3adaf631bab__add_fwd_path_and_in_mac_column.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/b3adaf631bab__add_fwd_path_and_in_mac_column.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/6185f1633a3d_add_correlation_as_pp_detail.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/ocata/expand/6185f1633a3d_add_correlation_as_pp_detail.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/contract/48072cb59133_initial.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/contract/48072cb59133_initial.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/5a475fc853e6_ovs_data_model.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/5a475fc853e6_ovs_data_model.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/24fc7241aa5_initial.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/24fc7241aa5_initial.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/d1002a1f97f6_update_flow_classifier.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/d1002a1f97f6_update_flow_classifier.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/fa75d46a7f11_add_port_pair_group_params.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/fa75d46a7f11_add_port_pair_group_params.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/9768e6a66c9_flowclassifier_data_model.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/9768e6a66c9_flowclassifier_data_model.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/c3e178d4a985_sfc_data_model.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/mitaka/expand/c3e178d4a985_sfc_data_model.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/8329e9be2d8a_modify_value_column_size_in_port_pair_.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/8329e9be2d8a_modify_value_column_size_in_port_pair_.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/61832141fb82_add_ppg_n_tuple_mapping_column.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/pike/expand/61832141fb82_add_ppg_n_tuple_mapping_column.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/versions/start_networking_sfc.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/versions/start_networking_sfc.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/migration/alembic_migrations/env.py` & `networking-sfc-9.0.1/networking_sfc/db/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/db/flowclassifier_db.py` & `networking-sfc-9.0.1/networking_sfc/db/flowclassifier_db.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/cli/port_pair.py` & `networking-sfc-9.0.1/networking_sfc/cli/port_pair.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/cli/port_pair_group.py` & `networking-sfc-9.0.1/networking_sfc/cli/port_pair_group.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/cli/port_chain.py` & `networking-sfc-9.0.1/networking_sfc/cli/port_chain.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/cli/flow_classifier.py` & `networking-sfc-9.0.1/networking_sfc/cli/flow_classifier.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/db/test_migrations.py` & `networking-sfc-9.0.1/networking_sfc/tests/functional/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/db/test_models.py` & `networking-sfc-9.0.1/networking_sfc/tests/functional/db/test_models.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/services/sfc/agent/extensions/test_ovs_agent_sfc_extension.py` & `networking-sfc-9.0.1/networking_sfc/tests/functional/services/sfc/agent/extensions/test_ovs_agent_sfc_extension.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/functional/test_service.py` & `networking-sfc-9.0.1/networking_sfc/tests/functional/test_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,18 +29,24 @@
 
 
 class TestService(test_server.TestPluginWorker):
     def _fake_start(self):
         with open(self.temp_file, 'ab') as f:
             f.write(test_server.FAKE_START_MSG)
 
+    def _fake_reset(self):
+        with open(self.temp_file, 'ab') as f:
+            f.write(test_server.FAKE_RESET_MSG)
+
     def _test_restart_service_on_sighup(self, service, workers=1):
         self._start_server(callback=service, workers=workers)
         os.kill(self.service_pid, signal.SIGHUP)
-        expected_msg = test_server.FAKE_START_MSG * workers * 2
+        expected_msg = (
+            test_server.FAKE_START_MSG * workers +
+            test_server.FAKE_RESET_MSG * (workers + 1))
         expected_size = len(expected_msg)
 
         utils.wait_until_true(
             lambda: (os.path.isfile(self.temp_file) and
                      os.stat(self.temp_file).st_size ==
                      expected_size),
             timeout=5, sleep=0.1,
```

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/db/test_sfc_db.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/db/test_sfc_db.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/db/test_flowclassifier_db.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/db/test_flowclassifier_db.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/test_port_pair.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/cli/test_port_pair.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/test_flow_classifier.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/cli/test_flow_classifier.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/test_port_pair_group.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/cli/test_port_pair_group.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/cli/test_port_chain.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/cli/test_port_chain.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/test_servicegraph.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/test_servicegraph.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/test_sfc.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/test_sfc.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/test_flowclassifier.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/test_flowclassifier.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/extensions/test_tap.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/extensions/test_tap.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/test_driver_manager.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/test_driver_manager.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/drivers/ovs/test_driver.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/drivers/ovs/test_driver.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/flowclassifier/test_plugin.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/services/flowclassifier/test_plugin.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/common/test_ovs_ext_lib.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/common/test_ovs_ext_lib.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/test_driver_manager.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/test_driver_manager.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/drivers/ovs/test_driver.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/drivers/ovs/test_driver.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/extensions/test_sfc.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/extensions/test_sfc.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/agent/extensions/openvswitch/test_sfc_driver.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/agent/extensions/openvswitch/test_sfc_driver.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/unit/services/sfc/test_plugin.py` & `networking-sfc-9.0.1/networking_sfc/tests/unit/services/sfc/test_plugin.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/tests/base.py` & `networking-sfc-9.0.1/networking_sfc/tests/base.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/extensions/flowclassifier.py` & `networking-sfc-9.0.1/networking_sfc/extensions/flowclassifier.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/extensions/servicegraph.py` & `networking-sfc-9.0.1/networking_sfc/extensions/servicegraph.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/extensions/tap.py` & `networking-sfc-9.0.1/networking_sfc/extensions/tap.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/extensions/sfc.py` & `networking-sfc-9.0.1/networking_sfc/extensions/sfc.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/policies/port_pair.py` & `networking-sfc-9.0.1/networking_sfc/policies/port_pair.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/policies/port_pair_group.py` & `networking-sfc-9.0.1/networking_sfc/policies/port_pair_group.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/policies/__init__.py` & `networking-sfc-9.0.1/networking_sfc/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/policies/port_chain.py` & `networking-sfc-9.0.1/networking_sfc/policies/port_chain.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/policies/base.py` & `networking-sfc-9.0.1/networking_sfc/policies/base.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/policies/flow_classifier.py` & `networking-sfc-9.0.1/networking_sfc/policies/flow_classifier.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/policies/service_graph.py` & `networking-sfc-9.0.1/networking_sfc/policies/service_graph.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/driver_manager.py` & `networking-sfc-9.0.1/networking_sfc/services/flowclassifier/driver_manager.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/common/config.py` & `networking-sfc-9.0.1/networking_sfc/services/flowclassifier/common/config.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/common/exceptions.py` & `networking-sfc-9.0.1/networking_sfc/services/flowclassifier/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/common/context.py` & `networking-sfc-9.0.1/networking_sfc/services/flowclassifier/common/context.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/base.py` & `networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/base.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/ovs/driver.py` & `networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/ovs/driver.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/drivers/dummy/dummy.py` & `networking-sfc-9.0.1/networking_sfc/services/flowclassifier/drivers/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/flowclassifier/plugin.py` & `networking-sfc-9.0.1/networking_sfc/services/flowclassifier/plugin.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/driver_manager.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/driver_manager.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/config.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/common/config.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/ovs_ext_lib.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/common/ovs_ext_lib.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/exceptions.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/common/context.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/common/context.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/base.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/base.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/db.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/db.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/driver.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/driver.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/rpc.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/rpc.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/rpc_topics.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/rpc_topics.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/ovs/constants.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/ovs/constants.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/drivers/dummy/dummy.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/drivers/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/plugin.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/plugin.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/extensions/sfc.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/agent/extensions/sfc.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/services/sfc/agent/extensions/openvswitch/sfc_driver.py` & `networking-sfc-9.0.1/networking_sfc/services/sfc/agent/extensions/openvswitch/sfc_driver.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc/opts.py` & `networking-sfc-9.0.1/networking_sfc/opts.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/api-ref/source/conf.py` & `networking-sfc-9.0.1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/api-ref/source/sfc-port-pair-groups.inc` & `networking-sfc-9.0.1/api-ref/source/sfc-port-pair-groups.inc`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/api-ref/source/sfc-port-pairs.inc` & `networking-sfc-9.0.1/api-ref/source/sfc-port-pairs.inc`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/api-ref/source/sfc-classifiers.inc` & `networking-sfc-9.0.1/api-ref/source/sfc-classifiers.inc`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/api-ref/source/sfc-chains.inc` & `networking-sfc-9.0.1/api-ref/source/sfc-chains.inc`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/api-ref/source/parameters.yaml` & `networking-sfc-9.0.1/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/releasenotes/notes/networking-sfc-0151b67501c641ef.yaml` & `networking-sfc-9.0.1/releasenotes/notes/networking-sfc-0151b67501c641ef.yaml`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/releasenotes/notes/unique-correlation-in-ppg-96d803a244425f66.yaml` & `networking-sfc-9.0.1/releasenotes/notes/unique-correlation-in-ppg-96d803a244425f66.yaml`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/releasenotes/source/conf.py` & `networking-sfc-9.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/.pylintrc` & `networking-sfc-9.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/devstack/README.md` & `networking-sfc-9.0.1/devstack/README.md`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/devstack/plugin.sh` & `networking-sfc-9.0.1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/AUTHORS` & `networking-sfc-9.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/tox.ini` & `networking-sfc-9.0.1/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
          OS_LOG_CAPTURE={env:OS_LOG_CAPTURE:true}
          OS_STDOUT_CAPTURE={env:OS_STDOUT_CAPTURE:true}
          OS_STDERR_CAPTURE={env:OS_STDERR_CAPTURE:true}
          PYTHONWARNINGS=default::DeprecationWarning
 passenv = TRACE_FAILONLY
 usedevelop = True
 install_command = pip install {opts} {packages}
-deps = -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+deps = -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 whitelist_externals =
     sh
     find
 commands =
   find . -type f -name "*.py[c|o]" -delete
```

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/PKG-INFO` & `networking-sfc-9.0.1/networking_sfc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: networking-sfc
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: API's and implementations to support Service Function Chaining in Neutron.
 Home-page: https://docs.openstack.org/networking-sfc/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ============================================================
         Service Function Chaining Extension for OpenStack Networking
```

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/SOURCES.txt` & `networking-sfc-9.0.1/networking_sfc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/networking_sfc.egg-info/entry_points.txt` & `networking-sfc-9.0.1/networking_sfc.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/test-requirements.txt` & `networking-sfc-9.0.1/test-requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,10 +16,11 @@
 testscenarios>=0.4 # Apache-2.0/BSD
 WebOb>=1.7.1 # MIT
 WebTest>=2.0.27 # MIT
 oslotest>=3.2.0 # Apache-2.0
 stestr>=2.0.0 # Apache-2.0
 astroid==1.6.5 # LGPLv2.1
 pylint==1.9.2 # GPLv2
+isort==4.3.21 # MIT
 psycopg2>=2.7.7 # LGPL/ZPL
 PyMySQL>=0.7.6 # MIT License
 reno>=2.5.0  # Apache-2.0
```

### Comparing `networking-sfc-9.0.0.0rc1/tools/check_unit_test_structure.sh` & `networking-sfc-9.0.1/tools/check_unit_test_structure.sh`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/lower-constraints.txt` & `networking-sfc-9.0.1/lower-constraints.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 futurist==1.6.0
 greenlet==0.4.13
 hacking==0.12.0
 httplib2==0.10.3
 idna==2.6
 imagesize==1.0.0
 iso8601==0.1.12
+isort==4.3.21
 Jinja2==2.10
 jmespath==0.9.3
 jsonpatch==1.21
 jsonpointer==2.0
 jsonschema==2.6.0
 keystoneauth1==3.4.0
 keystonemiddleware==4.21.0
@@ -56,14 +57,15 @@
 mox3==0.25.0
 msgpack-python==0.5.6
 msgpack==0.5.6
 munch==2.2.0
 netaddr==0.7.18
 netifaces==0.10.6
 neutron-lib==1.18.0
+neutron==13.0.0.0b2
 openstackdocstheme==1.18.1
 openstacksdk==0.12.0
 os-api-ref==1.4.0
 os-client-config==1.29.0
 os-service-types==1.2.0
 os-xenapi==0.3.1
 osc-lib==1.10.0
```

### Comparing `networking-sfc-9.0.0.0rc1/README.rst` & `networking-sfc-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `networking-sfc-9.0.0.0rc1/ChangeLog` & `networking-sfc-9.0.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 CHANGES
 =======
 
-9.0.0.0rc1
-----------
+9.0.1
+-----
+
+* Monkey patch original current\_thread \_active
+* Fix pep8 job
+* Switch tempest jobs for stable/train branch to train jobs
+* [Functional tests] Fix SIGHUP handling tests
+* Update TOX/UPPER\_CONSTRAINTS\_FILE for stable/train
+* Update .gitreview for stable/train
+
+9.0.0
+-----
 
 * Add Python 3 Train unit tests
 * Update the constraints url
 * Add libpq-dev to bindep.txt to fix gate error
 * Use opendev repository
 * Switch functional jobs to python 3
 * Switch functional job to Zuulv3 syntax
```

### Comparing `networking-sfc-9.0.0.0rc1/requirements.txt` & `networking-sfc-9.0.1/requirements.txt`

 * *Files identical despite different names*

