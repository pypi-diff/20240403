# Comparing `tmp/enosimulator-0.3.3.tar.gz` & `tmp/enosimulator-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enosimulator-0.3.3.tar", last modified: Sun Nov 19 02:22:49 2023, max compression
+gzip compressed data, was "enosimulator-0.3.4.tar", last modified: Wed Apr  3 14:05:25 2024, max compression
```

## Comparing `enosimulator-0.3.3.tar` & `enosimulator-0.3.4.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.654672 enosimulator-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-19 02:22:41.000000 enosimulator-0.3.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-11-19 02:22:41.000000 enosimulator-0.3.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-19 02:22:41.000000 enosimulator-0.3.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      642 2023-11-19 02:22:41.000000 enosimulator-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-19 02:22:41.000000 enosimulator-0.3.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-11-19 02:22:41.000000 enosimulator-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-11-19 02:22:41.000000 enosimulator-0.3.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-19 02:22:41.000000 enosimulator-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-19 02:22:41.000000 enosimulator-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2023-11-19 02:22:49.654672 enosimulator-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10160 2023-11-19 02:22:41.000000 enosimulator-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-19 02:22:41.000000 enosimulator-0.3.3/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-11-19 02:22:41.000000 enosimulator-0.3.3/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.638672 enosimulator-0.3.3/enosimulator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-19 02:22:49.000000 enosimulator-0.3.3/enosimulator/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.642672 enosimulator-0.3.3/enosimulator/backend/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/backend/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.642672 enosimulator-0.3.3/enosimulator/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/config/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.642672 enosimulator-0.3.3/enosimulator/config/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/config/examples/azure.config.json
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/config/examples/azure.secrets.json
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/config/examples/docker.config.json
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/config/examples/docker.secrets.json
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/config/examples/hetzner.config.json
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/config/examples/hetzner.secrets.json
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/config/secrets.json
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/containers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.634672 enosimulator-0.3.3/enosimulator/infra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.634672 enosimulator-0.3.3/enosimulator/infra/azure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.642672 enosimulator-0.3.3/enosimulator/infra/azure/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/config/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.642672 enosimulator-0.3.3/enosimulator/infra/azure/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/data/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.642672 enosimulator-0.3.3/enosimulator/infra/azure/logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/logs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.642672 enosimulator-0.3.3/enosimulator/infra/azure/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/configure.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.646672 enosimulator-0.3.3/enosimulator/infra/azure/templates/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/data/checker.sh
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/data/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/data/engine.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/data/vulnbox.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/outputs.tf
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/variables.tf
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/azure/templates/versions.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.634672 enosimulator-0.3.3/enosimulator/infra/hetzner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.646672 enosimulator-0.3.3/enosimulator/infra/hetzner/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/config/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.646672 enosimulator-0.3.3/enosimulator/infra/hetzner/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/data/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.646672 enosimulator-0.3.3/enosimulator/infra/hetzner/logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/logs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.646672 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/configure.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.646672 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/data/checker.sh
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/data/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/data/engine.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/data/vulnbox.sh
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/outputs.tf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/variables.tf
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/hetzner/templates/versions.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.634672 enosimulator-0.3.3/enosimulator/infra/local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.646672 enosimulator-0.3.3/enosimulator/infra/local/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/local/templates/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/infra/local/templates/versions.tf
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.646672 enosimulator-0.3.3/enosimulator/setup/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14440 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.650672 enosimulator-0.3.3/enosimulator/setup/setup_helper/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/setup_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/setup_helper/azure_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/setup_helper/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/setup_helper/hetzner_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/setup_helper/local_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/setup_helper/setup_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/setup_helper/team_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/setup_helper/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/setup/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.650672 enosimulator-0.3.3/enosimulator/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/simulation/flagsubmitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17353 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/simulation/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17032 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16711 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/simulation/statchecker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/simulation/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    14389 2023-11-19 02:22:41.000000 enosimulator-0.3.3/enosimulator/types_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.642672 enosimulator-0.3.3/enosimulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2023-11-19 02:22:49.000000 enosimulator-0.3.3/enosimulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2023-11-19 02:22:49.000000 enosimulator-0.3.3/enosimulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-19 02:22:49.000000 enosimulator-0.3.3/enosimulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-19 02:22:49.000000 enosimulator-0.3.3/enosimulator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-11-19 02:22:49.000000 enosimulator-0.3.3/enosimulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-19 02:22:49.000000 enosimulator-0.3.3/enosimulator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.634672 enosimulator-0.3.3/packer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.650672 enosimulator-0.3.3/packer/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-11-19 02:22:41.000000 enosimulator-0.3.3/packer/azure/engine.json
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-11-19 02:22:41.000000 enosimulator-0.3.3/packer/azure/engine.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.650672 enosimulator-0.3.3/packer/azure/util/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-19 02:22:41.000000 enosimulator-0.3.3/packer/azure/util/create_service_principal.sh
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-11-19 02:22:41.000000 enosimulator-0.3.3/packer/azure/vulnbox.json
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-11-19 02:22:41.000000 enosimulator-0.3.3/packer/azure/vulnbox.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.650672 enosimulator-0.3.3/packer/hetzner/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-11-19 02:22:41.000000 enosimulator-0.3.3/packer/hetzner/engine.json
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2023-11-19 02:22:41.000000 enosimulator-0.3.3/packer/hetzner/engine.sh
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-11-19 02:22:41.000000 enosimulator-0.3.3/packer/hetzner/vulnbox.json
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-11-19 02:22:41.000000 enosimulator-0.3.3/packer/hetzner/vulnbox.sh
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-11-19 02:22:41.000000 enosimulator-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-11-19 02:22:41.000000 enosimulator-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-11-19 02:22:49.654672 enosimulator-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 02:22:49.650672 enosimulator-0.3.3/util/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-11-19 02:22:41.000000 enosimulator-0.3.3/util/normal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2023-11-19 02:22:41.000000 enosimulator-0.3.3/util/scoreboard_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.446110 enosimulator-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 14:05:20.000000 enosimulator-0.3.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 14:05:20.000000 enosimulator-0.3.4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 14:05:20.000000 enosimulator-0.3.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-03 14:05:20.000000 enosimulator-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 14:05:20.000000 enosimulator-0.3.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 14:05:20.000000 enosimulator-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-03 14:05:20.000000 enosimulator-0.3.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 14:05:20.000000 enosimulator-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 14:05:20.000000 enosimulator-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-03 14:05:25.446110 enosimulator-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-04-03 14:05:20.000000 enosimulator-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 14:05:20.000000 enosimulator-0.3.4/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 14:05:20.000000 enosimulator-0.3.4/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.434110 enosimulator-0.3.4/enosimulator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 14:05:25.000000 enosimulator-0.3.4/enosimulator/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.434110 enosimulator-0.3.4/enosimulator/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/backend/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.434110 enosimulator-0.3.4/enosimulator/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/config/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/config/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/config/examples/azure.config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/config/examples/azure.secrets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/config/examples/docker.config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/config/examples/docker.secrets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/config/examples/hetzner.config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/config/examples/hetzner.secrets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/config/secrets.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/containers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.430110 enosimulator-0.3.4/enosimulator/infra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.430110 enosimulator-0.3.4/enosimulator/infra/azure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/infra/azure/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/config/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/infra/azure/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/data/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/infra/azure/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/logs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/infra/azure/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/configure.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/infra/azure/templates/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/data/checker.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/data/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/data/engine.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/data/vulnbox.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/outputs.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/variables.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/azure/templates/versions.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.430110 enosimulator-0.3.4/enosimulator/infra/hetzner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/infra/hetzner/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/config/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/infra/hetzner/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/data/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/infra/hetzner/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/logs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.438110 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/configure.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.442110 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/data/checker.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/data/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/data/engine.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/data/vulnbox.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/outputs.tf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/variables.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/hetzner/templates/versions.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.430110 enosimulator-0.3.4/enosimulator/infra/local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.442110 enosimulator-0.3.4/enosimulator/infra/local/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/local/templates/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/infra/local/templates/versions.tf
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.442110 enosimulator-0.3.4/enosimulator/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14438 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.442110 enosimulator-0.3.4/enosimulator/setup/setup_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/setup_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/setup_helper/azure_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/setup_helper/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/setup_helper/hetzner_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/setup_helper/local_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/setup_helper/setup_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/setup_helper/team_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/setup_helper/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/setup/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.442110 enosimulator-0.3.4/enosimulator/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/simulation/flagsubmitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17532 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/simulation/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17028 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16707 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/simulation/statchecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/simulation/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-04-03 14:05:20.000000 enosimulator-0.3.4/enosimulator/types_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.446110 enosimulator-0.3.4/enosimulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-03 14:05:25.000000 enosimulator-0.3.4/enosimulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-03 14:05:25.000000 enosimulator-0.3.4/enosimulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:05:25.000000 enosimulator-0.3.4/enosimulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 14:05:25.000000 enosimulator-0.3.4/enosimulator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 14:05:25.000000 enosimulator-0.3.4/enosimulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 14:05:25.000000 enosimulator-0.3.4/enosimulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.430110 enosimulator-0.3.4/packer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.446110 enosimulator-0.3.4/packer/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-03 14:05:20.000000 enosimulator-0.3.4/packer/azure/engine.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-03 14:05:20.000000 enosimulator-0.3.4/packer/azure/engine.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.446110 enosimulator-0.3.4/packer/azure/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 14:05:20.000000 enosimulator-0.3.4/packer/azure/util/create_service_principal.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-03 14:05:20.000000 enosimulator-0.3.4/packer/azure/vulnbox.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-03 14:05:20.000000 enosimulator-0.3.4/packer/azure/vulnbox.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.446110 enosimulator-0.3.4/packer/hetzner/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 14:05:20.000000 enosimulator-0.3.4/packer/hetzner/engine.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-03 14:05:20.000000 enosimulator-0.3.4/packer/hetzner/engine.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-03 14:05:20.000000 enosimulator-0.3.4/packer/hetzner/vulnbox.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-03 14:05:20.000000 enosimulator-0.3.4/packer/hetzner/vulnbox.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-03 14:05:20.000000 enosimulator-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-03 14:05:20.000000 enosimulator-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-03 14:05:25.446110 enosimulator-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:05:25.446110 enosimulator-0.3.4/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 14:05:20.000000 enosimulator-0.3.4/util/normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-03 14:05:20.000000 enosimulator-0.3.4/util/scoreboard_analysis.py
```

### Comparing `enosimulator-0.3.3/.dockerignore` & `enosimulator-0.3.4/.dockerignore`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/.gitignore` & `enosimulator-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/.pre-commit-config.yaml` & `enosimulator-0.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/Dockerfile` & `enosimulator-0.3.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/LICENSE` & `enosimulator-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/PKG-INFO` & `enosimulator-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: enosimulator
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simulating an attack defense CTF competition using the game engine and services provided by Enowars
 Home-page: https://github.com/ashiven/enosimulator
 Author: Jannik Novak
 Author-email: nevisha@pm.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aenum==3.1.15
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: beautifulsoup4==4.11.1
 Requires-Dist: dependency_injector==4.41.0
 Requires-Dist: enochecker_core==0.10.0
 Requires-Dist: Flask==2.3.1
 Requires-Dist: Flask_RESTful==0.3.10
 Requires-Dist: httpx==0.25.0
 Requires-Dist: jsons==1.6.3
 Requires-Dist: matplotlib==3.7.0
+Requires-Dist: numpy==1.24.2
 Requires-Dist: paramiko==3.3.1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: Requests==2.31.0
 Requires-Dist: rich==13.6.0
+Requires-Dist: scipy==1.11.3
 Requires-Dist: selenium==4.14.0
 Requires-Dist: tenacity==8.2.2
 Requires-Dist: webdriver_manager==4.0.1
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/ashiven/enosimulator/actions/workflows/tests.yml/badge.svg)](https://github.com/ashiven/enosimulator/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/enosimulator.svg)](https://badge.fury.io/py/enosimulator)
```

### Comparing `enosimulator-0.3.3/README.md` & `enosimulator-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/docker-compose.yml` & `enosimulator-0.3.4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/backend/app.py` & `enosimulator-0.3.4/enosimulator/backend/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import os
 import sqlite3
 from time import time
 from typing import Dict, Tuple
 
 from flask import Flask, request
 from flask_restful import Api, Resource
+from setup import Setup
+from simulation import Simulation
 from tenacity import retry, stop_after_attempt
 
-from ..setup import Setup
-from ..simulation import Simulation
-
 
 class Teams(Resource):
     """
     An API endpoint for team information.
 
     The response contains a dictionary of team names and their respective information.
```

### Comparing `enosimulator-0.3.3/enosimulator/backend/schema.sql` & `enosimulator-0.3.4/enosimulator/backend/schema.sql`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/config/config.json` & `enosimulator-0.3.4/enosimulator/config/config.json`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/config/examples/azure.config.json` & `enosimulator-0.3.4/enosimulator/config/examples/azure.config.json`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/config/examples/azure.secrets.json` & `enosimulator-0.3.4/enosimulator/config/examples/azure.secrets.json`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/config/examples/docker.config.json` & `enosimulator-0.3.4/enosimulator/config/examples/docker.config.json`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/config/examples/hetzner.config.json` & `enosimulator-0.3.4/enosimulator/config/examples/hetzner.config.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.986111111111111%*

 * *Differences: {"'settings'": "{'simulation-type': 'intensive-stress-test'}"}*

```diff
@@ -12,15 +12,15 @@
         ],
         "duration-in-minutes": 300,
         "scoreboard-file": "C:/Users/janni/Downloads/scoreboard_enowars7/scoreboard478.json",
         "services": [
             "enowars7-service-CVExchange",
             "enowars7-service-bollwerk"
         ],
-        "simulation-type": "realistic",
+        "simulation-type": "intensive-stress-test",
         "teams": 3
     },
     "setup": {
         "location": "hetzner",
         "ssh-config-path": "C:/Users/janni/.ssh/simconfig",
         "vm-image-references": {
             "checker": "vulnbox-checker",
```

### Comparing `enosimulator-0.3.3/enosimulator/config/secrets.json` & `enosimulator-0.3.4/enosimulator/config/secrets.json`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/containers.py` & `enosimulator-0.3.4/enosimulator/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from threading import Lock
 
+from backend import FlaskApp
 from dependency_injector import containers, providers
 from httpx import AsyncClient
 from rich.console import Console
-
-from .backend import FlaskApp
-from .setup import Setup
-from .setup.setup_helper import SetupHelper, TeamGenerator
-from .simulation import FlagSubmitter, Orchestrator, Simulation, StatChecker
-from .types_ import Config, Secrets
+from setup import Setup
+from setup.setup_helper import SetupHelper, TeamGenerator
+from simulation import FlagSubmitter, Orchestrator, Simulation, StatChecker
+from types_ import Config, Secrets
 
 
 class SetupContainer(containers.DeclarativeContainer):
     """
     Container for setup related classes.
 
     This container is used to inject dependencies into the setup module.
```

### Comparing `enosimulator-0.3.3/enosimulator/infra/azure/templates/build.sh` & `enosimulator-0.3.4/enosimulator/infra/azure/templates/build.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/azure/templates/configure.sh` & `enosimulator-0.3.4/enosimulator/infra/azure/templates/configure.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/azure/templates/data/checker.sh` & `enosimulator-0.3.4/enosimulator/infra/azure/templates/data/checker.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/azure/templates/data/docker-compose.yml` & `enosimulator-0.3.4/enosimulator/infra/azure/templates/data/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/azure/templates/data/engine.sh` & `enosimulator-0.3.4/enosimulator/infra/azure/templates/data/engine.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/azure/templates/data/vulnbox.sh` & `enosimulator-0.3.4/enosimulator/infra/azure/templates/data/vulnbox.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/azure/templates/main.tf` & `enosimulator-0.3.4/enosimulator/infra/azure/templates/main.tf`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/azure/templates/variables.tf` & `enosimulator-0.3.4/enosimulator/infra/azure/templates/variables.tf`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/hetzner/templates/build.sh` & `enosimulator-0.3.4/enosimulator/infra/hetzner/templates/build.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/hetzner/templates/configure.sh` & `enosimulator-0.3.4/enosimulator/infra/hetzner/templates/configure.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/hetzner/templates/data/checker.sh` & `enosimulator-0.3.4/enosimulator/infra/hetzner/templates/data/checker.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/hetzner/templates/data/docker-compose.yml` & `enosimulator-0.3.4/enosimulator/infra/hetzner/templates/data/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/hetzner/templates/data/engine.sh` & `enosimulator-0.3.4/enosimulator/infra/hetzner/templates/data/engine.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/hetzner/templates/data/vulnbox.sh` & `enosimulator-0.3.4/enosimulator/infra/hetzner/templates/data/vulnbox.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/infra/local/templates/main.tf` & `enosimulator-0.3.4/enosimulator/infra/local/templates/main.tf`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/main.py` & `enosimulator-0.3.4/enosimulator/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import argparse
 import asyncio
 import os
 import sys
 from threading import Thread
 
+from containers import Application
 from dotenv import load_dotenv
 
-from .containers import Application
-
 
 def get_args() -> argparse.Namespace:
     """
     Parse command line arguments.
 
     Raises:
         Exception: If no config file is supplied
```

### Comparing `enosimulator-0.3.3/enosimulator/setup/setup.py` & `enosimulator-0.3.4/enosimulator/setup/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import Dict
 
 import aiofiles
 import jsons
 from requests import get
 from rich.console import Console
 from rich.table import Table
+from types_ import Config, IpAddresses, Secrets, Service, SimulationType, VMType
 
-from ..types_ import Config, IpAddresses, Secrets, Service, SimulationType, VMType
 from .setup_helper import SetupHelper
 from .util import create_file, delete_files, execute_command, kebab_to_camel, parse_json
 
 
 class Setup:
     """
     A class representing the simulation setup.
```

### Comparing `enosimulator-0.3.3/enosimulator/setup/setup_helper/azure_converter.py` & `enosimulator-0.3.4/enosimulator/setup/setup_helper/azure_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 from typing import Dict, Tuple
 
 import aiofiles
+from types_ import Config, Secrets, VMType
 
-from ...types_ import Config, Secrets, VMType
 from .base_converter import TemplateConverter
 from .util import append_lines, copy_file, delete_lines, insert_after, replace_line
 
 
 class AzureConverter(TemplateConverter):
     """
     A class that converts configuration template files for Azure.
```

### Comparing `enosimulator-0.3.3/enosimulator/setup/setup_helper/base_converter.py` & `enosimulator-0.3.4/enosimulator/setup/setup_helper/base_converter.py`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/setup/setup_helper/hetzner_converter.py` & `enosimulator-0.3.4/enosimulator/setup/setup_helper/hetzner_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import Dict, Tuple
 
 import aiofiles
+from types_ import Config, Secrets, VMType
 
-from ...types_ import Config, Secrets, VMType
 from .base_converter import TemplateConverter
 from .util import append_lines, copy_file, delete_lines, insert_after, replace_line
 
 
 class HetznerConverter(TemplateConverter):
     """
     A class that converts configuration template files for Hetzner Cloud.
```

### Comparing `enosimulator-0.3.3/enosimulator/setup/setup_helper/local_converter.py` & `enosimulator-0.3.4/enosimulator/setup/setup_helper/local_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from typing import Dict, Tuple
 
-from ...types_ import Config, Secrets
+from types_ import Config, Secrets
+
 from .base_converter import TemplateConverter
 
 
 # TODO:
 # - implement
 class LocalConverter(TemplateConverter):
     """
```

### Comparing `enosimulator-0.3.3/enosimulator/setup/setup_helper/setup_helper.py` & `enosimulator-0.3.4/enosimulator/setup/setup_helper/setup_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, List, Tuple
 
-from ...types_ import Config, Secrets, SetupVariant, SimulationType
+from types_ import Config, Secrets, SetupVariant, SimulationType
+
 from .azure_converter import AzureConverter
 from .hetzner_converter import HetznerConverter
 from .local_converter import LocalConverter
 from .team_generator import TeamGenerator
 
 
 class SetupHelper:
```

### Comparing `enosimulator-0.3.3/enosimulator/setup/setup_helper/team_generator.py` & `enosimulator-0.3.4/enosimulator/setup/setup_helper/team_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
 import os
 from collections import Counter
 from typing import Dict, List, Tuple
 
 from aenum import extend_enum
 from rich.console import Console
-
-from ...types_ import Config, Experience, SimulationType, Team
+from types_ import Config, Experience, SimulationType, Team
 
 TEAM_NAMES = [
     "Edible Frog",
     "Jonah Crab",
     "English Cream Golden Retriever",
     "Vampire Squid",
     "Bolognese Dog",
```

### Comparing `enosimulator-0.3.3/enosimulator/setup/setup_helper/util.py` & `enosimulator-0.3.4/enosimulator/setup/setup_helper/util.py`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/setup/util.py` & `enosimulator-0.3.4/enosimulator/setup/util.py`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator/simulation/flagsubmitter.py` & `enosimulator-0.3.4/enosimulator/simulation/flagsubmitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List, Tuple
 
 import paramiko
 from rich.console import Console
-
-from ..setup import Setup
-from ..types_ import SetupVariant, VMType
+from setup import Setup
+from types_ import SetupVariant, VMType
 
 
 class FlagSubmitter:
     """
     A Class for submitting flags to the submission endpoint running on the engine.
 
     Connects to the engine by creating an SSH tunnel through the VM.
```

### Comparing `enosimulator-0.3.3/enosimulator/simulation/orchestrator.py` & `enosimulator-0.3.4/enosimulator/simulation/orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from typing import Dict, List, Tuple
 
 import jsons
 from bs4 import BeautifulSoup
 from enochecker_core import (
     CheckerInfoMessage,
     CheckerResultMessage,
@@ -13,19 +14,19 @@
 from rich.panel import Panel
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
+from setup import Setup
 from tenacity import retry, stop_after_attempt
+from types_ import SimulationType, Team, VMType
 from webdriver_manager.chrome import ChromeDriverManager
 
-from ..setup import Setup
-from ..types_ import SimulationType, Team, VMType
 from .flagsubmitter import FlagSubmitter
 from .statchecker import StatChecker
 from .util import (
     REQUEST_TIMEOUT,
     async_lock,
     checker_request,
     port_from_address,
@@ -384,52 +385,56 @@
             team (Team): The team to exploit for.
             exploit_requests (Dict): A dictionary mapping tuples containing the team name, service name, flagstore, and attack info to checker task requests.
 
         Returns:
             List[str]: A list of flags that were obtained by exploiting other teams.
         """
 
-        flags = []
-        for (
-            (team_name, service, flagstore, _info),
-            exploit_request,
-        ) in exploit_requests.items():
-            exploit_checker_ip = self.private_to_public_ip[team.address]
-            exploit_checker_port = self.service_info[service][0]
-            exploit_checker_address = (
-                f"http://{exploit_checker_ip}:{exploit_checker_port}"
-            )
-
-            if self.debug:
-                self.console.log(
-                    f"[bold green]{team.name} :anger_symbol: {team_name}-{service}-{flagstore}"
+        tasks = []
+        async with asyncio.TaskGroup() as task_group:
+            for (
+                (team_name, service, flagstore, _info),
+                exploit_request,
+            ) in exploit_requests.items():
+                exploit_checker_ip = self.private_to_public_ip[team.address]
+                exploit_checker_port = self.service_info[service][0]
+                exploit_checker_address = (
+                    f"http://{exploit_checker_ip}:{exploit_checker_port}"
                 )
-                self.console.log(exploit_request)
 
-            try:
-                # TODO: - do the following in an async task group for more performance
-                r = await self.client.post(
-                    exploit_checker_address,
-                    data=req_to_json(exploit_request),
-                    headers={"Content-Type": "application/json"},
-                    timeout=REQUEST_TIMEOUT,
-                )
+                if self.debug:
+                    self.console.log(
+                        f"[bold green]{team.name} :anger_symbol: {team_name}-{service}-{flagstore}"
+                    )
+                    self.console.log(exploit_request)
+
+                    exploit_task = task_group.create_task(
+                        self.client.post(
+                            exploit_checker_address,
+                            data=req_to_json(exploit_request),
+                            headers={"Content-Type": "application/json"},
+                            timeout=REQUEST_TIMEOUT,
+                        )
+                    )
+                    tasks.append(exploit_task)
 
-                exploit_result = jsons.loads(
-                    r.content,
-                    CheckerResultMessage,
-                    key_transformer=jsons.KEY_TRANSFORMER_SNAKECASE,
-                )
+        results = [task.result() for task in tasks]
 
-                if CheckerTaskResult(exploit_result.result) is not CheckerTaskResult.OK:
-                    if self.debug:
-                        self.console.print(exploit_result.message)
-                else:
-                    if self.debug:
-                        self.console.log(
-                            f"[bold green]:triangular_flag:: {exploit_result.flag}\n"
-                        )
-                    flags.append(exploit_result.flag)
-            except Exception:
-                pass
+        flags = []
+        for r in results:
+            exploit_result = jsons.loads(
+                r.content,
+                CheckerResultMessage,
+                key_transformer=jsons.KEY_TRANSFORMER_SNAKECASE,
+            )
+
+            if CheckerTaskResult(exploit_result.result) is not CheckerTaskResult.OK:
+                if self.debug:
+                    self.console.print(exploit_result.message)
+            else:
+                if self.debug:
+                    self.console.log(
+                        f"[bold green]:triangular_flag:: {exploit_result.flag}\n"
+                    )
+                flags.append(exploit_result.flag)
 
         return flags
```

### Comparing `enosimulator-0.3.3/enosimulator/simulation/simulation.py` & `enosimulator-0.3.4/enosimulator/simulation/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from time import time
 from typing import Dict, List, Tuple
 
 from rich.columns import Columns
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
+from setup import Setup
+from types_ import SimulationType, Team
 
-from ..setup import Setup
-from ..types_ import SimulationType, Team
 from .orchestrator import Orchestrator
 from .util import async_lock
 
 
 class Simulation:
     """
     A Class representing the simulation.
```

### Comparing `enosimulator-0.3.3/enosimulator/simulation/statchecker.py` & `enosimulator-0.3.4/enosimulator/simulation/statchecker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from typing import Dict, List, Tuple
 
 import paramiko
 from httpx import AsyncClient
 from rich.console import Console
 from rich.panel import Panel
-
-from ..types_ import Config, Secrets, SetupVariant
+from types_ import Config, Secrets, SetupVariant
 
 
 class StatChecker:
     """
     A Class for checking the system and Docker stats on the VMs.
 
     Connects to the VMs via SSH.
```

### Comparing `enosimulator-0.3.3/enosimulator/simulation/util.py` & `enosimulator-0.3.4/enosimulator/simulation/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import urllib
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import asynccontextmanager
 from typing import Dict
 
 import jsons
 from enochecker_core import CheckerMethod, CheckerTaskMessage
-
-from ..types_ import IpAddresses
+from types_ import IpAddresses
 
 CHAIN_ID_PREFIX = secrets.token_hex(20)
 REQUEST_TIMEOUT = 10
 _pool = ThreadPoolExecutor()
 
 
 @asynccontextmanager
```

### Comparing `enosimulator-0.3.3/enosimulator/types_.py` & `enosimulator-0.3.4/enosimulator/types_.py`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/enosimulator.egg-info/PKG-INFO` & `enosimulator-0.3.4/enosimulator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: enosimulator
-Version: 0.3.3
+Version: 0.3.4
 Summary: Simulating an attack defense CTF competition using the game engine and services provided by Enowars
 Home-page: https://github.com/ashiven/enosimulator
 Author: Jannik Novak
 Author-email: nevisha@pm.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aenum==3.1.15
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: beautifulsoup4==4.11.1
 Requires-Dist: dependency_injector==4.41.0
 Requires-Dist: enochecker_core==0.10.0
 Requires-Dist: Flask==2.3.1
 Requires-Dist: Flask_RESTful==0.3.10
 Requires-Dist: httpx==0.25.0
 Requires-Dist: jsons==1.6.3
 Requires-Dist: matplotlib==3.7.0
+Requires-Dist: numpy==1.24.2
 Requires-Dist: paramiko==3.3.1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: Requests==2.31.0
 Requires-Dist: rich==13.6.0
+Requires-Dist: scipy==1.11.3
 Requires-Dist: selenium==4.14.0
 Requires-Dist: tenacity==8.2.2
 Requires-Dist: webdriver_manager==4.0.1
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/ashiven/enosimulator/actions/workflows/tests.yml/badge.svg)](https://github.com/ashiven/enosimulator/actions/workflows/tests.yml)
 [![PyPI version](https://badge.fury.io/py/enosimulator.svg)](https://badge.fury.io/py/enosimulator)
```

### Comparing `enosimulator-0.3.3/enosimulator.egg-info/SOURCES.txt` & `enosimulator-0.3.4/enosimulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/packer/azure/engine.json` & `enosimulator-0.3.4/packer/azure/engine.json`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/packer/azure/engine.sh` & `enosimulator-0.3.4/packer/azure/engine.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/packer/azure/util/create_service_principal.sh` & `enosimulator-0.3.4/packer/azure/util/create_service_principal.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/packer/azure/vulnbox.json` & `enosimulator-0.3.4/packer/azure/vulnbox.json`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/packer/azure/vulnbox.sh` & `enosimulator-0.3.4/packer/azure/vulnbox.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/packer/hetzner/engine.json` & `enosimulator-0.3.4/packer/hetzner/engine.json`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/packer/hetzner/engine.sh` & `enosimulator-0.3.4/packer/hetzner/engine.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/packer/hetzner/vulnbox.json` & `enosimulator-0.3.4/packer/hetzner/vulnbox.json`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/packer/hetzner/vulnbox.sh` & `enosimulator-0.3.4/packer/hetzner/vulnbox.sh`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/pyproject.toml` & `enosimulator-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/setup.cfg` & `enosimulator-0.3.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,30 @@
 
 [options]
 packages = find:
 python_requires = >=3.11
 setup_requires = setuptools_scm
 include_package_data = True
 install_requires = 
+	aenum==3.1.15
 	aiofiles==23.2.1
 	beautifulsoup4==4.11.1
 	dependency_injector==4.41.0
 	enochecker_core==0.10.0
 	Flask==2.3.1
 	Flask_RESTful==0.3.10
 	httpx==0.25.0
 	jsons==1.6.3
 	matplotlib==3.7.0
+	numpy==1.24.2
 	paramiko==3.3.1
 	python-dotenv==1.0.0
 	Requests==2.31.0
 	rich==13.6.0
+	scipy==1.11.3
 	selenium==4.14.0
 	tenacity==8.2.2
 	webdriver_manager==4.0.1
 
 [options.entry_points]
 console_scripts = 
 	enosimulator = enosimulator.__main__:entry_point
```

### Comparing `enosimulator-0.3.3/util/normal_distribution.py` & `enosimulator-0.3.4/util/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `enosimulator-0.3.3/util/scoreboard_analysis.py` & `enosimulator-0.3.4/util/scoreboard_analysis.py`

 * *Files identical despite different names*

