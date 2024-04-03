# Comparing `tmp/spaceone-repository-2.0.dev8.tar.gz` & `tmp/spaceone-repository-2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-repository-2.0.dev8.tar", last modified: Tue Dec 19 17:20:26 2023, max compression
+gzip compressed data, was "spaceone-repository-2.0.dev9.tar", last modified: Thu Dec 21 05:44:20 2023, max compression
```

## Comparing `spaceone-repository-2.0.dev8.tar` & `spaceone-repository-2.0.dev9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.930014 spaceone-repository-2.0.dev8/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.930014 spaceone-repository-2.0.dev8/spaceone/repository/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.930014 spaceone-repository-2.0.dev8/spaceone/repository/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.934014 spaceone-repository-2.0.dev8/spaceone/repository/connector/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/connector/registry_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/connector/remote_repository_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.934014 spaceone-repository-2.0.dev8/spaceone/repository/error/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/error/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/error/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.934014 spaceone-repository-2.0.dev8/spaceone/repository/info/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/info/plugin_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/info/repository_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.934014 spaceone-repository-2.0.dev8/spaceone/repository/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.934014 spaceone-repository-2.0.dev8/spaceone/repository/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/interface/grpc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/interface/grpc/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.930014 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-api-direct-mon-webhook.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-cloud-service-inven-collector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-cloudtrail-mon-datasource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-cloudwatch-mon-datasource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-cost-explorer-cost-datasource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-ec2-inven-collector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-phd-inven-collector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-sns-mon-webhook.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-trusted-advisor-inven-collector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-azure-activity-log-mon-datasource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-azure-cost-mgmt-cost-datasource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-azure-inven-collector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-azure-monitor-mon-datasource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-email-noti-protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-google-cloud-inven-collector.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-google-cloud-log-mon-datasource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-google-monitoring-mon-webhook.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-google-stackdriver-mon-datasource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-grafana-mon-webhook.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-keycloak-identity-auth.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-ms-teams-noti-protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-prometheus-mon-webhook.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-slack-noti-protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      750 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-telegram-noti-protocol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/spaceone/repository/manager/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/manager/identity_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/spaceone/repository/manager/plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/manager/plugin_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/manager/plugin_manager/local_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/manager/plugin_manager/managed_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/manager/plugin_manager/remote_plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/spaceone/repository/manager/repository_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/manager/repository_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/manager/repository_manager/local_repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/spaceone/repository/model/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/model/capability_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/model/plugin_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/spaceone/repository/service/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14049 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/service/plugin_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-19 17:20:18.000000 spaceone-repository-2.0.dev8/spaceone/repository/service/repository_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 17:20:26.938014 spaceone-repository-2.0.dev8/spaceone_repository.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-19 17:20:26.000000 spaceone-repository-2.0.dev8/spaceone_repository.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2023-12-19 17:20:26.000000 spaceone-repository-2.0.dev8/spaceone_repository.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 17:20:26.000000 spaceone-repository-2.0.dev8/spaceone_repository.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 17:20:26.000000 spaceone-repository-2.0.dev8/spaceone_repository.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-19 17:20:26.000000 spaceone-repository-2.0.dev8/spaceone_repository.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-19 17:20:26.000000 spaceone-repository-2.0.dev8/spaceone_repository.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.491362 spaceone-repository-2.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-21 05:44:20.491362 spaceone-repository-2.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 05:44:20.491362 spaceone-repository-2.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.479362 spaceone-repository-2.0.dev9/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.479362 spaceone-repository-2.0.dev9/spaceone/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.479362 spaceone-repository-2.0.dev9/spaceone/repository/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.479362 spaceone-repository-2.0.dev9/spaceone/repository/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/connector/registry_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/connector/remote_repository_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.483362 spaceone-repository-2.0.dev9/spaceone/repository/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/error/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/error/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.483362 spaceone-repository-2.0.dev9/spaceone/repository/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/info/plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/info/repository_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.483362 spaceone-repository-2.0.dev9/spaceone/repository/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.483362 spaceone-repository-2.0.dev9/spaceone/repository/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/interface/grpc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/interface/grpc/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.479362 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.487362 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-api-direct-mon-webhook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-cloud-service-inven-collector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-cloudtrail-mon-datasource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-cloudwatch-mon-datasource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-cost-explorer-cost-datasource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-ec2-inven-collector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-phd-inven-collector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-sns-mon-webhook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-trusted-advisor-inven-collector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-azure-activity-log-mon-datasource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-azure-cost-mgmt-cost-datasource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-azure-inven-collector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-azure-monitor-mon-datasource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-email-noti-protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-google-cloud-inven-collector.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-google-cloud-log-mon-datasource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-google-monitoring-mon-webhook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-google-stackdriver-mon-datasource.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-grafana-mon-webhook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-keycloak-identity-auth.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-ms-teams-noti-protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-prometheus-mon-webhook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-slack-noti-protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-telegram-noti-protocol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.487362 spaceone-repository-2.0.dev9/spaceone/repository/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/manager/identity_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.487362 spaceone-repository-2.0.dev9/spaceone/repository/manager/plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/manager/plugin_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/manager/plugin_manager/local_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/manager/plugin_manager/managed_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/manager/plugin_manager/remote_plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.487362 spaceone-repository-2.0.dev9/spaceone/repository/manager/repository_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/manager/repository_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/manager/repository_manager/local_repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.487362 spaceone-repository-2.0.dev9/spaceone/repository/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/model/capability_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/model/plugin_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.487362 spaceone-repository-2.0.dev9/spaceone/repository/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14049 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/service/plugin_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-21 05:44:11.000000 spaceone-repository-2.0.dev9/spaceone/repository/service/repository_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 05:44:20.491362 spaceone-repository-2.0.dev9/spaceone_repository.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-21 05:44:20.000000 spaceone-repository-2.0.dev9/spaceone_repository.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2023-12-21 05:44:20.000000 spaceone-repository-2.0.dev9/spaceone_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 05:44:20.000000 spaceone-repository-2.0.dev9/spaceone_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 05:44:20.000000 spaceone-repository-2.0.dev9/spaceone_repository.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-21 05:44:20.000000 spaceone-repository-2.0.dev9/spaceone_repository.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-21 05:44:20.000000 spaceone-repository-2.0.dev9/spaceone_repository.egg-info/top_level.txt
```

### Comparing `spaceone-repository-2.0.dev8/setup.py` & `spaceone-repository-2.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/conf/global_conf.py` & `spaceone-repository-2.0.dev9/spaceone/repository/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/connector/registry_connector.py` & `spaceone-repository-2.0.dev9/spaceone/repository/connector/registry_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/connector/remote_repository_connector.py` & `spaceone-repository-2.0.dev9/spaceone/repository/connector/remote_repository_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/error/plugin.py` & `spaceone-repository-2.0.dev9/spaceone/repository/error/plugin.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/error/repository.py` & `spaceone-repository-2.0.dev9/spaceone/repository/error/repository.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/info/plugin_info.py` & `spaceone-repository-2.0.dev9/spaceone/repository/info/plugin_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/info/repository_info.py` & `spaceone-repository-2.0.dev9/spaceone/repository/info/repository_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/interface/grpc/plugin.py` & `spaceone-repository-2.0.dev9/spaceone/repository/interface/grpc/plugin.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/interface/grpc/repository.py` & `spaceone-repository-2.0.dev9/spaceone/repository/interface/grpc/repository.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-api-direct-mon-webhook.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-api-direct-mon-webhook.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-cloud-service-inven-collector.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-cloud-service-inven-collector.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-cloudtrail-mon-datasource.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-cloudtrail-mon-datasource.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-cloudwatch-mon-datasource.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-cloudwatch-mon-datasource.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-cost-explorer-cost-datasource.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-cost-explorer-cost-datasource.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-ec2-inven-collector.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-ec2-inven-collector.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-phd-inven-collector.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-phd-inven-collector.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-sns-mon-webhook.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-sns-mon-webhook.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-aws-trusted-advisor-inven-collector.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-aws-trusted-advisor-inven-collector.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-azure-activity-log-mon-datasource.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-azure-activity-log-mon-datasource.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-azure-cost-mgmt-cost-datasource.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-azure-cost-mgmt-cost-datasource.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-azure-inven-collector.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-azure-inven-collector.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-azure-monitor-mon-datasource.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-azure-monitor-mon-datasource.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-email-noti-protocol.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-email-noti-protocol.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-google-cloud-inven-collector.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-google-cloud-inven-collector.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-google-cloud-log-mon-datasource.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-google-cloud-log-mon-datasource.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-google-monitoring-mon-webhook.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-google-monitoring-mon-webhook.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-google-stackdriver-mon-datasource.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-google-stackdriver-mon-datasource.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-grafana-mon-webhook.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-grafana-mon-webhook.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-keycloak-identity-auth.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-keycloak-identity-auth.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-ms-teams-noti-protocol.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-ms-teams-noti-protocol.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-slack-noti-protocol.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-slack-noti-protocol.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/managed_resource/plugin/plugin-telegram-noti-protocol.yaml` & `spaceone-repository-2.0.dev9/spaceone/repository/managed_resource/plugin/plugin-telegram-noti-protocol.yaml`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/manager/__init__.py` & `spaceone-repository-2.0.dev9/spaceone/repository/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/manager/identity_manager.py` & `spaceone-repository-2.0.dev9/spaceone/repository/manager/identity_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/manager/plugin_manager/__init__.py` & `spaceone-repository-2.0.dev9/spaceone/repository/manager/plugin_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/manager/plugin_manager/local_plugin_manager.py` & `spaceone-repository-2.0.dev9/spaceone/repository/manager/plugin_manager/local_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/manager/plugin_manager/managed_plugin_manager.py` & `spaceone-repository-2.0.dev9/spaceone/repository/manager/plugin_manager/managed_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/manager/plugin_manager/remote_plugin_manager.py` & `spaceone-repository-2.0.dev9/spaceone/repository/manager/plugin_manager/remote_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/manager/repository_manager/__init__.py` & `spaceone-repository-2.0.dev9/spaceone/repository/manager/repository_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/manager/repository_manager/local_repository_manager.py` & `spaceone-repository-2.0.dev9/spaceone/repository/manager/repository_manager/local_repository_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/model/plugin_model.py` & `spaceone-repository-2.0.dev9/spaceone/repository/model/plugin_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/service/plugin_service.py` & `spaceone-repository-2.0.dev9/spaceone/repository/service/plugin_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone/repository/service/repository_service.py` & `spaceone-repository-2.0.dev9/spaceone/repository/service/repository_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-repository-2.0.dev8/spaceone_repository.egg-info/SOURCES.txt` & `spaceone-repository-2.0.dev9/spaceone_repository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

