# Comparing `tmp/aschot_pulumi_dbtcloud-0.0.4.tar.gz` & `tmp/aschot_pulumi_dbtcloud-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aschot_pulumi_dbtcloud-0.0.4.tar", last modified: Wed Apr  3 14:28:00 2024, max compression
+gzip compressed data, was "aschot_pulumi_dbtcloud-0.0.5.tar", last modified: Wed Apr  3 14:46:15 2024, max compression
```

## Comparing `aschot_pulumi_dbtcloud-0.0.4.tar` & `aschot_pulumi_dbtcloud-0.0.5.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:28:00.683090 aschot_pulumi_dbtcloud-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-03 14:28:00.683090 aschot_pulumi_dbtcloud-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:28:00.679090 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/
--rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    58910 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/big_query_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:28:00.683090 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    43921 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20961 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    29767 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/environment_variable_job_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    17517 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24517 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/fabric_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26022 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/fabric_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_azure_dev_ops_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_azure_dev_ops_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_big_query_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    15607 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    68732 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    55352 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_bigquery_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_bigquery_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    41127 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    18967 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    27784 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_bigquery_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    14434 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    21238 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_project_artefacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_project_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_project_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    37919 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    27682 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    20197 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/license_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    29517 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    15400 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/project_artefacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/project_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/project_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    38546 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    28683 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:28:00.683090 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:28:00.683090 aschot_pulumi_dbtcloud-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-03 14:28:00.000000 aschot_pulumi_dbtcloud-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:15.210246 aschot_pulumi_dbtcloud-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-03 14:46:15.210246 aschot_pulumi_dbtcloud-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:15.210246 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58910 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/big_query_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:15.210246 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43921 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20961 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29767 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/environment_variable_job_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17517 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24517 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/fabric_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26022 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/fabric_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_azure_dev_ops_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_azure_dev_ops_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_big_query_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15607 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68732 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55352 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_bigquery_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_bigquery_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41127 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18967 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27784 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_bigquery_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14434 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21238 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_project_artefacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_project_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_project_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37919 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27682 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20197 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/license_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29517 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15400 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22298 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/project_artefacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/project_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/project_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    38546 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28683 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21104 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:15.210246 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-03 14:46:15.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-03 14:46:15.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:46:15.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:46:15.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 14:46:15.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 14:46:15.000000 aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:46:15.210246 aschot_pulumi_dbtcloud-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-03 14:46:14.000000 aschot_pulumi_dbtcloud-0.0.5/setup.py
```

### Comparing `aschot_pulumi_dbtcloud-0.0.4/PKG-INFO` & `aschot_pulumi_dbtcloud-0.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-Metadata-Version: 2.1
-Name: aschot_pulumi_dbtcloud
-Version: 0.0.4
-Summary: A Pulumi package for creating and managing dbt Cloud resources.
-Home-page: https://www.pulumi.com
-License: Apache-2.0
-Project-URL: Repository, https://github.com/a-schot/pulumi-dbtcloud
-Keywords: pulumi dbtcloud dbt cloud category/cloud
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # dbt Cloud Resource Provider
 
 The dbt Cloud Resource Provider lets you manage dbt Cloud resources.
 
 ## Installation
 
 This package is available for several languages/platforms:
 
+- JavaScript/TypeScript: [`@aschot/pulumi-dbtcloud`](https://www.npmjs.com/package/@aschot/pulumi-dbtcloud)
+- Python: [`aschot-pulumi-dbtcloud`](https://pypi.org/project/aschot-pulumi-dbtcloud/)
+- Go: [`github.com/a-schot/pulumi-dbtcloud/sdk/go/dbtcloud`](https://pkg.go.dev/github.com/a-schot/pulumi-dbtcloud/sdk/go/dbtcloud)
+- .NET: [`ASchot.Pulumi.Dbtcloud`](https://www.nuget.org/packages/ASchot.Pulumi.Dbtcloud)
+
+## Provider Binary
+
+The dbt Cloud provider binary is a third party binary. It can be installed using the pulumi plugin command.
+
+```bash
+pulumi plugin install resource dbtcloud <version> --server github://api.github.com/a-schot/pulumi-dbtcloud
+```
+
+Replace `<version>` with your desired version.
+
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
 npm install @achot/pulumi_dbtcloud
 ```
@@ -61,9 +64,7 @@
 Use `pulumi config set dbtcloud:<option> (--secret)`.
 
 | Option     | Environment Variable   | Required/Optional | Default                                                      | Description                             | 
 |------------|------------------------|-------------------|--------------------------------------------------------------|-----------------------------------------|
 | `token`    | `DBT_CLOUD_TOKEN`      | Required          |                                                              | The API token for your dbt Cloud user   |
 | `accountId`| `DBT_CLOUD_ACCOUNT_ID` | Required          |                                                              | The ID for your dbt Cloud account       |
 | `hostUrl`  | `DBT_CLOUD_HOST_URL`   | Optional          | [https://cloud.getdbt.com/api](https://cloud.getdbt.com/api) | The host URL for your dbt Cloud account |
-
-
```

### Comparing `aschot_pulumi_dbtcloud-0.0.4/README.md` & `aschot_pulumi_dbtcloud-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,42 @@
+Metadata-Version: 2.1
+Name: aschot_pulumi_dbtcloud
+Version: 0.0.5
+Summary: A Pulumi package for creating and managing dbt Cloud resources.
+Home-page: https://www.pulumi.com
+License: Apache-2.0
+Project-URL: Repository, https://github.com/a-schot/pulumi-dbtcloud
+Keywords: pulumi dbtcloud dbt cloud category/cloud
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # dbt Cloud Resource Provider
 
 The dbt Cloud Resource Provider lets you manage dbt Cloud resources.
 
 ## Installation
 
 This package is available for several languages/platforms:
 
+- JavaScript/TypeScript: [`@aschot/pulumi-dbtcloud`](https://www.npmjs.com/package/@aschot/pulumi-dbtcloud)
+- Python: [`aschot-pulumi-dbtcloud`](https://pypi.org/project/aschot-pulumi-dbtcloud/)
+- Go: [`github.com/a-schot/pulumi-dbtcloud/sdk/go/dbtcloud`](https://pkg.go.dev/github.com/a-schot/pulumi-dbtcloud/sdk/go/dbtcloud)
+- .NET: [`ASchot.Pulumi.Dbtcloud`](https://www.nuget.org/packages/ASchot.Pulumi.Dbtcloud)
+
+## Provider Binary
+
+The dbt Cloud provider binary is a third party binary. It can be installed using the pulumi plugin command.
+
+```bash
+pulumi plugin install resource dbtcloud <version> --server github://api.github.com/a-schot/pulumi-dbtcloud
+```
+
+Replace `<version>` with your desired version.
+
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
 npm install @achot/pulumi_dbtcloud
 ```
@@ -49,7 +76,9 @@
 Use `pulumi config set dbtcloud:<option> (--secret)`.
 
 | Option     | Environment Variable   | Required/Optional | Default                                                      | Description                             | 
 |------------|------------------------|-------------------|--------------------------------------------------------------|-----------------------------------------|
 | `token`    | `DBT_CLOUD_TOKEN`      | Required          |                                                              | The API token for your dbt Cloud user   |
 | `accountId`| `DBT_CLOUD_ACCOUNT_ID` | Required          |                                                              | The ID for your dbt Cloud account       |
 | `hostUrl`  | `DBT_CLOUD_HOST_URL`   | Optional          | [https://cloud.getdbt.com/api](https://cloud.getdbt.com/api) | The host URL for your dbt Cloud account |
+
+
```

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/__init__.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/_inputs.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/_utilities.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/big_query_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/big_query_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/big_query_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/big_query_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/config/vars.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/databricks_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/databricks_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/environment.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/environment.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/environment_variable.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/environment_variable.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/environment_variable_job_override.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/environment_variable_job_override.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/extended_attributes.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/extended_attributes.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/fabric_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/fabric_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/fabric_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/fabric_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_azure_dev_ops_project.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_azure_dev_ops_project.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_azure_dev_ops_repository.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_azure_dev_ops_repository.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_big_query_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_big_query_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_big_query_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_big_query_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_databricks_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_databricks_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_environment.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_environment.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_environment_variable.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_environment_variable.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_extended_attributes.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_extended_attributes.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_group.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_group.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_group_users.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_group_users.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_job.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_job.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_notification.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_notification.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_postgres_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_postgres_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_privatelink_endpoint.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_project.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_project.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_repository.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_repository.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_service_token.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_service_token.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_snowflake_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_user.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_user.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_user_groups.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/get_webhook.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/get_webhook.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/group.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/group.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/job.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/job.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_bigquery_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_bigquery_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_bigquery_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_bigquery_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_databricks_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_databricks_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_environment.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_environment.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_environment_variable.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_environment_variable.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_big_query_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_big_query_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_bigquery_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_bigquery_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_databricks_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_databricks_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_environment.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_environment.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_environment_variable.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_environment_variable.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_group.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_group.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_job.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_job.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_postgres_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_postgres_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_privatelink_endpoint.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_project.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_project.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_repository.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_repository.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_service_token.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_service_token.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_snowflake_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_user.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_user.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_get_webhook.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_get_webhook.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_group.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_group.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_job.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_job.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_postgres_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_postgres_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_project.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_project.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_project_artefacts.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_project_artefacts.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_project_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_project_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_project_repository.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_project_repository.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_repository.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_repository.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_service_token.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_service_token.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_snowflake_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/legacy_webhook.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/legacy_webhook.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/license_map.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/license_map.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/notification.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/notification.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/outputs.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/outputs.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/postgres_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/postgres_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/project.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/project.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/project_artefacts.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/project_artefacts.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/project_connection.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/project_connection.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/project_repository.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/project_repository.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/provider.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/provider.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/repository.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/repository.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/service_token.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/service_token.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/snowflake_credential.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/user_groups.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/user_groups.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud/webhook.py` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud/webhook.py`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud.egg-info/PKG-INFO` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aschot-pulumi-dbtcloud
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Pulumi package for creating and managing dbt Cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/a-schot/pulumi-dbtcloud
 Keywords: pulumi dbtcloud dbt cloud category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -14,14 +14,29 @@
 
 The dbt Cloud Resource Provider lets you manage dbt Cloud resources.
 
 ## Installation
 
 This package is available for several languages/platforms:
 
+- JavaScript/TypeScript: [`@aschot/pulumi-dbtcloud`](https://www.npmjs.com/package/@aschot/pulumi-dbtcloud)
+- Python: [`aschot-pulumi-dbtcloud`](https://pypi.org/project/aschot-pulumi-dbtcloud/)
+- Go: [`github.com/a-schot/pulumi-dbtcloud/sdk/go/dbtcloud`](https://pkg.go.dev/github.com/a-schot/pulumi-dbtcloud/sdk/go/dbtcloud)
+- .NET: [`ASchot.Pulumi.Dbtcloud`](https://www.nuget.org/packages/ASchot.Pulumi.Dbtcloud)
+
+## Provider Binary
+
+The dbt Cloud provider binary is a third party binary. It can be installed using the pulumi plugin command.
+
+```bash
+pulumi plugin install resource dbtcloud <version> --server github://api.github.com/a-schot/pulumi-dbtcloud
+```
+
+Replace `<version>` with your desired version.
+
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
 npm install @achot/pulumi_dbtcloud
 ```
```

### Comparing `aschot_pulumi_dbtcloud-0.0.4/aschot_pulumi_dbtcloud.egg-info/SOURCES.txt` & `aschot_pulumi_dbtcloud-0.0.5/aschot_pulumi_dbtcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aschot_pulumi_dbtcloud-0.0.4/setup.py` & `aschot_pulumi_dbtcloud-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "dbtcloud Pulumi Package - Development Version"
```

