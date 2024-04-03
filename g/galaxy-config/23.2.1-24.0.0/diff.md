# Comparing `tmp/galaxy-config-23.2.1.tar.gz` & `tmp/galaxy-config-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/config/dist/.tmp-xua6y5ev/galaxy-config-23.2.1.tar", last modified: Thu Feb 22 03:51:28 2024, max compression
+gzip compressed data, was "galaxy-config-24.0.0.tar", last modified: Wed Apr  3 02:44:07 2024, max compression
```

## Comparing `galaxy-config-23.2.1.tar` & `galaxy-config-24.0.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy/config/
--rw-r--r--   0 runner    (1001) docker     (127)    65782 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20271 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/config_manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy/config/sample/
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/auth_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/build_sites.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/container_resolvers.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/data_manager_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)   119286 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/datatypes_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/disposable_email_blocklist.conf.sample
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/environment_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/error_report.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/file_sources_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)   131999 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/galaxy.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    53594 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/job_conf.sample.yml
--rw-r--r--   0 runner    (1001) docker     (127)    79501 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/job_conf.xml.sample_advanced
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/job_conf.xml.sample_basic
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/job_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/lmod_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/local_conda_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    20644 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/object_store_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/oidc_backends_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/oidc_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/reports.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/themes_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/tool_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/tool_data_table_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/tool_destinations.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/tool_shed.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/tool_sheds_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/trs_servers_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy/config/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   156261 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/schemas/config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/schemas/job_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/schemas/reports_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)    25120 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/schemas/tool_shed_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/config/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/galaxy_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-22 03:51:28.000000 galaxy-config-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-22 03:50:43.000000 galaxy-config-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.306464 galaxy-config-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16193 2024-04-03 02:44:07.306464 galaxy-config-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.294464 galaxy-config-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.298464 galaxy-config-24.0.0/galaxy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    65685 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20242 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/config_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.302464 galaxy-config-24.0.0/galaxy/config/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/auth_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/build_sites.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/container_resolvers.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/data_manager_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)   120374 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/datatypes_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/disposable_email_blocklist.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/environment_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/error_report.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/file_sources_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)   133108 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/galaxy.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    53508 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/job_conf.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    79501 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/job_conf.xml.sample_advanced
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/job_conf.xml.sample_basic
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/job_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/lmod_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/local_conda_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    18194 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/object_store_conf.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20644 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/object_store_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/oidc_backends_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/oidc_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/reports.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/themes_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_data_table_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_destinations.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_shed.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_sheds_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/trs_servers_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/user_preferences_extra_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/workflow_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/workflow_schedulers_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.302464 galaxy-config-24.0.0/galaxy/config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   158390 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schemas/config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schemas/job_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schemas/reports_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25120 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schemas/tool_shed_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.306464 galaxy-config-24.0.0/galaxy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16193 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-03 02:44:07.306464 galaxy-config-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-config-23.2.1/HISTORY.rst` & `galaxy-config-24.0.0/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,46 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Follow-up on #17274 and #17262 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17302 <https://github.com/galaxyproject/galaxy/pull/17302>`_
+* Fix minor oidc_backends_config comment bug by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17385 <https://github.com/galaxyproject/galaxy/pull/17385>`_
+
+============
+Enhancements
+============
+
+* Add harmonize collections tool (or whatever other name) by `@lldelisle <https://github.com/lldelisle>`_ in `#16662 <https://github.com/galaxyproject/galaxy/pull/16662>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Add support for (fast5.tar).xz binary compressed files by `@tuncK <https://github.com/tuncK>`_ in `#17106 <https://github.com/galaxyproject/galaxy/pull/17106>`_
+* Add a3m datatype by `@astrovsky01 <https://github.com/astrovsky01>`_ in `#17217 <https://github.com/galaxyproject/galaxy/pull/17217>`_
+* Convert sample object store configuration to YAML and support configuring inline by `@natefoo <https://github.com/natefoo>`_ in `#17222 <https://github.com/galaxyproject/galaxy/pull/17222>`_
+* Allow job files to consume TUS uploads by `@jmchilton <https://github.com/jmchilton>`_ in `#17242 <https://github.com/galaxyproject/galaxy/pull/17242>`_
+* Add OIDC backend configuration schema and validation by `@uwwint <https://github.com/uwwint>`_ in `#17274 <https://github.com/galaxyproject/galaxy/pull/17274>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* Use short link for TPV shared database by `@nuwang <https://github.com/nuwang>`_ in `#17467 <https://github.com/galaxyproject/galaxy/pull/17467>`_
+* Feature SBOL datatypes by `@guillaume-gricourt <https://github.com/guillaume-gricourt>`_ in `#17482 <https://github.com/galaxyproject/galaxy/pull/17482>`_
+* Add documentation on how to use vault keys in file sources by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17498 <https://github.com/galaxyproject/galaxy/pull/17498>`_
+* add npy datatype by `@astrovsky01 <https://github.com/astrovsky01>`_ in `#17517 <https://github.com/galaxyproject/galaxy/pull/17517>`_
+* Enhance Avivator display app to support regular Tiffs by `@davelopez <https://github.com/davelopez>`_ in `#17554 <https://github.com/galaxyproject/galaxy/pull/17554>`_
+* Allow admin to sharpen language about selected object stores. by `@jmchilton <https://github.com/jmchilton>`_ in `#17806 <https://github.com/galaxyproject/galaxy/pull/17806>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -30,15 +63,15 @@
 * Add new datatype: STL by `@TanguyGen <https://github.com/TanguyGen>`_ in `#16478 <https://github.com/galaxyproject/galaxy/pull/16478>`_
 * add new tabular file formats cns,cnr and cnn to datatypes_conf.xml.sample file as they are neaded for cnvkit galaxy tools by `@khaled196 <https://github.com/khaled196>`_ in `#16503 <https://github.com/galaxyproject/galaxy/pull/16503>`_
 * Tweak tool memory use and optimize shared memory when using preload by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16536 <https://github.com/galaxyproject/galaxy/pull/16536>`_
 * Implement datatype upload warnings by `@jmchilton <https://github.com/jmchilton>`_ in `#16564 <https://github.com/galaxyproject/galaxy/pull/16564>`_
 * Support new genome browser chain file format by `@claudiofr <https://github.com/claudiofr>`_ in `#16576 <https://github.com/galaxyproject/galaxy/pull/16576>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16577 <https://github.com/galaxyproject/galaxy/pull/16577>`_
 * Implement instance URLs in Galaxy markdown. by `@jmchilton <https://github.com/jmchilton>`_ in `#16675 <https://github.com/galaxyproject/galaxy/pull/16675>`_
-*  Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
+* Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
 * Update datatypes_conf.xml.sample with docx type by `@yvanlebras <https://github.com/yvanlebras>`_ in `#16713 <https://github.com/galaxyproject/galaxy/pull/16713>`_
 * Replace ELIXIR AAI button with Life Science login by `@sebastian-schaaf <https://github.com/sebastian-schaaf>`_ in `#16762 <https://github.com/galaxyproject/galaxy/pull/16762>`_
 * Add EGI Check-in as OIDC authentication option by `@enolfc <https://github.com/enolfc>`_ in `#16782 <https://github.com/galaxyproject/galaxy/pull/16782>`_
 * Updated path-based interactive tools with entry point path injection, support for ITs with relative links, shortened URLs, doc and config updates including Podman job_conf by `@sveinugu <https://github.com/sveinugu>`_ in `#16795 <https://github.com/galaxyproject/galaxy/pull/16795>`_
 * Galaxy help forum integration by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#16798 <https://github.com/galaxyproject/galaxy/pull/16798>`_
 * Remove record access handling for Invenio RDM plugin by `@davelopez <https://github.com/davelopez>`_ in `#16900 <https://github.com/galaxyproject/galaxy/pull/16900>`_
 * optimize object store cache operations by `@SergeyYakubov <https://github.com/SergeyYakubov>`_ in `#17025 <https://github.com/galaxyproject/galaxy/pull/17025>`_
```

### Comparing `galaxy-config-23.2.1/LICENSE` & `galaxy-config-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/PKG-INFO` & `galaxy-config-24.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-util
+Requires-Dist: boltons
+Requires-Dist: jinja2
+Requires-Dist: pykwalify
+Requires-Dist: PyYAML
 
 
 .. image:: https://badge.fury.io/py/galaxy-config.svg
    :target: https://pypi.org/project/galaxy-config/
 
 
 Overview
@@ -42,14 +47,47 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Follow-up on #17274 and #17262 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17302 <https://github.com/galaxyproject/galaxy/pull/17302>`_
+* Fix minor oidc_backends_config comment bug by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17385 <https://github.com/galaxyproject/galaxy/pull/17385>`_
+
+============
+Enhancements
+============
+
+* Add harmonize collections tool (or whatever other name) by `@lldelisle <https://github.com/lldelisle>`_ in `#16662 <https://github.com/galaxyproject/galaxy/pull/16662>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Add support for (fast5.tar).xz binary compressed files by `@tuncK <https://github.com/tuncK>`_ in `#17106 <https://github.com/galaxyproject/galaxy/pull/17106>`_
+* Add a3m datatype by `@astrovsky01 <https://github.com/astrovsky01>`_ in `#17217 <https://github.com/galaxyproject/galaxy/pull/17217>`_
+* Convert sample object store configuration to YAML and support configuring inline by `@natefoo <https://github.com/natefoo>`_ in `#17222 <https://github.com/galaxyproject/galaxy/pull/17222>`_
+* Allow job files to consume TUS uploads by `@jmchilton <https://github.com/jmchilton>`_ in `#17242 <https://github.com/galaxyproject/galaxy/pull/17242>`_
+* Add OIDC backend configuration schema and validation by `@uwwint <https://github.com/uwwint>`_ in `#17274 <https://github.com/galaxyproject/galaxy/pull/17274>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* Use short link for TPV shared database by `@nuwang <https://github.com/nuwang>`_ in `#17467 <https://github.com/galaxyproject/galaxy/pull/17467>`_
+* Feature SBOL datatypes by `@guillaume-gricourt <https://github.com/guillaume-gricourt>`_ in `#17482 <https://github.com/galaxyproject/galaxy/pull/17482>`_
+* Add documentation on how to use vault keys in file sources by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17498 <https://github.com/galaxyproject/galaxy/pull/17498>`_
+* add npy datatype by `@astrovsky01 <https://github.com/astrovsky01>`_ in `#17517 <https://github.com/galaxyproject/galaxy/pull/17517>`_
+* Enhance Avivator display app to support regular Tiffs by `@davelopez <https://github.com/davelopez>`_ in `#17554 <https://github.com/galaxyproject/galaxy/pull/17554>`_
+* Allow admin to sharpen language about selected object stores. by `@jmchilton <https://github.com/jmchilton>`_ in `#17806 <https://github.com/galaxyproject/galaxy/pull/17806>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -72,15 +110,15 @@
 * Add new datatype: STL by `@TanguyGen <https://github.com/TanguyGen>`_ in `#16478 <https://github.com/galaxyproject/galaxy/pull/16478>`_
 * add new tabular file formats cns,cnr and cnn to datatypes_conf.xml.sample file as they are neaded for cnvkit galaxy tools by `@khaled196 <https://github.com/khaled196>`_ in `#16503 <https://github.com/galaxyproject/galaxy/pull/16503>`_
 * Tweak tool memory use and optimize shared memory when using preload by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16536 <https://github.com/galaxyproject/galaxy/pull/16536>`_
 * Implement datatype upload warnings by `@jmchilton <https://github.com/jmchilton>`_ in `#16564 <https://github.com/galaxyproject/galaxy/pull/16564>`_
 * Support new genome browser chain file format by `@claudiofr <https://github.com/claudiofr>`_ in `#16576 <https://github.com/galaxyproject/galaxy/pull/16576>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16577 <https://github.com/galaxyproject/galaxy/pull/16577>`_
 * Implement instance URLs in Galaxy markdown. by `@jmchilton <https://github.com/jmchilton>`_ in `#16675 <https://github.com/galaxyproject/galaxy/pull/16675>`_
-*  Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
+* Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
 * Update datatypes_conf.xml.sample with docx type by `@yvanlebras <https://github.com/yvanlebras>`_ in `#16713 <https://github.com/galaxyproject/galaxy/pull/16713>`_
 * Replace ELIXIR AAI button with Life Science login by `@sebastian-schaaf <https://github.com/sebastian-schaaf>`_ in `#16762 <https://github.com/galaxyproject/galaxy/pull/16762>`_
 * Add EGI Check-in as OIDC authentication option by `@enolfc <https://github.com/enolfc>`_ in `#16782 <https://github.com/galaxyproject/galaxy/pull/16782>`_
 * Updated path-based interactive tools with entry point path injection, support for ITs with relative links, shortened URLs, doc and config updates including Podman job_conf by `@sveinugu <https://github.com/sveinugu>`_ in `#16795 <https://github.com/galaxyproject/galaxy/pull/16795>`_
 * Galaxy help forum integration by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#16798 <https://github.com/galaxyproject/galaxy/pull/16798>`_
 * Remove record access handling for Invenio RDM plugin by `@davelopez <https://github.com/davelopez>`_ in `#16900 <https://github.com/galaxyproject/galaxy/pull/16900>`_
 * optimize object store cache operations by `@SergeyYakubov <https://github.com/SergeyYakubov>`_ in `#17025 <https://github.com/galaxyproject/galaxy/pull/17025>`_
```

### Comparing `galaxy-config-23.2.1/galaxy/config/__init__.py` & `galaxy-config-24.0.0/galaxy/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Universe configuration builder.
 """
+
 # absolute_import needed for tool_shed package.
 
 import configparser
 import json
 import locale
 import logging
 import logging.config
@@ -55,19 +56,18 @@
     VERSION_MAJOR,
     VERSION_MINOR,
 )
 
 if TYPE_CHECKING:
     from galaxy.model import User
 
-try:
-    from importlib.resources import files  # type: ignore[attr-defined]
-except ImportError:
-    # Python < 3.9
-    from importlib_resources import files  # type: ignore[no-redef]
+if sys.version_info >= (3, 9):
+    from importlib.resources import files
+else:
+    from importlib_resources import files
 
 log = logging.getLogger(__name__)
 
 DEFAULT_LOCALE_FORMAT = "%a %b %e %H:%M:%S %Y"
 ISO_DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 GALAXY_APP_NAME = "galaxy"
@@ -228,17 +228,17 @@
 
 
 class BaseAppConfiguration(HasDynamicProperties):
     # Override in subclasses (optional): {KEY: config option, VALUE: deprecated directory name}
     # If VALUE == first directory in a user-supplied path that resolves to KEY, it will be stripped from that path
     renamed_options: Optional[Dict[str, str]] = None
     deprecated_dirs: Dict[str, str] = {}
-    paths_to_check_against_root: Set[
-        str
-    ] = set()  # backward compatibility: if resolved path doesn't exist, try resolving w.r.t root
+    paths_to_check_against_root: Set[str] = (
+        set()
+    )  # backward compatibility: if resolved path doesn't exist, try resolving w.r.t root
     add_sample_file_to_defaults: Set[str] = set()  # for these options, add sample config files to their defaults
     listify_options: Set[str] = set()  # values for these options are processed as lists of values
     object_store_store_by: str
 
     def __init__(self, **kwargs):
         self._preprocess_kwargs(kwargs)
         self._kwargs = kwargs  # Save these as a record of explicitly set options
@@ -1175,15 +1175,14 @@
                 "level": "DEBUG",
                 "qualname": "COMPLIANCE",
             }
 
         log_destination = kwargs.get("log_destination")
         log_rotate_size = size_to_bytes(unicodify(kwargs.get("log_rotate_size", 0)))
         log_rotate_count = int(kwargs.get("log_rotate_count", 0))
-        galaxy_daemon_log_destination = os.environ.get("GALAXY_DAEMON_LOG")
         if log_destination == "stdout":
             LOGGING_CONFIG_DEFAULT["handlers"]["console"] = {
                 "class": "logging.StreamHandler",
                 "formatter": "stack",
                 "level": "DEBUG",
                 "stream": "ext://sys.stdout",
                 "filters": ["stack"],
@@ -1194,15 +1193,15 @@
                 "formatter": "stack",
                 "level": "DEBUG",
                 "filename": log_destination,
                 "filters": ["stack"],
                 "maxBytes": log_rotate_size,
                 "backupCount": log_rotate_count,
             }
-        if galaxy_daemon_log_destination:
+        if galaxy_daemon_log_destination := os.environ.get("GALAXY_DAEMON_LOG"):
             LOGGING_CONFIG_DEFAULT["handlers"]["files"] = {
                 "class": "logging.handlers.RotatingFileHandler",
                 "formatter": "stack",
                 "level": "DEBUG",
                 "filename": galaxy_daemon_log_destination,
                 "filters": ["stack"],
                 "maxBytes": log_rotate_size,
```

### Comparing `galaxy-config-23.2.1/galaxy/config/config_manage.py` & `galaxy-config-24.0.0/galaxy/config/config_manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,16 +424,15 @@
     else:
         shutil.move(from_path, backup_path)
 
 
 def _build_sample_yaml(args: Namespace, app_desc: App) -> None:
     schema = app_desc.schema
     f = StringIO()
-    description = getattr(schema, "description", None)
-    if description:
+    if description := getattr(schema, "description", None):
         description = description.lstrip()
         as_comment = "\n".join(f"# {line}" for line in description.split("\n")) + "\n"
         f.write(as_comment)
     if app_desc.app_name == "galaxy":
         if settings_to_sample is None:
             raise Exception("Please install gravity to rebuild the sample config")
         f.write(settings_to_sample())
@@ -515,16 +514,15 @@
 
 def _warn(message: str) -> None:
     print(f"WARNING: {message}")
 
 
 def _get_option_desc(option: Dict[str, Any]) -> str:
     desc = option["desc"]
-    parent_dir = option.get("path_resolves_to")
-    if parent_dir:
+    if parent_dir := option.get("path_resolves_to"):
         path_resolves = f"The value of this option will be resolved with respect to <{parent_dir}>."
         return f"{desc}\n{path_resolves}" if desc else path_resolves
     return desc
 
 
 ACTIONS: Dict[str, Callable] = {
     "convert": _run_conversion,
```

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/auth_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/auth_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/build_sites.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/build_sites.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/container_resolvers.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/container_resolvers.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/datatypes_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/datatypes_conf.xml.sample`

 * *Files 1% similar despite different names*

#### Comparing `galaxy-config-23.2.1/galaxy/config/sample/datatypes_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/datatypes_conf.xml.sample`

```diff
@@ -114,15 +114,15 @@
     <datatype extension="csfasta" type="galaxy.datatypes.sequence:csFasta" display_in_upload="true"/>
     <datatype extension="data" type="galaxy.datatypes.data:Data" mimetype="application/octet-stream" max_optional_metadata_filesize="1048576"/>
     <datatype extension="gz" type="galaxy.datatypes.binary:Binary" subclass="true"/>
     <datatype extension="binary" type="galaxy.datatypes.binary:Binary" mimetype="application/octet-stream" max_optional_metadata_filesize="1048576"/>
     <datatype extension="d3_hierarchy" type="galaxy.datatypes.text:Json" mimetype="application/json" subclass="true" display_in_upload="true"/>
     <datatype extension="imgt.json" type="galaxy.datatypes.text:ImgtJson" mimetype="application/json" display_in_upload="True"/>
     <datatype extension="geojson" type="galaxy.datatypes.text:GeoJson" mimetype="application/json" display_in_upload="True"/>
-    <datatype extension="data_manager_json" type="galaxy.datatypes.text:Json" mimetype="application/json" subclass="true" display_in_upload="false"/>
+    <datatype extension="data_manager_json" type="galaxy.datatypes.text:DataManagerJson" mimetype="application/json" subclass="true" display_in_upload="false"/>
     <datatype extension="dbn" type="galaxy.datatypes.sequence:DotBracket" display_in_upload="true" description="Dot-Bracket format is a text-based format for storing both an RNA sequence and its corresponding 2D structure." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#Dbn"/>
     <datatype extension="fai" type="galaxy.datatypes.tabular:Tabular" display_in_upload="true" subclass="true" description="A Fasta Index File is a text file consisting of lines each with five TAB-delimited columns : Name, Length, offset, linebases, Linewidth" description_url="http://www.htslib.org/doc/faidx.html"/>
     <datatype extension="fasta" auto_compressed_types="gz" type="galaxy.datatypes.sequence:Fasta" display_in_upload="true" description="A sequence in FASTA format consists of a single-line description, followed by lines of sequence data. The first character of the description line is a greater-than ('&gt;') symbol in the first column. All lines should be shorter than 80 characters." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#Fasta">
       <infer_from suffix="fa"/>
       <converter file="fasta_to_tabular_converter.xml" target_datatype="tabular"/>
       <converter file="fasta_to_bowtie_base_index_converter.xml" target_datatype="bowtie_base_index"/>
       <converter file="fasta_to_bowtie_color_index_converter.xml" target_datatype="bowtie_color_index"/>
@@ -153,14 +153,15 @@
     </datatype>
     <datatype extension="fqtoc" type="galaxy.datatypes.sequence:SequenceSplitLocations" display_in_upload="true"/>
     <datatype extension="eland" type="galaxy.datatypes.tabular:Eland" display_in_upload="true"/>
     <datatype extension="elandmulti" type="galaxy.datatypes.tabular:ElandMulti" display_in_upload="true"/>
     <datatype extension="genetrack" type="galaxy.datatypes.tracks:GeneTrack">
       <!-- <display file="genetrack.xml" /> -->
     </datatype>
+    <datatype extension="a3m" type="galaxy.datatypes.sequence:Fasta" subclass="true" display_in_upload="true"/>
     <datatype extension="gff" type="galaxy.datatypes.interval:Gff" display_in_upload="true" description="GFF lines have nine required fields that must be tab-separated." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#GFF">
       <converter file="gff_to_bed_converter.xml" target_datatype="bed"/>
       <converter file="gff_to_interval_index_converter.xml" target_datatype="interval_index"/>
       <converter file="bed_gff_or_vcf_to_bigwig_converter.xml" target_datatype="bigwig"/>
       <converter file="gff_to_fli_converter.xml" target_datatype="fli"/>
       <converter file="interval_to_bgzip_converter.xml" target_datatype="bgzip"/>
       <converter file="interval_to_tabix_converter.xml" target_datatype="tabix" depends_on="bgzip"/>
@@ -208,14 +209,15 @@
       <display file="rviewer/bed.xml" inherit="true"/>
       <display file="igv/interval_as_bed.xml" inherit="true"/>
     </datatype>
     <datatype extension="jellyfish" type="galaxy.datatypes.binary:Binary" subclass="true" display_in_upload="true" description="Jellyfish database files are k-mer counts in binary format with a readable head. They are operated on and converted to human-readable text through jellyfish commands."/>
     <datatype extension="ktab" type="galaxy.datatypes.binary:Binary" subclass="true" description="A table of canonical k‑mers and their counts for the fastk toolkit." display_in_upload="true" description_url="https://github.com/thegenemyers/FASTK?tab=readme-ov-file#file-encodings"/>
     <datatype extension="hist" type="galaxy.datatypes.binary:Binary" subclass="true" description="A binary histogram file of kmers and frequencies for the fastk toolkit." display_in_upload="true" description_url="https://github.com/thegenemyers/FASTK?tab=readme-ov-file#file-encodings"/>
     <datatype extension="prof" type="galaxy.datatypes.binary:Binary" subclass="true" description="Read profile file for the fastk toolkit." display_in_upload="true" description_url="https://github.com/thegenemyers/FASTK?tab=readme-ov-file#file-encodings"/>
+    <datatype extension="npy" type="galaxy.datatypes.binary:Numpy" description="Standard format for saving numpy arrays" display_in_upload="true" description_url="https://numpy.org/devdocs/reference/generated/numpy.lib.format.html"/>
     <!-- ISA data types -->
     <datatype extension="isa-tab" type="galaxy.datatypes.isa:IsaTab" mimetype="application/isa-tools" display_in_upload="true" description="ISA-Tab data type." description_url="https://isa-tools.org"/>
     <datatype extension="isa-json" type="galaxy.datatypes.isa:IsaJson" mimetype="application/isa-tools" display_in_upload="true" description="ISA-JSON data type." description_url="https://isa-tools.org"/>
     <datatype extension="picard_interval_list" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true">
       <converter file="picard_interval_list_to_bed6_converter.xml" target_datatype="bed6"/>
     </datatype>
     <datatype extension="gatk_interval" type="galaxy.datatypes.data:Text" subclass="true" display_in_upload="true"/>
@@ -224,15 +226,17 @@
     <datatype extension="gatk_tranche" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true"/>
     <datatype extension="gatk_recal" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true"/>
     <datatype extension="cnn" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true"/>
     <datatype extension="cns" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true"/>
     <datatype extension="cnr" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true"/>
     <datatype extension="hhr" type="galaxy.datatypes.data:Text" subclass="true" display_in_upload="true"/>
     <datatype extension="jpg" type="galaxy.datatypes.images:Jpg" mimetype="image/jpeg"/>
-    <datatype extension="tiff" type="galaxy.datatypes.images:Tiff" mimetype="image/tiff" display_in_upload="true"/>
+    <datatype extension="tiff" type="galaxy.datatypes.images:Tiff" mimetype="image/tiff" display_in_upload="true">
+      <display file="image/avivator.xml"/>
+    </datatype>
     <datatype extension="tf2" type="galaxy.datatypes.images:Tiff" subclass="true" display_in_upload="false"/>
     <datatype extension="tf8" type="galaxy.datatypes.images:Tiff" subclass="true" display_in_upload="false"/>
     <datatype extension="btf" type="galaxy.datatypes.images:Tiff" subclass="true" display_in_upload="false"/>
     <datatype extension="tif" type="galaxy.datatypes.images:Tiff" subclass="true" display_in_upload="false"/>
     <datatype extension="svs" type="galaxy.datatypes.images:Tiff" subclass="true" display_in_upload="false"/>
     <datatype extension="scn" type="galaxy.datatypes.images:Tiff" subclass="true" display_in_upload="false"/>
     <datatype extension="bif" type="galaxy.datatypes.images:Tiff" subclass="true" display_in_upload="false"/>
@@ -342,14 +346,15 @@
     <datatype extension="postgresql" type="galaxy.datatypes.binary:PostgresqlArchive" display_in_upload="True"/>
     <datatype extension="mongodb" type="galaxy.datatypes.binary:MongoDBArchive" display_in_upload="True"/>
     <datatype extension="genenotebook" type="galaxy.datatypes.binary:GeneNoteBook" display_in_upload="True"/>
     <datatype extension="searchgui_archive" type="galaxy.datatypes.binary:SearchGuiArchive" display_in_upload="true"/>
     <datatype extension="fast5.tar" type="galaxy.datatypes.binary:Fast5Archive" display_in_upload="true"/>
     <datatype extension="fast5.tar.gz" type="galaxy.datatypes.binary:Fast5ArchiveGz" display_in_upload="true"/>
     <datatype extension="fast5.tar.bz2" type="galaxy.datatypes.binary:Fast5ArchiveBz2" display_in_upload="true"/>
+    <datatype extension="fast5.tar.xz" type="galaxy.datatypes.binary:Fast5ArchiveXz" display_in_upload="true"/>
     <datatype extension="peptideshaker_archive" type="galaxy.datatypes.binary:CompressedArchive" subclass="true" display_in_upload="true"/>
     <datatype extension="percin" type="galaxy.datatypes.tabular:Tabular" subclass="true"/>
     <datatype extension="percout" type="galaxy.datatypes.xml:GenericXml" subclass="true"/>
     <datatype extension="hardklor" type="galaxy.datatypes.tabular:Tabular" subclass="true"/>
     <datatype extension="kronik" type="galaxy.datatypes.tabular:Tabular" subclass="true"/>
     <datatype extension="imzml" type="galaxy.datatypes.proteomics:ImzML" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="analyze75" type="galaxy.datatypes.images:Analyze75" mimetype="application/xml" display_in_upload="true"/>
@@ -553,14 +558,15 @@
     <datatype extension="triples" type="galaxy.datatypes.triples:Triples" display_in_upload="false"/>
     <datatype extension="hdt" type="galaxy.datatypes.triples:HDT" display_in_upload="true"/>
     <datatype extension="nt" type="galaxy.datatypes.triples:NTriples" display_in_upload="true"/>
     <datatype extension="n3" type="galaxy.datatypes.triples:N3" display_in_upload="true"/>
     <datatype extension="ttl" type="galaxy.datatypes.triples:Turtle" display_in_upload="true"/>
     <datatype extension="rdf" type="galaxy.datatypes.triples:Rdf" display_in_upload="true"/>
     <datatype extension="jsonld" type="galaxy.datatypes.triples:Jsonld" display_in_upload="true"/>
+    <datatype extension="sbol" type="galaxy.datatypes.triples:Sbol" description="The SBOL (Synthetic Biology Open Language) standard was developed by the synthetic biology community to create a standardized format for the electronic exchange of information on the structural and functional aspects of biological designs." description_url="https://sbolstandard.org" display_in_upload="true"/>
     <!-- Excel datatypes -->
     <datatype extension="excel.xls" type="galaxy.datatypes.binary:ExcelXls" display_in_upload="true"/>
     <datatype extension="xlsx" type="galaxy.datatypes.binary:Xlsx" display_in_upload="true"/>
     <datatype extension="docx" type="galaxy.datatypes.binary:Binary" subclass="true"/>
     <datatype extension="btwisted" type="galaxy.datatypes.data:Text" subclass="true"/>
     <datatype extension="cai" type="galaxy.datatypes.data:Text" subclass="true"/>
     <datatype extension="cat_db" type="galaxy.datatypes.data:Text" subclass="true"/>
@@ -1045,28 +1051,30 @@
     <sniffer type="galaxy.datatypes.binary:BafTar"/>
     <sniffer type="galaxy.datatypes.binary:TdfTar"/>
     <sniffer type="galaxy.datatypes.binary:MassHunterTar"/>
     <sniffer type="galaxy.datatypes.binary:MassLynxTar"/>
     <sniffer type="galaxy.datatypes.binary:YepTar"/>
     <sniffer type="galaxy.datatypes.binary:WiffTar"/>
     <sniffer type="galaxy.datatypes.binary:Fast5ArchiveGz"/>
+    <sniffer type="galaxy.datatypes.binary:Fast5ArchiveXz"/>
     <sniffer type="galaxy.datatypes.binary:Fast5ArchiveBz2"/>
     <sniffer type="galaxy.datatypes.binary:Fast5Archive"/>
     <sniffer type="galaxy.datatypes.binary:Meryldb"/>
     <sniffer type="galaxy.datatypes.binary:Bref3"/>
     <sniffer type="galaxy.datatypes.binary:PostgresqlArchive"/>
     <sniffer type="galaxy.datatypes.binary:ICM"/>
     <sniffer type="galaxy.datatypes.binary:Idat"/>
     <sniffer type="galaxy.datatypes.binary:Trr"/>
     <sniffer type="galaxy.datatypes.binary:Dcd"/>
     <sniffer type="galaxy.datatypes.binary:Xtc"/>
     <sniffer type="galaxy.datatypes.binary:Cpt"/>
     <sniffer type="galaxy.datatypes.binary:Edr"/>
     <sniffer type="galaxy.datatypes.binary:Vel"/>
     <sniffer type="galaxy.datatypes.binary:Xlsx"/>
+    <sniffer type="galaxy.datatypes.binary:Numpy"/>
     <sniffer type="galaxy.datatypes.qiime2:QIIME2Metadata"/>
     <sniffer type="galaxy.datatypes.qiime2:QIIME2Artifact"/>
     <sniffer type="galaxy.datatypes.qiime2:QIIME2Visualization"/>
     <sniffer type="galaxy.datatypes.binary:CompressedZipArchive"/>
     <sniffer type="galaxy.datatypes.binary:Pretext"/>
     <sniffer type="galaxy.datatypes.annotation:Augustus"/>
     <sniffer type="galaxy.datatypes.xml:Owl"/>
@@ -1108,14 +1116,15 @@
     <sniffer type="galaxy.datatypes.proteomics:UniProtXML"/>
     <sniffer type="galaxy.datatypes.proteomics:XquestXML"/>
     <sniffer type="galaxy.datatypes.proteomics:XquestSpecXML"/>
     <sniffer type="galaxy.datatypes.proteomics:QCML"/>
     <sniffer type="galaxy.datatypes.proteomics:Wiff"/>
     <sniffer type="galaxy.datatypes.proteomics:PEFF"/>
     <sniffer type="galaxy.datatypes.molecules:CML"/>
+    <sniffer type="galaxy.datatypes.triples:Sbol"/>
     <sniffer type="galaxy.datatypes.xml:GenericXml"/>
     <sniffer type="galaxy.datatypes.triples:HDT"/>
     <sniffer type="galaxy.datatypes.triples:Turtle"/>
     <sniffer type="galaxy.datatypes.triples:NTriples"/>
     <sniffer type="galaxy.datatypes.triples:Jsonld"/>
     <sniffer type="galaxy.datatypes.sequence:Maf"/>
     <sniffer type="galaxy.datatypes.sequence:Lav"/>
```

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/environment_modules_mapping.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/environment_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/error_report.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/error_report.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/file_sources_conf.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/file_sources_conf.yml.sample`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,17 @@
   id: owncloud1
   label: OwnCloud
   doc: External OwnCloud files (configure access in user preferences)
   url: ${user.preferences['owncloud|url']}
   root: ${user.preferences['owncloud|root']}
   login: ${user.preferences['owncloud|username']}
   password: ${user.preferences['owncloud|password']}
+  # for accessing passwords stored in a vault:
+  # password: ${user.user_vault.read_secret('preferences/owncloud/password')}
+
   # By default, the plugin will use temp files to avoid loading entire files into memory. 
   # You can change the directory here or omit to use the default temp directory.
   temp_path: /your/temp/path
   # Set writable to true if you have write access to this source
   # and want to allow exporting files to it, by default is read only.
   writable: false
```

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/galaxy.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/galaxy.yml.sample`

 * *Files 1% similar despite different names*

```diff
@@ -1021,14 +1021,24 @@
 
   # Configuration file for the object store If this is set and exists,
   # it overrides any other objectstore settings.
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #object_store_config_file: object_store_conf.xml
 
+  # Rather than specifying an object_store_config_file, the object store
+  # configuration can be embedded into Galaxy's config with this option.
+  # This option has no effect if the file specified by
+  # object_store_config_file exists. Otherwise, if this option is set,
+  # it overrides any other objectstore settings.
+  # The syntax, available instrumenters, and documentation of their
+  # options is explained in detail in the object store sample
+  # configuration file, `object_store_conf.sample.yml`
+  #object_store_config: null
+
   # Specify where cache monitoring is driven for caching object stores
   # such as S3, Azure, and iRODS. This option has no affect on disk
   # object stores. For production instances, the cache should be
   # monitored by external tools such as tmpwatch and this value should
   # be set to 'external'. This will disable all cache monitoring in
   # Galaxy. Alternatively, 'celery' can monitor caches using a periodic
   # task or an 'inprocess' thread can be used - but this last option
@@ -2175,14 +2185,23 @@
   #oidc_config_file: oidc_config.xml
 
   # Sets the path to OIDC backends configuration file.
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #oidc_backends_config_file: oidc_backends_config.xml
 
+  # Sets the prefix for OIDC scopes specific to this Galaxy instance.
+  # If an API call is made against this Galaxy instance using an OIDC bearer token,
+  # any scopes must be prefixed with this value e.g. https://galaxyproject.org/api.
+  # More concretely, to request all permissions that the user has, the scope
+  # would have to be specified as "<prefix>:*". e.g "https://galaxyproject.org/api:*".
+  # Currently, only * is recognised as a valid scope, and future iterations may
+  # provide more fine-grained scopes.
+  #oidc_scope_prefix: https://galaxyproject.org/api
+
   # XML config file that allows the use of different authentication
   # providers (e.g. LDAP) instead or in addition to local authentication
   # (.sample is used if default does not exist).
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #auth_config_file: auth_conf.xml
```

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/job_conf.sample.yml` & `galaxy-config-24.0.0/galaxy/config/sample/job_conf.sample.yml`

 * *Files 2% similar despite different names*

```diff
@@ -795,15 +795,15 @@
       # Demonstrates how to use total-perspective-vortex, which enables dynamic destination
       # selection for entities (Tools, Users, Groups) based on a configurable yaml file.
       # See: https://total-perspective-vortex.readthedocs.io/ for documentation.
       type: python
       function: map_tool_to_destination
       rules_module: tpv.rules
       tpv_config_files:
-        - https://raw.githubusercontent.com/galaxyproject/total-perspective-vortex/main/tests/fixtures/mapping-sample.yml
+        - https://gxy.io/tpv/db.yml
         # - config/tpv_rules_local.yml
 
     docker_dispatch:
       runner: dynamic
       # Follow dynamic destination type will send all tool's that
       # support docker to static destination defined by
       # docker_destination_id (docker_cluster in this example) and all
```

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/job_conf.xml.sample_advanced` & `galaxy-config-24.0.0/galaxy/config/sample/job_conf.xml.sample_advanced`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/job_resource_params_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/job_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/lmod_modules_mapping.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/lmod_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/object_store_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/object_store_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/oidc_backends_config.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/oidc_backends_config.xml.sample`

 * *Files 1% similar despite different names*

#### Comparing `galaxy-config-23.2.1/galaxy/config/sample/oidc_backends_config.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/oidc_backends_config.xml.sample`

```diff
@@ -141,14 +141,16 @@
     <!-- (Optional) Override the default idp hint -->
     <!-- <idphint>cilogon</idphint> -->
     <!-- (Optional) Enable logging out of the IDP when user logs out of Galaxy -->
     <!-- <enable_idp_logout>false</enable_idp_logout> -->
     <!-- <icon>https://path/to/icon</icon>  -->
     <!-- (Optional) Enable PKCE for this IDP -->
     <!-- <pkce_support>false</pkce_support> -->
+    <!-- (Optional) the audiences accepted on the access-token for this IDP. -->
+    <!-- <accepted_audiences>galaxy</accepted_audiences> -->
   </provider>
   <!-- Documentation: https://galaxyproject.org/authnz/config/oidc/idps/elixir-aai  -->
   <provider name="Elixir">
     <client_id>...</client_id>
     <client_secret>...</client_secret>
     <redirect_uri>http://localhost:8080/authnz/elixir/callback</redirect_uri>
     <prompt>consent</prompt>
```

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/oidc_config.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/oidc_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/reports.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/reports.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/themes_conf.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/themes_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/tool_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/tool_conf.xml.sample`

 * *Files 1% similar despite different names*

#### Comparing `galaxy-config-23.2.1/galaxy/config/sample/tool_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/tool_conf.xml.sample`

```diff
@@ -33,14 +33,15 @@
     <tool file="${model_tools_path}/filter_failed_collection.xml"/>
     <tool file="${model_tools_path}/filter_empty_collection.xml"/>
     <tool file="${model_tools_path}/flatten_collection.xml"/>
     <tool file="${model_tools_path}/merge_collection.xml"/>
     <tool file="${model_tools_path}/relabel_from_file.xml"/>
     <tool file="${model_tools_path}/filter_from_file.xml"/>
     <tool file="${model_tools_path}/sort_collection_list.xml"/>
+    <tool file="${model_tools_path}/harmonize_two_collections_list.xml"/>
     <tool file="${model_tools_path}/tag_collection_from_file.xml"/>
     <tool file="${model_tools_path}/apply_rules.xml"/>
     <tool file="${model_tools_path}/build_list.xml"/>
     <tool file="${model_tools_path}/build_list_1.2.0.xml"/>
     <tool file="${model_tools_path}/extract_dataset.xml"/>
     <tool file="${model_tools_path}/duplicate_file_to_collection.xml"/>
   </section>
```

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/tool_data_table_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/tool_data_table_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/tool_destinations.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/tool_destinations.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/tool_recommendations_overwrite.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/tool_shed.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/tool_shed.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/trs_servers_conf.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/trs_servers_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/user_preferences_extra_conf.yml.sample`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,16 @@
             - name: username
               label: Username
               type: text
               required: False
             - name: password
               label: Password
               type:  password
+              # for storing the password in a vault (instead of plaintext in the DB)
+              # store: vault
               required: False
 
     invenio:
         description: Your Invenio RDM Integration Settings
         inputs:
             - name: token
               label: Personal Token used to create draft records and to upload files
```

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/workflow_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample` & `galaxy-config-24.0.0/galaxy/config/sample/workflow_schedulers_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/schema.py` & `galaxy-config-24.0.0/galaxy/config/schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/schemas/config_schema.yml` & `galaxy-config-24.0.0/galaxy/config/schemas/config_schema.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1030,14 +1030,28 @@
         default: object_store_conf.xml
         path_resolves_to: config_dir
         required: false
         desc: |
           Configuration file for the object store
           If this is set and exists, it overrides any other objectstore settings.
 
+      object_store_config:
+        type: seq
+        sequence:
+          - type: any
+        desc: |
+          Rather than specifying an object_store_config_file, the object store configuration can be embedded into
+          Galaxy's config with this option.
+
+          This option has no effect if the file specified by object_store_config_file exists. Otherwise, if this option
+          is set, it overrides any other objectstore settings.
+
+          The syntax, available storage plugins, and documentation of their options is explained in detail in the
+          object store sample configuration file, `object_store_conf.sample.yml`
+
       object_store_cache_monitor_driver:
         type: str
         default: 'auto'
         required: false
         enum: ['auto', 'inprocess', 'celery', 'external']
         desc: |
           Specify where cache monitoring is driven for caching object stores
@@ -1076,14 +1090,24 @@
         type: int
         default: -1
         required: false
         desc: |
           Default cache size for caching object stores if cache not configured for
           that object store entry.
 
+      object_store_always_respect_user_selection:
+        type: bool
+        default: false
+        required: false
+        desc: |
+          Set this to true to indicate in the UI that a user's object store selection
+          isn't simply a "preference" that job destinations often respect but in fact
+          will always be respected. This should be set to true to simplify the UI as
+          long as job destinations never override 'object_store_id's for a jobs.
+
       object_store_store_by:
         type: str
         required: false
         desc: |
           What Dataset attribute is used to reference files in an ObjectStore implementation,
           this can be 'uuid' or 'id'. The default will depend on how the object store is configured,
           starting with 20.05 Galaxy will try to default to 'uuid' if it can be sure this
@@ -1868,17 +1892,25 @@
           corresponding nginx configuration.
 
       tus_upload_store:
         type: str
         required: False
         desc: |
           The upload store is a temporary directory in which files uploaded by the
-          tus middleware or server will be placed.
+          tus middleware or server for user uploads will be placed.
           Defaults to new_file_path if not set.
 
+      tus_upload_store_job_files:
+        type: str
+        required: False
+        desc: |
+          The upload store is a temporary directory in which files uploaded by the
+          tus middleware or server for remote job files (Pulsar) will be placed.
+          Defaults to tus_upload_store if not set.
+
       chunk_upload_size:
         type: int
         default: 10485760
         required: false
         desc: |
           Galaxy can upload user files in chunks without using nginx. Enable the chunk
           uploader by specifying a chunk size larger than 0. The chunk size is specified
@@ -2899,14 +2931,27 @@
         type: str
         default: oidc_backends_config.xml
         path_resolves_to: config_dir
         required: false
         desc: |
           Sets the path to OIDC backends configuration file.
 
+      oidc_scope_prefix:
+        type: str
+        default: https://galaxyproject.org/api
+        required: false
+        desc: |
+          Sets the prefix for OIDC scopes specific to this Galaxy instance.
+          If an API call is made against this Galaxy instance using an OIDC bearer token,
+          any scopes must be prefixed with this value e.g. https://galaxyproject.org/api.
+          More concretely, to request all permissions that the user has, the scope
+          would have to be specified as "<prefix>:*". e.g "https://galaxyproject.org/api:*".
+          Currently, only * is recognised as a valid scope, and future iterations may
+          provide more fine-grained scopes.
+
       auth_config_file:
         type: str
         default: auth_conf.xml
         path_resolves_to: config_dir
         required: false
         desc: |
           XML config file that allows the use of different authentication providers
```

### Comparing `galaxy-config-23.2.1/galaxy/config/schemas/job_config_schema.yml` & `galaxy-config-24.0.0/galaxy/config/schemas/job_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/schemas/reports_config_schema.yml` & `galaxy-config-24.0.0/galaxy/config/schemas/reports_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/schemas/tool_shed_config_schema.yml` & `galaxy-config-24.0.0/galaxy/config/schemas/tool_shed_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/script.py` & `galaxy-config-24.0.0/galaxy/config/script.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.2.1/galaxy/config/templates.py` & `galaxy-config-24.0.0/galaxy/config/templates.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,32 +6,35 @@
 template will be read from `config/templates` in the Galaxy root.
 """
 
 from pathlib import Path
 
 from jinja2 import Environment
 
-from galaxy.util.resources import resource_path
+from galaxy.util.resources import (
+    resource_path,
+    Traversable,
+)
 
 TEMPLATE_SEP = ">>>>>>"  # Used to split templates into doc/body sections
 
 
 def render(template_path: str, context: dict, custom_templates_dir: str) -> str:
     """Read and return templated content as string."""
-    with open(_get_template_path(template_path, custom_templates_dir)) as f:
+    with _get_template_path(template_path, custom_templates_dir).open() as f:
         template_str = _get_template_body(f.read())
     tmpl = Environment().from_string(template_str)
     return tmpl.render(**context)
 
 
 def _get_template_body(template: str) -> str:
     """Remove comment/doc header to return the template body."""
     return template.split(TEMPLATE_SEP, 1)[-1].split("\n", 1)[1]
 
 
-def _get_template_path(relpath: str, custom_templates_dir: str) -> Path:
+def _get_template_path(relpath: str, custom_templates_dir: str) -> Traversable:
     """Return template file path."""
     default_path = resource_path("galaxy.config", "templates") / relpath
     custom_path = Path(custom_templates_dir) / relpath
     if custom_path.exists():
         return custom_path
     return default_path
```

### Comparing `galaxy-config-23.2.1/galaxy_config.egg-info/PKG-INFO` & `galaxy-config-24.0.0/galaxy_config.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-util
+Requires-Dist: boltons
+Requires-Dist: jinja2
+Requires-Dist: pykwalify
+Requires-Dist: PyYAML
 
 
 .. image:: https://badge.fury.io/py/galaxy-config.svg
    :target: https://pypi.org/project/galaxy-config/
 
 
 Overview
@@ -42,14 +47,47 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Follow-up on #17274 and #17262 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17302 <https://github.com/galaxyproject/galaxy/pull/17302>`_
+* Fix minor oidc_backends_config comment bug by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17385 <https://github.com/galaxyproject/galaxy/pull/17385>`_
+
+============
+Enhancements
+============
+
+* Add harmonize collections tool (or whatever other name) by `@lldelisle <https://github.com/lldelisle>`_ in `#16662 <https://github.com/galaxyproject/galaxy/pull/16662>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Add support for (fast5.tar).xz binary compressed files by `@tuncK <https://github.com/tuncK>`_ in `#17106 <https://github.com/galaxyproject/galaxy/pull/17106>`_
+* Add a3m datatype by `@astrovsky01 <https://github.com/astrovsky01>`_ in `#17217 <https://github.com/galaxyproject/galaxy/pull/17217>`_
+* Convert sample object store configuration to YAML and support configuring inline by `@natefoo <https://github.com/natefoo>`_ in `#17222 <https://github.com/galaxyproject/galaxy/pull/17222>`_
+* Allow job files to consume TUS uploads by `@jmchilton <https://github.com/jmchilton>`_ in `#17242 <https://github.com/galaxyproject/galaxy/pull/17242>`_
+* Add OIDC backend configuration schema and validation by `@uwwint <https://github.com/uwwint>`_ in `#17274 <https://github.com/galaxyproject/galaxy/pull/17274>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* Use short link for TPV shared database by `@nuwang <https://github.com/nuwang>`_ in `#17467 <https://github.com/galaxyproject/galaxy/pull/17467>`_
+* Feature SBOL datatypes by `@guillaume-gricourt <https://github.com/guillaume-gricourt>`_ in `#17482 <https://github.com/galaxyproject/galaxy/pull/17482>`_
+* Add documentation on how to use vault keys in file sources by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17498 <https://github.com/galaxyproject/galaxy/pull/17498>`_
+* add npy datatype by `@astrovsky01 <https://github.com/astrovsky01>`_ in `#17517 <https://github.com/galaxyproject/galaxy/pull/17517>`_
+* Enhance Avivator display app to support regular Tiffs by `@davelopez <https://github.com/davelopez>`_ in `#17554 <https://github.com/galaxyproject/galaxy/pull/17554>`_
+* Allow admin to sharpen language about selected object stores. by `@jmchilton <https://github.com/jmchilton>`_ in `#17806 <https://github.com/galaxyproject/galaxy/pull/17806>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -72,15 +110,15 @@
 * Add new datatype: STL by `@TanguyGen <https://github.com/TanguyGen>`_ in `#16478 <https://github.com/galaxyproject/galaxy/pull/16478>`_
 * add new tabular file formats cns,cnr and cnn to datatypes_conf.xml.sample file as they are neaded for cnvkit galaxy tools by `@khaled196 <https://github.com/khaled196>`_ in `#16503 <https://github.com/galaxyproject/galaxy/pull/16503>`_
 * Tweak tool memory use and optimize shared memory when using preload by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16536 <https://github.com/galaxyproject/galaxy/pull/16536>`_
 * Implement datatype upload warnings by `@jmchilton <https://github.com/jmchilton>`_ in `#16564 <https://github.com/galaxyproject/galaxy/pull/16564>`_
 * Support new genome browser chain file format by `@claudiofr <https://github.com/claudiofr>`_ in `#16576 <https://github.com/galaxyproject/galaxy/pull/16576>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16577 <https://github.com/galaxyproject/galaxy/pull/16577>`_
 * Implement instance URLs in Galaxy markdown. by `@jmchilton <https://github.com/jmchilton>`_ in `#16675 <https://github.com/galaxyproject/galaxy/pull/16675>`_
-*  Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
+* Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
 * Update datatypes_conf.xml.sample with docx type by `@yvanlebras <https://github.com/yvanlebras>`_ in `#16713 <https://github.com/galaxyproject/galaxy/pull/16713>`_
 * Replace ELIXIR AAI button with Life Science login by `@sebastian-schaaf <https://github.com/sebastian-schaaf>`_ in `#16762 <https://github.com/galaxyproject/galaxy/pull/16762>`_
 * Add EGI Check-in as OIDC authentication option by `@enolfc <https://github.com/enolfc>`_ in `#16782 <https://github.com/galaxyproject/galaxy/pull/16782>`_
 * Updated path-based interactive tools with entry point path injection, support for ITs with relative links, shortened URLs, doc and config updates including Podman job_conf by `@sveinugu <https://github.com/sveinugu>`_ in `#16795 <https://github.com/galaxyproject/galaxy/pull/16795>`_
 * Galaxy help forum integration by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#16798 <https://github.com/galaxyproject/galaxy/pull/16798>`_
 * Remove record access handling for Invenio RDM plugin by `@davelopez <https://github.com/davelopez>`_ in `#16900 <https://github.com/galaxyproject/galaxy/pull/16900>`_
 * optimize object store cache operations by `@SergeyYakubov <https://github.com/SergeyYakubov>`_ in `#17025 <https://github.com/galaxyproject/galaxy/pull/17025>`_
```

### Comparing `galaxy-config-23.2.1/galaxy_config.egg-info/SOURCES.txt` & `galaxy-config-24.0.0/galaxy_config.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 galaxy/config/sample/galaxy.yml.sample
 galaxy/config/sample/job_conf.sample.yml
 galaxy/config/sample/job_conf.xml.sample_advanced
 galaxy/config/sample/job_conf.xml.sample_basic
 galaxy/config/sample/job_resource_params_conf.xml.sample
 galaxy/config/sample/lmod_modules_mapping.yml.sample
 galaxy/config/sample/local_conda_mapping.yml.sample
+galaxy/config/sample/object_store_conf.sample.yml
 galaxy/config/sample/object_store_conf.xml.sample
 galaxy/config/sample/oidc_backends_config.xml.sample
 galaxy/config/sample/oidc_config.xml.sample
 galaxy/config/sample/reports.yml.sample
 galaxy/config/sample/themes_conf.yml.sample
 galaxy/config/sample/tool_conf.xml.sample
 galaxy/config/sample/tool_data_table_conf.xml.sample
```

### Comparing `galaxy-config-23.2.1/setup.cfg` & `galaxy-config-24.0.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -5,44 +5,44 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy configuration
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-config
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	boltons
 	jinja2
 	pykwalify
 	PyYAML
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	galaxy-config = galaxy.config.script:main
 
 [options.packages.find]
 exclude =
```

