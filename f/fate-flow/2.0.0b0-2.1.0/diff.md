# Comparing `tmp/fate_flow-2.0.0b0.tar.gz` & `tmp/fate_flow-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fate_flow-2.0.0b0.tar", last modified: Tue Sep 19 04:32:15 2023, max compression
+gzip compressed data, was "fate_flow-2.1.0.tar", last modified: Wed Apr  3 06:56:24 2024, max compression
```

## Comparing `fate_flow-2.0.0b0.tar` & `fate_flow-2.1.0.tar`

### file list

```diff
@@ -1,336 +1,379 @@
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.965545 fate_flow-2.0.0b0/
--rw-r--r--   0 tonly      (501) staff       (20)     1690 2023-09-19 04:32:15.965350 fate_flow-2.0.0b0/PKG-INFO
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.917958 fate_flow-2.0.0b0/fate_flow/
--rw-r--r--   0 tonly      (501) staff       (20)      659 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)      668 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/_info.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.919362 fate_flow-2.0.0b0/fate_flow/apps/
--rw-r--r--   0 tonly      (501) staff       (20)     5685 2023-09-19 04:28:40.000000 fate_flow-2.0.0b0/fate_flow/apps/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.921847 fate_flow-2.0.0b0/fate_flow/apps/client/
--rw-r--r--   0 tonly      (501) staff       (20)      613 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/apps/client/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     4209 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/client_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     3631 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/data_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     8680 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/job_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     2494 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/log_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     3476 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/model_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     9853 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/output_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     4259 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/permission_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     2850 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/provider_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     4411 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/server_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     1107 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/site_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     2680 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/client/table_app.py
--rw-r--r--   0 tonly      (501) staff       (20)     3141 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/desc.py
--rw-r--r--   0 tonly      (501) staff       (20)     2883 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/desc_zh.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.922343 fate_flow-2.0.0b0/fate_flow/apps/partner/
--rw-r--r--   0 tonly      (501) staff       (20)      652 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/apps/partner/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)    11887 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/partner/partner_app.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.923007 fate_flow-2.0.0b0/fate_flow/apps/scheduler/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/apps/scheduler/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     2634 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/scheduler/scheduler_app.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.923425 fate_flow-2.0.0b0/fate_flow/apps/worker/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/apps/worker/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     8593 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/apps/worker/worker_app.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.924058 fate_flow-2.0.0b0/fate_flow/commands/
--rw-r--r--   0 tonly      (501) staff       (20)        0 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/commands/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     5707 2023-09-19 03:09:13.000000 fate_flow-2.0.0b0/fate_flow/commands/server_cli.py
--rw-r--r--   0 tonly      (501) staff       (20)     5601 2023-09-19 03:09:13.000000 fate_flow-2.0.0b0/fate_flow/commands/service.py
--rw-r--r--   0 tonly      (501) staff       (20)     4177 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/commands/service.sh
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.924418 fate_flow-2.0.0b0/fate_flow/components/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/components/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.924945 fate_flow-2.0.0b0/fate_flow/components/components/
--rw-r--r--   0 tonly      (501) staff       (20)      713 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/components/components/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     2000 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/components/components/download.py
--rw-r--r--   0 tonly      (501) staff       (20)    12008 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/components/components/upload.py
--rw-r--r--   0 tonly      (501) staff       (20)     1474 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/components/cpn.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.925322 fate_flow-2.0.0b0/fate_flow/components/entrypoint/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/components/entrypoint/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1173 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/components/entrypoint/component.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.926171 fate_flow-2.0.0b0/fate_flow/conf/
--rw-r--r--   0 tonly      (501) staff       (20)      223 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/conf/casbin_model.conf
--rw-r--r--   0 tonly      (501) staff       (20)      497 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/conf/job_default_config.yaml
--rw-r--r--   0 tonly      (501) staff       (20)      226 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/conf/permission_casbin_model.conf
--rw-r--r--   0 tonly      (501) staff       (20)      507 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/conf/pulsar_route_table.yaml
--rw-r--r--   0 tonly      (501) staff       (20)       80 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/conf/rabbitmq_route_table.yaml
--rw-r--r--   0 tonly      (501) staff       (20)     2499 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/conf/service_conf.yaml
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.927305 fate_flow-2.0.0b0/fate_flow/controller/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/controller/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     5141 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/controller/app_controller.py
--rw-r--r--   0 tonly      (501) staff       (20)      980 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/controller/config_manager.py
--rw-r--r--   0 tonly      (501) staff       (20)    21704 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/controller/job_controller.py
--rw-r--r--   0 tonly      (501) staff       (20)     6180 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/controller/permission_controller.py
--rw-r--r--   0 tonly      (501) staff       (20)    18131 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/controller/task_controller.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.928822 fate_flow-2.0.0b0/fate_flow/db/
--rw-r--r--   0 tonly      (501) staff       (20)      738 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/db/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)    15178 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/db/base_models.py
--rw-r--r--   0 tonly      (501) staff       (20)     7946 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/db/casbin_models.py
--rw-r--r--   0 tonly      (501) staff       (20)     9533 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/db/db_models.py
--rw-r--r--   0 tonly      (501) staff       (20)     1234 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/db/permission_models.py
--rw-r--r--   0 tonly      (501) staff       (20)     3064 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/db/schedule_models.py
--rw-r--r--   0 tonly      (501) staff       (20)     2457 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/db/storage_models.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.929223 fate_flow-2.0.0b0/fate_flow/detection/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/detection/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     6931 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/detection/detector.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.929729 fate_flow-2.0.0b0/fate_flow/engine/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/engine/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.930939 fate_flow-2.0.0b0/fate_flow/engine/backend/
--rw-r--r--   0 tonly      (501) staff       (20)      712 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/backend/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     5061 2023-09-19 03:09:13.000000 fate_flow-2.0.0b0/fate_flow/engine/backend/_base.py
--rw-r--r--   0 tonly      (501) staff       (20)     1652 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/backend/_eggroll.py
--rw-r--r--   0 tonly      (501) staff       (20)     1540 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/backend/_session.py
--rw-r--r--   0 tonly      (501) staff       (20)     2336 2023-09-19 03:09:13.000000 fate_flow-2.0.0b0/fate_flow/engine/backend/_spark.py
--rw-r--r--   0 tonly      (501) staff       (20)     8405 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/backend/eggroll_deepspeed.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.931555 fate_flow-2.0.0b0/fate_flow/engine/devices/
--rw-r--r--   0 tonly      (501) staff       (20)     1331 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/devices/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1158 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/devices/_base.py
--rw-r--r--   0 tonly      (501) staff       (20)     2766 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/devices/_container.py
--rw-r--r--   0 tonly      (501) staff       (20)     2986 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/devices/_local.py
--rw-r--r--   0 tonly      (501) staff       (20)     2974 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/relation_ship.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.932351 fate_flow-2.0.0b0/fate_flow/engine/storage/
--rw-r--r--   0 tonly      (501) staff       (20)      889 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     4967 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/_abc.py
--rw-r--r--   0 tonly      (501) staff       (20)    10760 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/_session.py
--rw-r--r--   0 tonly      (501) staff       (20)    12542 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/_table.py
--rw-r--r--   0 tonly      (501) staff       (20)     2477 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/_types.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.932930 fate_flow-2.0.0b0/fate_flow/engine/storage/eggroll/
--rw-r--r--   0 tonly      (501) staff       (20)      796 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/eggroll/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     2202 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/eggroll/_session.py
--rw-r--r--   0 tonly      (501) staff       (20)     2274 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/eggroll/_table.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.933654 fate_flow-2.0.0b0/fate_flow/engine/storage/file/
--rw-r--r--   0 tonly      (501) staff       (20)      790 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/file/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1514 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/file/_session.py
--rw-r--r--   0 tonly      (501) staff       (20)     4381 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/file/_table.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.934214 fate_flow-2.0.0b0/fate_flow/engine/storage/hdfs/
--rw-r--r--   0 tonly      (501) staff       (20)      790 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/hdfs/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1591 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/hdfs/_session.py
--rw-r--r--   0 tonly      (501) staff       (20)     4710 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/hdfs/_table.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.935450 fate_flow-2.0.0b0/fate_flow/engine/storage/standalone/
--rw-r--r--   0 tonly      (501) staff       (20)      802 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/standalone/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1878 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/standalone/_session.py
--rw-r--r--   0 tonly      (501) staff       (20)    39298 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/standalone/_standalone.py
--rw-r--r--   0 tonly      (501) staff       (20)     2413 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/engine/storage/standalone/_table.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.935757 fate_flow-2.0.0b0/fate_flow/entity/
--rw-r--r--   0 tonly      (501) staff       (20)      723 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1353 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/_base.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.936361 fate_flow-2.0.0b0/fate_flow/entity/code/
--rw-r--r--   0 tonly      (501) staff       (20)      685 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/code/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1974 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/code/_api.py
--rw-r--r--   0 tonly      (501) staff       (20)      782 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/code/_process.py
--rw-r--r--   0 tonly      (501) staff       (20)      828 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/code/_schedule.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.936522 fate_flow-2.0.0b0/fate_flow/entity/spec/
--rw-r--r--   0 tonly      (501) staff       (20)      616 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.938342 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/
--rw-r--r--   0 tonly      (501) staff       (20)     1953 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     5545 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_artifact.py
--rw-r--r--   0 tonly      (501) staff       (20)     2561 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_component.py
--rw-r--r--   0 tonly      (501) staff       (20)     1350 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_computing.py
--rw-r--r--   0 tonly      (501) staff       (20)      946 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_device.py
--rw-r--r--   0 tonly      (501) staff       (20)     3950 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_federation.py
--rw-r--r--   0 tonly      (501) staff       (20)     2709 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_job.py
--rw-r--r--   0 tonly      (501) staff       (20)     5186 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_logger.py
--rw-r--r--   0 tonly      (501) staff       (20)      907 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_mlmd.py
--rw-r--r--   0 tonly      (501) staff       (20)     2998 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_output.py
--rw-r--r--   0 tonly      (501) staff       (20)      864 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_party.py
--rw-r--r--   0 tonly      (501) staff       (20)     2506 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_task.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.939085 fate_flow-2.0.0b0/fate_flow/entity/spec/flow/
--rw-r--r--   0 tonly      (501) staff       (20)     1082 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/flow/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1645 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/flow/_model.py
--rw-r--r--   0 tonly      (501) staff       (20)     1576 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/flow/_provider.py
--rw-r--r--   0 tonly      (501) staff       (20)      978 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/flow/_scheduler.py
--rw-r--r--   0 tonly      (501) staff       (20)     1014 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/spec/flow/_storage.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.941257 fate_flow-2.0.0b0/fate_flow/entity/types/
--rw-r--r--   0 tonly      (501) staff       (20)      927 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     6774 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_address.py
--rw-r--r--   0 tonly      (501) staff       (20)      671 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_api.py
--rw-r--r--   0 tonly      (501) staff       (20)     1563 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_artificats.py
--rw-r--r--   0 tonly      (501) staff       (20)      737 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_command.py
--rw-r--r--   0 tonly      (501) staff       (20)     1524 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_engine.py
--rw-r--r--   0 tonly      (501) staff       (20)      923 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_federation.py
--rw-r--r--   0 tonly      (501) staff       (20)      957 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_input.py
--rw-r--r--   0 tonly      (501) staff       (20)     1351 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_instance.py
--rw-r--r--   0 tonly      (501) staff       (20)     1008 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_output.py
--rw-r--r--   0 tonly      (501) staff       (20)     2031 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_permission.py
--rw-r--r--   0 tonly      (501) staff       (20)      778 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_provider.py
--rw-r--r--   0 tonly      (501) staff       (20)     4060 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_status.py
--rw-r--r--   0 tonly      (501) staff       (20)      952 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entity/types/_work.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.941781 fate_flow-2.0.0b0/fate_flow/entrypoint/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entrypoint/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     4242 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entrypoint/cli.py
--rw-r--r--   0 tonly      (501) staff       (20)     1006 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/entrypoint/runner.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.942388 fate_flow-2.0.0b0/fate_flow/errors/
--rw-r--r--   0 tonly      (501) staff       (20)      599 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/errors/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     3974 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/errors/server_error.py
--rw-r--r--   0 tonly      (501) staff       (20)      729 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/errors/zookeeper_error.py
--rw-r--r--   0 tonly      (501) staff       (20)     4538 2023-09-19 04:28:40.000000 fate_flow-2.0.0b0/fate_flow/fate_flow_server.py
--rw-r--r--   0 tonly      (501) staff       (20)       46 2023-09-19 04:31:20.000000 fate_flow-2.0.0b0/fate_flow/fateflow.env
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.942609 fate_flow-2.0.0b0/fate_flow/hook/
--rw-r--r--   0 tonly      (501) staff       (20)     2432 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hook/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.943220 fate_flow-2.0.0b0/fate_flow/hook/common/
--rw-r--r--   0 tonly      (501) staff       (20)      615 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hook/common/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1706 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hook/common/parameters.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.944078 fate_flow-2.0.0b0/fate_flow/hook/flow/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hook/flow/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1684 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hook/flow/client_authentication.py
--rw-r--r--   0 tonly      (501) staff       (20)      882 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hook/flow/permission.py
--rw-r--r--   0 tonly      (501) staff       (20)     3091 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hook/flow/site_authentication.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.944553 fate_flow-2.0.0b0/fate_flow/hub/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/hub/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.944749 fate_flow-2.0.0b0/fate_flow/hub/components_wraps/
--rw-r--r--   0 tonly      (501) staff       (20)      801 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/components_wraps/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.945159 fate_flow-2.0.0b0/fate_flow/hub/components_wraps/fate/
--rw-r--r--   0 tonly      (501) staff       (20)      704 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/components_wraps/fate/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)    25032 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/components_wraps/fate/_wraps.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.945764 fate_flow-2.0.0b0/fate_flow/hub/database/
--rw-r--r--   0 tonly      (501) staff       (20)        0 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/database/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)      990 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/database/mysql.py
--rw-r--r--   0 tonly      (501) staff       (20)      987 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/database/sqlite.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.946072 fate_flow-2.0.0b0/fate_flow/hub/encrypt/
--rw-r--r--   0 tonly      (501) staff       (20)        0 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/encrypt/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1295 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/encrypt/password_encrypt.py
--rw-r--r--   0 tonly      (501) staff       (20)     2762 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/flow_hub.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.946273 fate_flow-2.0.0b0/fate_flow/hub/parser/
--rw-r--r--   0 tonly      (501) staff       (20)     1552 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/parser/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.946812 fate_flow-2.0.0b0/fate_flow/hub/parser/fate/
--rw-r--r--   0 tonly      (501) staff       (20)      759 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/parser/fate/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)    24968 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/parser/fate/_parser.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.947251 fate_flow-2.0.0b0/fate_flow/hub/provider/
--rw-r--r--   0 tonly      (501) staff       (20)      746 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/provider/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1232 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/provider/fate.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.947441 fate_flow-2.0.0b0/fate_flow/hub/scheduler/
--rw-r--r--   0 tonly      (501) staff       (20)     1863 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/scheduler/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.947778 fate_flow-2.0.0b0/fate_flow/hub/scheduler/fate/
--rw-r--r--   0 tonly      (501) staff       (20)      715 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/scheduler/fate/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)    34695 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/hub/scheduler/fate/_scheduler.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.948041 fate_flow-2.0.0b0/fate_flow/manager/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/manager/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.948898 fate_flow-2.0.0b0/fate_flow/manager/components/
--rw-r--r--   0 tonly      (501) staff       (20)      616 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/components/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1945 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/components/base.py
--rw-r--r--   0 tonly      (501) staff       (20)     3883 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/components/component_manager.py
--rw-r--r--   0 tonly      (501) staff       (20)     1633 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/components/download.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.949357 fate_flow-2.0.0b0/fate_flow/manager/container/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/container/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     2136 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/container/docker_manager.py
--rw-r--r--   0 tonly      (501) staff       (20)     4040 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/container/k8s_manager.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.949671 fate_flow-2.0.0b0/fate_flow/manager/data/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/data/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)    13250 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/data/data_manager.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.950055 fate_flow-2.0.0b0/fate_flow/manager/log/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/log/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     3093 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/log/log_manager.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.950399 fate_flow-2.0.0b0/fate_flow/manager/metric/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/metric/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     5558 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/metric/metric_manager.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.950930 fate_flow-2.0.0b0/fate_flow/manager/model/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.951444 fate_flow-2.0.0b0/fate_flow/manager/model/engine/
--rw-r--r--   0 tonly      (501) staff       (20)      810 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/engine/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     5191 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/engine/_mysql.py
--rw-r--r--   0 tonly      (501) staff       (20)     3136 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/engine/_tencent_cos.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.952213 fate_flow-2.0.0b0/fate_flow/manager/model/handel/
--rw-r--r--   0 tonly      (501) staff       (20)      941 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/handel/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     6652 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/handel/_base.py
--rw-r--r--   0 tonly      (501) staff       (20)     2692 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/handel/_file.py
--rw-r--r--   0 tonly      (501) staff       (20)     2517 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/handel/_mysql.py
--rw-r--r--   0 tonly      (501) staff       (20)     2503 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/handel/_tencent_cos.py
--rw-r--r--   0 tonly      (501) staff       (20)     4443 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/model_manager.py
--rw-r--r--   0 tonly      (501) staff       (20)     1180 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/model/model_meta.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.952454 fate_flow-2.0.0b0/fate_flow/manager/pipeline/
--rw-r--r--   0 tonly      (501) staff       (20)        0 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/pipeline/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     3906 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/pipeline/pipeline.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.953643 fate_flow-2.0.0b0/fate_flow/manager/service/
--rw-r--r--   0 tonly      (501) staff       (20)        0 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/service/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     5332 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/service/app_manager.py
--rw-r--r--   0 tonly      (501) staff       (20)     1169 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/service/output_manager.py
--rw-r--r--   0 tonly      (501) staff       (20)     7285 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/service/provider_manager.py
--rw-r--r--   0 tonly      (501) staff       (20)    13862 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/service/resource_manager.py
--rw-r--r--   0 tonly      (501) staff       (20)    18309 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/manager/service/service_manager.py
--rw-r--r--   0 tonly      (501) staff       (20)     6484 2023-09-19 03:09:13.000000 fate_flow-2.0.0b0/fate_flow/manager/service/worker_manager.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.954385 fate_flow-2.0.0b0/fate_flow/operation/
--rw-r--r--   0 tonly      (501) staff       (20)      617 2023-02-10 07:46:12.000000 fate_flow-2.0.0b0/fate_flow/operation/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)    13745 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/operation/base_saver.py
--rw-r--r--   0 tonly      (501) staff       (20)     5507 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/operation/job_saver.py
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/operation/job_tracker.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.954566 fate_flow-2.0.0b0/fate_flow/proto/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/proto/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.955122 fate_flow-2.0.0b0/fate_flow/proto/osx/
--rw-r--r--   0 tonly      (501) staff       (20)      761 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/proto/osx/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     6499 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/proto/osx/osx_pb2.py
--rw-r--r--   0 tonly      (501) staff       (20)     6398 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/proto/osx/osx_pb2_grpc.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.955712 fate_flow-2.0.0b0/fate_flow/proto/rollsite/
--rw-r--r--   0 tonly      (501) staff       (20)      761 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/proto/rollsite/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     8859 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/proto/rollsite/basic_meta_pb2.py
--rw-r--r--   0 tonly      (501) staff       (20)     9559 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/proto/rollsite/proxy_pb2.py
--rw-r--r--   0 tonly      (501) staff       (20)    10154 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/proto/rollsite/proxy_pb2_grpc.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.956857 fate_flow-2.0.0b0/fate_flow/runtime/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/runtime/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     2012 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/runtime/component_provider.py
--rw-r--r--   0 tonly      (501) staff       (20)      190 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/runtime/env.py
--rw-r--r--   0 tonly      (501) staff       (20)     1588 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/runtime/job_default_config.py
--rw-r--r--   0 tonly      (501) staff       (20)     1024 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/runtime/reload_config_base.py
--rw-r--r--   0 tonly      (501) staff       (20)     2302 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/runtime/runtime_config.py
--rw-r--r--   0 tonly      (501) staff       (20)     5681 2023-09-19 04:28:40.000000 fate_flow-2.0.0b0/fate_flow/runtime/system_settings.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.957373 fate_flow-2.0.0b0/fate_flow/scheduler/
--rw-r--r--   0 tonly      (501) staff       (20)     1695 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/scheduler/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     6891 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/scheduler/federated_scheduler.py
--rw-r--r--   0 tonly      (501) staff       (20)     1313 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/scheduler/job_scheduler.py
--rw-r--r--   0 tonly      (501) staff       (20)     1026 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/settings.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.961510 fate_flow-2.0.0b0/fate_flow/utils/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     7292 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/api_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     5167 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/base_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     1626 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/conf_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     2739 2023-02-10 07:46:12.000000 fate_flow-2.0.0b0/fate_flow/utils/cron.py
--rw-r--r--   0 tonly      (501) staff       (20)      812 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/utils/db_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     4110 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/engine_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     2709 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/file_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     6024 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/grpc_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     5409 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/io_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     4376 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/job_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     8179 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/log.py
--rw-r--r--   0 tonly      (501) staff       (20)     5358 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/log_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)      945 2023-03-09 11:15:03.000000 fate_flow-2.0.0b0/fate_flow/utils/object_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     1705 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/password_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     1479 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/permission_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     9168 2023-09-19 03:09:13.000000 fate_flow-2.0.0b0/fate_flow/utils/process_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     1203 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/utils/requests_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     2778 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/schedule_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     1042 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/version.py
--rw-r--r--   0 tonly      (501) staff       (20)    11053 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/wraps_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)     6507 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/utils/xthread.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.962013 fate_flow-2.0.0b0/fate_flow/worker/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/fate_flow/worker/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)      814 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/worker/fate_executor.py
--rw-r--r--   0 tonly      (501) staff       (20)     1033 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/fate_flow/worker/fate_flow_executor.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.918826 fate_flow-2.0.0b0/fate_flow.egg-info/
--rw-r--r--   0 tonly      (501) staff       (20)     1690 2023-09-19 04:32:15.000000 fate_flow-2.0.0b0/fate_flow.egg-info/PKG-INFO
--rw-r--r--   0 tonly      (501) staff       (20)     9275 2023-09-19 04:32:15.000000 fate_flow-2.0.0b0/fate_flow.egg-info/SOURCES.txt
--rw-r--r--   0 tonly      (501) staff       (20)        1 2023-09-19 04:32:15.000000 fate_flow-2.0.0b0/fate_flow.egg-info/dependency_links.txt
--rw-r--r--   0 tonly      (501) staff       (20)       76 2023-09-19 04:32:15.000000 fate_flow-2.0.0b0/fate_flow.egg-info/entry_points.txt
--rw-r--r--   0 tonly      (501) staff       (20)      572 2023-09-19 04:32:15.000000 fate_flow-2.0.0b0/fate_flow.egg-info/requires.txt
--rw-r--r--   0 tonly      (501) staff       (20)       14 2023-09-19 04:32:15.000000 fate_flow-2.0.0b0/fate_flow.egg-info/top_level.txt
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.962179 fate_flow-2.0.0b0/ofx/
--rw-r--r--   0 tonly      (501) staff       (20)      615 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.962542 fate_flow-2.0.0b0/ofx/api/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     1652 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/ofx/api/client.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.963343 fate_flow-2.0.0b0/ofx/api/models/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/models/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     3100 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/ofx/api/models/federated.py
--rw-r--r--   0 tonly      (501) staff       (20)    14222 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/ofx/api/models/resource.py
--rw-r--r--   0 tonly      (501) staff       (20)     1852 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/ofx/api/models/scheduler.py
--rw-r--r--   0 tonly      (501) staff       (20)     3940 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/ofx/api/models/worker.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.963507 fate_flow-2.0.0b0/ofx/api/proto/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-09-15 10:15:49.000000 fate_flow-2.0.0b0/ofx/api/proto/__init__.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.964066 fate_flow-2.0.0b0/ofx/api/proto/osx/
--rw-r--r--   0 tonly      (501) staff       (20)      761 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/proto/osx/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     6499 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/proto/osx/osx_pb2.py
--rw-r--r--   0 tonly      (501) staff       (20)     6398 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/proto/osx/osx_pb2_grpc.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.964767 fate_flow-2.0.0b0/ofx/api/proto/rollsite/
--rw-r--r--   0 tonly      (501) staff       (20)      761 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/proto/rollsite/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     8859 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/proto/rollsite/basic_meta_pb2.py
--rw-r--r--   0 tonly      (501) staff       (20)     9559 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/proto/rollsite/proxy_pb2.py
--rw-r--r--   0 tonly      (501) staff       (20)    10154 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/proto/rollsite/proxy_pb2_grpc.py
-drwxr-xr-x   0 tonly      (501) staff       (20)        0 2023-09-19 04:32:15.965118 fate_flow-2.0.0b0/ofx/api/utils/
--rw-r--r--   0 tonly      (501) staff       (20)      614 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/utils/__init__.py
--rw-r--r--   0 tonly      (501) staff       (20)     3107 2023-05-12 02:53:34.000000 fate_flow-2.0.0b0/ofx/api/utils/grpc_utils.py
--rw-r--r--   0 tonly      (501) staff       (20)       38 2023-09-19 04:32:15.965598 fate_flow-2.0.0b0/setup.cfg
--rw-r--r--   0 tonly      (501) staff       (20)     2704 2023-09-19 03:09:13.000000 fate_flow-2.0.0b0/setup.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.781722 fate_flow-2.1.0/
+-rw-r--r--   0 tonly      (501) staff       (20)     1998 2024-04-03 06:56:24.781441 fate_flow-2.1.0/PKG-INFO
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.717653 fate_flow-2.1.0/fate_flow/
+-rw-r--r--   0 tonly      (501) staff       (20)      659 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)      663 2024-02-29 07:21:57.000000 fate_flow-2.1.0/fate_flow/_info.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.719094 fate_flow-2.1.0/fate_flow/adapter/
+-rw-r--r--   0 tonly      (501) staff       (20)       99 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1254 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/_controller.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2532 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/_loader.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.719681 fate_flow-2.1.0/fate_flow/adapter/bfia/
+-rw-r--r--   0 tonly      (501) staff       (20)      114 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.720389 fate_flow-2.1.0/fate_flow/adapter/bfia/apps/
+-rw-r--r--   0 tonly      (501) staff       (20)       74 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/apps/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5568 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/apps/interconn_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3381 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/apps/platform_app.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.720769 fate_flow-2.1.0/fate_flow/adapter/bfia/bridge/
+-rw-r--r--   0 tonly      (501) staff       (20)       60 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/bridge/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2811 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/bridge/job.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.720991 fate_flow-2.1.0/fate_flow/adapter/bfia/container/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/container/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.721426 fate_flow-2.1.0/fate_flow/adapter/bfia/container/entrypoint/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/container/entrypoint/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2283 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/container/entrypoint/cli.py
+-rw-r--r--   0 tonly      (501) staff       (20)      952 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/container/entrypoint/runner.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.721660 fate_flow-2.1.0/fate_flow/adapter/bfia/container/wraps/
+-rw-r--r--   0 tonly      (501) staff       (20)        0 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/container/wraps/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)    20086 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/container/wraps/wraps.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.722391 fate_flow-2.1.0/fate_flow/adapter/bfia/db/
+-rw-r--r--   0 tonly      (501) staff       (20)       92 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/db/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)      739 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/db/output.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.723483 fate_flow-2.1.0/fate_flow/adapter/bfia/engine_storage/
+-rw-r--r--   0 tonly      (501) staff       (20)     1072 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/engine_storage/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2765 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/engine_storage/client.py
+-rw-r--r--   0 tonly      (501) staff       (20)      162 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/engine_storage/consts.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2345 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/engine_storage/meta.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3584 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/engine_storage/session.py
+-rw-r--r--   0 tonly      (501) staff       (20)     8093 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/engine_storage/table.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1171 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/runtime_config.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.724190 fate_flow-2.1.0/fate_flow/adapter/bfia/scheduler/
+-rw-r--r--   0 tonly      (501) staff       (20)      729 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/scheduler/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3662 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/scheduler/detector.py
+-rw-r--r--   0 tonly      (501) staff       (20)    21470 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/scheduler/scheduler.py
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/settings.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.724789 fate_flow-2.1.0/fate_flow/adapter/bfia/translator/
+-rw-r--r--   0 tonly      (501) staff       (20)      616 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/translator/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1166 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/translator/component_spec.py
+-rw-r--r--   0 tonly      (501) staff       (20)    22049 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/translator/dsl_translator.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.726373 fate_flow-2.1.0/fate_flow/adapter/bfia/wheels/
+-rw-r--r--   0 tonly      (501) staff       (20)        0 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/wheels/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2079 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/wheels/federated.py
+-rw-r--r--   0 tonly      (501) staff       (20)     8783 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/wheels/job.py
+-rw-r--r--   0 tonly      (501) staff       (20)      562 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/wheels/output.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5548 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/wheels/parser.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1267 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/wheels/saver.py
+-rw-r--r--   0 tonly      (501) staff       (20)    10008 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/adapter/bfia/wheels/task.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.727118 fate_flow-2.1.0/fate_flow/apps/
+-rw-r--r--   0 tonly      (501) staff       (20)     5939 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.729470 fate_flow-2.1.0/fate_flow/apps/client/
+-rw-r--r--   0 tonly      (501) staff       (20)      613 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4184 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/client_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4963 2024-02-26 10:11:49.000000 fate_flow-2.1.0/fate_flow/apps/client/data_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)    10327 2024-02-22 07:15:32.000000 fate_flow-2.1.0/fate_flow/apps/client/job_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2490 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/log_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3470 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/model_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)    10360 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/output_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4201 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/permission_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3136 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/provider_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4411 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/server_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1107 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/site_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2749 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/client/table_app.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3195 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/desc.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2923 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/desc_zh.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.729776 fate_flow-2.1.0/fate_flow/apps/partner/
+-rw-r--r--   0 tonly      (501) staff       (20)      652 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/partner/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)    12135 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/partner/partner_app.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.730159 fate_flow-2.1.0/fate_flow/apps/scheduler/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/scheduler/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2754 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/scheduler/scheduler_app.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.730473 fate_flow-2.1.0/fate_flow/apps/worker/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/worker/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     8540 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/apps/worker/worker_app.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.731225 fate_flow-2.1.0/fate_flow/commands/
+-rw-r--r--   0 tonly      (501) staff       (20)        0 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/commands/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     6694 2024-02-26 10:01:08.000000 fate_flow-2.1.0/fate_flow/commands/server_cli.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5601 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/commands/service.py
+-rw-r--r--   0 tonly      (501) staff       (20)    13388 2024-02-26 10:11:09.000000 fate_flow-2.1.0/fate_flow/commands/service.sh
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.731797 fate_flow-2.1.0/fate_flow/components/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/components/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)      892 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/components/__main__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.732216 fate_flow-2.1.0/fate_flow/components/components/
+-rw-r--r--   0 tonly      (501) staff       (20)      713 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/components/components/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2460 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/components/components/download.py
+-rw-r--r--   0 tonly      (501) staff       (20)    14710 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/components/components/upload.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1492 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/components/cpn.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.732614 fate_flow-2.1.0/fate_flow/components/entrypoint/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/components/entrypoint/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4792 2024-02-26 05:55:20.000000 fate_flow-2.1.0/fate_flow/components/entrypoint/cli.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.733860 fate_flow-2.1.0/fate_flow/conf/
+-rw-r--r--   0 tonly      (501) staff       (20)      223 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/conf/casbin_model.conf
+-rw-r--r--   0 tonly      (501) staff       (20)      328 2024-02-22 06:53:13.000000 fate_flow-2.1.0/fate_flow/conf/job_default_config.yaml
+-rw-r--r--   0 tonly      (501) staff       (20)      226 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/conf/permission_casbin_model.conf
+-rw-r--r--   0 tonly      (501) staff       (20)      507 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/conf/pulsar_route_table.yaml
+-rw-r--r--   0 tonly      (501) staff       (20)       80 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/conf/rabbitmq_route_table.yaml
+-rw-r--r--   0 tonly      (501) staff       (20)     2448 2024-02-27 05:22:40.000000 fate_flow-2.1.0/fate_flow/conf/service_conf.yaml
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.735972 fate_flow-2.1.0/fate_flow/controller/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/controller/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     6866 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/controller/federated.py
+-rw-r--r--   0 tonly      (501) staff       (20)    25291 2024-02-22 07:17:06.000000 fate_flow-2.1.0/fate_flow/controller/job.py
+-rw-r--r--   0 tonly      (501) staff       (20)    34090 2024-02-23 06:31:42.000000 fate_flow-2.1.0/fate_flow/controller/parser.py
+-rw-r--r--   0 tonly      (501) staff       (20)    11283 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/controller/permission.py
+-rw-r--r--   0 tonly      (501) staff       (20)    18865 2024-03-05 02:46:06.000000 fate_flow-2.1.0/fate_flow/controller/task.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.738240 fate_flow-2.1.0/fate_flow/db/
+-rw-r--r--   0 tonly      (501) staff       (20)      738 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/db/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)    15211 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/db/base_models.py
+-rw-r--r--   0 tonly      (501) staff       (20)     8075 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/db/casbin_models.py
+-rw-r--r--   0 tonly      (501) staff       (20)     9856 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/db/db_models.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1234 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/db/permission_models.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3178 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/db/schedule_models.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2457 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/db/storage_models.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.738649 fate_flow-2.1.0/fate_flow/engine/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.739862 fate_flow-2.1.0/fate_flow/engine/backend/
+-rw-r--r--   0 tonly      (501) staff       (20)      712 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/backend/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5093 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/backend/_base.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1845 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/backend/_eggroll.py
+-rw-r--r--   0 tonly      (501) staff       (20)     8150 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/backend/_eggroll_deepspeed.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1515 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/backend/_session.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2567 2024-02-23 06:31:42.000000 fate_flow-2.1.0/fate_flow/engine/backend/_spark.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.741065 fate_flow-2.1.0/fate_flow/engine/devices/
+-rw-r--r--   0 tonly      (501) staff       (20)     1859 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/devices/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1179 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/devices/_base.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3076 2024-02-28 07:49:11.000000 fate_flow-2.1.0/fate_flow/engine/devices/container.py
+-rw-r--r--   0 tonly      (501) staff       (20)     9179 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/devices/deepspeed.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3038 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/devices/local.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2974 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/relation_ship.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.742473 fate_flow-2.1.0/fate_flow/engine/storage/
+-rw-r--r--   0 tonly      (501) staff       (20)      889 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5042 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/_abc.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2191 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/_partitioner.py
+-rw-r--r--   0 tonly      (501) staff       (20)    11944 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/_session.py
+-rw-r--r--   0 tonly      (501) staff       (20)    14377 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/_table.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2555 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/_types.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.743538 fate_flow-2.1.0/fate_flow/engine/storage/eggroll/
+-rw-r--r--   0 tonly      (501) staff       (20)      796 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/eggroll/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4355 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/eggroll/_session.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2538 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/eggroll/_table.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.744515 fate_flow-2.1.0/fate_flow/engine/storage/file/
+-rw-r--r--   0 tonly      (501) staff       (20)      790 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/file/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1977 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/file/_session.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4823 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/file/_table.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.745314 fate_flow-2.1.0/fate_flow/engine/storage/hdfs/
+-rw-r--r--   0 tonly      (501) staff       (20)      790 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/hdfs/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2116 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/hdfs/_session.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5589 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/hdfs/_table.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.747075 fate_flow-2.1.0/fate_flow/engine/storage/serdes/
+-rw-r--r--   0 tonly      (501) staff       (20)      994 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/serdes/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)      897 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/serdes/_integer_serdes.py
+-rw-r--r--   0 tonly      (501) staff       (20)      784 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/serdes/_serdes_base.py
+-rw-r--r--   0 tonly      (501) staff       (20)      917 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/serdes/_unrestricted_serdes.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.747860 fate_flow-2.1.0/fate_flow/engine/storage/standalone/
+-rw-r--r--   0 tonly      (501) staff       (20)      802 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/standalone/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3990 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/standalone/_session.py
+-rw-r--r--   0 tonly      (501) staff       (20)    47135 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/standalone/_standalone.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2029 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/engine/storage/standalone/_table.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.748182 fate_flow-2.1.0/fate_flow/entity/
+-rw-r--r--   0 tonly      (501) staff       (20)      723 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1353 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/_base.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.749000 fate_flow-2.1.0/fate_flow/entity/code/
+-rw-r--r--   0 tonly      (501) staff       (20)      685 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/code/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2013 2024-02-21 09:42:57.000000 fate_flow-2.1.0/fate_flow/entity/code/_api.py
+-rw-r--r--   0 tonly      (501) staff       (20)      782 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/code/_process.py
+-rw-r--r--   0 tonly      (501) staff       (20)      828 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/code/_schedule.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.749163 fate_flow-2.1.0/fate_flow/entity/spec/
+-rw-r--r--   0 tonly      (501) staff       (20)      616 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.750962 fate_flow-2.1.0/fate_flow/entity/spec/dag/
+-rw-r--r--   0 tonly      (501) staff       (20)     1976 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5110 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_artifact.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2688 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_component.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1602 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_computing.py
+-rw-r--r--   0 tonly      (501) staff       (20)      858 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_device.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3950 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_federation.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2841 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_job.py
+-rw-r--r--   0 tonly      (501) staff       (20)     6267 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_logger.py
+-rw-r--r--   0 tonly      (501) staff       (20)      907 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_mlmd.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3704 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_output.py
+-rw-r--r--   0 tonly      (501) staff       (20)      864 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_party.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2506 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/dag/_task.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.751850 fate_flow-2.1.0/fate_flow/entity/spec/flow/
+-rw-r--r--   0 tonly      (501) staff       (20)     1400 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/flow/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1645 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/flow/_model.py
+-rw-r--r--   0 tonly      (501) staff       (20)      735 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/flow/_protocol.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1576 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/flow/_provider.py
+-rw-r--r--   0 tonly      (501) staff       (20)      978 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/flow/_scheduler.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1014 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/spec/flow/_storage.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.754066 fate_flow-2.1.0/fate_flow/entity/types/
+-rw-r--r--   0 tonly      (501) staff       (20)      927 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     6774 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_address.py
+-rw-r--r--   0 tonly      (501) staff       (20)      730 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_api.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1563 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_artificats.py
+-rw-r--r--   0 tonly      (501) staff       (20)      737 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_command.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1524 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_engine.py
+-rw-r--r--   0 tonly      (501) staff       (20)      990 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_federation.py
+-rw-r--r--   0 tonly      (501) staff       (20)      957 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_input.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1351 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_instance.py
+-rw-r--r--   0 tonly      (501) staff       (20)      853 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_output.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2031 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_permission.py
+-rw-r--r--   0 tonly      (501) staff       (20)      778 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_provider.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4120 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_status.py
+-rw-r--r--   0 tonly      (501) staff       (20)      979 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/entity/types/_work.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.754553 fate_flow-2.1.0/fate_flow/errors/
+-rw-r--r--   0 tonly      (501) staff       (20)      599 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/errors/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3974 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/errors/server_error.py
+-rw-r--r--   0 tonly      (501) staff       (20)      729 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/errors/zookeeper_error.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4599 2024-04-03 06:50:59.000000 fate_flow-2.1.0/fate_flow/fate_flow_server.py
+-rw-r--r--   0 tonly      (501) staff       (20)       37 2024-04-03 06:52:54.000000 fate_flow-2.1.0/fate_flow/fateflow.env
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.754720 fate_flow-2.1.0/fate_flow/hook/
+-rw-r--r--   0 tonly      (501) staff       (20)     2432 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hook/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.755046 fate_flow-2.1.0/fate_flow/hook/common/
+-rw-r--r--   0 tonly      (501) staff       (20)      615 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hook/common/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1706 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hook/common/parameters.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.755644 fate_flow-2.1.0/fate_flow/hook/flow/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hook/flow/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1680 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hook/flow/client_authentication.py
+-rw-r--r--   0 tonly      (501) staff       (20)      871 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hook/flow/permission.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3087 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hook/flow/site_authentication.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.755923 fate_flow-2.1.0/fate_flow/hub/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.756057 fate_flow-2.1.0/fate_flow/hub/components_wraps/
+-rw-r--r--   0 tonly      (501) staff       (20)      801 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/components_wraps/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.756326 fate_flow-2.1.0/fate_flow/hub/components_wraps/fate/
+-rw-r--r--   0 tonly      (501) staff       (20)      704 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/components_wraps/fate/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)    28181 2024-02-26 05:36:06.000000 fate_flow-2.1.0/fate_flow/hub/components_wraps/fate/_wraps.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.757001 fate_flow-2.1.0/fate_flow/hub/database/
+-rw-r--r--   0 tonly      (501) staff       (20)        0 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/database/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)      990 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/database/mysql.py
+-rw-r--r--   0 tonly      (501) staff       (20)      987 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/database/sqlite.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.757238 fate_flow-2.1.0/fate_flow/hub/encrypt/
+-rw-r--r--   0 tonly      (501) staff       (20)        0 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/encrypt/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1295 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/encrypt/password_encrypt.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2552 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/flow_hub.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.757676 fate_flow-2.1.0/fate_flow/hub/provider/
+-rw-r--r--   0 tonly      (501) staff       (20)      862 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/provider/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1415 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/provider/docker.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1666 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/hub/provider/local.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.757827 fate_flow-2.1.0/fate_flow/manager/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.758572 fate_flow-2.1.0/fate_flow/manager/components/
+-rw-r--r--   0 tonly      (501) staff       (20)      616 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/components/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2067 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/components/base.py
+-rw-r--r--   0 tonly      (501) staff       (20)     6485 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/components/component_manager.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1603 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/components/download.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.759320 fate_flow-2.1.0/fate_flow/manager/container/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/container/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2220 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/container/docker_manager.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4113 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/container/k8s_manager.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.763951 fate_flow-2.1.0/fate_flow/manager/operation/
+-rw-r--r--   0 tonly      (501) staff       (20)      617 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/operation/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)    14220 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/operation/base_saver.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5825 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/operation/job_saver.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.764624 fate_flow-2.1.0/fate_flow/manager/outputs/
+-rw-r--r--   0 tonly      (501) staff       (20)        0 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)    13756 2024-02-29 08:40:07.000000 fate_flow-2.1.0/fate_flow/manager/outputs/data.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3109 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/log.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5558 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/metric.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.765079 fate_flow-2.1.0/fate_flow/manager/outputs/model/
+-rw-r--r--   0 tonly      (501) staff       (20)      795 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.765566 fate_flow-2.1.0/fate_flow/manager/outputs/model/engine/
+-rw-r--r--   0 tonly      (501) staff       (20)      826 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/engine/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5191 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/engine/_mysql.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3136 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/engine/_tencent_cos.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.766428 fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/
+-rw-r--r--   0 tonly      (501) staff       (20)      972 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     6649 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/_base.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2700 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/_file.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2523 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/_mysql.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2519 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/_tencent_cos.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4459 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/model_manager.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1180 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/outputs/model/model_meta.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.766573 fate_flow-2.1.0/fate_flow/manager/permission/
+-rw-r--r--   0 tonly      (501) staff       (20)        0 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/permission/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.766764 fate_flow-2.1.0/fate_flow/manager/pipeline/
+-rw-r--r--   0 tonly      (501) staff       (20)        0 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/pipeline/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2745 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/pipeline/pipeline.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.768189 fate_flow-2.1.0/fate_flow/manager/service/
+-rw-r--r--   0 tonly      (501) staff       (20)        0 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/service/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5332 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/service/app_manager.py
+-rw-r--r--   0 tonly      (501) staff       (20)      980 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/service/config_manager.py
+-rw-r--r--   0 tonly      (501) staff       (20)     8665 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/service/provider_manager.py
+-rw-r--r--   0 tonly      (501) staff       (20)    14252 2024-02-21 09:50:17.000000 fate_flow-2.1.0/fate_flow/manager/service/resource_manager.py
+-rw-r--r--   0 tonly      (501) staff       (20)    18498 2024-02-20 06:52:57.000000 fate_flow-2.1.0/fate_flow/manager/service/service_manager.py
+-rw-r--r--   0 tonly      (501) staff       (20)     7396 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/service/worker_manager.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.768983 fate_flow-2.1.0/fate_flow/manager/worker/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/worker/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2058 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/worker/deepspeed_download_model.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1895 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/worker/fate_ds_executor.py
+-rw-r--r--   0 tonly      (501) staff       (20)      814 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/worker/fate_executor.py
+-rw-r--r--   0 tonly      (501) staff       (20)      937 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/manager/worker/fate_flow_executor.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.769132 fate_flow-2.1.0/fate_flow/proto/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/proto/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.769729 fate_flow-2.1.0/fate_flow/proto/rollsite/
+-rw-r--r--   0 tonly      (501) staff       (20)      761 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/proto/rollsite/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     8859 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/proto/rollsite/basic_meta_pb2.py
+-rw-r--r--   0 tonly      (501) staff       (20)     9559 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/proto/rollsite/proxy_pb2.py
+-rw-r--r--   0 tonly      (501) staff       (20)    10154 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/proto/rollsite/proxy_pb2_grpc.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.770849 fate_flow-2.1.0/fate_flow/runtime/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/runtime/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2012 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/runtime/component_provider.py
+-rw-r--r--   0 tonly      (501) staff       (20)      190 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/runtime/env.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1592 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/runtime/job_default_config.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1024 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/runtime/reload_config_base.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2081 2024-02-26 10:11:18.000000 fate_flow-2.1.0/fate_flow/runtime/runtime_config.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5762 2024-02-20 08:46:46.000000 fate_flow-2.1.0/fate_flow/runtime/system_settings.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.771582 fate_flow-2.1.0/fate_flow/scheduler/
+-rw-r--r--   0 tonly      (501) staff       (20)     1571 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/scheduler/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)    12955 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/scheduler/detector.py
+-rw-r--r--   0 tonly      (501) staff       (20)    31599 2024-02-22 08:46:10.000000 fate_flow-2.1.0/fate_flow/scheduler/scheduler.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1063 2024-02-26 10:11:49.000000 fate_flow-2.1.0/fate_flow/settings.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.776624 fate_flow-2.1.0/fate_flow/utils/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     7375 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/api_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5139 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/base_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1706 2024-02-20 06:32:46.000000 fate_flow-2.1.0/fate_flow/utils/conf_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2739 2023-12-21 09:45:57.000000 fate_flow-2.1.0/fate_flow/utils/cron.py
+-rw-r--r--   0 tonly      (501) staff       (20)      812 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/db_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4110 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/engine_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2827 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/file_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     4142 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/grpc_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5409 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/io_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     6781 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/job_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     8179 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/log.py
+-rw-r--r--   0 tonly      (501) staff       (20)     5369 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/log_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)      945 2023-12-21 09:45:57.000000 fate_flow-2.1.0/fate_flow/utils/object_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1705 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/password_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2610 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/permission_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     9118 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/process_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1203 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/requests_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2778 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/schedule_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1043 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/version.py
+-rw-r--r--   0 tonly      (501) staff       (20)    10632 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/wraps_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)     6507 2024-02-20 02:58:11.000000 fate_flow-2.1.0/fate_flow/utils/xthread.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.718550 fate_flow-2.1.0/fate_flow.egg-info/
+-rw-r--r--   0 tonly      (501) staff       (20)     1998 2024-04-03 06:56:24.000000 fate_flow-2.1.0/fate_flow.egg-info/PKG-INFO
+-rw-r--r--   0 tonly      (501) staff       (20)    11070 2024-04-03 06:56:24.000000 fate_flow-2.1.0/fate_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 tonly      (501) staff       (20)        1 2024-04-03 06:56:24.000000 fate_flow-2.1.0/fate_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 tonly      (501) staff       (20)       77 2024-04-03 06:56:24.000000 fate_flow-2.1.0/fate_flow.egg-info/entry_points.txt
+-rw-r--r--   0 tonly      (501) staff       (20)      467 2024-04-03 06:56:24.000000 fate_flow-2.1.0/fate_flow.egg-info/requires.txt
+-rw-r--r--   0 tonly      (501) staff       (20)       14 2024-04-03 06:56:24.000000 fate_flow-2.1.0/fate_flow.egg-info/top_level.txt
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.776777 fate_flow-2.1.0/ofx/
+-rw-r--r--   0 tonly      (501) staff       (20)      615 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.777333 fate_flow-2.1.0/ofx/api/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3824 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/client.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1558 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/entity.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.777484 fate_flow-2.1.0/ofx/api/models/
+-rw-r--r--   0 tonly      (501) staff       (20)      686 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.778305 fate_flow-2.1.0/ofx/api/models/bfia/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/bfia/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1923 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/bfia/federated.py
+-rw-r--r--   0 tonly      (501) staff       (20)     7927 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/bfia/resource.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1597 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/bfia/scheduler.py
+-rw-r--r--   0 tonly      (501) staff       (20)      952 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/bfia/worker.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.779196 fate_flow-2.1.0/ofx/api/models/fate_flow/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/fate_flow/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3100 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/fate_flow/federated.py
+-rw-r--r--   0 tonly      (501) staff       (20)    12834 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/fate_flow/resource.py
+-rw-r--r--   0 tonly      (501) staff       (20)     1852 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/fate_flow/scheduler.py
+-rw-r--r--   0 tonly      (501) staff       (20)     3940 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/models/fate_flow/worker.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.779412 fate_flow-2.1.0/ofx/api/proto/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/proto/__init__.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.780444 fate_flow-2.1.0/ofx/api/proto/rollsite/
+-rw-r--r--   0 tonly      (501) staff       (20)      761 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/proto/rollsite/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     8859 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/proto/rollsite/basic_meta_pb2.py
+-rw-r--r--   0 tonly      (501) staff       (20)     9559 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/proto/rollsite/proxy_pb2.py
+-rw-r--r--   0 tonly      (501) staff       (20)    10154 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/proto/rollsite/proxy_pb2_grpc.py
+drwxr-xr-x   0 tonly      (501) staff       (20)        0 2024-04-03 06:56:24.781015 fate_flow-2.1.0/ofx/api/utils/
+-rw-r--r--   0 tonly      (501) staff       (20)      614 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/utils/__init__.py
+-rw-r--r--   0 tonly      (501) staff       (20)     2237 2024-02-20 02:58:11.000000 fate_flow-2.1.0/ofx/api/utils/grpc_utils.py
+-rw-r--r--   0 tonly      (501) staff       (20)       38 2024-04-03 06:56:24.781797 fate_flow-2.1.0/setup.cfg
+-rw-r--r--   0 tonly      (501) staff       (20)     2572 2024-02-20 02:58:11.000000 fate_flow-2.1.0/setup.py
```

### Comparing `fate_flow-2.0.0b0/PKG-INFO` & `fate_flow-2.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 Metadata-Version: 2.1
 Name: fate_flow
-Version: 2.0.0b0
+Version: 2.1.0
+Summary: UNKNOWN
 Home-page: https://fate.fedai.org/
 Author: FederatedAI
 Author-email: contact@FedAI.org
 License: Apache-2.0 License
+Description: [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![CodeStyle](https://img.shields.io/badge/Check%20Style-Google-brightgreen)](https://checkstyle.sourceforge.io/google_style.html) [![Style](https://img.shields.io/badge/Check%20Style-Black-black)](https://checkstyle.sourceforge.io/google_style.html)
+        
+        [中文](./README.zh.md)
+        
+        FATE Flow is a multi-party federated task security scheduling platform for federated learning end-to-end pipeline
+        
+        - [Shared-State Scheduling Architecture](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/41684.pdf)
+        - Secure Multi-Party Communication Across Data Centers
+        
+        Providing production-level service capabilities:
+        
+        - Data Access
+        - Component Registry
+        - Federated Job&Task Scheduling
+        - Multi-Party Resource Coordination
+        - Data Flow Tracking
+        - Real-Time Job Monitoring
+        - Multi-Party Federated Model Registry
+        - Multi-Party Cooperation Authority Management
+        - High Availability
+        - CLI, REST API, Python API
+        
+        ## Deployment
+        
+        Please refer to [FATE](https://github.com/FederatedAI/FATE)
+        
+        ## Documentation
+        
+        The official FATE Flow documentation is here [https://federatedai.github.io/FATE-Flow/latest/](https://federatedai.github.io/FATE-Flow/latest/)
+        
+        ## License
+        [Apache License 2.0](LICENSE)
+        
 Keywords: federated learning scheduler
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rabbitmq
 Provides-Extra: pulsar
 Provides-Extra: spark
 Provides-Extra: eggroll
-Provides-Extra: all
-
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![CodeStyle](https://img.shields.io/badge/Check%20Style-Google-brightgreen)](https://checkstyle.sourceforge.io/google_style.html) [![Style](https://img.shields.io/badge/Check%20Style-Black-black)](https://checkstyle.sourceforge.io/google_style.html)
-
-[中文](./README.zh.md)
-
-FATE Flow is a multi-party federated task security scheduling platform for federated learning end-to-end pipeline
-
-- [Shared-State Scheduling Architecture](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/41684.pdf)
-- Secure Multi-Party Communication Across Data Centers
-
-Providing production-level service capabilities:
-
-- Data Access
-- Component Registry
-- Federated Job&Task Scheduling
-- Multi-Party Resource Coordination
-- Data Flow Tracking
-- Real-Time Job Monitoring
-- Multi-Party Federated Model Registry
-- Multi-Party Cooperation Authority Management
-- High Availability
-- CLI, REST API, Python API
-
-## Deployment
-
-Please refer to [FATE](https://github.com/FederatedAI/FATE)
-
-## Documentation
-
-The official FATE Flow documentation is here [https://federatedai.github.io/FATE-Flow/latest/](https://federatedai.github.io/FATE-Flow/latest/)
-
-## License
-[Apache License 2.0](LICENSE)
+Provides-Extra: fate_flow
```

### Comparing `fate_flow-2.0.0b0/fate_flow/__init__.py` & `fate_flow-2.1.0/fate_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/_info.py` & `fate_flow-2.1.0/fate_flow/_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-__version__ = "2.0.0-beta"
+__version__ = "2.1.0"
 __provider__ = "fate_flow"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/__init__.py` & `fate_flow-2.1.0/fate_flow/apps/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,47 +20,52 @@
 
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 
 from flask import Blueprint, Flask, request
 from werkzeug.wrappers.request import Request
 
-from fate_flow.controller.app_controller import PermissionController
+from fate_flow.controller.permission import PermissionController
 from fate_flow.entity.code import ReturnCode
 from fate_flow.hook import HookManager
 from fate_flow.hook.common.parameters import AuthenticationParameters
 from fate_flow.runtime.runtime_config import RuntimeConfig
 from fate_flow.runtime.system_settings import API_VERSION, CLIENT_AUTHENTICATION, SITE_AUTHENTICATION, \
-    ADMIN_PAGE, PARTY_ID, INTERCONN_API_VERSION
+    ADMIN_PAGE, PARTY_ID
 from fate_flow.utils.api_utils import API
 from fate_flow.utils.base_utils import CustomJSONEncoder
 
 
 __all__ = ['app']
 
 app_list = ["client", "partner", "scheduler", "worker"]
-interop_app_list = ["interop"]
 
 Request.json = property(lambda self: self.get_json(force=True, silent=True))
 
 app = Flask(__name__)
 app.url_map.strict_slashes = False
 app.errorhandler(422)(API.Output.args_error_response)
 app.errorhandler(Exception)(API.Output.server_error_response)
 app.json_provider_class = CustomJSONEncoder
 
 
 def search_pages_path(pages_dir):
     return [path for path in pages_dir.glob('*_app.py') if not path.name.startswith('.')]
 
 
-def register_page(page_path, func=None, prefix=API_VERSION):
+def get_app_module(page_path):
     page_name = page_path.stem.rstrip('app').rstrip("_")
-    module_name = '.'.join(page_path.parts[page_path.parts.index('apps')-1:-1] + (page_name, ))
+    module_name = '.'.join(page_path.parts[page_path.parts.index('fate_flow')+2:-1] + (page_name, ))
+    return module_name
+
 
+def register_page(page_path, func=None, prefix=API_VERSION):
+    page_name = page_path.stem.rstrip('app').rstrip("_")
+    fate_flow_index = len(page_path.parts) - 1 - page_path.parts[::-1].index("fate_flow")
+    module_name = '.'.join(page_path.parts[fate_flow_index:-1] + (page_name, ))
     spec = spec_from_file_location(module_name, page_path)
     page = module_from_spec(spec)
     page.app = app
     page.manager = Blueprint(page_name, module_name)
     rule_methods_list = []
 
     # rewrite blueprint route to get rule_list
@@ -111,16 +116,20 @@
     before_request_func = {
         "client": client_authentication_before_request,
         "partner": site_authentication_before_request,
         "scheduler": site_authentication_before_request
     }
     for key in app_list:
         urls_dict[key] = [register_page(path, before_request_func.get(key)) for path in search_pages_path(Path(__file__).parent / key)]
-    for key in interop_app_list:
-        urls_dict[key] = [register_page(path, prefix=INTERCONN_API_VERSION) for path in search_pages_path(Path(__file__).parent / key)]
+    # adapter extend apps
+    try:
+        from fate_flow.adapter import load_adapter_apps
+        urls_dict.update(load_adapter_apps(register_page, search_pages_path))
+    except:
+        pass
     if CLIENT_AUTHENTICATION or SITE_AUTHENTICATION:
         _init_permission_group(urls=urls_dict)
 
 
 def _init_permission_group(urls: dict):
     for role, role_items in urls.items():
         super_role = "super_" + role
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/__init__.py` & `fate_flow-2.1.0/fate_flow/apps/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/client_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/client_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     return API.Output.json(data={"status": status})
 
 
 @manager.route('/client/query', methods=['GET'])
 @API.Input.params(app_id=fields.String(required=False), desc=APP_ID)
 @API.Input.params(app_name=fields.String(required=False), desc=APP_NAME)
 def query_client_app(app_id=None, app_name=None):
-    apps = AppManager.query_app(app_id=app_id, app_name=app_name, app_type=AppType.CLIENT)
+    apps = AppManager.query_app(app_id=app_id, app_name=app_name)
     return API.Output.json(code=ReturnCode.Base.SUCCESS, message="success", data=[app.to_human_model_dict() for app in apps])
 
 
 @manager.route('/site/create', methods=['POST'])
 @API.Input.json(party_id=fields.String(required=True), desc=PARTY_ID)
 def create_site_app(party_id):
     data = AppManager.create_app(app_name=party_id, app_type=AppType.SITE)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/data_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/data_app.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,39 +9,72 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-from webargs import fields
+import json
+import os.path
 
+from webargs import fields
+from flask import request
 from fate_flow.apps.desc import SERVER_FILE_PATH, HEAD, PARTITIONS, META, EXTEND_SID, NAMESPACE, NAME, DATA_WAREHOUSE, \
     DROP, SITE_NAME
 from fate_flow.engine import storage
 from fate_flow.manager.components.component_manager import ComponentManager
-from fate_flow.manager.data.data_manager import DataManager
+from fate_flow.manager.outputs.data import DataManager
+from fate_flow.settings import UPLOAD_DATA_HOME
 from fate_flow.utils.api_utils import API
-from fate_flow.errors.server_error import NoFoundTable
+from fate_flow.errors.server_error import NoFoundTable, NoFoundFile
 
 page_name = "data"
 
 
 @manager.route('/component/upload', methods=['POST'])
 @API.Input.json(file=fields.String(required=True), desc=SERVER_FILE_PATH)
 @API.Input.json(head=fields.Bool(required=True), desc=HEAD)
 @API.Input.json(partitions=fields.Integer(required=True), desc=PARTITIONS)
 @API.Input.json(meta=fields.Dict(required=True), desc=META)
 @API.Input.json(extend_sid=fields.Bool(required=False), desc=EXTEND_SID)
 @API.Input.json(namespace=fields.String(required=False), desc=NAMESPACE)
 @API.Input.json(name=fields.String(required=False), desc=NAME)
 def upload_data(file, head, partitions, meta, namespace=None, name=None, extend_sid=False):
-    result = ComponentManager.upload(
-        file=file, head=head, partitions=partitions, meta=meta, namespace=namespace, name=name, extend_sid=extend_sid
+    if not os.path.isabs(file):
+        if UPLOAD_DATA_HOME:
+            file = os.path.join(UPLOAD_DATA_HOME, file)
+    if namespace and name:
+        result = ComponentManager.upload_dataframe(
+            file=file, head=head, partitions=partitions, meta=meta, namespace=namespace, name=name, extend_sid=extend_sid
+        )
+    else:
+        result = ComponentManager.upload(
+            file=file, head=head, partitions=partitions, meta=meta, namespace=namespace, name=name,
+            extend_sid=extend_sid
+        )
+    return API.Output.json(**result)
+
+
+@manager.route('/component/upload/file', methods=['POST'])
+@API.Input.form(head=fields.Bool(required=True), desc=HEAD)
+@API.Input.form(partitions=fields.Integer(required=True), desc=PARTITIONS)
+@API.Input.form(meta=fields.String(required=True), desc=META)
+@API.Input.form(extend_sid=fields.Bool(required=False), desc=EXTEND_SID)
+@API.Input.form(namespace=fields.String(required=False), desc=NAMESPACE)
+@API.Input.form(name=fields.String(required=False), desc=NAME)
+def upload_file(head, partitions, meta, namespace=None, name=None, extend_sid=False):
+
+    file = request.files.get('file')
+    if not file:
+        raise NoFoundFile()
+    result = ComponentManager.upload_file(
+        file=file, head=head, partitions=partitions, meta=json.loads(meta), namespace=namespace, name=name,
+        extend_sid=extend_sid
     )
+
     return API.Output.json(**result)
 
 
 @manager.route('/component/download', methods=['POST'])
 @API.Input.json(name=fields.String(required=True), desc=NAME)
 @API.Input.json(namespace=fields.String(required=True), desc=NAMESPACE)
 @API.Input.json(path=fields.String(required=False), desc=SERVER_FILE_PATH)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/job_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/job_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,47 +17,72 @@
 import os
 import tarfile
 
 from webargs import fields
 
 from fate_flow.apps.desc import DAG_SCHEMA, USER_NAME, JOB_ID, ROLE, PARTY_ID, STATUS, LIMIT, PAGE, PARTNER, ORDER_BY, \
     ORDER, DESCRIPTION, TASK_NAME, TASK_ID, TASK_VERSION, NODES
-from fate_flow.controller.job_controller import JobController
+from fate_flow.controller.job import JobController
 from fate_flow.entity.code import ReturnCode
+from fate_flow.entity.spec.dag import DAGSchema
+from fate_flow.entity.spec.flow import SubmitJobInput, QueryJobInput, StopJobInput, QueryTaskInput
+from fate_flow.entity.types import PROTOCOL
 from fate_flow.errors.server_error import NoFoundJob, NoFoundTask, FileNoFound
+from fate_flow.manager.operation.job_saver import JobSaver
 from fate_flow.utils import job_utils
 from fate_flow.utils.api_utils import API
 from fate_flow.manager.pipeline import pipeline as pipeline_manager
 
 
 @manager.route('/submit', methods=['POST'])
 @API.Input.json(dag_schema=fields.Dict(required=True), desc=DAG_SCHEMA)
 @API.Input.headers(user_name=fields.String(required=False), desc=USER_NAME)
 def submit_job(dag_schema, user_name=None):
-    submit_result = JobController.request_create_job(dag_schema, user_name)
+    dag_schema = DAGSchema(**dag_schema)
+    if dag_schema.kind == PROTOCOL.FATE_FLOW:
+        submit_result = JobController.request_create_job(dag_schema, user_name)
+    else:
+        from fate_flow.adapter import AdapterJobController
+        submit_result = AdapterJobController(dag_schema.kind).create_job(SubmitJobInput(dag_schema=dag_schema)).dict()
     return API.Output.json(**submit_result)
 
 
 @manager.route('/query', methods=['GET'])
 @API.Input.params(job_id=fields.String(required=False), desc=JOB_ID)
 @API.Input.params(role=fields.String(required=False), desc=ROLE)
 @API.Input.params(party_id=fields.String(required=False), desc=PARTY_ID)
 @API.Input.params(status=fields.String(required=False), desc=STATUS)
 @API.Input.headers(user_name=fields.String(required=False), desc=USER_NAME)
 def query_job(job_id=None, role=None, party_id=None, status=None, user_name=None):
     jobs = JobController.query_job(job_id=job_id, role=role, party_id=party_id, status=status, user_name=user_name)
     if not jobs:
         return API.Output.fate_flow_exception(NoFoundJob(job_id=job_id, role=role, party_id=party_id, status=status))
+    kind = jobs[0].f_protocol
+
+    if kind != PROTOCOL.FATE_FLOW:
+        from fate_flow.adapter import AdapterJobController
+        jobs = AdapterJobController(kind).query_job(QueryJobInput(jobs=jobs)).jobs
+
     return API.Output.json(data=[job.to_human_model_dict() for job in jobs])
 
 
 @manager.route('/stop', methods=['POST'])
 @API.Input.json(job_id=fields.String(required=True), desc=JOB_ID)
 def request_stop_job(job_id=None):
-    stop_result = JobController.request_stop_job(job_id=job_id)
+    jobs = JobSaver.query_job(job_id=job_id)
+    if not jobs:
+        raise NoFoundJob(job_id=job_id)
+    kind = jobs[0].f_protocol
+
+    if kind != PROTOCOL.FATE_FLOW:
+        from fate_flow.adapter import AdapterJobController
+        stop_result = AdapterJobController(kind).stop_job(StopJobInput(job_id=job_id)).dict()
+
+    else:
+        stop_result = JobController.request_stop_job(job_id, jobs=jobs)
     return API.Output.json(**stop_result)
 
 
 @manager.route('/rerun', methods=['POST'])
 @API.Input.json(job_id=fields.String(required=True), desc=JOB_ID)
 def request_rerun_job(job_id=None):
     jobs = JobController.query_job(job_id=job_id)
@@ -94,19 +119,24 @@
 @API.Input.params(party_id=fields.String(required=False), desc=PARTY_ID)
 @API.Input.params(status=fields.String(required=False), desc=STATUS)
 @API.Input.params(task_name=fields.String(required=False), desc=TASK_NAME)
 @API.Input.params(task_id=fields.String(required=False), desc=TASK_ID)
 @API.Input.params(task_version=fields.Integer(required=False), desc=TASK_VERSION)
 def query_task(job_id=None, role=None, party_id=None, status=None, task_name=None, task_id=None, task_version=None):
     tasks = JobController.query_tasks(job_id=job_id, role=role, party_id=party_id, status=status, task_name=task_name,
-                                      task_id=task_id, task_version=task_version)
+                                      task_id=task_id, task_version=task_version, ignore_protocol=True)
     if not tasks:
         return API.Output.fate_flow_exception(NoFoundTask())
-    return API.Output.json(code=ReturnCode.Base.SUCCESS, message="success",
-                           data=[task.to_human_model_dict() for task in tasks])
+
+    kind = tasks[0].f_protocol
+    if kind != PROTOCOL.FATE_FLOW:
+        from fate_flow.adapter import AdapterJobController
+        tasks = AdapterJobController(kind).query_task(QueryTaskInput(tasks=tasks)).tasks
+
+    return API.Output.json(data=[task.to_human_model_dict() for task in tasks])
 
 
 @manager.route('/task/list/query', methods=['GET'])
 @API.Input.params(limit=fields.Integer(required=False), desc=LIMIT)
 @API.Input.params(page=fields.Integer(required=False), desc=PAGE)
 @API.Input.params(job_id=fields.String(required=False), desc=JOB_ID)
 @API.Input.params(role=fields.String(required=False), desc=ROLE)
@@ -152,14 +182,23 @@
 @manager.route('/clean', methods=['POST'])
 @API.Input.json(job_id=fields.String(required=True), desc=JOB_ID)
 def clean_job(job_id):
     JobController.clean_job(job_id=job_id)
     return API.Output.json()
 
 
+@manager.route('/data/view', methods=['GET'])
+@API.Input.params(job_id=fields.String(required=True), desc=JOB_ID)
+@API.Input.params(role=fields.String(required=True), desc=ROLE)
+@API.Input.params(party_id=fields.String(required=True), desc=PARTY_ID)
+def data_view(job_id, role, party_id):
+    data = JobController.data_view(job_id, role, party_id)
+    return API.Output.json(data=data)
+
+
 @manager.route('/notes/add', methods=['POST'])
 @API.Input.json(job_id=fields.String(required=True), desc=JOB_ID)
 @API.Input.json(role=fields.String(required=True), desc=ROLE)
 @API.Input.json(party_id=fields.String(required=True), desc=PARTY_ID)
 @API.Input.json(notes=fields.String(required=True), desc=NODES)
 def add_notes(job_id, role, party_id, notes):
     JobController.add_notes(job_id=job_id, role=role, party_id=party_id, notes=notes)
@@ -169,10 +208,10 @@
 @manager.route('/dag/dependency', methods=['GET'])
 @API.Input.params(job_id=fields.String(required=True), desc=JOB_ID)
 @API.Input.params(role=fields.String(required=True), desc=ROLE)
 @API.Input.params(party_id=fields.String(required=True), desc=PARTY_ID)
 def dag_dependency(job_id, role, party_id):
     jobs = JobController.query_job(job_id=job_id, role=role, party_id=party_id)
     if not jobs:
-        return API.Output.fate_flow_exception(NoFoundJob(job_id=job_id))
+        return API.Output.fate_flow_exception(NoFoundJob(job_id=job_id, role=role, party_id=party_id))
     data = pipeline_manager.pipeline_dag_dependency(jobs[0])
     return API.Output.json(data=data)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/log_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/log_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from webargs import fields
 
 from fate_flow.apps.desc import LOG_TYPE, JOB_ID, ROLE, PARTY_ID, TASK_NAME, INSTANCE_ID, BEGIN, END
-from fate_flow.manager.log.log_manager import LogManager
+from fate_flow.manager.outputs.log import LogManager
 from fate_flow.utils.api_utils import API
 from fate_flow.utils.wraps_utils import cluster_route
 
 
 @manager.route('/count', methods=['GET'])
 @API.Input.params(log_type=fields.String(required=True), desc=LOG_TYPE)
 @API.Input.params(job_id=fields.String(required=True), desc=JOB_ID)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/model_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/model_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from tempfile import TemporaryDirectory
 
 from flask import request
 from webargs import fields
 
 from fate_flow.apps.desc import MODEL_ID, MODEL_VERSION, PARTY_ID, ROLE, SERVER_DIR_PATH, TASK_NAME, OUTPUT_KEY
 from fate_flow.errors.server_error import NoFoundFile
-from fate_flow.manager.model.model_manager import PipelinedModel
+from fate_flow.manager.outputs.model import PipelinedModel
 from fate_flow.utils.api_utils import API
 
 
 @manager.route('/load', methods=['POST'])
 def load():
     # todo:
     return API.Output.json()
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/output_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/output_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from webargs import fields
 
 from fate_flow.apps.desc import JOB_ID, ROLE, PARTY_ID, TASK_NAME, FILTERS, OUTPUT_KEY
 from fate_flow.entity.code import ReturnCode
+from fate_flow.entity.types import PROTOCOL
 from fate_flow.errors.server_error import NoFoundTask
-from fate_flow.manager.data.data_manager import DataManager
-from fate_flow.manager.model.model_manager import PipelinedModel
-from fate_flow.manager.metric.metric_manager import OutputMetric
-from fate_flow.operation.job_saver import JobSaver
+from fate_flow.manager.outputs.data import DataManager
+from fate_flow.manager.outputs.model import PipelinedModel
+from fate_flow.manager.outputs.metric import OutputMetric
+from fate_flow.manager.operation.job_saver import JobSaver
 from fate_flow.utils.api_utils import API
 
 
 @manager.route('/metric/key/query', methods=['GET'])
 @API.Input.params(job_id=fields.String(required=True), desc=JOB_ID)
 @API.Input.params(role=fields.String(required=True), desc=ROLE)
 @API.Input.params(party_id=fields.String(required=True), desc=PARTY_ID)
@@ -43,20 +44,33 @@
 @manager.route('/metric/query', methods=['GET'])
 @API.Input.params(job_id=fields.String(required=True), desc=PARTY_ID)
 @API.Input.params(role=fields.String(required=True), desc=ROLE)
 @API.Input.params(party_id=fields.String(required=True), desc=PARTY_ID)
 @API.Input.params(task_name=fields.String(required=True), desc=TASK_NAME)
 @API.Input.params(filters=fields.Dict(required=False), desc=FILTERS)
 def query_metric(job_id, role, party_id, task_name, filters=None):
-    tasks = JobSaver.query_task(job_id=job_id, role=role, party_id=party_id, task_name=task_name)
+    tasks = JobSaver.query_task(job_id=job_id, role=role, party_id=party_id, task_name=task_name, ignore_protocol=True)
     if not tasks:
-        return API.Output.fate_flow_exception(e=NoFoundTask(job_id=job_id, role=role, party_id=party_id,
-                                                            task_name=task_name))
-    metrics = OutputMetric(job_id=job_id, role=role, party_id=party_id, task_name=task_name, task_id=tasks[0].f_task_id,
-                           task_version=tasks[0].f_task_version).read_metrics(filters)
+        return API.Output.fate_flow_exception(
+            e=NoFoundTask(job_id=job_id, role=role, party_id=party_id, task_name=task_name)
+        )
+
+    kind = tasks[0].f_protocol
+    if kind != PROTOCOL.FATE_FLOW:
+        from fate_flow.adapter import AdapterJobController
+        metrics = AdapterJobController(kind).query_output_metric()
+    else:
+        metrics = OutputMetric(
+            job_id=job_id,
+            role=role,
+            party_id=party_id,
+            task_name=task_name,
+            task_id=tasks[0].f_task_id,
+            task_version=tasks[0].f_task_version
+        ).read_metrics(filters)
     return API.Output.json(code=ReturnCode.Base.SUCCESS, message='success', data=metrics)
 
 
 @manager.route('/metric/delete', methods=['POST'])
 @API.Input.json(job_id=fields.String(required=True), desc=JOB_ID)
 @API.Input.json(role=fields.String(required=True), desc=ROLE)
 @API.Input.json(party_id=fields.String(required=True), desc=PARTY_ID)
@@ -75,20 +89,26 @@
 
 @manager.route('/model/query', methods=['GET'])
 @API.Input.params(job_id=fields.String(required=True), desc=JOB_ID)
 @API.Input.params(role=fields.String(required=True), desc=ROLE)
 @API.Input.params(party_id=fields.String(required=True), desc=PARTY_ID)
 @API.Input.params(task_name=fields.String(required=True), desc=TASK_NAME)
 def query_model(job_id, role, party_id, task_name):
-    tasks = JobSaver.query_task(job_id=job_id, role=role, party_id=party_id, task_name=task_name)
+    tasks = JobSaver.query_task(job_id=job_id, role=role, party_id=party_id, task_name=task_name, ignore_protocol=True)
     if not tasks:
         return API.Output.fate_flow_exception(e=NoFoundTask(job_id=job_id, role=role, party_id=party_id,
                                                             task_name=task_name))
     task = tasks[0]
-    model_data = PipelinedModel.read_model(task.f_job_id, task.f_role, task.f_party_id, task.f_task_name)
+
+    kind = task.f_protocol
+    if kind != PROTOCOL.FATE_FLOW:
+        from fate_flow.adapter import AdapterJobController
+        model_data = AdapterJobController(kind).query_output_model()
+    else:
+        model_data = PipelinedModel.read_model(task.f_job_id, task.f_role, task.f_party_id, task.f_task_name)
     return API.Output.json(data=model_data)
 
 
 @manager.route('/model/download', methods=['GET'])
 @API.Input.params(job_id=fields.String(required=True), desc=JOB_ID)
 @API.Input.params(role=fields.String(required=True), desc=ROLE)
 @API.Input.params(party_id=fields.String(required=True), desc=PARTY_ID)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/permission_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/permission_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from webargs import fields
 
 from fate_flow.apps.desc import PERMISSION_APP_ID, PERMISSION_ROLE, PARTY_ID, COMPONENT, DATASET
-from fate_flow.controller.app_controller import PermissionController
-from fate_flow.controller.permission_controller import ResourcePermissionController
+from fate_flow.controller.permission import ResourcePermissionController, PermissionController
 from fate_flow.entity.code import ReturnCode
 from fate_flow.entity.types import PermissionParameters
 from fate_flow.runtime.runtime_config import RuntimeConfig
 from fate_flow.runtime.system_settings import PERMISSION_MANAGER_PAGE
 from fate_flow.utils.api_utils import API
 
 page_name = PERMISSION_MANAGER_PAGE
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/provider_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/provider_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,32 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from webargs import fields
 
-from fate_flow.apps.desc import PROVIDER_NAME, DEVICE, VERSION, COMPONENT_METADATA, PROVIDER_ALL_NAME
+from fate_flow.apps.desc import PROVIDER_NAME, DEVICE, VERSION, COMPONENT_METADATA, PROVIDER_ALL_NAME, \
+    COMPONENTS_DESCRIPTION, PROTOCOL
 from fate_flow.errors.server_error import DeviceNotSupported
 from fate_flow.manager.service.provider_manager import ProviderManager
 from fate_flow.utils.api_utils import API
 
 
 @manager.route('/register', methods=['POST'])
 @API.Input.json(name=fields.String(required=True), desc=PROVIDER_NAME)
 @API.Input.json(device=fields.String(required=True), desc=DEVICE)
 @API.Input.json(version=fields.String(required=True), desc=VERSION)
 @API.Input.json(metadata=fields.Dict(required=True), desc=COMPONENT_METADATA)
-def register(name, device, version, metadata):
+@API.Input.json(protocol=fields.String(required=False), desc=PROTOCOL)
+@API.Input.json(components_description=fields.Dict(required=False), desc=COMPONENTS_DESCRIPTION)
+def register(name, device, version, metadata, components_description=None, protocol=None):
     provider = ProviderManager.get_provider(name=name, device=device, version=version, metadata=metadata, check=True)
     if provider:
-        operator_type = ProviderManager.register_provider(provider)
+        operator_type = ProviderManager.register_provider(provider, components_description, protocol)
         return API.Output.json(message=f"{operator_type} success")
     else:
         return API.Output.fate_flow_exception(DeviceNotSupported(device=device))
 
 
 @manager.route('/query', methods=['GET'])
 @API.Input.params(name=fields.String(required=False), desc=PROVIDER_NAME)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/server_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/server_app.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/site_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/site_app.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/client/table_app.py` & `fate_flow-2.1.0/fate_flow/apps/client/table_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from webargs import fields
 
 from fate_flow.apps.desc import NAMESPACE, NAME, DISPLAY, SERVER_FILE_PATH
 from fate_flow.engine import storage
-from fate_flow.engine.storage import Session, StorageEngine
-from fate_flow.entity.code import ReturnCode
+from fate_flow.engine.storage import StorageEngine, DataType
 from fate_flow.errors.server_error import NoFoundTable
-from fate_flow.manager.data.data_manager import DataManager
+from fate_flow.manager.outputs.data import DataManager
 from fate_flow.utils.api_utils import API
 
 page_name = "table"
 
 
 @manager.route('/query', methods=['GET'])
 @API.Input.params(namespace=fields.String(required=True), desc=NAMESPACE)
@@ -54,11 +53,14 @@
 @API.Input.json(namespace=fields.String(required=True), desc=NAMESPACE)
 @API.Input.json(name=fields.String(required=True), desc=NAME)
 @API.Input.json(path=fields.String(required=True), desc=SERVER_FILE_PATH)
 def bind_path(namespace, name, path):
     address = storage.StorageTableMeta.create_address(storage_engine=StorageEngine.PATH, address_dict={"path": path})
     storage_meta = storage.StorageTableBase(
         namespace=namespace, name=name, address=address,
-        engine=StorageEngine.PATH, options=None, partitions=None
+        engine=StorageEngine.PATH, options=None, partitions=None,
+        key_serdes_type=0,
+        value_serdes_type=0,
+        partitioner_type=0,
     )
-    storage_meta.create_meta()
+    storage_meta.create_meta(data_type=DataType.DATA_DIRECTORY)
     return API.Output.json()
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/desc.py` & `fate_flow-2.1.0/fate_flow/apps/desc.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,26 +55,27 @@
 DISPLAY = "Whether to return preview data"
 
 # server
 SERVER_NAME = "Server name"
 SERVICE_NAME = "Service name"
 HOST = "Host IP"
 PORT = "Service port"
-PROTOCOL = "Protocol: http/https"
+PROTOCOL = "Protocol: fate/bfia,etc."
 URI = "Service path"
 METHOD = "Request method: POST/GET, etc."
 PARAMS = "Request header parameters"
 DATA = "Request body parameters"
 HEADERS = "Request headers"
 
 # provider
 PROVIDER_NAME = "Component provider name"
 DEVICE = "Component running mode"
 VERSION = "Component version"
 COMPONENT_METADATA = "Detailed information about component registration"
+COMPONENTS_DESCRIPTION = "Components description"
 PROVIDER_ALL_NAME = "Registered algorithm full name, provider + ':' + version + '@' + running mode, e.g., fate:2.0.0@local"
 
 # permission
 PERMISSION_APP_ID = "App ID"
 PERMISSION_ROLE = "Permission name"
 COMPONENT = "Component name"
 DATASET = "List of datasets"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/desc_zh.py` & `fate_flow-2.1.0/fate_flow/apps/desc_zh.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 HEADERS = "请求头"
 
 # provider
 PROVIDER_NAME = "组件提供方名称"
 DEVICE = "组件运行模式"
 VERSION = "组件版本"
 COMPONENT_METADATA = "组件注册详细信息"
+COMPONENTS_DESCRIPTION = "组件描述"
 PROVIDER_ALL_NAME = "注册的算法全名，提供方+':'+版本+'@'+运行模式，如: fate:2.0.0@local"
 
 # permission
 PERMISSION_APP_ID = "App id"
 PERMISSION_ROLE = "权限名称"
 COMPONENT = "组件名"
 DATASET = "数据集列表"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/partner/__init__.py` & `fate_flow-2.1.0/fate_flow/apps/partner/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/partner/partner_app.py` & `fate_flow-2.1.0/fate_flow/apps/partner/partner_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,37 +11,39 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from webargs import fields
 
-from fate_flow.controller.job_controller import JobController
-from fate_flow.controller.task_controller import TaskController
+from fate_flow.controller.job import JobController
+from fate_flow.controller.task import TaskController
 from fate_flow.entity.types import TaskStatus
 from fate_flow.entity.code import ReturnCode
 from fate_flow.errors.server_error import CreateJobFailed, UpdateJobFailed, KillFailed, JobResourceException,\
     NoFoundTask, StartTaskFailed, UpdateTaskFailed, KillTaskFailed, TaskResourceException
 from fate_flow.manager.service.resource_manager import ResourceManager
-from fate_flow.operation.job_saver import JobSaver
+from fate_flow.manager.operation.job_saver import JobSaver
 from fate_flow.utils.api_utils import API, stat_logger
-from fate_flow.utils.wraps_utils import task_request_proxy, create_job_request_check
+from fate_flow.utils.permission_utils import create_job_request_check
+from fate_flow.utils.wraps_utils import task_request_proxy
 
 page_name = 'partner'
 
 
 @manager.route('/job/create', methods=['POST'])
-@API.Input.json(dag_schema=fields.Dict(required=True))
+@API.Input.json(dag=fields.Dict(required=True))
+@API.Input.json(schema_version=fields.String(required=True))
 @API.Input.json(job_id=fields.String(required=True))
 @API.Input.json(role=fields.String(required=True))
 @API.Input.json(party_id=fields.String(required=True))
 @create_job_request_check
-def partner_create_job(dag_schema, job_id, role, party_id):
+def partner_create_job(dag, schema_version, job_id, role, party_id):
     try:
-        JobController.create_job(dag_schema, job_id, role, party_id)
+        JobController.create_job(dag, schema_version, job_id, role, party_id)
         return API.Output.json()
     except Exception as e:
         stat_logger.exception(e)
         return API.Output.fate_flow_exception(CreateJobFailed(detail=str(e)))
 
 
 @manager.route('/job/start', methods=['POST'])
@@ -174,15 +176,20 @@
 @API.Input.json(job_id=fields.String(required=True))
 @API.Input.json(role=fields.String(required=True))
 @API.Input.json(party_id=fields.String(required=True))
 @API.Input.json(task_id=fields.String(required=True))
 @API.Input.json(task_version=fields.Integer(required=True))
 @task_request_proxy(filter_local=True)
 def start_task(job_id, role, party_id, task_id, task_version):
-    if TaskController.start_task(job_id, role, party_id, task_id, task_version):
+    task = JobSaver.query_task(task_id=task_id, task_version=task_version, role=role, party_id=party_id)[0]
+    if not task:
+        return API.Output.fate_flow_exception(
+            NoFoundTask(job_id=job_id, role=role, party_id=party_id, task_id=task_id, task_version=task_version)
+        )
+    if TaskController.start_task(task):
         return API.Output.json(code=ReturnCode.Base.SUCCESS, message='success')
     else:
         return API.Output.fate_flow_exception(StartTaskFailed(
             job_id=job_id, role=role, party_id=party_id,
             task_id=task_id, task_version=task_version
         ))
 
@@ -253,14 +260,13 @@
 
 @manager.route('/task/rerun', methods=['POST'])
 @API.Input.json(job_id=fields.String(required=True))
 @API.Input.json(role=fields.String(required=True))
 @API.Input.json(party_id=fields.String(required=True))
 @API.Input.json(task_id=fields.String(required=True))
 @API.Input.json(task_version=fields.Integer(required=True))
-@API.Input.json(new_version=fields.Integer())
+@API.Input.json(new_version=fields.Integer(required=True))
 def rerun_task(job_id, role, party_id, task_id, task_version, new_version):
     tasks = JobSaver.query_task(job_id=job_id, task_id=task_id, role=role, party_id=party_id)
-    if not tasks:
-        return API.Output.fate_flow_exception(NoFoundTask(job_id=job_id, role=role, party_id=party_id, task_id=task_id))
-    TaskController.create_new_version_task(task=tasks[0], new_version=new_version)
+    if tasks:
+        TaskController.create_new_version_task(task=tasks[0], new_version=new_version)
     return API.Output.json()
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/scheduler/__init__.py` & `fate_flow-2.1.0/fate_flow/adapter/bfia/container/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/scheduler/scheduler_app.py` & `fate_flow-2.1.0/fate_flow/apps/scheduler/scheduler_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from webargs import fields
 
+from fate_flow.entity.spec.dag import DAGSchema
 from fate_flow.errors.server_error import UpdateTaskFailed
-from fate_flow.operation.job_saver import ScheduleJobSaver
-from fate_flow.scheduler.job_scheduler import DAGScheduler
+from fate_flow.manager.operation.job_saver import ScheduleJobSaver
+from fate_flow.scheduler.scheduler import DAGScheduler
 from fate_flow.utils.api_utils import API
 
 page_name = 'scheduler'
 
 
 @manager.route('/job/create', methods=['POST'])
-@API.Input.json(dag_schema=fields.Dict(required=True))
-def create_job(dag_schema):
-    submit_result = DAGScheduler.submit(dag_schema)
+@API.Input.json(dag=fields.Dict(required=True))
+@API.Input.json(schema_version=fields.String(required=True))
+def create_job(dag, schema_version):
+    dag = DAGSchema(dag=dag, schema_version=schema_version)
+    submit_result = DAGScheduler.create_all_job(dag.dict())
     return API.Output.json(**submit_result)
 
 
 @manager.route('/task/report', methods=['POST'])
 @API.Input.json(job_id=fields.String(required=True))
 @API.Input.json(role=fields.String(required=True))
 @API.Input.json(party_id=fields.String(required=True))
@@ -53,16 +56,15 @@
     )
 
 
 @manager.route('/job/stop', methods=['POST'])
 @API.Input.json(job_id=fields.String(required=True))
 @API.Input.json(stop_status=fields.String(required=False))
 def stop_job(job_id, stop_status=None):
-    retcode, retmsg = DAGScheduler.stop_job(job_id=job_id,
-                                            stop_status=stop_status)
+    retcode, retmsg = DAGScheduler.stop_job(job_id, stop_status)
     return API.Output.json(code=retcode, message=retmsg)
 
 
 @manager.route('/job/rerun', methods=['POST'])
 @API.Input.json(job_id=fields.String(required=True))
 def rerun_job(job_id):
     DAGScheduler.rerun_job(job_id=job_id, auto=False)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/worker/__init__.py` & `fate_flow-2.1.0/fate_flow/adapter/bfia/container/entrypoint/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/apps/worker/worker_app.py` & `fate_flow-2.1.0/fate_flow/apps/worker/worker_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,25 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-import json
 
 from flask import request
 from webargs import fields
 
-from fate_flow.controller.task_controller import TaskController
+from fate_flow.controller.task import TaskController
 from fate_flow.entity.code import ReturnCode
 from fate_flow.errors.server_error import NoFoundTask
-from fate_flow.manager.data.data_manager import DataManager
-from fate_flow.manager.model.model_manager import PipelinedModel
-from fate_flow.manager.metric.metric_manager import OutputMetric
-from fate_flow.manager.service.output_manager import OutputDataTracking
-from fate_flow.operation.job_saver import JobSaver
+from fate_flow.manager.outputs.data import DataManager, OutputDataTracking
+from fate_flow.manager.outputs.model import PipelinedModel
+from fate_flow.manager.outputs.metric import OutputMetric
+from fate_flow.manager.operation.job_saver import JobSaver
 from fate_flow.utils.api_utils import API
 
 page_name = 'worker'
 
 
 @manager.route('/task/status', methods=['POST'])
 @API.Input.json(execution_id=fields.String(required=True))
@@ -161,19 +159,20 @@
         "task_version": task.f_task_version,
         "task_name": task.f_task_name,
         "namespace": namespace,
         "name": name,
         "index": index
     }
     OutputDataTracking.create(data_info)
-    DataManager.create_data_table(
-        namespace=namespace, name=name, uri=uri, partitions=partitions,
-        data_meta=meta_data, source=source, data_type=data_type,
-        count=overview.get("count", None), part_of_data=overview.get("samples", [])
-    )
+    if uri:
+        DataManager.create_data_table(
+            namespace=namespace, name=name, uri=uri, partitions=partitions,
+            data_meta=meta_data, source=source, data_type=data_type,
+            count=overview.get("count", None), part_of_data=overview.get("samples", [])
+        )
     return API.Output.json(code=ReturnCode.Base.SUCCESS, message="success")
 
 
 @manager.route('/metric/save', methods=["POST"])
 @API.Input.json(execution_id=fields.String(required=True))
 @API.Input.json(data=fields.List(fields.Dict()))
 @API.Output.runtime_exception(code=ReturnCode.API.COMPONENT_OUTPUT_EXCEPTION)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/commands/server_cli.py` & `fate_flow-2.1.0/fate_flow/commands/server_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import os
+import shutil
 import subprocess
 import platform
 import click
 from ruamel import yaml
 
 import fate_flow
 from fate_flow.commands.service import manage_fate_service
+from fate_flow.settings import DEFAULT_SERVER_CONF_PATH
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 HOME = os.path.dirname(fate_flow.__file__)
-SERVER_CONF_PATH = os.path.join(HOME, "conf", "service_conf.yaml")
+CONF_PATH = DEFAULT_SERVER_CONF_PATH or os.path.join(HOME, "conf")
+SERVER_CONF_PATH = os.path.join(CONF_PATH, "service_conf.yaml")
 SETTING_PATH = os.path.join(HOME, "settings.py")
 SERVICE_SH = os.path.join(HOME, "commands", "service.sh")
 
 
 @click.group(short_help='Fate Flow', context_settings=CONTEXT_SETTINGS)
 @click.pass_context
 def flow_server_cli(ctx):
@@ -134,59 +137,77 @@
 
 @flow_server_cli.command('version', short_help='Flow Server Version Command')
 def get_version():
     import fate_flow
     print(fate_flow.__version__)
 
 
-def replace_settings(home_path):
+def set_conf_home(home_path):
+    default_conf = os.path.join(HOME, "conf")
+    conf_home = f"{home_path}/conf"
+    shutil.copytree(default_conf, conf_home)
+    return conf_home
+
+
+def replace_settings(home_path, data_home):
     import re
     with open(SETTING_PATH, "r") as file:
         content = file.read()
     content = re.sub(r"DATA_DIR.*", f"DATA_DIR = \"{home_path}/data\"", content)
     content = re.sub(r"MODEL_DIR.*", f"MODEL_DIR = \"{home_path}/model\"", content)
     content = re.sub(r"JOB_DIR.*", f"JOB_DIR = \"{home_path}/jobs\"", content)
     content = re.sub(r"LOG_DIR.*", f"LOG_DIR = \"{home_path}/logs\"", content)
+    content = re.sub(r"UPLOAD_DATA_HOME.*", f"UPLOAD_DATA_HOME = \"{data_home}\"", content)
     content = re.sub(r"SQLITE_FILE_NAME.*", f"SQLITE_FILE_NAME = \"{home_path}/fate_flow_sqlite.db\"", content)
+
+    content = re.sub(r"DEFAULT_SERVER_CONF_PATH.*", f"DEFAULT_SERVER_CONF_PATH = \"{home_path}/conf\"", content)
+
     with open(SETTING_PATH, "w") as file:
         file.write(content)
 
     with open(SERVICE_SH, "r") as file:
         content = file.read()
         content = re.sub(r"LOG_DIR.*=.*", f"LOG_DIR=\"{home_path}/logs\"", content)
     with open(SERVICE_SH, "w") as file:
         file.write(content)
 
 
 def init_server(ip, port, home):
+    conf_home = CONF_PATH
     with open(SERVER_CONF_PATH, "r") as file:
         config = yaml.safe_load(file)
     if ip:
         print(f"ip: {ip}")
         config["fateflow"]["host"] = ip
     if port:
         print(f"port: {port}")
         config["fateflow"]["http_port"] = port
     if home:
         if not os.path.isabs(home):
             raise RuntimeError(f"Please use an absolute path: {home}")
         os.makedirs(home, exist_ok=True)
+        data_home = os.path.join(home, "upload")
+        os.makedirs(data_home, exist_ok=True)
         print(f"home: {home}")
-        replace_settings(home)
+        conf_home = set_conf_home(home)
+        replace_settings(home, data_home)
 
     if ip or port:
-        with open(SERVER_CONF_PATH, "w") as file:
-            yaml.dump(config, file)
+        service_conf_path = SERVER_CONF_PATH if not conf_home else os.path.join(conf_home, "service_conf.yaml")
+        print(f"Conf path: {service_conf_path}")
+        with open(service_conf_path, "w") as file:
+            yaml.dump(config, file, default_flow_style=False)
 
     print("Init server completed!")
 
 
 def run_command(command):
     try:
-        command = f"sh {SERVICE_SH} {HOME} {command}"
+        service_conf_path = os.path.join(CONF_PATH, "service_conf.yaml")
+        command = f"bash {SERVICE_SH} {HOME} {command} {service_conf_path}"
         result = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, text=True)
         if result.returncode == 0:
             print(result.stdout)
             return result.stdout
         else:
             print(result.stdout)
             print(f"Error: {result.stderr}")
```

### Comparing `fate_flow-2.0.0b0/fate_flow/commands/service.py` & `fate_flow-2.1.0/fate_flow/commands/service.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/components/__init__.py` & `fate_flow-2.1.0/fate_flow/apps/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/components/components/__init__.py` & `fate_flow-2.1.0/fate_flow/components/components/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/components/components/download.py` & `fate_flow-2.1.0/fate_flow/components/components/download.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,32 +12,35 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import logging
 
 from fate_flow.components import cpn
 from fate_flow.engine import storage
+from fate_flow.entity.spec.dag import IOMeta, ArtifactOutputSpec, Metadata, TaskConfigSpec
 from fate_flow.errors.server_error import NoFoundTable
-from fate_flow.manager.data.data_manager import DataManager
+from fate_flow.manager.outputs.data import DataManager
 
 
 @cpn.component()
 def download(
-    config
+    config,
+    outputs: IOMeta.OutputMeta
 ):
-    download_data(config)
+    download_data(config, outputs)
 
 
-def download_data(config):
-    job_id = config.pop("job_id")
+def download_data(config: TaskConfigSpec, outputs: IOMeta.OutputMeta):
+    parameters = config.parameters
     download_object = Download()
     download_object.run(
         parameters=DownloadParam(
-            **config
-        )
+            **parameters
+        ),
+        outputs=outputs
     )
 
 
 class DownloadParam(object):
     def __init__(
             self,
             namespace,
@@ -51,18 +54,23 @@
 
 class Download:
     def __init__(self):
         self.parameters = None
         self.table = None
         self.data_meta = {}
 
-    def run(self, parameters: DownloadParam):
+    def run(self, parameters: DownloadParam, outputs: IOMeta.OutputMeta):
         data_table_meta = storage.StorageTableMeta(name=parameters.name, namespace=parameters.namespace)
         if not data_table_meta:
             raise NoFoundTable(name=parameters.name, namespace=parameters.namespace)
         download_dir = parameters.path
         logging.info("start download data")
         DataManager.send_table(
             output_tables_meta={"data": data_table_meta},
             download_dir=download_dir
         )
+        outputs.data = {"output_data": ArtifactOutputSpec(
+            uri="",
+            metadata=Metadata(namespace=parameters.namespace, name=parameters.name),
+            type_name=data_table_meta.data_type,
+        ).dict()}
         logging.info(f"download data success, download path: {parameters.path}")
```

### Comparing `fate_flow-2.0.0b0/fate_flow/components/components/upload.py` & `fate_flow-2.1.0/fate_flow/components/components/upload.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,42 +8,52 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+import json
 import logging
 import os
 import secrets
+import uuid
 from typing import Union
 
 from fate_flow.components import cpn
-from fate_flow.engine.storage import Session, StorageEngine, DataType, StorageTableMeta, StorageOrigin
-from fate_flow.entity.spec.dag import ArtifactSource
-from fate_flow.manager.data.data_manager import DatasetManager
-from fate_flow.runtime.system_settings import STANDALONE_DATA_HOME
+from fate_flow.engine.storage import Session, StorageEngine, DataType, StorageTableMeta
+from fate_flow.entity.spec.dag import IOMeta, ArtifactOutputSpec, Metadata, ArtifactSource, MetricData, TaskConfigSpec
+from fate_flow.entity.types import JsonMetricArtifactType, EngineType
+from fate_flow.manager.outputs.data import DatasetManager
+from fate_flow.runtime.system_settings import STANDALONE_DATA_HOME, ENGINES
 from fate_flow.utils.file_utils import get_fate_flow_directory
+from fate_flow.utils.io_utils import URI
 
 
 @cpn.component()
 def upload(
-    config
+    config, outputs: IOMeta.OutputMeta
 ):
-    upload_data(config)
+    upload_data(config, outputs)
 
 
-def upload_data(config):
-    job_id = config.pop("job_id")
+def upload_data(config: TaskConfigSpec, outputs):
+    parameters = config.parameters
+    job_id = config.job_id
     upload_object = Upload()
+    engine_options = {}
+    if config.conf.computing.metadata and config.conf.computing.metadata.options:
+        engine_options = config.conf.computing.metadata.options
     data = upload_object.run(
         parameters=UploadParam(
-            **config
+            **parameters
         ),
-        job_id=job_id
+        job_id=job_id,
+        outputs=outputs,
+        engine_options=engine_options
     )
 
 
 class Param(object):
     def to_dict(self):
         d = {}
         for k, v in self.__dict__.items():
@@ -95,43 +105,49 @@
             namespace="",
             name="",
             file="",
             storage_engine="",
             head=1,
             partitions=10,
             extend_sid=False,
+            is_temp_file=False,
             address: dict = {},
             meta: dict = {}
     ):
         self.name = name
         self.namespace = namespace
         self.file = file
         self.storage_engine = storage_engine
         self.head = head
         self.partitions = partitions
         self.extend_sid = extend_sid
         self.meta = MetaParam(**meta)
         self.storage_address = address
+        self.is_temp_file = is_temp_file
 
 
 class Upload:
     def __init__(self):
         self.parameters = None
         self.table = None
         self.data_meta = {}
 
-    def run(self, parameters: UploadParam, job_id=""):
+    def run(self, parameters: UploadParam, outputs: IOMeta.OutputMeta = None, job_id="", engine_options={}):
         self.parameters = parameters
         logging.info(self.parameters.to_dict())
         storage_address = self.parameters.storage_address
         if not os.path.isabs(parameters.file):
             parameters.file = os.path.join(
                 get_fate_flow_directory(), parameters.file
             )
         name, namespace = parameters.name, parameters.namespace
+        if not name or not namespace:
+            namespace, name = self.parameters.namespace, self.parameters.name = self.generate_table_name()
+        if not parameters.storage_engine:
+            parameters.storage_engine = ENGINES.get(EngineType.STORAGE)
         with Session() as sess:
             # clean table
             table = sess.get_table(namespace=namespace, name=name)
             if table:
                 logging.info(
                     f"destroy table name: {name} namespace: {namespace} engine: {table.engine}"
                 )
@@ -142,68 +158,75 @@
             else:
                 logging.info(
                     f"can not found table name: {name} namespace: {namespace}, pass destroy"
                 )
             address_dict = storage_address.copy()
             storage_engine = self.parameters.storage_engine
             storage_session = sess.storage(
-                storage_engine=storage_engine
+                storage_engine=storage_engine, options=engine_options
             )
             if storage_engine in {StorageEngine.EGGROLL, StorageEngine.STANDALONE}:
                 upload_address = {
                     "name": name,
                     "namespace": namespace
                 }
                 if storage_engine == StorageEngine.STANDALONE:
-                    upload_address.update({"home": STANDALONE_DATA_HOME})
+                    home = os.getenv("STANDALONE_DATA_HOME") or STANDALONE_DATA_HOME
+                    upload_address.update({"home": home})
             elif storage_engine in {StorageEngine.HDFS, StorageEngine.FILE}:
                 upload_address = {
                     "path": DatasetManager.upload_data_path(
                         name=name,
                         namespace=namespace,
                         storage_engine=storage_engine
                     )
                 }
             else:
                 raise RuntimeError(f"can not support this storage engine: {storage_engine}")
             address_dict.update(upload_address)
             logging.info(f"upload to {storage_engine} storage, address: {address_dict}")
+            logging.info(f"engine options: {engine_options}")
             address = StorageTableMeta.create_address(
                 storage_engine=storage_engine, address_dict=address_dict
             )
             self.table = storage_session.create_table(
                 address=address,
                 source=ArtifactSource(
                     task_id="",
                     party_task_id="",
                     task_name="upload",
                     component="upload",
                     output_artifact_key="data"
                 ).dict(),
-                **self.parameters.to_dict()
+                **self.parameters.to_dict(),
+                options=engine_options
             )
             data_table_count = self.save_data_table(job_id)
             logging.info("------------load data finish!-----------------")
 
             logging.info("file: {}".format(self.parameters.file))
             logging.info("total data_count: {}".format(data_table_count))
             logging.info("table name: {}, table namespace: {}".format(name, namespace))
-            return {"name": name, "namespace": namespace, "count": data_table_count}
+            if outputs:
+                self.save_outputs(job_id, outputs, data_table_count)
+            return {"name": name, "namespace": namespace, "count": data_table_count, "data_meta": self.data_meta}
 
     def save_data_table(self, job_id):
         input_file = self.parameters.file
         input_feature_count = self.get_count(input_file)
         self.upload_file(input_file, job_id, input_feature_count)
         table_count = self.table.count()
         metas_info = {
             "count": table_count,
             "partitions": self.parameters.partitions,
             "data_type": DataType.TABLE
         }
         self.table.meta.update_metas(**metas_info)
+        # cleanup temp file
+        self.cleanup()
         return table_count
 
     def update_schema(self, fp):
         id_index = 0
         read_status = False
         if self.parameters.head is True:
             data_head = fp.readline()
@@ -321,7 +344,42 @@
     @staticmethod
     def join_in_index_line(delimiter, values, id_index):
         return delimiter.join([
             values[id_index],
             delimiter.join(values[:id_index]),
             delimiter.join(values[id_index + 1:])
         ]).strip(delimiter)
+
+    def save_outputs(self, job_id, outputs: IOMeta.OutputMeta, data_count):
+        data = ArtifactOutputSpec(
+            uri="",
+            metadata=Metadata(namespace=self.parameters.namespace, name=self.parameters.name),
+            type_name=DataType.TABLE,
+        )
+        uri = DatasetManager.output_local_uri(
+            task_info=dict(job_id=job_id, role="local", party_id="0", task_name="upload_0", task_version="0"),
+            name="metric",
+            type_name=JsonMetricArtifactType.type_name
+        )
+
+        path = URI.from_string(uri).to_schema().path
+        os.makedirs(os.path.dirname(path), exist_ok=True)
+        metrics = [MetricData(name="upload", data={"name": self.parameters.name, "namespace": self.parameters.namespace,
+                                                   "count": data_count}).dict()]
+        with open(path, "w") as f:
+            json.dump(metrics, f)
+        metric = ArtifactOutputSpec(
+            uri=uri,
+            metadata=Metadata(metadata={}),
+            type_name=JsonMetricArtifactType.type_name
+        )
+        outputs.data = {"table": data.dict()}
+        outputs.metric = {"metric": metric.dict()}
+
+    @staticmethod
+    def generate_table_name():
+        return "upload", uuid.uuid1().hex
+
+    def cleanup(self):
+        if self.parameters.is_temp_file:
+            if os.path.exists(self.parameters.file):
+                os.remove(self.parameters.file)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/components/cpn.py` & `fate_flow-2.1.0/fate_flow/components/cpn.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         self,
         name: str,
         callback
     ) -> None:
         self.name = name
         self.callback = callback
 
-    def execute(self, config):
-        return self.callback(config)
+    def execute(self, config, outputs):
+        return self.callback(config, outputs)
 
 
 def component(*args, **kwargs):
     def decorator(f):
         cpn_name = f.__name__.lower()
         if isinstance(f, _Component):
             raise TypeError("Attempted to convert a callback into a component twice.")
```

### Comparing `fate_flow-2.0.0b0/fate_flow/components/entrypoint/__init__.py` & `fate_flow-2.1.0/fate_flow/apps/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/components/entrypoint/component.py` & `fate_flow-2.1.0/fate_flow/hub/database/sqlite.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,29 +8,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-import logging
-
-from fate_flow.entity.spec.dag import TaskConfigSpec
-
-logger = logging.getLogger(__name__)
-
-
-def execute_component(config: TaskConfigSpec):
-    component = load_component(config.component)
-    cpn_config = config.parameters
-    cpn_config["job_id"] = config.job_id
-    logger.info(f"cpn_config： {cpn_config}")
-
-    component.execute(cpn_config)
+#
+from peewee import Insert
 
+from fate_flow.runtime.system_settings import SQLITE_PATH
 
-def load_component(cpn_name: str):
-    from fate_flow.components.components import BUILDIN_COMPONENTS
 
-    for cpn in BUILDIN_COMPONENTS:
-        if cpn.name == cpn_name:
-            return cpn
+def get_database_connection(config, decrypt_key):
+    Insert.on_conflict = lambda self, *args, **kwargs: self.on_conflict_replace()
+    from playhouse.apsw_ext import APSWDatabase
+    path = config.get("path")
+    if not path:
+        path = SQLITE_PATH
+    return APSWDatabase(path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fate_flow-2.0.0b0/fate_flow/conf/service_conf.yaml` & `fate_flow-2.1.0/fate_flow/conf/service_conf.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 party_id: "9999"
 use_registry: false
+# DEBUG 10/INFO 20
+log_level: 20
 encrypt:
   key_0:
     module: fate_flow.hub.encrypt.password_encrypt#pwdecrypt
     # base on: fate_flow/conf/
     private_path: private_key.pem
 fateflow:
   host: 127.0.0.1
   http_port: 9380
   grpc_port: 9360
-  proxy_name: rollsite
-  nginx:
-    host:
-    http_port:
-    grpc_port:
+  proxy_name: osx
+#  nginx:
+#    host:
+#    http_port:
+#    grpc_port:
 database:
   engine: sqlite
   # encrypt passwd key
   decrypt_key:
   mysql:
     name: fate_flow
     user: fate
@@ -35,60 +37,54 @@
   federation: standalone
   storage: standalone
 default_provider:
   name: fate
   # version default: fateflow.env
   version:
   device: local
-federation:
-  pulsar:
-    host: 192.168.0.5
-    port: 6650
-    mng_port: 8080
-    cluster: standalone
-    tenant: fl-tenant
-    topic_ttl: 30
-    # default conf/pulsar_route_table.yaml
-    route_table:
-    # mode: replication / client, default: replication
-    mode: replication
-    max_message_size: 1048576
-  nginx:
-    host: 127.0.0.1
-    http_port: 9300
-    grpc_port: 9310
-    # http or grpc
-    protocol: http
-  rabbitmq:
-    host: 192.168.0.4
-    mng_port: 12345
-    port: 5672
-    user: fate
-    password: fate
-    # default conf/rabbitmq_route_table.yaml
-    route_table:
-    # mode: replication / client, default: replication
-    mode: replication
-    max_message_size: 1048576
-  rollsite:
-    host: 127.0.0.1
-    port: 9370
-  osx:
-    host: 127.0.0.1
-    port: 9370
 computing:
   standalone:
     cores: 32
   eggroll:
     cores: 32
-    nodes: 2
+    nodes: 1
+    # cluster manager host and port
+    host: 127.0.0.1
+    port: 4670
   spark:
     # default use SPARK_HOME environment variable
     home:
     cores: 32
+federation:
+  osx:
+    host: 127.0.0.1
+    port: 9370
+    # stream or queue
+    mode: stream
+#  pulsar:
+#    host: 192.168.0.5
+#    port: 6650
+#    mng_port: 8080
+#    cluster: standalone
+#    tenant: fl-tenant
+#    topic_ttl: 30
+#    # default conf/pulsar_route_table.yaml
+#    route_table:
+#    # mode: replication / client, default: replication
+#    mode: replication
+#  rabbitmq:
+#    host: 192.168.0.4
+#    mng_port: 12345
+#    port: 5672
+#    user: fate
+#    password: fate
+#    # default conf/rabbitmq_route_table.yaml
+#    route_table:
+#    # mode: replication / client, default: replication
+#    mode: replication
 storage:
   hdfs:
     name_node: hdfs://fate-cluster
 hook_module:
   client_authentication: fate_flow.hook.flow.client_authentication
   site_authentication: fate_flow.hook.flow.site_authentication
   permission: fate_flow.hook.flow.permission
```

### Comparing `fate_flow-2.0.0b0/fate_flow/controller/__init__.py` & `fate_flow-2.1.0/fate_flow/components/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/controller/app_controller.py` & `fate_flow-2.1.0/fate_flow/manager/service/app_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,126 +8,130 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-import hashlib
-import time
+from functools import wraps
 
-from fate_flow.db.casbin_models import FATE_CASBIN
-from fate_flow.errors.server_error import RequestExpired, NoFoundAppid, InvalidParameter, RoleTypeError
-from fate_flow.manager.service.app_manager import AppManager
-from fate_flow.runtime.runtime_config import RuntimeConfig
-from fate_flow.runtime.system_settings import CLIENT_AUTHENTICATION, SITE_AUTHENTICATION
+from fate_flow.db.base_models import BaseModelOperate
+from fate_flow.db.permission_models import AppInfo, PartnerAppInfo
+from fate_flow.entity.types import AppType
+from fate_flow.errors.server_error import NoFoundAppid, RoleTypeError
+from fate_flow.runtime.system_settings import ADMIN_KEY, CLIENT_AUTHENTICATION, APP_TOKEN_LENGTH, SITE_AUTHENTICATION, \
+    PARTY_ID
 from fate_flow.utils.base_utils import generate_random_id
-from fate_flow.utils.wraps_utils import switch_function,  check_permission
+from fate_flow.utils.wraps_utils import filter_parameters, switch_function, check_permission
 
 
-class Authentication(object):
+class AppManager(BaseModelOperate):
     @classmethod
-    def md5_sign(cls, app_id, app_token, user_name, initiator_party_id, timestamp, nonce):
-        key = hashlib.md5(str(app_id + user_name + initiator_party_id + nonce + timestamp).encode("utf8")).hexdigest().lower()
-        sign = hashlib.md5(str(key + app_token).encode("utf8")).hexdigest().lower()
-        return sign
-
-    @classmethod
-    def md5_verify(cls, app_id, timestamp, nonce, signature, user_name="", initiator_party_id=""):
-        if cls.check_if_expired(timestamp):
-            raise RequestExpired()
-        apps = AppManager.query_app(app_id=app_id)
-        if apps:
-            _signature = cls.md5_sign(
-                app_id=app_id,
-                app_token=apps[0].f_app_token,
-                user_name=user_name,
-                initiator_party_id=initiator_party_id,
-                timestamp=timestamp,
-                nonce=nonce
-            )
-            return _signature == signature
-        else:
-            raise NoFoundAppid(app_id=app_id)
-
-    @staticmethod
-    def generate_timestamp():
-        return str(int(time.time()*1000))
+    def init(cls):
+        if CLIENT_AUTHENTICATION or SITE_AUTHENTICATION:
+            if cls.query_app(app_name="admin", init=True):
+                cls._delete(AppInfo, app_name="admin")
+            cls.create_app(app_name="admin", app_id="admin", app_token=ADMIN_KEY, app_type="admin", init=True)
+            app_info = cls.create_app(app_name=PARTY_ID, app_id=PARTY_ID, app_type=AppType.SITE, init=True)
+            if app_info:
+                cls.create_partner_app(party_id=PARTY_ID, app_id=app_info.get("app_id"),
+                                       app_token=app_info.get("app_token"))
 
-    @staticmethod
-    def generate_nonce():
-        return generate_random_id(length=4, only_number=True)
-
-    @staticmethod
-    def check_if_expired(timestamp, timeout=60):
-        expiration = int(timestamp) + timeout * 1000
-        if expiration < int(time.time() * 1000):
-            return True
-        else:
-            return False
-
-
-class PermissionController(object):
-    @staticmethod
+    @classmethod
     @switch_function(CLIENT_AUTHENTICATION or SITE_AUTHENTICATION)
-    def add_policy(role, resource, permission):
-        return FATE_CASBIN.add_policy(role, resource, permission)
+    @check_permission(operate="create", types="client")
+    def create_app(cls, app_type, app_name, app_id=None, app_token=None, init=True):
+        if not app_id:
+            app_id = cls.generate_app_id()
+        if not app_token:
+            app_token = cls.generate_app_token()
+        app_info = {
+            "app_name": app_name,
+            "app_id": app_id,
+            "app_token": app_token,
+            "app_type": app_type
+        }
+        status = cls._create_entity(AppInfo, app_info)
+        if status:
+            return app_info
+        else:
+            return {}
 
-    @staticmethod
+    @classmethod
     @switch_function(CLIENT_AUTHENTICATION or SITE_AUTHENTICATION)
-    @AppManager.check_app_id
-    @check_permission(operate="grant", types="permission")
-    @AppManager.check_app_type
-    def add_role_for_user(app_id, role, init=False):
-        PermissionController.check_permission_role(role)
-        return FATE_CASBIN.add_role_for_user(app_id, role)
+    def create_partner_app(cls, party_id, app_id=None, app_token=None):
+        app_info = {
+            "party_id": party_id,
+            "app_id": app_id,
+            "app_token": app_token,
+        }
+        status = cls._create_entity(PartnerAppInfo, app_info)
+        if status:
+            return app_info
+        else:
+            return {}
 
-    @staticmethod
+    @classmethod
     @switch_function(CLIENT_AUTHENTICATION or SITE_AUTHENTICATION)
-    @AppManager.check_app_id
-    @check_permission(operate="delete", types="permission")
-    # @AppManager.check_app_type
-    def delete_role_for_user(app_id, role, grant_role=None, init=False):
-        role_type = role
-        PermissionController.check_permission_role(role)
-        app_info = AppManager.query_app(app_id=app_id)
-        if grant_role == "super_client":
-            grant_role = "client"
-        if grant_role and grant_role != app_info[0].f_app_type:
-            raise RoleTypeError(role=grant_role)
-        return FATE_CASBIN.delete_role_for_suer(app_id, role_type)
+    @filter_parameters()
+    @check_permission(operate="delete", types="client")
+    def delete_app(cls, init=False, **kwargs):
+        return cls._delete(AppInfo, **kwargs)
 
-    @staticmethod
+    @classmethod
     @switch_function(CLIENT_AUTHENTICATION or SITE_AUTHENTICATION)
-    @AppManager.check_app_id
-    @check_permission(operate="query", types="permission")
-    def get_roles_for_user(app_id):
-        return FATE_CASBIN.get_roles_for_user(app_id)
+    @filter_parameters()
+    def delete_partner_app(cls, init=False, **kwargs):
+        return cls._delete(PartnerAppInfo, **kwargs)
 
-    @staticmethod
+    @classmethod
     @switch_function(CLIENT_AUTHENTICATION or SITE_AUTHENTICATION)
-    def get_permissions_for_user(app_id):
-        return FATE_CASBIN.get_permissions_for_user(app_id)
+    @filter_parameters()
+    @check_permission(operate="query", types="client")
+    def query_app(cls, init=False, **kwargs):
+        return cls._query(AppInfo, **kwargs)
 
-    @staticmethod
+    @classmethod
     @switch_function(CLIENT_AUTHENTICATION or SITE_AUTHENTICATION)
-    @AppManager.check_app_id
-    def delete_roles_for_user(app_id):
-        return FATE_CASBIN.delete_roles_for_user(app_id)
+    @filter_parameters()
+    def query_partner_app(cls, **kwargs):
+        return cls._query(PartnerAppInfo, **kwargs)
 
-    @staticmethod
+    @classmethod
     @switch_function(CLIENT_AUTHENTICATION or SITE_AUTHENTICATION)
-    @AppManager.check_app_id
-    def has_role_for_user(app_id, role):
-        return FATE_CASBIN.has_role_for_user(app_id, role)
+    def generate_app_id(cls, length=8):
+        app_id = generate_random_id(length=length, only_number=True)
+        if cls.query_app(app_id=app_id):
+            cls.generate_app_id()
+        else:
+            return app_id
 
-    @staticmethod
+    @classmethod
     @switch_function(CLIENT_AUTHENTICATION or SITE_AUTHENTICATION)
-    @AppManager.check_app_id
-    def enforcer(app_id, resource, permission):
-        return FATE_CASBIN.enforcer(app_id, resource, permission)
+    def generate_app_token(cls, length=APP_TOKEN_LENGTH):
+        return generate_random_id(length=length)
 
     @staticmethod
-    def check_permission_role(role):
-        if role not in RuntimeConfig.CLIENT_ROLE:
-            raise InvalidParameter(role=role)
+    def check_app_id(func):
+        @wraps(func)
+        def _wrapper(*args, **kwargs):
+            if kwargs.get("app_id"):
+                if not AppManager.query_app(app_id=kwargs.get("app_id")):
+                    raise NoFoundAppid(app_id=kwargs.get("app_id"))
+            return func(*args, **kwargs)
+        return _wrapper
+
+    @staticmethod
+    def check_app_type(func):
+        @wraps(func)
+        def _wrapper(*args, **kwargs):
+            if kwargs.get("app_id"):
+                app_info = AppManager.query_app(app_id=kwargs.get("app_id"))
+                if not app_info:
+                    raise NoFoundAppid(app_id=kwargs.get("app_id"))
+                role = kwargs.get("role")
+                if role == "super_client":
+                    role = "client"
+                if role != app_info[0].f_app_type:
+                    raise RoleTypeError(role=kwargs.get("role"))
+            return func(*args, **kwargs)
+        return _wrapper
```

### Comparing `fate_flow-2.0.0b0/fate_flow/controller/config_manager.py` & `fate_flow-2.1.0/fate_flow/manager/service/config_manager.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/controller/job_controller.py` & `fate_flow-2.1.0/fate_flow/controller/job.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,58 +11,57 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import os
 import shutil
+from copy import deepcopy
 
-from fate_flow.controller.task_controller import TaskController
+from fate_flow.controller.parser import JobParser
+from fate_flow.controller.task import TaskController
 from fate_flow.db import Job
 from fate_flow.engine.storage import Session
-from fate_flow.entity.spec.dag import DAGSchema, JobConfSpec, InheritConfSpec
-from fate_flow.entity.types import EndStatus, JobStatus, TaskStatus
+from fate_flow.entity.spec.dag import DAGSchema, InheritConfSpec, JobConfSpec
+from fate_flow.entity.types import EndStatus, JobStatus, TaskStatus, EngineType, ComputingEngine
 from fate_flow.entity.code import ReturnCode
-from fate_flow.errors.server_error import NoFoundJob, InheritanceFailed
-from fate_flow.manager.metric.metric_manager import OutputMetric
-from fate_flow.manager.model.model_manager import PipelinedModel
-from fate_flow.manager.model.model_meta import ModelMeta
-from fate_flow.manager.service.output_manager import OutputDataTracking
+from fate_flow.errors.server_error import NoFoundJob, JobParamsError
+from fate_flow.manager.outputs.metric import OutputMetric
+from fate_flow.manager.outputs.model import PipelinedModel, ModelMeta
+from fate_flow.manager.outputs.data import OutputDataTracking
 from fate_flow.manager.service.resource_manager import ResourceManager
-from fate_flow.operation.job_saver import JobSaver
-from fate_flow.runtime.runtime_config import RuntimeConfig
-from fate_flow.scheduler.federated_scheduler import FederatedScheduler
+from fate_flow.manager.operation.job_saver import JobSaver
+from fate_flow.controller.federated import FederatedScheduler
+from fate_flow.runtime.job_default_config import JobDefaultConfig
+from fate_flow.runtime.system_settings import ENGINES, IGNORE_RESOURCE_ROLES, PARTY_ID, LOCAL_PARTY_ID, COMPUTING_CONF
+from fate_flow.utils import job_utils
 from fate_flow.utils.base_utils import current_timestamp
 from fate_flow.utils.job_utils import get_job_log_directory, save_job_dag
 from fate_flow.utils.log_utils import schedule_logger
 
 
 class JobController(object):
     @classmethod
-    def request_create_job(cls, dag_schema: dict, user_name: str = None, is_local=False):
-        dag_schema = DAGSchema(**dag_schema)
-        RuntimeConfig.SCHEDULER.check_job_parameters(dag_schema, is_local)
+    def request_create_job(cls, schema: DAGSchema, user_name: str = None, is_local=False):
+        cls.update_job_default_params(schema, is_local=is_local)
+        cls.check_job_params(schema)
         response = FederatedScheduler.request_create_job(
-            party_id=dag_schema.dag.conf.scheduler_party_id,
-            initiator_party_id=dag_schema.dag.conf.initiator_party_id,
-            command_body={
-                "dag_schema": dag_schema.dict(exclude_defaults=True)
-            })
+            party_id=schema.dag.conf.scheduler_party_id,
+            initiator_party_id=schema.dag.conf.initiator_party_id,
+            command_body=schema.dict()
+        )
         if user_name and response.get("code") == ReturnCode.Base.SUCCESS:
             JobSaver.update_job_user(job_id=response.get("job_id"), user_name=user_name)
         if response and isinstance(response, dict) and response.get("code") == ReturnCode.Base.SUCCESS:
-            save_job_dag(job_id=response.get("job_id"), dag=dag_schema.dict(exclude_defaults=True))
+            save_job_dag(job_id=response.get("job_id"), dag=schema.dict(exclude_unset=True))
         return response
 
     @classmethod
-    def request_stop_job(cls, job_id):
+    def request_stop_job(cls, job_id, jobs):
         schedule_logger(job_id).info(f"stop job on this party")
-        jobs = JobSaver.query_job(job_id=job_id)
-        if not jobs:
-            raise NoFoundJob(job_id=job_id)
         status = JobStatus.CANCELED
         kill_status, kill_details = JobController.stop_jobs(job_id=job_id, stop_status=status)
         schedule_logger(job_id).info(f"stop job on this party status {kill_status}")
         schedule_logger(job_id).info(f"request stop job to {status}")
         response = FederatedScheduler.request_stop_job(
             party_id=jobs[0].f_scheduler_party_id,
             job_id=job_id, stop_status=status
@@ -74,35 +73,37 @@
     def request_rerun_job(cls, job):
         schedule_logger(job.f_job_id).info(f"request rerun job {job.f_job_id}")
         response = FederatedScheduler.request_rerun_job(party_id=job.f_scheduler_party_id, job_id=job.f_job_id)
         schedule_logger(job.f_job_id).info(f"rerun job response: {response}")
         return response
 
     @classmethod
-    def create_job(cls, dag_schema: dict, job_id: str, role: str, party_id: str):
+    def create_job(cls, dag, schema_version, job_id: str, role: str, party_id: str):
+        # create job and task
         schedule_logger(job_id).info(f"start create job {job_id} {role} {party_id}")
-        dag_schema = DAGSchema(**dag_schema)
+        dag_schema = DAGSchema(dag=dag, schema_version=schema_version)
         job_info = {
             "job_id": job_id,
             "role": role,
             "party_id": party_id,
             "dag": dag_schema.dict(),
             "progress": 0,
             "parties": [party.dict() for party in dag_schema.dag.parties],
             "initiator_party_id": dag_schema.dag.conf.initiator_party_id,
             "scheduler_party_id": dag_schema.dag.conf.scheduler_party_id,
             "status": JobStatus.READY,
             "model_id": dag_schema.dag.conf.model_id,
             "model_version": dag_schema.dag.conf.model_version
         }
-        party_parameters, task_run, task_cores = RuntimeConfig.SCHEDULER.adapt_party_parameters(dag_schema, role)
+        party_parameters, task_run, task_cores = cls.adapt_party_parameters(dag_schema, role)
         schedule_logger(job_id).info(f"party_job_parameters: {party_parameters}")
         schedule_logger(job_id).info(f"role {role} party_id {party_id} task run: {task_run}, task cores {task_cores}")
         job_info.update(party_parameters)
         JobSaver.create_job(job_info=job_info)
+        # create task
         TaskController.create_tasks(job_id, role, party_id, dag_schema, task_run=task_run, task_cores=task_cores)
 
     @classmethod
     def start_job(cls, job_id, role, party_id, extra_info=None):
         schedule_logger(job_id).info(f"try to start job on {role} {party_id}")
         job_info = {
             "job_id": job_id,
@@ -195,16 +196,16 @@
         query = {'tag': ('!=', 'submit_failed')}
         if job_id:
             query["job_id"] = ('contains', job_id)
         if description:
             query["description"] = ('contains', description)
         if party_id:
             query["party_id"] = ('contains', party_id)
-        if partner:
-            query["partner"] = ('contains', partner)
+        # if partner:
+        #     query["parties"] = ('contains', partner)
         if role:
             query["role"] = ('in_', set(role))
         if status:
             query["status"] = ('in_', set(status))
         by = []
         if order_by:
             by.append(order_by)
@@ -212,21 +213,25 @@
             by.append(order)
         if not by:
             by = ['create_time', 'desc']
         if user_name:
             query["user_name"] = ("==", user_name)
         jobs, count = JobSaver.list_job(limit, offset, query, by)
         jobs = [job.to_human_model_dict() for job in jobs]
+        lst_job = []
         for job in jobs:
             job['partners'] = set()
             for _r in job['parties']:
                 job['partners'].update(_r.get("party_id"))
             job['partners'].discard(job['party_id'])
             job['partners'] = sorted(job['partners'])
-        return count, jobs
+            if partner and str(partner) not in job['partners']:
+                continue
+            lst_job.append(job)
+        return count, lst_job
 
     @classmethod
     def query_task_list(cls, limit, page, job_id, role, party_id, task_name, order_by, order):
         offset = limit * (page - 1)
 
         query = {}
         if job_id:
@@ -274,21 +279,22 @@
             raise NoFoundJob(job_id=job_id)
         FederatedScheduler.request_stop_job(
             party_id=jobs[0].f_scheduler_party_id,job_id=jobs[0].f_job_id, stop_status=JobStatus.CANCELED
         )
         for task in tasks:
             # metric
             try:
-                OutputMetric(job_id=task.f_job_id, role=task.f_role, party_id=task.f_party_id,
-                             task_name=task.f_task_name,
-                             task_id=task.f_task_id, task_version=task.f_task_version).delete_metrics()
+                OutputMetric(
+                    job_id=task.f_job_id, role=task.f_role, party_id=task.f_party_id, task_name=task.f_task_name,
+                    task_id=task.f_task_id, task_version=task.f_task_version
+                ).delete_metrics()
                 schedule_logger(task.f_job_id).info(f'delete {task.f_job_id} {task.f_role} {task.f_party_id}'
                                                     f' {task.f_task_name} metric data success')
             except Exception as e:
-                pass
+                schedule_logger(job_id).exception(e)
 
             # data
             try:
                 datas = OutputDataTracking.query(
                     job_id=task.f_job_id,
                     role=task.f_role,
                     party_id=task.f_party_id,
@@ -298,68 +304,145 @@
                 )
                 with Session() as sess:
                     for data in datas:
                         table = sess.get_table(name=data.f_name, namespace=data.f_namespace)
                         if table:
                             table.destroy()
             except Exception as e:
-                pass
+                schedule_logger(job_id).exception(e)
 
             # model
             try:
                 PipelinedModel.delete_model(job_id=task.f_job_id, role=task.f_role,
                                             party_id=task.f_party_id, task_name=task.f_task_name)
                 schedule_logger(task.f_job_id).info(f'delete {task.f_job_id} {task.f_role} {task.f_party_id}'
                                                     f' {task.f_task_name} model success')
             except Exception as e:
-                pass
-        # JobSaver.delete_job(job_id=job_id)
+                schedule_logger(job_id).exception(e)
+
+        try:
+            JobSaver.delete_job(job_id=job_id)
+        except Exception as e:
+            schedule_logger(job_id).exception(e)
+
+        try:
+            JobSaver.delete_task(job_id=job_id)
+        except Exception as e:
+            schedule_logger(job_id).exception(e)
 
     @staticmethod
     def add_notes(job_id, role, party_id, notes):
         job_info = {
             "job_id": job_id,
             "role": role,
             "party_id": party_id,
             "description": notes
         }
         return JobSaver.update_job(job_info)
 
-
-class JobInheritance:
     @classmethod
-    def check(cls, inheritance: InheritConfSpec = None):
-        if not inheritance:
-            return
-        if not inheritance.task_list:
-            raise InheritanceFailed(
-                task_list=inheritance.task_list,
-                position="dag_schema.dag.conf.inheritance.task_list"
-            )
-        inheritance_jobs = JobSaver.query_job(job_id=inheritance.job_id)
-        inheritance_tasks = JobSaver.query_task(job_id=inheritance.job_id)
-        if not inheritance_jobs:
-            raise InheritanceFailed(job_id=inheritance.job_id, detail=f"no found job {inheritance.job_id}")
-        task_status = {}
-        for task in inheritance_tasks:
-            task_status[task.f_task_name] = task.f_status
-
-        for task_name in inheritance.task_list:
-            if task_name not in task_status.keys():
-                raise InheritanceFailed(job_id=inheritance.job_id, task_name=task_name, detail="no found task name")
-            elif task_status[task_name] not in [TaskStatus.SUCCESS, TaskStatus.PASS]:
-                raise InheritanceFailed(
-                    job_id=inheritance.job_id,
-                    task_name=task_name,
-                    task_status=task_status[task_name],
-                    detail=f"task status need in [{TaskStatus.SUCCESS}, {TaskStatus.PASS}]"
+    def data_view(cls, job_id, role, party_id):
+        jobs = JobSaver.query_job(job_id=job_id, role=role, party_id=party_id)
+        if not jobs:
+            raise NoFoundJob(job_id=job_id, role=role, party_id=party_id)
+        job = jobs[0]
+        dag = DAGSchema(**job.f_dag)
+        job_parser = JobParser(dag)
+        data_view = {}
+        for party in dag.dag.parties:
+            data_view[party.role] = {}
+            for party_id in party.party_id:
+                dataset = job_parser.dataset_list(party.role, party_id)
+                data_view[party.role][party_id] = [data.to_dict() for data in dataset]
+        return dict(role=role, party_id=party_id, data_view=data_view)
+
+    @classmethod
+    def adapt_party_parameters(cls, dag_schema: DAGSchema, role):
+        cores, task_run, task_cores = cls.calculate_resource(dag_schema, role)
+        job_info = {"cores": cores, "remaining_cores": cores}
+        if dag_schema.dag.conf.inheritance:
+            job_info.update({"inheritance": dag_schema.dag.conf.inheritance.dict()})
+        return job_info, task_run, task_cores
+
+    @classmethod
+    def calculate_resource(cls, dag_schema: DAGSchema, role):
+        cores = dag_schema.dag.conf.cores if dag_schema.dag.conf.cores else JobDefaultConfig.job_cores
+        if dag_schema.dag.conf.task and dag_schema.dag.conf.task.engine_run:
+            task_run = dag_schema.dag.conf.task.engine_run
+        else:
+            task_run = {}
+
+        task_cores = cores
+
+        default_task_run = deepcopy(JobDefaultConfig.task_run.get(ENGINES.get(EngineType.COMPUTING), {}))
+
+        if ENGINES.get(EngineType.COMPUTING) == ComputingEngine.SPARK:
+            if "num-executors" not in task_run:
+                task_run["num-executors"] = default_task_run.get("num-executors")
+            if "executor-cores" not in task_run:
+                task_run["executor-cores"] = default_task_run.get("executor-cores")
+            if role in IGNORE_RESOURCE_ROLES:
+                task_run["num-executors"] = 1
+                task_run["executor-cores"] = 1
+            task_cores = int(task_run.get("num-executors")) * (task_run.get("executor-cores"))
+
+        if ENGINES.get(EngineType.COMPUTING) == ComputingEngine.EGGROLL:
+            total_cores = task_run.get("cores", None) or default_task_run.get("cores")
+
+            task_run["nodes"] = COMPUTING_CONF.get(ComputingEngine.EGGROLL).get("nodes")
+            task_run["task_cores_per_node"] = max(total_cores // task_run["nodes"], 1)
+            task_cores = task_run["task_cores_per_node"] * task_run["nodes"]
+
+            if role in IGNORE_RESOURCE_ROLES:
+                task_run["task_cores_per_node"] = 1
+
+        if ENGINES.get(EngineType.COMPUTING) == ComputingEngine.STANDALONE:
+            task_cores = task_run["cores"] = task_run.pop("cores", None) or default_task_run.get("cores")
+            if role in IGNORE_RESOURCE_ROLES:
+                task_run["cores"] = 1
+        if role in IGNORE_RESOURCE_ROLES:
+            cores = 0
+            task_cores = 0
+
+        if task_cores > cores:
+            cores = task_cores
+        return cores, task_run, task_cores
+
+    @classmethod
+    def check_job_params(cls, dag_schema: DAGSchema):
+        # check inheritance
+        job_utils.inheritance_check(dag_schema.dag.conf.inheritance)
+
+        # check model warehouse
+        model_warehouse = dag_schema.dag.conf.model_warehouse
+        if model_warehouse:
+            if not ModelMeta.query(model_id=model_warehouse.model_id, model_version=model_warehouse.model_version):
+                raise JobParamsError(
+                    model_id=model_warehouse.model_id,
+                    model_version=model_warehouse.model_version,
+                    position="dag_schema.dag.conf.model_warehouse"
                 )
-        # todo: parsing and judging whether job can be inherited
 
     @classmethod
+    def update_job_default_params(cls, dag_schema: DAGSchema, is_local: bool = False):
+        if not dag_schema.dag.conf:
+            dag_schema.dag.conf = JobConfSpec()
+        dag_schema.dag.conf.initiator_party_id = PARTY_ID
+        if not dag_schema.dag.conf.scheduler_party_id:
+            if not is_local:
+                dag_schema.dag.conf.scheduler_party_id = PARTY_ID
+            else:
+                dag_schema.dag.conf.scheduler_party_id = LOCAL_PARTY_ID
+        if not dag_schema.dag.conf.computing_partitions:
+            dag_schema.dag.conf.computing_partitions = JobDefaultConfig.computing_partitions
+        return dag_schema
+
+
+class JobInheritance:
+    @classmethod
     def load(cls, job: Job):
         # load inheritance: data、model、metric、logs
         inheritance = InheritConfSpec(**job.f_inheritance)
         source_task_list = JobSaver.query_task(job_id=inheritance.job_id, role=job.f_role, party_id=job.f_party_id)
         task_list = JobSaver.query_task(job_id=job.f_job_id, role=job.f_role, party_id=job.f_party_id)
         target_task_list = [task for task in task_list if task.f_task_name in inheritance.task_list]
         cls.load_logs(job, inheritance)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/controller/task_controller.py` & `fate_flow-2.1.0/fate_flow/controller/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,182 +14,191 @@
 #  limitations under the License.
 #
 import copy
 import os
 
 import yaml
 
+from fate_flow.controller.parser import JobParser
 from fate_flow.db.db_models import Task
 from fate_flow.db.schedule_models import ScheduleTask, ScheduleJob, ScheduleTaskStatus
-from fate_flow.engine.devices import build_engine
-from fate_flow.entity.spec.dag import DAGSchema, LauncherSpec
-from fate_flow.hub.flow_hub import FlowHub
+from fate_flow.engine.devices import build_engine, EngineABC
+from fate_flow.entity.spec.dag import DAGSchema
 from fate_flow.manager.service.resource_manager import ResourceManager
 from fate_flow.manager.service.worker_manager import WorkerManager
-from fate_flow.runtime.job_default_config import JobDefaultConfig
 from fate_flow.runtime.runtime_config import RuntimeConfig
-from fate_flow.scheduler.federated_scheduler import FederatedScheduler
+from fate_flow.controller.federated import FederatedScheduler
 from fate_flow.entity.types import EndStatus, TaskStatus, FederatedCommunicationType, LauncherType
 from fate_flow.entity.code import FederatedSchedulingStatusCode
-from fate_flow.operation.job_saver import JobSaver, ScheduleJobSaver
+from fate_flow.manager.operation.job_saver import JobSaver, ScheduleJobSaver
 from fate_flow.utils import job_utils
-from fate_flow.utils.base_utils import current_timestamp, json_dumps
+from fate_flow.utils.base_utils import current_timestamp
 from fate_flow.utils.log_utils import schedule_logger
+from fate_flow.utils.wraps_utils import asynchronous_function
 
 
 class TaskController(object):
     INITIATOR_COLLECT_FIELDS = ["status", "party_status", "start_time", "update_time", "end_time", "elapsed"]
 
     @classmethod
     def create_tasks(cls, job_id: str, role: str, party_id: str, dag_schema: DAGSchema, task_run=None, task_cores=None,
                      is_scheduler=False):
         schedule_logger(job_id).info(f"start create {'scheduler' if is_scheduler else 'partner'} tasks ...")
-        job_parser = FlowHub.load_job_parser(dag_schema)
-        task_list = job_parser.topological_sort()
+        job_parser = JobParser(dag_schema)
+        task_list = job_parser.global_topological_sort()
         for task_name in task_list:
-            cls.create_task(job_id, role, party_id, task_name, dag_schema, job_parser, task_run=task_run,
-                            is_scheduler=is_scheduler, task_cores=task_cores)
+            parties = job_parser.get_task_runtime_parties(task_name=task_name)
+            need_run = job_utils.check_party_in(role, party_id, parties)
+            schedule_logger(job_id).info(f"task {task_name} role {role} party id {party_id} need run status {need_run}")
+            if need_run:
+                cls.create_task(job_id, role, party_id, task_name, dag_schema, job_parser, task_run=task_run,
+                                is_scheduler=is_scheduler, task_cores=task_cores)
         schedule_logger(job_id).info("create tasks success")
 
     @classmethod
     def create_task(cls, job_id, role, party_id, task_name, dag_schema, job_parser, is_scheduler, task_run=None,
                     task_cores=None, task_version=0):
         task_id = job_utils.generate_task_id(job_id=job_id, component_name=task_name)
         execution_id = job_utils.generate_session_id(task_id, task_version, role, party_id)
-        task_node = job_parser.get_task_node(task_name=task_name)
+        task_node = job_parser.get_task_node(role=role, party_id=party_id, task_name=task_name)
         task_parser = job_parser.task_parser(
             task_node=task_node, job_id=job_id, task_name=task_name, role=role, party_id=party_id,
-            task_id=task_id, execution_id=execution_id, task_version=task_version, parties=dag_schema.dag.parties,
+            task_id=task_id, execution_id=execution_id, task_version=task_version,
+            parties=job_parser.get_task_runtime_parties(task_name),
             model_id=dag_schema.dag.conf.model_id, model_version=dag_schema.dag.conf.model_version
         )
-        need_run = task_parser.need_run
-        schedule_logger(job_id).info(f"task {task_name} role {role} part id {party_id} need run status {need_run}")
         if is_scheduler:
-            if need_run:
-                task = ScheduleTask()
-                task.f_job_id = job_id
-                task.f_role = role
-                task.f_party_id = party_id
-                task.f_task_name = task_name
-                task.f_component = task_parser.component_ref
-                task.f_task_id = task_id
-                task.f_task_version = task_version
-                task.f_status = TaskStatus.WAITING
-                task.f_parties = [party.dict() for party in dag_schema.dag.parties]
-                ScheduleJobSaver.create_task(task.to_human_model_dict())
+            task = ScheduleTask()
+            task.f_job_id = job_id
+            task.f_role = role
+            task.f_party_id = party_id
+            task.f_task_name = task_name
+            task.f_component = task_parser.component_ref
+            task.f_task_id = task_id
+            task.f_task_version = task_version
+            task.f_status = TaskStatus.WAITING
+            task.f_parties = [party.dict() for party in dag_schema.dag.parties]
+            ScheduleJobSaver.create_task(task.to_human_model_dict())
         else:
             task_parameters = task_parser.task_parameters
+            if task_parser.engine_run:
+                task_run.update(task_parser.engine_run)
             task_parameters.engine_run = task_run
             task_parameters.computing_partitions = dag_schema.dag.conf.computing_partitions
             schedule_logger(job_id).info(f"task {task_name} role {role} part id {party_id} task_parameters"
                                          f" {task_parameters.dict()}, provider: {task_parser.provider}")
             task = Task()
             task.f_job_id = job_id
             task.f_role = role
             task.f_party_id = party_id
             task.f_task_name = task_name
             task.f_component = task_parser.component_ref
             task.f_task_id = task_id
             task.f_task_version = task_version
             task.f_scheduler_party_id = dag_schema.dag.conf.scheduler_party_id
-            task.f_status = TaskStatus.WAITING if need_run else TaskStatus.PASS
+            task.f_status = TaskStatus.WAITING
             task.f_party_status = TaskStatus.WAITING
             task.f_execution_id = execution_id
             task.f_provider_name = task_parser.provider
+            task.f_timeout = task_parser.timeout
             task.f_sync_type = dag_schema.dag.conf.sync_type
             task.f_task_run = task_run
             task.f_task_cores = task_cores
             cls.update_local(task)
             cls.update_launcher_config(task, task_parser.task_runtime_launcher, task_parameters)
             task.f_component_parameters = task_parameters.dict()
-            JobSaver.create_task(task.to_human_model_dict())
+            status = JobSaver.create_task(task.to_human_model_dict())
+            schedule_logger(job_id).info(task.to_human_model_dict())
+            schedule_logger(job_id).info(status)
 
     @staticmethod
     def update_local(task):
         # HA need route to local
         if task.f_role == "local":
             task.f_run_ip = RuntimeConfig.JOB_SERVER_HOST
             task.f_run_port = RuntimeConfig.HTTP_PORT
 
     @staticmethod
-    def update_launcher_config(task, task_runtime_launcher, task_parameters):
+    def update_launcher_config(task, launcher_name, task_parameters):
         # support deepspeed and other launcher
-        schedule_logger(task.f_job_id).info(f"task runtime launcher: {task_runtime_launcher}")
-        launcher = LauncherSpec.parse_obj(task_runtime_launcher)
-        if launcher.name and launcher.name != LauncherType.DEFAULT:
-            task_parameters.launcher_name = task.f_launcher_name = launcher.name
-            launcher_conf = copy.deepcopy(JobDefaultConfig.launcher.get(task_parameters.launcher_name))
-            if launcher.conf:
-                launcher_conf.update(launcher.conf)
-            task_parameters.launcher_conf = task.f_launcher_conf = launcher_conf
+        # if task.f_role == "arbiter":
+        #     return
+        schedule_logger(task.f_job_id).info(f"task runtime launcher name: {launcher_name}")
+        if launcher_name and launcher_name != LauncherType.DEFAULT:
+            task_parameters.launcher_name = task.f_launcher_name = launcher_name
 
     @staticmethod
     def create_schedule_tasks(job: ScheduleJob, dag_schema):
         for party in job.f_parties:
             role = party.get("role")
             party_ids = party.get("party_id")
             for party_id in party_ids:
                 TaskController.create_tasks(job.f_job_id, role, party_id, dag_schema, is_scheduler=True)
         TaskController.create_scheduler_tasks_status(job.f_job_id, dag_schema)
 
     @classmethod
     def create_scheduler_tasks_status(cls, job_id, dag_schema, task_version=0, auto_retries=None, task_name=None):
         schedule_logger(job_id).info("start create schedule task status info")
-        job_parser = FlowHub.load_job_parser(dag_schema)
+        job_parser = JobParser(dag_schema)
         if task_name:
             task_list = [task_name]
         else:
-            task_list = job_parser.topological_sort()
+            task_list = job_parser.global_topological_sort()
         for _task_name in task_list:
             task_info = {
                 "job_id": job_id,
                 "task_name": _task_name,
                 "task_id": job_utils.generate_task_id(job_id=job_id, component_name=_task_name),
                 "task_version": task_version,
                 "status": TaskStatus.WAITING,
                 "auto_retries": dag_schema.dag.conf.auto_retries if auto_retries is None else auto_retries,
                 "sync_type": dag_schema.dag.conf.sync_type
             }
             ScheduleJobSaver.create_task_scheduler_status(task_info)
         schedule_logger(job_id).info("create schedule task status success")
 
     @classmethod
-    def start_task(cls, job_id, role, party_id, task_id, task_version):
+    def start_task(cls, task: Task):
+        job_id = task.f_job_id
+        role = task.f_role
+        party_id = task.f_party_id
+        task_id = task.f_task_id
+        task_version = task.f_task_version
         schedule_logger(job_id).info(
             f"try to start task {task_id} {task_version} on {role} {party_id} executor subprocess")
         task_executor_process_start_status = False
         task_info = {
             "job_id": job_id,
             "task_id": task_id,
             "task_version": task_version,
             "role": role,
             "party_id": party_id,
         }
         is_failed = False
         try:
-            task = JobSaver.query_task(task_id=task_id, task_version=task_version, role=role, party_id=party_id)[0]
             run_parameters = task.f_component_parameters
             schedule_logger(job_id).info(f"task run parameters: {run_parameters}")
             task_executor_process_start_status = False
 
             config_dir = job_utils.get_task_directory(
                 job_id, role, party_id, task.f_task_name, task.f_task_version, input=True
             )
             os.makedirs(config_dir, exist_ok=True)
             run_parameters_path = os.path.join(config_dir, 'preprocess_parameters.yaml')
             with open(run_parameters_path, 'w') as fw:
                 yaml.dump(run_parameters, fw)
-            backend_engine = build_engine(task.f_provider_name)
-            run_info = backend_engine.run(task=task,
-                                          run_parameters=run_parameters,
-                                          run_parameters_path=run_parameters_path,
-                                          config_dir=config_dir,
-                                          log_dir=job_utils.get_job_log_directory(job_id, role, party_id,
-                                                                                  task.f_task_name),
-                                          cwd_dir=job_utils.get_job_directory(job_id, role, party_id, task.f_task_name))
+            backend_engine = cls.build_task_engine(task.f_provider_name, task.f_launcher_name)
+            run_info = backend_engine.run(
+                task=task,
+                run_parameters=run_parameters,
+                run_parameters_path=run_parameters_path,
+                config_dir=config_dir,
+                log_dir=job_utils.get_job_log_directory(job_id, role, party_id, task.f_task_name),
+                cwd_dir=job_utils.get_job_directory(job_id, role, party_id, task.f_task_name)
+            )
             task_info.update(run_info)
             task_info["start_time"] = current_timestamp()
             task_executor_process_start_status = True
         except Exception as e:
             schedule_logger(job_id).exception(e)
             is_failed = True
         finally:
@@ -199,53 +208,68 @@
                 cls.update_task_status(task_info=task_info)
                 if is_failed:
                     task_info["party_status"] = TaskStatus.FAILED
                     cls.update_task_status(task_info=task_info)
             except Exception as e:
                 schedule_logger(job_id).exception(e)
             schedule_logger(job_id).info(
-                "task {} {} on {} {} executor subprocess start {}".format(task_id, task_version, role, party_id,
-                                                                          "success" if task_executor_process_start_status else "failed"))
+                "task {} {} on {} {} executor subprocess start {}".format(
+                    task_id, task_version, role, party_id, "success" if task_executor_process_start_status else "failed"
+                ))
         return not is_failed
 
     @classmethod
     def create_new_version_task(cls, task: Task, new_version):
         jobs = JobSaver.query_job(job_id=task.f_job_id, role=task.f_role, party_id=task.f_party_id)
         if not jobs:
             return False
         dag_schema = DAGSchema(**jobs[0].f_dag)
-        job_parser = FlowHub.load_job_parser(dag_schema)
+        job_parser = JobParser(dag_schema)
         cls.create_task(
             task.f_job_id, task.f_role, task.f_party_id, task.f_task_name, dag_schema, job_parser,
             task_run=task.f_task_run, task_cores=task.f_task_cores, is_scheduler=False, task_version=new_version
         )
 
     @classmethod
     def create_new_version_schedule_task(cls, job, task, auto):
         # stop old version task
         FederatedScheduler.stop_task(task_id=task.f_task_id, command_body={"status": task.f_status})
         # create new version task
-        task.f_task_version = task.f_task_version + 1
         if auto:
             task.f_auto_retries = task.f_auto_retries - 1
-        status_code, response = FederatedScheduler.rerun_task(task_id=task.f_task_id, task_version=task.f_task_version)
+        retry_time = 3
+        new_version = task.f_task_version
+        while True:
+            if retry_time == 0:
+                raise Exception(f"create {task.f_task_id} new version {new_version} failed")
+            new_version = new_version + 1
+            status_code, response = FederatedScheduler.rerun_task(task_id=task.f_task_id, task_version=new_version)
+            if status_code == FederatedSchedulingStatusCode.SUCCESS:
+                schedule_logger(job_id=job.f_job_id).info(
+                    f"create {task.f_task_id} new version {new_version} success"
+                )
+                break
+            retry_time -= 1
         dag_schema = DAGSchema(**job.f_dag)
-        if status_code != FederatedSchedulingStatusCode.SUCCESS:
-            raise Exception(f"create {task.f_task_id} new version failed")
-        job_parser = FlowHub.load_job_parser(dag_schema)
-        for party in job.f_parties:
-            _role = party.get("role")
-            for _party_id in party.get("party_id"):
+        job_parser = JobParser(dag_schema)
+        parties = job_parser.get_task_runtime_parties(task_name=task.f_task_name)
+        for party in parties:
+            for party_id in party.party_id:
                 cls.create_task(
-                    job.f_job_id, _role, _party_id, task.f_task_name, dag_schema, job_parser,
-                    is_scheduler=True, task_version=task.f_task_version
+                    job.f_job_id, party.role, party_id, task.f_task_name, dag_schema, job_parser,
+                    is_scheduler=True, task_version=new_version
                 )
-        TaskController.create_scheduler_tasks_status(job.f_job_id, dag_schema, task_version=task.f_task_version,
-                                                     auto_retries=task.f_auto_retries, task_name=task.f_task_name)
-        schedule_logger(job.f_job_id).info(f"create task {task.f_task_id} new version {task.f_task_version} successfully")
+        TaskController.create_scheduler_tasks_status(
+            job.f_job_id,
+            dag_schema,
+            task_version=new_version,
+            auto_retries=task.f_auto_retries,
+            task_name=task.f_task_name
+        )
+        schedule_logger(job.f_job_id).info(f"create task {task.f_task_id} new version {new_version} successfully")
 
     @classmethod
     def prepare_rerun_task(cls, job: ScheduleJob, task: ScheduleTaskStatus, auto=False, force=False):
         job_id = job.f_job_id
         can_rerun = False
         if force:
             can_rerun = True
@@ -272,34 +296,37 @@
         except Exception as e:
             schedule_logger(task_info["job_id"]).exception(e)
         finally:
             return update_status
 
     @classmethod
     def update_task_status(cls, task_info, scheduler_party_id=None, sync_type=None):
-        if not scheduler_party_id or not sync_type:
-            task = JobSaver.query_task(
-                task_id=task_info.get("task_id"),
-                task_version=task_info.get("task_version")
-            )[0]
-            scheduler_party_id, sync_type = task.f_scheduler_party_id, task.f_sync_type
+        task = JobSaver.query_task(
+            task_id=task_info.get("task_id"),
+            task_version=task_info.get("task_version"),
+            role=task_info.get("role"),
+            party_id=task_info.get("party_id")
+        )[0]
+        scheduler_party_id, sync_type = task.f_scheduler_party_id, task.f_sync_type
         update_status = JobSaver.update_task_status(task_info=task_info)
         if update_status and EndStatus.contains(task_info.get("party_status")):
             ResourceManager.return_task_resource(**task_info)
         if "party_status" in task_info:
             report_task_info = {
                 "job_id": task_info.get("job_id"),
                 "role": task_info.get("role"),
                 "party_id": task_info.get("party_id"),
                 "task_id": task_info.get("task_id"),
                 "task_version": task_info.get("task_version"),
                 "status": task_info.get("party_status")
             }
             if sync_type == FederatedCommunicationType.CALLBACK:
                 cls.report_task_to_scheduler(task_info=report_task_info, scheduler_party_id=scheduler_party_id)
+        if update_status and EndStatus.contains(task_info.get("party_status")):
+            cls.callback_task_output(task)
         return update_status
 
     @classmethod
     def report_task_to_scheduler(cls, task_info, scheduler_party_id):
         FederatedScheduler.report_task_to_scheduler(party_id=scheduler_party_id, command_body=task_info)
 
     @classmethod
@@ -308,14 +335,15 @@
                                     party_id=party_id)
         if tasks:
             return tasks[0].to_human_model_dict(only_primary_with=cls.INITIATOR_COLLECT_FIELDS)
         else:
             return None
 
     @classmethod
+    @asynchronous_function
     def stop_task(cls, task: Task, stop_status):
         kill_status = cls.kill_task(task=task)
         task_info = {
             "job_id": task.f_job_id,
             "task_id": task.f_task_id,
             "task_version": task.f_task_version,
             "role": task.f_role,
@@ -327,36 +355,48 @@
         cls.update_task(task_info=task_info)
         return kill_status
 
     @classmethod
     def kill_task(cls, task: Task):
         kill_status = False
         try:
-            backend_engine = build_engine(task.f_provider_name)
+            backend_engine = cls.build_task_engine(task.f_provider_name, task.f_launcher_name)
             if backend_engine:
                 backend_engine.kill(task)
                 backend_engine.cleanup(task)
             WorkerManager.kill_task_all_workers(task)
         except Exception as e:
             schedule_logger(task.f_job_id).exception(e)
         else:
             kill_status = True
         finally:
             schedule_logger(task.f_job_id).info(
-                'task {} {} on {} {} process {} kill {}'.format(task.f_task_id,
-                                                                task.f_task_version,
-                                                                task.f_role,
-                                                                task.f_party_id,
-                                                                task.f_run_pid,
-                                                                'success' if kill_status else 'failed'))
+                'task {} {} on {} {} process {} kill {}'.format(
+                    task.f_task_id,
+                    task.f_task_version,
+                    task.f_role,
+                    task.f_party_id,
+                    task.f_run_pid,
+                    'success' if kill_status else 'failed'
+                ))
             return kill_status
 
     @classmethod
     def clean_task(cls, task):
         try:
-            backend_engine = build_engine(task.f_provider_name)
+            backend_engine = cls.build_task_engine(task.f_provider_name, task.f_launcher_name)
             if backend_engine:
                 schedule_logger(task.f_job_id).info(f"start clean task:[{task.f_task_id} {task.f_task_version}]")
                 backend_engine.cleanup(task)
             WorkerManager.kill_task_all_workers(task)
         except Exception as e:
             schedule_logger(task.f_job_id).exception(e)
+
+    @classmethod
+    def build_task_engine(cls, provider_name, launcher_name=LauncherType.DEFAULT) -> EngineABC:
+        return build_engine(provider_name, launcher_name)
+
+    @classmethod
+    def callback_task_output(cls, task: Task):
+        if task.f_launcher_name == LauncherType.DEEPSPEED:
+            engine = cls.build_task_engine(provider_name=task.f_provider_name, launcher_name=task.f_launcher_name)
+            engine.download_output(task)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/db/__init__.py` & `fate_flow-2.1.0/fate_flow/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/db/base_models.py` & `fate_flow-2.1.0/fate_flow/db/base_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,14 +423,15 @@
                 raise Exception("Create {} failed".format(entity_model))
             return obj
         except peewee.IntegrityError as e:
             # if e.args[0] == 1062 or (isinstance(e.args[0], str) and "UNIQUE constraint failed" in e.args[0]):
             #     sql_logger(job_id=entity_info.get("job_id", "fate_flow")).warning(e)
             # else:
             #     raise Exception("Create {} failed:\n{}".format(entity_model, e))
+            # raise Exception(e)
             pass
         except Exception as e:
             raise Exception("Create {} failed:\n{}".format(entity_model, e))
 
     @classmethod
     @DB.connection_context()
     def _query(cls, entity_model, force=False, **kwargs):
```

### Comparing `fate_flow-2.0.0b0/fate_flow/db/casbin_models.py` & `fate_flow-2.1.0/fate_flow/db/casbin_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def add_policy(self, sec, ptype, rule):
         """adds a policy rule to the storage."""
         self._save_policy_line(ptype, rule)
 
     def remove_policy(self, sec, ptype, rule):
         """removes a policy rule from the storage."""
         if sec in ["p", "g"]:
-            condition = [self.rule.ptype==ptype]
+            condition = [self.rule.ptype == ptype]
             data = dict(zip(['v0', 'v1', 'v2', 'v3', 'v4', 'v5'], rule))
             condition.extend([getattr(self.rule, k) == data[k] for k in data])
             check = self.rule.select().filter(*condition)
             if check.exists():
                 self.rule.delete().where(*condition).execute()
                 return True
             else:
@@ -78,14 +78,15 @@
         """
         pass
 
 
 class FlowCasbinRule(pw.Model):
     class Meta:
         table_name = CASBIN_TABLE_NAME
+
     ptype = pw.CharField(max_length=255, null=True)
     v0 = pw.CharField(max_length=255, null=True)
     v1 = pw.CharField(max_length=255, null=True)
     v2 = pw.CharField(max_length=255, null=True)
     v3 = pw.CharField(max_length=255, null=True)
     v4 = pw.CharField(max_length=255, null=True)
     v5 = pw.CharField(max_length=255, null=True)
@@ -99,14 +100,15 @@
             return "<{cls}: {desc}>".format(cls=self.__class__.__name__, desc=self)
         return "<{cls} {pk}: {desc}>".format(cls=self.__class__.__name__, pk=self.id, desc=self)
 
 
 class PermissionCasbinRule(pw.Model):
     class Meta:
         table_name = PERMISSION_TABLE_NAME
+
     ptype = pw.CharField(max_length=255, null=True)
     v0 = pw.CharField(max_length=255, null=True)
     v1 = pw.CharField(max_length=255, null=True)
     v2 = pw.CharField(max_length=255, null=True)
     v3 = pw.CharField(max_length=255, null=True)
     v4 = pw.CharField(max_length=255, null=True)
     v5 = pw.CharField(max_length=255, null=True)
@@ -235,9 +237,16 @@
     def enforce(self, party_id, type, value):
         try:
             return self.re.enforce(party_id, type, str(value))
         except Exception as e:
             raise Exception(f"{party_id}, {type}, {value} {e}")
 
 
-FATE_CASBIN = FateCasbin()
-PERMISSION_CASBIN = PermissionCasbin()
+FATE_CASBIN = None
+PERMISSION_CASBIN = None
+
+
+def init_casbin():
+    global FATE_CASBIN
+    global PERMISSION_CASBIN
+    FATE_CASBIN = FateCasbin()
+    PERMISSION_CASBIN = PermissionCasbin()
```

### Comparing `fate_flow-2.0.0b0/fate_flow/db/db_models.py` & `fate_flow-2.1.0/fate_flow/db/db_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import datetime
 
 from peewee import CharField, TextField, BigIntegerField, IntegerField, BooleanField, CompositeKey, BigAutoField
 from fate_flow.db.base_models import DataBaseModel, JSONField
+from fate_flow.entity.types import PROTOCOL
 
 
 class Job(DataBaseModel):
+    f_protocol = CharField(max_length=50, default=PROTOCOL.FATE_FLOW)
+    f_flow_id = CharField(max_length=25, default='')
     f_job_id = CharField(max_length=25, index=True)
     f_user_name = CharField(max_length=500, null=True, default='')
     f_description = TextField(null=True, default='')
     f_tag = CharField(max_length=50, null=True, default='')
     f_dag = JSONField()
     f_parties = JSONField()
 
@@ -56,14 +59,15 @@
 
     class Meta:
         db_table = "t_job"
         primary_key = CompositeKey('f_job_id', 'f_role', 'f_party_id')
 
 
 class Task(DataBaseModel):
+    f_protocol = CharField(max_length=50, default=PROTOCOL.FATE_FLOW)
     f_job_id = CharField(max_length=25, index=True)
     f_role = CharField(max_length=50, index=True)
     f_party_id = CharField(max_length=50, index=True)
     f_task_name = CharField(max_length=50)
     f_component = CharField(max_length=50)
     f_task_id = CharField(max_length=100)
     f_task_version = BigIntegerField()
@@ -85,17 +89,17 @@
     f_party_status = CharField(max_length=50)
     f_provider_name = CharField(max_length=50)
     f_task_parameters = JSONField(null=True)
     f_engine_conf = JSONField(null=True)
     f_kill_status = BooleanField(default=False)
     f_error_report = TextField(default="")
     f_sync_type = CharField(max_length=20)
+    f_timeout = IntegerField(null=True)
 
     f_launcher_name = CharField(max_length=20, null=True)
-    f_launcher_conf = JSONField(null=True)
 
     f_start_time = BigIntegerField(null=True)
     f_end_time = BigIntegerField(null=True)
     f_elapsed = BigIntegerField(null=True)
 
     class Meta:
         db_table = "t_task"
@@ -200,24 +204,25 @@
 
     class Meta:
         db_table = "t_provider_info"
 
 
 class ComponentInfo(DataBaseModel):
     f_provider_name = CharField(max_length=100)
+    f_protocol = CharField(max_length=20, default=PROTOCOL.FATE_FLOW)
     f_name = CharField(max_length=20, index=True)
     f_version = CharField(max_length=20)
     f_device = CharField(max_length=20)
     f_component_name = CharField(max_length=50)
     f_component_entrypoint = JSONField(null=True)
-    f_component_params = JSONField(null=True)
+    f_component_description = JSONField(null=True)
 
     class Meta:
         db_table = "t_component_info"
-        primary_key = CompositeKey("f_provider_name", "f_component_name")
+        primary_key = CompositeKey("f_provider_name", "f_component_name", "f_protocol")
 
 
 class PipelineModelMeta(DataBaseModel):
     f_model_id = CharField(max_length=100)
     f_model_version = CharField(max_length=10)
     f_job_id = CharField(max_length=25, index=True)
     f_role = CharField(max_length=50, index=True)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/db/permission_models.py` & `fate_flow-2.1.0/fate_flow/db/permission_models.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/db/schedule_models.py` & `fate_flow-2.1.0/fate_flow/db/schedule_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from peewee import CharField, TextField, IntegerField, BooleanField, BigIntegerField, CompositeKey
 
 from fate_flow.db.base_models import DataBaseModel, JSONField
+from fate_flow.entity.types import PROTOCOL
 
 
 class ScheduleJob(DataBaseModel):
+    f_protocol = CharField(max_length=50, default=PROTOCOL.FATE_FLOW)
     f_job_id = CharField(max_length=25, index=True)
     f_priority = IntegerField(default=0)
     f_tag = CharField(max_length=50, null=True, default='')
     f_dag = JSONField(null=True)
     f_parties = JSONField()
     f_initiator_party_id = CharField(max_length=50)
     f_scheduler_party_id = CharField(max_length=50)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/db/storage_models.py` & `fate_flow-2.1.0/fate_flow/db/storage_models.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/detection/__init__.py` & `fate_flow-2.1.0/fate_flow/components/entrypoint/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/detection/detector.py` & `fate_flow-2.1.0/fate_flow/utils/job_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,155 +1,205 @@
-#
 #  Copyright 2019 The FATE Authors. All Rights Reserved.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import time
-
-from fate_flow.engine.devices import build_engine
-from fate_flow.entity.types import TaskStatus, JobStatus
-from fate_flow.operation.job_saver import JobSaver
-from fate_flow.runtime.runtime_config import RuntimeConfig
-from fate_flow.scheduler.federated_scheduler import FederatedScheduler
-from fate_flow.utils.cron import Cron
-from fate_flow.utils.log_utils import detect_logger
-
-
-class Detector(Cron):
-    def run_do(self):
-        self.detect_running_task()
-        self.detect_end_task()
-        self.detect_running_job()
-        self.detect_expired_session()
-
-    @classmethod
-    def detect_running_task(cls):
-        detect_logger().info('start to detect running task..')
-        count = 0
-        try:
-            running_tasks = JobSaver.query_task(party_status=TaskStatus.RUNNING)
-            detect_logger().info(f'running task: {running_tasks}')
-            stop_job_ids = set()
-            for task in running_tasks:
-                if task.f_run_ip != RuntimeConfig.JOB_SERVER_HOST:
-                    cls.detect_cluster_instance_status(task, stop_job_ids)
-                    continue
-                count += 1
-                try:
-                    process_exist = build_engine(task.f_provider_name).is_alive(task)
-                    if not process_exist:
-                        msg = f"task {task.f_task_id} {task.f_task_version} on {task.f_role} {task.f_party_id}"
-                        detect_logger(job_id=task.f_job_id).info(
-                            f"{msg} with {task.f_party_status} process {task.f_run_pid} does not exist")
-                        time.sleep(3)
-                        _tasks = JobSaver.query_task(task_id=task.f_task_id, task_version=task.f_task_version,
-                                                     role=task.f_role, party_id=task.f_party_id)
-                        if _tasks:
-                            if _tasks[0].f_party_status == TaskStatus.RUNNING:
-                                stop_job_ids.add(task.f_job_id)
-                                detect_logger(job_id=task.f_job_id).info(
-                                    f"{msg} party status has been checked twice, try to stop job")
-                            else:
-                                detect_logger(job_id=task.f_job_id).info(
-                                    f"{msg} party status has changed to {_tasks[0].f_party_status}, may be stopped by task_controller.stop_task, pass stop job again")
-                        else:
-                            detect_logger(job_id=task.f_job_id).warning(f"{msg} can not found on db")
-                except Exception as e:
-                    detect_logger(job_id=task.f_job_id).exception(e)
-            if stop_job_ids:
-                detect_logger().info('start to stop jobs: {}'.format(stop_job_ids))
-            stop_jobs = set()
-            for job_id in stop_job_ids:
-                jobs = JobSaver.query_job(job_id=job_id)
-                if jobs:
-                    stop_jobs.add(jobs[0])
-            cls.request_stop_jobs(jobs=stop_jobs, stop_msg="task executor process abort", stop_status=JobStatus.FAILED)
-        except Exception as e:
-            detect_logger().exception(e)
-        finally:
-            detect_logger().info(f"finish detect {count} running task")
-
-    @classmethod
-    def detect_end_task(cls):
-        pass
-
-    @classmethod
-    def detect_running_job(cls):
-        pass
-
-    @classmethod
-    def detect_expired_session(cls):
-        pass
-
-    @classmethod
-    def request_stop_jobs(cls, jobs, stop_msg, stop_status):
-        if not len(jobs):
-            return
-        detect_logger().info(f"have {len(jobs)} should be stopped, because of {stop_msg}")
-        for job in jobs:
-            try:
-                detect_logger(job_id=job.f_job_id).info(
-                    f"detector request start to stop job {job.f_job_id}, because of {stop_msg}")
-                status = FederatedScheduler.request_stop_job(job_id=job.f_job_id, party_id=job.f_scheduler_party_id,
-                                                             stop_status=stop_status)
-                detect_logger(job_id=job.f_job_id).info(f"detector request stop job {job.f_job_id} {status}")
-            except Exception as e:
-                detect_logger(job_id=job.f_job_id).exception(e)
-
-    @classmethod
-    def detect_cluster_instance_status(cls, task, stop_job_ids):
-        detect_logger(job_id=task.f_job_id).info('start detect running task instance status')
-        try:
-            latest_tasks = JobSaver.query_task(task_id=task.f_task_id, role=task.f_role, party_id=task.f_party_id)
-
-            if len(latest_tasks) != 1:
-                detect_logger(job_id=task.f_job_id).error(
-                    f'query latest tasks of {task.f_task_id} failed, '
-                    f'have {len(latest_tasks)} tasks'
-                )
-                return
-
-            if task.f_task_version != latest_tasks[0].f_task_version:
-                detect_logger(job_id=task.f_job_id).info(
-                    f'{task.f_task_id} {task.f_task_version} is not the latest task, '
-                     'update task status to failed'
-                )
-                JobSaver.update_task_status({
-                    'task_id': task.f_task_id,
-                    'role': task.f_role,
-                    'party_id': task.f_party_id,
-                    'task_version': task.f_task_version,
-                    'status': JobStatus.FAILED,
-                    'party_status': JobStatus.FAILED,
-                })
-                return
-
-            instance_list = RuntimeConfig.SERVICE_DB.get_servers()
-            instance_list = {instance.http_address for instance_id, instance in instance_list.items()}
-
-            if f'{task.f_run_ip}:{task.f_run_port}' not in instance_list:
-                detect_logger(job_id=task.f_job_id).error(
-                     'detect cluster instance status failed, '
-                     'add task {task.f_task_id} {task.f_task_version} to stop list'
-                )
-                stop_job_ids.add(task.f_job_id)
-        except Exception as e:
-            detect_logger(job_id=task.f_job_id).exception(e)
-
-
-class FederatedDetector(Detector):
-    def run_do(self):
-        self.detect_running_job_federated()
-
-    @classmethod
-    def detect_running_job_federated(cls):
-        pass
+import datetime
+import os
+import threading
+
+import yaml
+
+from fate_flow.db.base_models import DB
+from fate_flow.db.db_models import Job, Task
+from fate_flow.entity.spec.dag import InheritConfSpec
+from fate_flow.entity.types import TaskStatus
+from fate_flow.errors.server_error import InheritanceFailed
+from fate_flow.manager.operation.job_saver import JobSaver
+from fate_flow.runtime.system_settings import LOG_DIR, JOB_DIR, WORKERS_DIR
+from fate_flow.utils.base_utils import fate_uuid, current_timestamp
+from fate_flow.utils.log_utils import schedule_logger
+
+
+class JobIdGenerator(object):
+    _lock = threading.RLock()
+
+    def __init__(self, initial_value=0):
+        self._value = initial_value
+        self._pre_timestamp = None
+        self._max = 99999
+
+    def next_id(self):
+        """
+        generate next job id with locking
+        """
+        now = datetime.datetime.now()
+        with JobIdGenerator._lock:
+            if self._pre_timestamp == now:
+                if self._value < self._max:
+                    self._value += 1
+                else:
+                    now += datetime.timedelta(microseconds=1)
+                    self._pre_timestamp = now
+                    self._value = 0
+            else:
+                self._pre_timestamp = now
+                self._value = 0
+            return "{}{}".format(now.strftime("%Y%m%d%H%M%S%f"), self._value)
+
+
+job_id_generator = JobIdGenerator()
+
+
+def generate_job_id():
+    return job_id_generator.next_id()
+
+
+def generate_deepspeed_id(task_id):
+    return f"deepspeed_{task_id}"
+
+
+def generate_task_id(job_id, component_name):
+    return '{}_{}'.format(job_id, component_name)
+
+
+def generate_task_version_id(task_id, task_version):
+    return "{}_{}".format(task_id, task_version)
+
+
+def generate_session_id(task_id, task_version, role, party_id, suffix=None, random_end=False):
+    items = [task_id, str(task_version), role, party_id]
+    if suffix:
+        items.append(suffix)
+    if random_end:
+        items.append(fate_uuid())
+    return "_".join(items)
+
+
+def get_job_directory(job_id, *args):
+    return os.path.join(JOB_DIR, job_id, *args)
+
+
+def get_job_log_directory(job_id, *args):
+    return os.path.join(LOG_DIR, job_id, *args)
+
+
+def get_task_directory(job_id, role, party_id, task_name, task_version, input=False, output=False, base_dir="", **kwargs):
+    if not base_dir:
+        base_path = get_job_directory(job_id)
+    else:
+        base_path = f"{base_dir}/{job_id}"
+
+    if input:
+        return os.path.join(base_path, role, party_id, task_name, str(task_version), "input")
+    if output:
+        return os.path.join(base_path, role, party_id, task_name, str(task_version), "output")
+    else:
+        return os.path.join(base_path, role, party_id, task_name, str(task_version))
+
+
+def get_general_worker_directory(worker_name, worker_id, *args):
+    return os.path.join(WORKERS_DIR, worker_name, worker_id, *args)
+
+
+def get_general_worker_log_directory(worker_name, worker_id, *args):
+    return os.path.join(LOG_DIR, worker_name, worker_id, *args)
+
+
+def generate_model_info(job_id):
+    model_id = job_id
+    model_version = "0"
+    return model_id, model_version
+
+
+@DB.connection_context()
+def get_job_resource_info(job_id, role, party_id):
+    jobs = Job.select(Job.f_cores, Job.f_memory).where(
+        Job.f_job_id == job_id,
+        Job.f_role == role,
+        Job.f_party_id == party_id)
+    if jobs:
+        job = jobs[0]
+        return job.f_cores, job.f_memory
+    else:
+        return None, None
+
+
+@DB.connection_context()
+def get_task_resource_info(job_id, role, party_id, task_id, task_version):
+    tasks = Task.select(Task.f_task_cores, Task.f_memory, Task.f_launcher_name).where(
+        Task.f_job_id == job_id,
+        Task.f_role == role,
+        Task.f_party_id == party_id,
+        Task.f_task_id == task_id,
+        Task.f_task_version == task_version
+    )
+    if tasks:
+        task = tasks[0]
+        return task.f_task_cores, task.f_memory, task.f_launcher_name
+    else:
+        return None, None
+
+
+def save_job_dag(job_id, dag):
+    job_conf_file = os.path.join(JOB_DIR, job_id, "dag.yaml")
+    os.makedirs(os.path.dirname(job_conf_file), exist_ok=True)
+    with open(job_conf_file, "w") as f:
+        f.write(yaml.dump(dag))
+
+
+def inheritance_check(inheritance: InheritConfSpec = None):
+    if not inheritance:
+        return
+    if not inheritance.task_list:
+        raise InheritanceFailed(
+            task_list=inheritance.task_list,
+            position="dag_schema.dag.conf.inheritance.task_list"
+        )
+    inheritance_jobs = JobSaver.query_job(job_id=inheritance.job_id)
+    inheritance_tasks = JobSaver.query_task(job_id=inheritance.job_id)
+    if not inheritance_jobs:
+        raise InheritanceFailed(job_id=inheritance.job_id, detail=f"no found job {inheritance.job_id}")
+    task_status = {}
+    for task in inheritance_tasks:
+        task_status[task.f_task_name] = task.f_status
+
+    for task_name in inheritance.task_list:
+        if task_name not in task_status.keys():
+            raise InheritanceFailed(job_id=inheritance.job_id, task_name=task_name, detail="no found task name")
+        elif task_status[task_name] not in [TaskStatus.SUCCESS, TaskStatus.PASS]:
+            raise InheritanceFailed(
+                job_id=inheritance.job_id,
+                task_name=task_name,
+                task_status=task_status[task_name],
+                detail=f"task status need in [{TaskStatus.SUCCESS}, {TaskStatus.PASS}]"
+            )
+
+
+def check_task_is_timeout(task: Task):
+    now_time = current_timestamp()
+    if not task.f_start_time:
+        return False
+    running_time = (now_time - task.f_start_time)/1000
+    if task.f_timeout and running_time > task.f_timeout:
+        schedule_logger(task.f_job_id).info(f'task {task.f_task_name} run time {running_time}s timeout')
+        schedule_logger(task.f_job_id).error(f'task {task.f_task_name} timeout[{task.f_timeout}s]')
+        return True
+    else:
+        return False
+
+
+def check_party_in(role, party_id, parties):
+    for party in parties:
+        if party.role == role:
+            if party_id in party.party_id:
+                return True
+    return False
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/__init__.py` & `fate_flow-2.1.0/fate_flow/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/backend/__init__.py` & `fate_flow-2.1.0/fate_flow/engine/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/backend/_base.py` & `fate_flow-2.1.0/fate_flow/engine/backend/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,19 +87,19 @@
     def cleanup(self, provider_name, task_info, config, party_task_id, **kwargs):
         self._cleanup1(session_id=party_task_id, task_info=task_info)
         self._cleanup2(provider_name, task_info, config, **kwargs)
 
     @staticmethod
     def generate_component_run_cmd(provider_name, conf_path, output_path=""):
         if provider_name == ProviderName.FATE:
-            from fate_flow.worker.fate_executor import FateSubmit
+            from fate_flow.manager.worker.fate_executor import FateSubmit
             module_file_path = sys.modules[FateSubmit.__module__].__file__
 
         elif provider_name == ProviderName.FATE_FLOW:
-            from fate_flow.worker.fate_flow_executor import FateFlowSubmit
+            from fate_flow.manager.worker.fate_flow_executor import FateFlowSubmit
             module_file_path = sys.modules[FateFlowSubmit.__module__].__file__
 
         else:
             raise ValueError(f"load provider {provider_name} failed")
         os.environ.pop("FATE_TASK_CONFIG", None)
         common_cmd = [
             module_file_path,
@@ -113,15 +113,15 @@
 
         return common_cmd
 
     @staticmethod
     def generate_component_define_cmd(provider_name, component_ref, role, stage, define_file):
         cmd = []
         if provider_name == ProviderName.FATE:
-            from fate_flow.worker.fate_executor import FateSubmit
+            from fate_flow.manager.worker.fate_executor import FateSubmit
             module_file_path = sys.modules[FateSubmit.__module__].__file__
             cmd = [
                 module_file_path,
                 "component",
                 "artifact-type",
                 "--name",
                 component_ref,
@@ -134,15 +134,15 @@
             ]
         return cmd
 
     @staticmethod
     def generate_cleanup_cmd(provider_name):
         cmd = []
         if provider_name == ProviderName.FATE:
-            from fate_flow.worker.fate_executor import FateSubmit
+            from fate_flow.manager.worker.fate_executor import FateSubmit
             module_file_path = sys.modules[FateSubmit.__module__].__file__
             cmd = [
                 module_file_path,
                 "component",
                 "cleanup",
                 "--env-name",
                 "FATE_TASK_CONFIG",
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/backend/_eggroll.py` & `fate_flow-2.1.0/fate_flow/engine/backend/_eggroll.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,21 @@
 
 
 class EggrollEngine(LocalEngine):
     def run(self, task_info, run_parameters, engine_run, provider_name, output_path, conf_path, sync=False, **kwargs):
         parameters = TaskConfigSpec.parse_obj(run_parameters)
         if parameters.conf.computing.type == ComputingEngine.EGGROLL:
             # update eggroll options
+            cores = engine_run.pop("task_cores_per_node", None)
+            if cores:
+                engine_run["eggroll.session.processors.per.node"] = cores
             parameters.conf.computing.metadata.options.update(engine_run)
             with open(conf_path, "w") as f:
                 # update parameters
                 yaml.dump(parameters.dict(), f)
         return WorkerManager.start_task_worker(
             worker_name=WorkerName.TASK_EXECUTE,
             task_info=task_info,
             common_cmd=self.generate_component_run_cmd(provider_name, conf_path, output_path, ),
-            sync=sync
-        )
+            sync=sync,
+            **kwargs
+        ).returncode
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/backend/_session.py` & `fate_flow-2.1.0/fate_flow/engine/backend/_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from fate_flow.engine.backend._eggroll import EggrollEngine
 from fate_flow.engine.backend._spark import SparkEngine
-from fate_flow.engine.backend.eggroll_deepspeed import EggrollDeepspeedEngine
+from fate_flow.engine.backend._eggroll_deepspeed import Deepspeed
 from fate_flow.entity.types import ComputingEngine, LauncherType
 
 
 def build_backend(backend_name: str, launcher_name: str = LauncherType.DEFAULT):
     if backend_name in {ComputingEngine.EGGROLL, ComputingEngine.STANDALONE}:
         if launcher_name == LauncherType.DEEPSPEED:
-            backend = EggrollDeepspeedEngine()
+            backend = Deepspeed()
         elif not launcher_name or launcher_name == LauncherType.DEFAULT:
             backend = EggrollEngine()
         else:
             raise ValueError(f'backend "{backend_name}" launcher {launcher_name} is not supported')
     elif backend_name == ComputingEngine.SPARK:
         backend = SparkEngine()
     else:
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/backend/_spark.py` & `fate_flow-2.1.0/fate_flow/engine/backend/_spark.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,21 +12,25 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import os
 
 from fate_flow.engine.backend._base import LocalEngine
+from fate_flow.entity.spec.dag import TaskConfigSpec
 from fate_flow.entity.types import WorkerName
 from fate_flow.manager.service.worker_manager import WorkerManager
 
 
 class SparkEngine(LocalEngine):
     def run(self, task_info, run_parameters, conf_path, output_path, engine_run, provider_name, **kwargs):
-        spark_home = os.environ.get("SPARK_HOME", None)
+        spark_home = None
+        parameters = TaskConfigSpec.parse_obj(run_parameters)
+        if parameters.conf.computing.metadata.options:
+            spark_home = parameters.conf.computing.metadata.options.get("home")
         if not spark_home:
             try:
                 import pyspark
                 spark_home = pyspark.__path__[0]
             except ImportError as e:
                 raise RuntimeError("can not import pyspark")
             except Exception as e:
@@ -49,8 +53,8 @@
         return WorkerManager.start_task_worker(
             worker_name=WorkerName.TASK_EXECUTE,
             task_info=task_info,
             common_cmd=self.generate_component_run_cmd(provider_name, conf_path, output_path),
             extra_env=extra_env,
             executable=process_cmd,
             sync=True
-        )
+        ).returncode
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/devices/__init__.py` & `fate_flow-2.1.0/fate_flow/manager/worker/fate_flow_executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,27 +8,24 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from fate_flow.entity.types import ProviderDevice
-from fate_flow.manager.service.provider_manager import ProviderManager
-
-
-def build_engine(provider_name: str):
-    provider = ProviderManager.get_provider_by_provider_name(provider_name)
+#
+import argparse
+import sys
 
-    if provider.device in {ProviderDevice.DOCKER, ProviderDevice.K8S}:
-        from fate_flow.engine.devices._container import ContainerdEngine
-        engine_session = ContainerdEngine(provider)
+from fate_flow.entity import BaseEntity
+from fate_flow.utils.log import getLogger
 
-    elif provider.device in {ProviderDevice.LOCAL}:
-        from fate_flow.engine.devices._local import LocalEngine
-        engine_session = LocalEngine(provider)
 
-    else:
-        raise ValueError(f'engine device "{provider.device}" is not supported')
+class FateFlowSubmit:
+    @staticmethod
+    def run():
+        import runpy
+        runpy.run_module(mod_name='fate_flow.components', run_name='__main__')
 
-    return engine_session
 
+if __name__ == "__main__":
+    FateFlowSubmit.run()
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/devices/_base.py` & `fate_flow-2.1.0/fate_flow/engine/devices/_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,19 +12,17 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 
 import abc
-import sys
 import typing
 
 from fate_flow.db.db_models import Task
-from fate_flow.entity.types import ProviderName
 
 
 class EngineABC(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def run(self, task: Task, run_parameters, run_parameters_path, config_dir, log_dir, cwd_dir, **kwargs) -> typing.Dict:
         ...
 
@@ -35,7 +33,11 @@
     @abc.abstractmethod
     def is_alive(self, task: Task):
         ...
 
     @abc.abstractmethod
     def cleanup(self, task: Task):
         ...
+
+    @abc.abstractmethod
+    def download_output(self, task: Task):
+        ...
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/devices/_container.py` & `fate_flow-2.1.0/fate_flow/engine/devices/local.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,71 +9,79 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import yaml
+import sys
 
 from fate_flow.db.db_models import Task
 from fate_flow.engine.devices._base import EngineABC
-from fate_flow.entity.types import ProviderDevice
-from fate_flow.runtime.runtime_config import RuntimeConfig
-from fate_flow.utils.log_utils import schedule_logger
+from fate_flow.entity.types import WorkerName
+from fate_flow.manager.service.worker_manager import WorkerManager
+from fate_flow.manager.worker.fate_flow_executor import FateFlowSubmit
+from fate_flow.runtime.component_provider import ComponentProvider
+from fate_flow.utils import process_utils
 
 
-class ContainerdEngine(EngineABC):
-    def __init__(self, provider):
-        if provider.device == ProviderDevice.DOCKER:
-            from fate_flow.manager.container.docker_manager import DockerManager
-            self.manager = DockerManager(provider)
-        elif provider.device == ProviderDevice.K8S:
-            from fate_flow.manager.container.k8s_manager import K8sManager
-            self.manager = K8sManager(provider)
-        else:
-            raise ValueError(f'worker "{provider.device}" is not supported')
-
-    @staticmethod
-    def _get_name(task: Task):
-        return f'{task.f_role}-{task.f_party_id}-{task.f_task_id}-{task.f_task_version}'
-
-    @staticmethod
-    def _get_command(task: Task):
-        return [
-            '-m',
-            'fate.components',
-            'component',
-            'execute',
-            '--process-tag',
-            task.f_execution_id,
-            '--env-name',
-            'FATE_TASK_CONFIG',
-        ]
-
-    @staticmethod
-    def _get_environment(task: Task, run_parameters):
-        return {
-            'FATE_JOB_ID': task.f_job_id,
-            'FATE_TASK_CONFIG': yaml.dump(run_parameters),
-        }
+class LocalEngine(EngineABC):
+    def __init__(self, provider: ComponentProvider = None):
+        self.provider = provider
 
     def run(self, task: Task, run_parameters, run_parameters_path, config_dir, log_dir, cwd_dir, **kwargs):
-        name = self._get_name(task)
-        cmd = self._get_command(task)
-        env = self._get_environment(task, run_parameters)
-        schedule_logger(job_id=task.f_job_id).info(f"start run container {name}, cmd: {cmd}, env: {env}")
-        self.manager.start(name, cmd, env)
-        return {
-            'run_ip': RuntimeConfig.JOB_SERVER_HOST,
-            'cmd': cmd
-        }
+        return WorkerManager.start_task_worker(
+            worker_name=WorkerName.TASK_ENTRYPOINT,
+            task_info=task.to_human_model_dict(),
+            extra_env={"PYTHONPATH": self.provider.python_path},
+            executable=[self.provider.python_env],
+            common_cmd=self.generate_cmd(),
+            task_parameters=run_parameters,
+            record=True
+        )
 
-    def kill(self, task: Task):
-        self.manager.stop(self._get_name(task))
+    def kill(self, task):
+        process_utils.kill_task_executor_process(task)
 
-    def is_alive(self, task: Task):
-        return self.manager.is_running(self._get_name(task))
+    def is_alive(self, task):
+        return process_utils.check_process(pid=int(task.f_run_pid), task=task)
 
     def cleanup(self, task: Task):
+        return self._cleanup(task)
+
+    def _cleanup(self, task: Task, sync=False):
+        return WorkerManager.start_task_worker(
+            worker_name=WorkerName.TASK_CLEAN,
+            task_info=task.to_human_model_dict(),
+            extra_env={"PYTHONPATH": self.provider.python_path},
+            executable=[self.provider.python_env],
+            common_cmd=self.generate_cleanup_cmd(),
+            task_parameters=task.f_component_parameters,
+            sync=sync
+        )
+
+    def download_output(self, task):
         pass
 
+    @staticmethod
+    def generate_cmd():
+        module_file_path = sys.modules[FateFlowSubmit.__module__].__file__
+        common_cmd = [
+            module_file_path,
+            "component",
+            "entrypoint",
+            "--env-name",
+            "FATE_TASK_CONFIG",
+        ]
+        return common_cmd
+
+    @staticmethod
+    def generate_cleanup_cmd():
+        module_file_path = sys.modules[FateFlowSubmit.__module__].__file__
+        common_cmd = [
+            module_file_path,
+            "component",
+            "cleanup",
+            "--env-name",
+            "FATE_TASK_CONFIG",
+        ]
+        return common_cmd
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/devices/_local.py` & `fate_flow-2.1.0/fate_flow/engine/devices/container.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,74 +9,78 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import sys
+import json
+
+import yaml
 
 from fate_flow.db.db_models import Task
 from fate_flow.engine.devices._base import EngineABC
-from fate_flow.entity.types import TaskStatus, WorkerName, ProviderName
-from fate_flow.entity.code import KillProcessRetCode
-from fate_flow.manager.service.worker_manager import WorkerManager
+from fate_flow.entity.types import ProviderDevice
 from fate_flow.runtime.component_provider import ComponentProvider
-from fate_flow.utils import job_utils, process_utils
+from fate_flow.runtime.runtime_config import RuntimeConfig
+from fate_flow.utils.log_utils import schedule_logger
 
 
-class LocalEngine(EngineABC):
+class ContainerdEngine(EngineABC):
     def __init__(self, provider: ComponentProvider):
-        self.provider = provider
+
+        if provider.device == ProviderDevice.K8S:
+            from fate_flow.manager.container.k8s_manager import K8sManager
+            self.manager = K8sManager(provider)
+
+        elif provider.device == ProviderDevice.DOCKER:
+            from fate_flow.manager.container.docker_manager import DockerManager
+            self.manager = DockerManager(provider)
+
+        else:
+            raise ValueError(f'worker "{provider.device}" is not supported')
+
+    @staticmethod
+    def _get_name(task: Task):
+        return f'{task.f_role}-{task.f_party_id}-{task.f_task_id}-{task.f_task_version}'
+
+    @classmethod
+    def _flatten_dict(cls, data, parent_key='', sep='.'):
+        items = {}
+        for key, value in data.items():
+            new_key = f"{parent_key}{sep}{key}" if parent_key else key
+            if isinstance(value, dict):
+                items.update(cls._flatten_dict(value, new_key, sep=sep))
+            else:
+                items[new_key] = value
+        return items
+
+    @classmethod
+    def _get_environment(cls, task: Task, run_parameters):
+        # return cls._flatten_dict(run_parameters)
+        return {"CONFIG": json.dumps(run_parameters)}
+
+    @classmethod
+    def _get_volume(cls, task):
+        return None
 
     def run(self, task: Task, run_parameters, run_parameters_path, config_dir, log_dir, cwd_dir, **kwargs):
-        return WorkerManager.start_task_worker(
-            worker_name=WorkerName.TASK_ENTRYPOINT,
-            task_info=task.to_human_model_dict(),
-            extra_env={"PYTHONPATH": self.provider.python_path},
-            executable=[self.provider.python_env],
-            common_cmd=self.generate_cmd(),
-            task_parameters=run_parameters,
-            record=True
-        )
+        name = self._get_name(task)
+        cmd = None
+        env = self._get_environment(task, run_parameters)
+        schedule_logger(job_id=task.f_job_id).info(f"start run container {name}, cmd: {cmd}, env: {json.dumps(env)}")
+        self.manager.start(name, cmd, env, volumes=self._get_volume(task))
+        return {
+            'run_ip': RuntimeConfig.JOB_SERVER_HOST
+        }
 
-    def kill(self, task):
-        process_utils.kill_task_executor_process(task)
+    def kill(self, task: Task):
+        self.manager.stop(self._get_name(task))
 
-    def is_alive(self, task):
-        return process_utils.check_process(pid=int(task.f_run_pid), task=task)
+    def is_alive(self, task: Task):
+        return self.manager.is_running(self._get_name(task))
 
     def cleanup(self, task: Task):
-        return WorkerManager.start_task_worker(
-            worker_name=WorkerName.TASK_CLEAN,
-            task_info=task.to_human_model_dict(),
-            extra_env={"PYTHONPATH": self.provider.python_path},
-            executable=[self.provider.python_env],
-            common_cmd=self.generate_cleanup_cmd(),
-            task_parameters=task.f_component_parameters
-        )
-
-    @staticmethod
-    def generate_cmd():
-        from fate_flow.entrypoint.runner import Submit
-        module_file_path = sys.modules[Submit.__module__].__file__
-        common_cmd = [
-            module_file_path,
-            "component",
-            "entrypoint",
-            "--env-name",
-            "FATE_TASK_CONFIG",
-        ]
-        return common_cmd
+        pass
 
-    @staticmethod
-    def generate_cleanup_cmd():
-        from fate_flow.entrypoint.runner import Submit
-        module_file_path = sys.modules[Submit.__module__].__file__
-        common_cmd = [
-            module_file_path,
-            "component",
-            "cleanup",
-            "--env-name",
-            "FATE_TASK_CONFIG",
-        ]
-        return common_cmd
+    def download_output(self, task: Task):
+        pass
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/relation_ship.py` & `fate_flow-2.1.0/fate_flow/engine/relation_ship.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/__init__.py` & `fate_flow-2.1.0/fate_flow/engine/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/_abc.py` & `fate_flow-2.1.0/fate_flow/engine/storage/_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,16 @@
     @abc.abstractmethod
     def check_address(self):
         ...
 
 
 class StorageSessionABC(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def create_table(self, address, name, namespace, partitions, storage_type=None, options=None,
+    def create_table(self, address, name, namespace, partitions, key_serdes_type, value_serdes_type, partitioner_type,
+                     storage_type=None, options=None,
                      **kwargs) -> StorageTableABC:
         ...
 
     @abc.abstractmethod
     def get_table(self, name, namespace) -> StorageTableABC:
         ...
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/_session.py` & `fate_flow-2.1.0/fate_flow/engine/storage/_session.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,76 +16,126 @@
 import typing
 import uuid
 
 import peewee
 
 from fate_flow.db.base_models import DB
 from fate_flow.db.storage_models import SessionRecord
-from fate_flow.engine.storage._abc import StorageSessionABC, StorageTableABC, StorageTableMetaABC
+from fate_flow.engine.storage._abc import (
+    StorageSessionABC,
+    StorageTableABC,
+    StorageTableMetaABC,
+)
 
 from fate_flow.engine.storage._table import StorageTableMeta
 from fate_flow.entity.types import EngineType, StorageEngine
-from fate_flow.runtime.system_settings import ENGINES
+from fate_flow.runtime.system_settings import ENGINES, COMPUTING_CONF
 from fate_flow.utils import base_utils
 from fate_flow.utils.log import getLogger
 
 LOGGER = getLogger("storage")
 
 
 class StorageSessionBase(StorageSessionABC):
     def __init__(self, session_id, engine):
         self._session_id = session_id
         self._engine = engine
 
-    def create_table(self, address, name, namespace, partitions=None, **kwargs):
-        table = self.table(address=address, name=name, namespace=namespace, partitions=partitions, **kwargs)
+    def create_table(
+        self,
+        address,
+        name,
+        namespace,
+        partitions,
+        key_serdes_type=0,
+        value_serdes_type=0,
+        partitioner_type=0,
+        **kwargs,
+    ):
+        table = self.table(
+            address=address,
+            name=name,
+            namespace=namespace,
+            partitions=partitions,
+            key_serdes_type=key_serdes_type,
+            value_serdes_type=value_serdes_type,
+            partitioner_type=partitioner_type,
+            **kwargs,
+        )
         table.create_meta(**kwargs)
         return table
 
     @staticmethod
     def meta_table_name(name):
         return f"{name}.meta"
 
     def get_table(self, name, namespace):
         meta = StorageTableMeta(name=name, namespace=namespace)
         if meta and meta.exists():
-            table = self.table(name=meta.get_name(),
-                               namespace=meta.get_namespace(),
-                               address=meta.get_address(),
-                               partitions=meta.get_partitions(),
-                               store_type=meta.get_store_type(),
-                               options=meta.get_options())
+            table = self.load(
+                name=meta.get_name(),
+                namespace=meta.get_namespace(),
+                address=meta.get_address(),
+                partitions=meta.get_partitions(),
+                store_type=meta.get_store_type(),
+                options=meta.get_options(),
+            )
             table.meta = meta
             return table
         else:
             return None
 
     @classmethod
     def get_table_meta(cls, name, namespace):
         meta = StorageTableMeta(name=name, namespace=namespace)
         if meta and meta.exists():
             return meta
         else:
             return None
 
-
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.destroy()
 
     def destroy(self):
         try:
             self.stop()
         except Exception as e:
-            LOGGER.warning(f"stop storage session {self._session_id} failed, try to kill", e)
+            LOGGER.warning(
+                f"stop storage session {self._session_id} failed, try to kill", e
+            )
             self.kill()
 
-    def table(self, name, namespace, address, store_type, partitions=None, **kwargs):
+    def table(
+        self,
+        name,
+        namespace,
+        address,
+        partitions,
+        key_serdes_type,
+        value_serdes_type,
+        partitioner_type,
+        store_type,
+        options,
+        **kwargs,
+    ):
+        raise NotImplementedError()
+
+    def load(
+        self,
+        name,
+        namespace,
+        address,
+        store_type,
+        partitions,
+        options=None,
+        **kwargs,
+    ):
         raise NotImplementedError()
 
     def stop(self):
         raise NotImplementedError()
 
     def kill(self):
         raise NotImplementedError()
@@ -114,17 +164,21 @@
         self._as_global(self)
         return self
 
     def __init__(self, session_id: str = None, options=None):
         if options is None:
             options = {}
         self._storage_engine = ENGINES.get(EngineType.STORAGE, None)
-        self._storage_session: typing.Dict[StorageSessionABC] = {}
+        self._storage_session: typing.Dict[str, StorageSessionABC] = {}
         self._session_id = str(uuid.uuid1()) if not session_id else session_id
-        self._logger = LOGGER if options.get("logger", None) is None else options.get("logger", None)
+        self._logger = (
+            LOGGER
+            if options.get("logger", None) is None
+            else options.get("logger", None)
+        )
 
         self._logger.info(f"create manager session {self._session_id}")
 
     @property
     def session_id(self) -> str:
         return self._session_id
 
@@ -138,57 +192,72 @@
         return self._open()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_tb:
             self._logger.exception("", exc_info=(exc_type, exc_val, exc_tb))
         return self._close()
 
-    def _get_or_create_storage(self,
-                               storage_session_id=None,
-                               storage_engine=None,
-                               record: bool = True,
-                               **kwargs) -> StorageSessionABC:
-        storage_session_id = f"{self._session_id}_storage_{uuid.uuid1()}" if not storage_session_id else storage_session_id
+    def _get_or_create_storage(
+        self,
+        storage_session_id=None,
+        storage_engine=None,
+        record: bool = True,
+        **kwargs,
+    ) -> StorageSessionABC:
+        storage_session_id = (
+            f"{self._session_id}_storage_{uuid.uuid1()}"
+            if not storage_session_id
+            else storage_session_id
+        )
 
         if storage_session_id in self._storage_session:
             return self._storage_session[storage_session_id]
         else:
             if storage_engine is None:
                 storage_engine = self._storage_engine
 
         for session in self._storage_session.values():
             if storage_engine == session.engine:
                 return session
 
         if record:
-            self.save_record(engine_type=EngineType.STORAGE,
-                             engine_name=storage_engine,
-                             engine_session_id=storage_session_id)
-
+            self.save_record(
+                engine_type=EngineType.STORAGE,
+                engine_name=storage_engine,
+                engine_session_id=storage_session_id,
+            )
         if storage_engine == StorageEngine.EGGROLL:
             from fate_flow.engine.storage.eggroll import StorageSession
+            kwargs["host"] = COMPUTING_CONF.get(StorageEngine.EGGROLL).get("host")
+            kwargs["port"] = COMPUTING_CONF.get(StorageEngine.EGGROLL).get("port")
 
         elif storage_engine == StorageEngine.STANDALONE:
             from fate_flow.engine.storage.standalone import StorageSession
 
         elif storage_engine == StorageEngine.FILE:
             from fate_flow.engine.storage.file import StorageSession
 
         elif storage_engine == StorageEngine.HDFS:
             from fate_flow.engine.storage.hdfs import StorageSession
 
         else:
-            raise NotImplementedError(f"can not be initialized with storage engine: {storage_engine}")
-        storage_session = StorageSession(session_id=storage_session_id, options=kwargs.get("options", {}))
+            raise NotImplementedError(
+                f"can not be initialized with storage engine: {storage_engine}"
+            )
+        storage_session = StorageSession(
+            session_id=storage_session_id, **kwargs
+        )
 
         self._storage_session[storage_session_id] = storage_session
 
         return storage_session
 
-    def get_table(self, name, namespace, ignore_disable=False) -> typing.Union[StorageTableABC, None]:
+    def get_table(
+        self, name, namespace, ignore_disable=False
+    ) -> typing.Union[StorageTableABC, None]:
         meta = Session.get_table_meta(name=name, namespace=namespace)
         if meta is None:
             return None
         if meta.get_disable() and not ignore_disable:
             raise Exception(f"table {namespace} {name} disable: {meta.get_disable()}")
         engine = meta.get_engine()
         storage_session = self._get_or_create_storage(storage_engine=engine)
@@ -199,19 +268,19 @@
     def get_table_meta(cls, name, namespace) -> typing.Union[StorageTableMetaABC, None]:
         meta = StorageSessionBase.get_table_meta(name=name, namespace=namespace)
         return meta
 
     def storage(self, **kwargs):
         return self._get_or_create_storage(**kwargs)
 
-
     @DB.connection_context()
     def save_record(self, engine_type, engine_name, engine_session_id):
         self._logger.info(
-            f"try to save session record for manager {self._session_id}, {engine_type} {engine_name} {engine_session_id}")
+            f"try to save session record for manager {self._session_id}, {engine_type} {engine_name} {engine_session_id}"
+        )
         session_record = SessionRecord()
         session_record.f_manager_session_id = self._session_id
         session_record.f_engine_type = engine_type
         session_record.f_engine_name = engine_name
         session_record.f_engine_session_id = engine_session_id
         # TODO: engine address
         session_record.f_engine_address = {}
@@ -222,57 +291,76 @@
             if effect_count != 1:
                 raise RuntimeError(f"{msg} failed")
         except peewee.IntegrityError as e:
             LOGGER.warning(e)
         except Exception as e:
             raise RuntimeError(f"{msg} exception", e)
         self._logger.info(
-            f"save session record for manager {self._session_id}, {engine_type} {engine_name} {engine_session_id} successfully")
+            f"save session record for manager {self._session_id}, {engine_type} {engine_name} {engine_session_id} successfully"
+        )
 
     @DB.connection_context()
     def delete_session_record(self, engine_session_id):
-        rows = SessionRecord.delete().where(SessionRecord.f_engine_session_id == engine_session_id).execute()
+        rows = (
+            SessionRecord.delete()
+            .where(SessionRecord.f_engine_session_id == engine_session_id)
+            .execute()
+        )
         if rows > 0:
             self._logger.info(f"delete session {engine_session_id} record successfully")
         else:
             self._logger.warning(f"delete session {engine_session_id} record failed")
 
     @classmethod
     @DB.connection_context()
     def query_sessions(cls, reverse=None, order_by=None, **kwargs):
         return SessionRecord.query(reverse=reverse, order_by=order_by, **kwargs)
 
     @DB.connection_context()
     def get_session_from_record(self, **kwargs):
         self._logger.info(f"query by manager session id {self._session_id}")
-        session_records = self.query_sessions(manager_session_id=self._session_id, **kwargs)
-        self._logger.info([session_record.f_engine_session_id for session_record in session_records])
+        session_records = self.query_sessions(
+            manager_session_id=self._session_id, **kwargs
+        )
+        self._logger.info(
+            [session_record.f_engine_session_id for session_record in session_records]
+        )
         for session_record in session_records:
             try:
                 engine_session_id = session_record.f_engine_session_id
                 if session_record.f_engine_type == EngineType.STORAGE:
-                    self._get_or_create_storage(storage_session_id=engine_session_id,
-                                                storage_engine=session_record.f_engine_name,
-                                                record=False)
+                    self._get_or_create_storage(
+                        storage_session_id=engine_session_id,
+                        storage_engine=session_record.f_engine_name,
+                        record=False,
+                    )
             except Exception as e:
                 self._logger.error(e)
-                self.delete_session_record(engine_session_id=session_record.f_engine_session_id)
+                self.delete_session_record(
+                    engine_session_id=session_record.f_engine_session_id
+                )
 
     def destroy_all_sessions(self, **kwargs):
-        self._logger.info(f"start destroy manager session {self._session_id} all sessions")
+        self._logger.info(
+            f"start destroy manager session {self._session_id} all sessions"
+        )
         self.get_session_from_record(**kwargs)
         self.destroy_storage_session()
-        self._logger.info(f"finish destroy manager session {self._session_id} all sessions")
+        self._logger.info(
+            f"finish destroy manager session {self._session_id} all sessions"
+        )
 
     def destroy_storage_session(self):
         for session_id, session in self._storage_session.items():
             try:
                 self._logger.info(f"try to destroy storage session {session_id}")
                 session.destroy()
                 self._logger.info(f"destroy storage session {session_id} successfully")
             except Exception as e:
-                self._logger.exception(f"destroy storage session {session_id} failed", e)
+                self._logger.exception(
+                    f"destroy storage session {session_id} failed", e
+                )
             self.delete_session_record(engine_session_id=session_id)
 
 
 def get_session() -> Session:
-    return Session.get_global()
+    return Session.get_global()
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/_table.py` & `fate_flow-2.1.0/fate_flow/engine/storage/_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,44 +12,87 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 
 import operator
-from typing import Iterable
+from typing import Iterable, Tuple
 
 import peewee
 
 from fate_flow.db.base_models import DB
 from fate_flow.db.storage_models import StorageTableMetaModel
-from fate_flow.engine.storage._abc import StorageTableMetaABC, StorageTableABC
-
 from fate_flow.engine.relation_ship import Relationship
+from fate_flow.engine.storage._abc import StorageTableMetaABC, StorageTableABC
 from fate_flow.entity.types import AddressABC
 from fate_flow.utils.base_utils import current_timestamp
 from fate_flow.utils.log import getLogger
+from ._partitioner import get_partitioner_by_type
+from .serdes import get_serdes_by_type
 
 LOGGER = getLogger("storage")
 
 
+def _wrapped_iterable_with_serdes(
+    kv_list: Iterable[Tuple[bytes, bytes]], key_serdes, value_serdes
+):
+    for k, v in kv_list:
+        yield key_serdes.serialize(k), value_serdes.serialize(v)
+
+
 class StorageTableBase(StorageTableABC):
-    def __init__(self, name, namespace, address, partitions, options, engine):
+    def __init__(
+        self,
+        name,
+        namespace,
+        address,
+        partitions,
+        options,
+        engine,
+        key_serdes_type,
+        value_serdes_type,
+        partitioner_type,
+    ):
         self._name = name
         self._namespace = namespace
         self._address = address
         self._partitions = partitions
         self._options = options if options else {}
         self._engine = engine
+        self._key_serdes_type = key_serdes_type
+        self._value_serdes_type = value_serdes_type
+        self._partitioner_type = partitioner_type
+        self._key_serdes = None
+        self._value_serdes = None
+        self._partitioner = None
 
         self._meta = None
         self._read_access_time = None
         self._write_access_time = None
 
     @property
+    def key_serdes(self):
+        if self._key_serdes is None:
+            self._key_serdes = get_serdes_by_type(self._key_serdes_type)
+        return self._key_serdes
+
+    @property
+    def value_serdes(self):
+        if self._value_serdes is None:
+            self._value_serdes = get_serdes_by_type(self._value_serdes_type)
+        return self._value_serdes
+
+    @property
+    def partitioner(self):
+        if self._partitioner is None:
+            self._partitioner = get_partitioner_by_type(self._partitioner_type)
+        return self._partitioner
+
+    @property
     def name(self):
         return self._name
 
     @property
     def namespace(self):
         return self._namespace
 
@@ -85,31 +128,37 @@
     def read_access_time(self):
         return self._read_access_time
 
     @property
     def write_access_time(self):
         return self._write_access_time
 
-    def update_meta(self,
-                    data_meta=None,
-                    count=None,
-                    part_of_data=None,
-                    description=None,
-                    partitions=None,
-                    **kwargs):
-        self._meta.update_metas(data_meta=data_meta,
-                                count=count,
-                                part_of_data=part_of_data,
-                                description=description,
-                                partitions=partitions,
-                                **kwargs)
+    def update_meta(
+        self,
+        data_meta=None,
+        count=None,
+        part_of_data=None,
+        description=None,
+        partitions=None,
+        **kwargs
+    ):
+        self._meta.update_metas(
+            data_meta=data_meta,
+            count=count,
+            part_of_data=part_of_data,
+            description=description,
+            partitions=partitions,
+            **kwargs
+        )
 
     def create_meta(self, **kwargs):
         self.destroy_if_exists()
-        table_meta = StorageTableMeta(name=self._name, namespace=self._namespace, new=True)
+        table_meta = StorageTableMeta(
+            name=self._name, namespace=self._namespace, new=True
+        )
         table_meta.set_metas(**kwargs)
         table_meta.address = self._address
         table_meta.partitions = self._partitions
         table_meta.engine = self._engine
         table_meta.options = self._options
         table_meta.create()
         self._meta = table_meta
@@ -124,19 +173,24 @@
         return False
 
     def check_address(self):
         return True
 
     def put_all(self, kv_list: Iterable, **kwargs):
         # self._update_write_access_time()
-        self._put_all(kv_list, **kwargs)
+        self._put_all(
+            _wrapped_iterable_with_serdes(kv_list, self.key_serdes, self.value_serdes),
+            self.partitioner,
+            **kwargs
+        )
 
     def collect(self, **kwargs) -> list:
         # self._update_read_access_time()
-        return self._collect(**kwargs)
+        for k, v in self._collect(**kwargs):
+            yield self.key_serdes.deserialize(k), self.value_serdes.deserialize(v)
 
     def count(self):
         # self._update_read_access_time()
         count = self._count()
         self.meta.update_metas(count=count)
         return count
 
@@ -145,35 +199,36 @@
         return self._read()
 
     def destroy(self):
         self.meta.destroy_metas()
         self._destroy()
 
     # to be implemented
-    def _put_all(self, kv_list: Iterable, **kwargs):
+    def _put_all(self, kv_list: Iterable[Tuple[bytes, bytes]], partitioner, **kwargs):
         raise NotImplementedError()
 
     def _collect(self, **kwargs) -> list:
         raise NotImplementedError()
 
     def _count(self):
         raise NotImplementedError()
 
     def _read(self):
         raise NotImplementedError()
 
     def _destroy(self):
         raise NotImplementedError()
 
-    def _save_as(self, address, name, namespace, partitions=None, schema=None, **kwargs):
+    def _save_as(
+        self, address, name, namespace, partitions=None, schema=None, **kwargs
+    ):
         raise NotImplementedError()
 
 
 class StorageTableMeta(StorageTableMetaABC):
-
     def __init__(self, name, namespace, new=False, create_address=True):
         self.name = name
         self.namespace = namespace
         self.address = None
         self.engine = None
         self.store_type = None
         self.options = None
@@ -201,22 +256,26 @@
         if not new:
             self.build(create_address)
 
     def build(self, create_address):
         for k, v in self.table_meta.__dict__["__data__"].items():
             setattr(self, k.lstrip("f_"), v)
         if create_address:
-            self.address = self.create_address(storage_engine=self.engine, address_dict=self.address)
+            self.address = self.create_address(
+                storage_engine=self.engine, address_dict=self.address
+            )
 
     def __new__(cls, *args, **kwargs):
         if not kwargs.get("new", False):
             name, namespace = kwargs.get("name"), kwargs.get("namespace")
             if not name or not namespace:
                 return None
-            tables_meta = cls.query_table_meta(filter_fields=dict(name=name, namespace=namespace))
+            tables_meta = cls.query_table_meta(
+                filter_fields=dict(name=name, namespace=namespace)
+            )
             if not tables_meta:
                 return None
             self = super().__new__(cls)
             setattr(self, "table_meta", tables_meta[0])
             return self
         else:
             return super().__new__(cls)
@@ -231,17 +290,21 @@
     def create(self):
         table_meta = StorageTableMetaModel()
         table_meta.f_create_time = current_timestamp()
         table_meta.f_data_meta = {}
         table_meta.f_part_of_data = []
         table_meta.f_source = {}
         for k, v in self.to_dict().items():
-            attr_name = 'f_%s' % k
+            attr_name = "f_%s" % k
             if hasattr(StorageTableMetaModel, attr_name):
-                setattr(table_meta, attr_name, v if not issubclass(type(v), AddressABC) else v.__dict__)
+                setattr(
+                    table_meta,
+                    attr_name,
+                    v if not issubclass(type(v), AddressABC) else v.__dict__,
+                )
         try:
             rows = table_meta.save(force_insert=True)
             if rows != 1:
                 raise Exception("create table meta failed")
         except peewee.IntegrityError as e:
             # if e.args[0] == 1062:
             #     # warning
@@ -261,76 +324,97 @@
 
     @classmethod
     @DB.connection_context()
     def query_table_meta(cls, filter_fields, query_fields=None):
         filters = []
         querys = []
         for f_n, f_v in filter_fields.items():
-            attr_name = 'f_%s' % f_n
+            attr_name = "f_%s" % f_n
             if hasattr(StorageTableMetaModel, attr_name):
-                filters.append(operator.attrgetter('f_%s' % f_n)(StorageTableMetaModel) == f_v)
+                filters.append(
+                    operator.attrgetter("f_%s" % f_n)(StorageTableMetaModel) == f_v
+                )
         if query_fields:
             for f_n in query_fields:
-                attr_name = 'f_%s' % f_n
+                attr_name = "f_%s" % f_n
                 if hasattr(StorageTableMetaModel, attr_name):
-                    querys.append(operator.attrgetter('f_%s' % f_n)(StorageTableMetaModel))
+                    querys.append(
+                        operator.attrgetter("f_%s" % f_n)(StorageTableMetaModel)
+                    )
         if filters:
             if querys:
                 tables_meta = StorageTableMetaModel.select(querys).where(*filters)
             else:
                 tables_meta = StorageTableMetaModel.select().where(*filters)
             return [table_meta for table_meta in tables_meta]
         else:
             # not allow query all table
             return []
 
     @DB.connection_context()
-    def update_metas(self, data_meta=None, count=None, part_of_data=None, description=None, partitions=None,
-                     in_serialized=None, **kwargs):
+    def update_metas(
+        self,
+        data_meta=None,
+        count=None,
+        part_of_data=None,
+        description=None,
+        partitions=None,
+        in_serialized=None,
+        **kwargs
+    ):
         meta_info = {}
         for k, v in locals().items():
             if k not in ["self", "kwargs", "meta_info"] and v is not None:
                 meta_info[k] = v
         meta_info.update(kwargs)
         meta_info["name"] = meta_info.get("name", self.name)
         meta_info["namespace"] = meta_info.get("namespace", self.namespace)
         update_filters = []
         primary_keys = StorageTableMetaModel._meta.primary_key.field_names
         for p_k in primary_keys:
-            update_filters.append(operator.attrgetter(p_k)(StorageTableMetaModel) == meta_info[p_k.lstrip("f_")])
+            update_filters.append(
+                operator.attrgetter(p_k)(StorageTableMetaModel)
+                == meta_info[p_k.lstrip("f_")]
+            )
         table_meta = StorageTableMetaModel()
         update_fields = {}
         for k, v in meta_info.items():
-            attr_name = 'f_%s' % k
-            if hasattr(StorageTableMetaModel, attr_name) and attr_name not in primary_keys:
+            attr_name = "f_%s" % k
+            if (
+                hasattr(StorageTableMetaModel, attr_name)
+                and attr_name not in primary_keys
+            ):
                 if k == "part_of_data":
                     if len(v) < 100:
                         tmp = v
                     else:
                         tmp = v[:100]
-                    update_fields[operator.attrgetter(attr_name)(StorageTableMetaModel)] = tmp
+                    update_fields[
+                        operator.attrgetter(attr_name)(StorageTableMetaModel)
+                    ] = tmp
                 else:
-                    update_fields[operator.attrgetter(attr_name)(StorageTableMetaModel)] = v
+                    update_fields[
+                        operator.attrgetter(attr_name)(StorageTableMetaModel)
+                    ] = v
         if update_filters:
             operate = table_meta.update(update_fields).where(*update_filters)
         else:
             operate = table_meta.update(update_fields)
         if count:
             self.count = count
         _return = operate.execute()
         _meta = StorageTableMeta(name=self.name, namespace=self.namespace)
         return _return > 0, _meta
 
     @DB.connection_context()
     def destroy_metas(self):
-        StorageTableMetaModel \
-            .delete() \
-            .where(StorageTableMetaModel.f_name == self.name,
-                   StorageTableMetaModel.f_namespace == self.namespace) \
-            .execute()
+        StorageTableMetaModel.delete().where(
+            StorageTableMetaModel.f_name == self.name,
+            StorageTableMetaModel.f_namespace == self.namespace,
+        ).execute()
 
     @classmethod
     def create_address(cls, storage_engine, address_dict):
         address_class = Relationship.EngineToAddress.get(storage_engine)
         kwargs = {}
         for k in address_class.__init__.__code__.co_varnames:
             if k == "self":
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/_types.py` & `fate_flow-2.1.0/fate_flow/engine/storage/_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 DEFAULT_ID_DELIMITER = ","
 
 
 class DataType:
     TABLE = "table"
     DATAFRAME = "dataframe"
     FILE = "file"
+    DATA_DIRECTORY = "data_directory"
+    DATA_UNRESOLVED = "data_unresolved"
 
 
 class StorageOrigin(object):
     TABLE_BIND = "table_bind"
     READER = "reader"
     UPLOAD = "upload"
     OUTPUT = "output"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/eggroll/__init__.py` & `fate_flow-2.1.0/fate_flow/engine/storage/eggroll/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/eggroll/_session.py` & `fate_flow-2.1.0/fate_flow/engine/storage/file/_session.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,40 +9,45 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-
-from eggroll.core.session import session_init
-from eggroll.roll_pair.roll_pair import RollPairContext
-from fate_flow.engine.storage import EggRollStoreType, StorageEngine, StorageSessionBase
-from fate_flow.engine.storage.eggroll import StorageTable
-from fate_flow.entity.types import AddressABC, EggRollAddress
+from fate_flow.engine.storage import StorageSessionBase, StorageEngine
+from fate_flow.engine.storage.file._table import StorageTable
+from fate_flow.entity.types import AddressABC, FileAddress
 
 
 class StorageSession(StorageSessionBase):
     def __init__(self, session_id, options=None):
-        super(StorageSession, self).__init__(session_id=session_id, engine=StorageEngine.EGGROLL)
-        self._options = options if options else {}
-        self._options['eggroll.session.deploy.mode'] = "cluster"
-        self._rp_session = session_init(session_id=self._session_id, options=self._options)
-        self._rpc = RollPairContext(session=self._rp_session)
-        self._session_id = self._rp_session.get_session_id()
-
-    def table(self, name, namespace,
-              address: AddressABC, partitions,
-              store_type: EggRollStoreType = EggRollStoreType.ROLLPAIR_LMDB, options=None, **kwargs):
-        if isinstance(address, EggRollAddress):
-            return StorageTable(context=self._rpc, name=name, namespace=namespace, address=address,
-                                partitions=partitions, store_type=store_type, options=options)
-        raise NotImplementedError(f"address type {type(address)} not supported with eggroll storage")
+        super(StorageSession, self).__init__(session_id=session_id, engine=StorageEngine.FILE)
+
+    def table(self, address: AddressABC, name, namespace, partitions, storage_type=None, options=None, **kwargs):
+        if isinstance(address, FileAddress):
+            return StorageTable(address=address, name=name, namespace=namespace,
+                                partitions=partitions)
+        raise NotImplementedError(f"address type {type(address)} not supported with hdfs storage")
+
+    def load(
+        self,
+        name,
+        namespace,
+        address,
+        store_type,
+        partitions,
+        options=None,
+        **kwargs,
+    ):
+        if isinstance(address, FileAddress):
+            return StorageTable(address=address, name=name, namespace=namespace,
+                                partitions=partitions, options=options)
+        raise NotImplementedError(f"address type {type(address)} not supported with hdfs storage")
 
     def cleanup(self, name, namespace):
-        self._rpc.cleanup(name=name, namespace=namespace)
+        pass
 
     def stop(self):
-        return self._rp_session.stop()
+        pass
 
     def kill(self):
-        return self._rp_session.kill()
+        pass
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/eggroll/_table.py` & `fate_flow-2.1.0/fate_flow/engine/storage/eggroll/_table.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,55 +12,64 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 from typing import Iterable
 from fate_flow.engine.storage import StorageTableBase, EggRollStoreType, StorageEngine
+from eggroll.computing import RollPairContext, RollPair
 
 
 class StorageTable(StorageTableBase):
     def __init__(
         self,
-        context,
+        context: RollPairContext,
+        table: RollPair,
+        key_serdes_type,
+        value_serdes_type,
+        partitioner_type,
         name,
         namespace,
         address,
         partitions: int = 1,
-        store_type: EggRollStoreType = EggRollStoreType.ROLLPAIR_LMDB,
+        store_type: str = EggRollStoreType.ROLLPAIR_LMDB,
         options=None,
     ):
+        self._context = context
+        self._store_type = store_type
+        self._table = table
         super(StorageTable, self).__init__(
             name=name,
             namespace=namespace,
             address=address,
             partitions=partitions,
             options=options,
-            engine=StorageEngine.EGGROLL
+            engine=StorageEngine.EGGROLL,
+            key_serdes_type=key_serdes_type,
+            value_serdes_type=value_serdes_type,
+            partitioner_type=partitioner_type,
         )
-        self._store_type = store_type
-        self._context = context
         self._options["store_type"] = self._store_type
         self._options["total_partitions"] = partitions
         self._options["create_if_missing"] = True
-        self._table = self._context.load(namespace=self.address.namespace, name=self.address.name, options=self._options)
 
-    def _save_as(self, address, name, namespace, partitions=None, **kwargs):
-        self._table.save_as(name=address.name, namespace=address.namespace)
-        table = StorageTable(
-            context=self._context,
-            address=address,
-            partitions=partitions,
-            name=name,
-            namespace=namespace
-        )
-        return table
+    #
+    # def _save_as(self, address, name, namespace, partitions=None, **kwargs):
+    #     self._table.save_as(name=address.name, namespace=address.namespace)
+    #     table = StorageTable(
+    #         context=self._context,
+    #         address=address,
+    #         partitions=partitions,
+    #         name=name,
+    #         namespace=namespace,
+    #     )
+    #     return table
 
-    def _put_all(self, kv_list: Iterable, **kwargs):
-        return self._table.put_all(kv_list)
+    def _put_all(self, kv_list: Iterable, partitioner, **kwargs):
+        return self._table.put_all(kv_list, partitioner)
 
     def _collect(self, **kwargs) -> list:
         return self._table.get_all(**kwargs)
 
     def _destroy(self):
         self._table.destroy()
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/file/__init__.py` & `fate_flow-2.1.0/fate_flow/engine/storage/file/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/file/_session.py` & `fate_flow-2.1.0/fate_flow/engine/storage/hdfs/_session.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,26 +10,51 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from fate_flow.engine.storage import StorageSessionBase, StorageEngine
-from fate_flow.engine.storage.file._table import StorageTable
-from fate_flow.entity.types import AddressABC, FileAddress
+from fate_flow.engine.storage.hdfs._table import StorageTable
+from fate_flow.entity.types import AddressABC, HDFSAddress
 
 
 class StorageSession(StorageSessionBase):
     def __init__(self, session_id, options=None):
-        super(StorageSession, self).__init__(session_id=session_id, engine=StorageEngine.FILE)
+        super(StorageSession, self).__init__(session_id=session_id, engine=StorageEngine.HDFS)
 
-    def table(self, address: AddressABC, name, namespace, partitions, storage_type=None, options=None, **kwargs):
-        if isinstance(address, FileAddress):
-            return StorageTable(address=address, name=name, namespace=namespace,
-                                partitions=partitions)
+    def table(self, address: AddressABC, name, namespace, partitions, store_type=None, options=None, **kwargs):
+        if isinstance(address, HDFSAddress):
+            return StorageTable(
+                address=address,
+                name=name,
+                namespace=namespace,
+                partitions=partitions,
+                options=options
+            )
+        raise NotImplementedError(f"address type {type(address)} not supported with hdfs storage")
+
+    def load(
+        self,
+        name,
+        namespace,
+        address,
+        store_type,
+        partitions,
+        options=None,
+        **kwargs,
+    ):
+        if isinstance(address, HDFSAddress):
+            return StorageTable(
+                address=address,
+                name=name,
+                namespace=namespace,
+                partitions=partitions,
+                options=options
+            )
         raise NotImplementedError(f"address type {type(address)} not supported with hdfs storage")
 
     def cleanup(self, name, namespace):
         pass
 
     def stop(self):
         pass
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/file/_table.py` & `fate_flow-2.1.0/fate_flow/engine/storage/file/_table.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,24 +12,38 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 import io
 import os
-from typing import Iterable
+import struct
+from typing import Iterable, Tuple
 
 from pyarrow import fs
 
 from fate_flow.engine.storage import StorageTableBase, StorageEngine
-from fate_flow.manager.data.data_manager import DataManager
 from fate_flow.utils.log import getLogger
 
 LOGGER = getLogger()
 
+class FileCoder:
+    @staticmethod
+    def encode(key: bytes, value: bytes):
+        size = struct.pack(">Q", len(key))
+        return (size + key + value).hex()
+
+    @staticmethod
+    def decode(data: str) -> Tuple[bytes, bytes]:
+        data = bytes.fromhex(data)
+        size = struct.unpack(">Q", data[:8])[0]
+        key = data[8 : 8 + size]
+        value = data[8 + size :]
+        return key, value
+
 
 class StorageTable(StorageTableBase):
     def __init__(
         self,
         address=None,
         name: str = None,
         namespace: str = None,
@@ -38,15 +52,18 @@
     ):
         super(StorageTable, self).__init__(
             name=name,
             namespace=namespace,
             address=address,
             partitions=partitions,
             options=options,
-            engine=StorageEngine.FILE
+            engine=StorageEngine.FILE,
+            key_serdes_type=0,
+            value_serdes_type=0,
+            partitioner_type=0
         )
         self._local_fs_client = fs.LocalFileSystem()
 
     @property
     def path(self):
         return self._address.path
 
@@ -65,22 +82,22 @@
             stream = self._local_fs_client.open_output_stream(
                 path=self.path, compression=None
             )
 
         counter = self._meta.get_count() if self._meta.get_count() else 0
         with io.TextIOWrapper(stream) as writer:
             for k, v in kv_list:
-                writer.write(DataManager.serialize_data(k, v))
+                writer.write(FileCoder.encode(k, v))
                 writer.write("\n")
                 counter = counter + 1
         self._meta.update_metas(count=counter)
 
     def _collect(self, **kwargs) -> list:
         for line in self._as_generator():
-            yield DataManager.deserialize_data(line.rstrip())
+            yield FileCoder.decode(line.rstrip())
 
     def _read(self) -> list:
         for line in self._as_generator():
             yield line
 
     def _destroy(self):
         # use try/catch to avoid stop while deleting an non-exist file
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/hdfs/__init__.py` & `fate_flow-2.1.0/fate_flow/engine/storage/hdfs/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/hdfs/_table.py` & `fate_flow-2.1.0/fate_flow/engine/storage/hdfs/_table.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,27 +10,42 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import io
-from typing import Iterable
+from typing import Iterable, Tuple
 
 from pyarrow import fs
 
 from fate_flow.engine.storage import StorageTableBase
 from fate_flow.engine.storage._types import StorageEngine
-from fate_flow.manager.data.data_manager import DataManager
 from fate_flow.utils.log import getLogger
+import struct
 
 
 LOGGER = getLogger()
 
 
+class HDFSCoder:
+    @staticmethod
+    def encode(key: bytes, value: bytes):
+        size = struct.pack(">Q", len(key))
+        return (size + key + value).hex()
+
+    @staticmethod
+    def decode(data: str) -> Tuple[bytes, bytes]:
+        data = bytes.fromhex(data)
+        size = struct.unpack(">Q", data[:8])[0]
+        key = data[8 : 8 + size]
+        value = data[8 + size :]
+        return key, value
+
+
 class StorageTable(StorageTableBase):
     def __init__(
             self,
             address=None,
             name: str = None,
             namespace: str = None,
             partitions: int = 1,
@@ -38,22 +53,31 @@
     ):
         super(StorageTable, self).__init__(
             name=name,
             namespace=namespace,
             address=address,
             partitions=partitions,
             options=options,
-            engine=StorageEngine.HDFS
+            engine=StorageEngine.HDFS,
+            key_serdes_type=0,
+            value_serdes_type=0,
+            partitioner_type=0,
         )
         try:
+            # noinspection PyUnresolvedReferences
             from pyarrow import HadoopFileSystem
             HadoopFileSystem(self.path)
         except Exception as e:
             LOGGER.warning(f"load libhdfs failed: {e}")
 
+        # pyarrow.fs.HadoopFileSystem.from_uri(uri, **kwargs) supports the following formats:
+        #   * ``HadoopFileSystem.from_uri('hdfs://localhost:8020/?user=test&replication=1')``
+        #   * ``HadoopFileSystem('localhost', port=8020, user='test', replication=1)``
+        # your IDE may complain about the following line, but it works.
+        # noinspection PyArgumentList
         self._hdfs_client = fs.HadoopFileSystem.from_uri(self.path)
 
     def check_address(self):
         return self._exist()
 
     def _put_all(
             self, kv_list: Iterable, append=True, assume_file_exist=False, **kwargs
@@ -70,22 +94,22 @@
             stream = client.open_output_stream(
                 path=path, compression=None
             )
 
         counter = self._meta.get_count() if self._meta.get_count() else 0
         with io.TextIOWrapper(stream) as writer:
             for k, v in kv_list:
-                writer.write(DataManager.serialize_data(k, v))
+                writer.write(HDFSCoder.encode(k, v))
                 writer.write("\n")
                 counter = counter + 1
         self._meta.update_metas(count=counter)
 
     def _collect(self, **kwargs) -> list:
         for line in self._as_generator():
-            yield DataManager.deserialize_data(line.rstrip())
+            yield HDFSCoder.decode(line.rstrip())
 
     def _read(self) -> list:
         for line in self._as_generator():
             yield line
 
     def _destroy(self):
         self._hdfs_client.delete_file(self.file_path)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/standalone/__init__.py` & `fate_flow-2.1.0/fate_flow/engine/storage/standalone/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/standalone/_session.py` & `fate_flow-2.1.0/fate_flow/engine/storage/standalone/_table.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,33 +9,58 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-from fate_flow.engine.storage import StorageSessionBase, StorageEngine
+from typing import Iterable
+
+from fate_flow.engine.storage import (
+    StandaloneStoreType,
+    StorageEngine,
+    StorageTableBase,
+)
 from fate_flow.engine.storage.standalone._standalone import Session
-from fate_flow.entity.types import AddressABC, StandaloneAddress
 
 
-class StorageSession(StorageSessionBase):
-    def __init__(self, session_id, options=None):
-        super(StorageSession, self).__init__(session_id=session_id, engine=StorageEngine.STANDALONE)
-        self._options = options if options else {}
-        self._session = Session(session_id=self._session_id)
-
-    def table(self, address: AddressABC, name, namespace, partitions, store_type=None, options=None, **kwargs):
-        if isinstance(address, StandaloneAddress):
-            from fate_flow.engine.storage.standalone._table import StorageTable
-            return StorageTable(session=self._session, name=name, namespace=namespace, address=address,
-                                partitions=partitions, store_type=store_type, options=options)
-        raise NotImplementedError(f"address type {type(address)} not supported with standalone storage")
+class StorageTable(StorageTableBase):
+    def __init__(
+        self,
+        session: Session,
+        table,
+        key_serdes_type,
+        value_serdes_type,
+        partitioner_type,
+        address=None,
+        name: str = None,
+        namespace: str = None,
+        partitions: int = 1,
+        store_type: StandaloneStoreType = StandaloneStoreType.ROLLPAIR_LMDB,
+        options=None,
+    ):
+        super(StorageTable, self).__init__(
+            name=name,
+            namespace=namespace,
+            address=address,
+            partitions=partitions,
+            options=options,
+            engine=StorageEngine.STANDALONE,
+            key_serdes_type=key_serdes_type,
+            value_serdes_type=value_serdes_type,
+            partitioner_type=partitioner_type,
+        )
+        self._store_type = store_type
+        self._session = session
+        self._table = table
+
+    def _put_all(self, kv_list: Iterable, partitioner, **kwargs):
+        return self._table.put_all(kv_list, partitioner)
 
-    def cleanup(self, name, namespace):
-        self._session.cleanup(name=name, namespace=namespace)
+    def _collect(self, **kwargs):
+        return self._table.collect(**kwargs)
 
-    def stop(self):
-        self._session.stop()
+    def _count(self):
+        return self._table.count()
 
-    def kill(self):
-        self._session.kill()
+    def _destroy(self):
+        self._table.destroy()
```

### Comparing `fate_flow-2.0.0b0/fate_flow/engine/storage/standalone/_table.py` & `fate_flow-2.1.0/fate_flow/manager/components/download.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,66 +9,50 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-from typing import Iterable
+import os
 
-from fate_flow.engine.storage import StandaloneStoreType, StorageEngine, StorageTableBase
-from fate_flow.engine.storage.standalone._standalone import Session
+from fate_flow.engine import storage
+from fate_flow.manager.outputs.data import DataManager
 
 
-class StorageTable(StorageTableBase):
-    def __init__(
-        self,
-        session: Session,
-        address=None,
-        name: str = None,
-        namespace: str = None,
-        partitions: int = 1,
-        store_type: StandaloneStoreType = StandaloneStoreType.ROLLPAIR_LMDB,
-        options=None,
-    ):
-        super(StorageTable, self).__init__(
-            name=name,
-            namespace=namespace,
-            address=address,
-            partitions=partitions,
-            options=options,
-            engine=StorageEngine.STANDALONE,
-        )
-        self._store_type = store_type
-        self._session = session
-        self._table = self._session.create_table(
-            namespace=self.address.namespace,
-            name=self.address.name,
-            partitions=partitions,
-            need_cleanup=self._store_type == StandaloneStoreType.ROLLPAIR_IN_MEMORY,
-            error_if_exist=False,
-        )
+class Param(object):
+    def to_dict(self):
+        d = {}
+        for k, v in self.__dict__.items():
+            if v is None:
+                continue
+            d[k] = v
+        return d
 
-    def _put_all(self, kv_list: Iterable, **kwargs):
-        return self._table.put_all(kv_list)
 
-    def _collect(self, **kwargs):
-        return self._table.collect(**kwargs)
+class DownloadParam(Param):
+    def __init__(
+            self,
+            dir_name="",
+            namespace="",
+            name=""
+    ):
+        self.dir_name = dir_name
+        self.namespace = namespace
+        self.name = name
 
-    def _count(self):
-        return self._table.count()
 
-    def _destroy(self):
-        self._table.destroy()
-
-    def _save_as(self, address, name, namespace, partitions=None, **kwargs):
-        self._table.save_as(name=address.name, namespace=address.namespace)
-
-        table = StorageTable(
-            session=self._session,
-            address=address,
-            partitions=partitions,
-            name=name,
-            namespace=namespace,
-            **kwargs,
+class Download:
+    def __init__(self):
+        self.table = None
+        self.schema = {}
+
+    def run(self, parameters: DownloadParam, job_id=""):
+        data_table_meta = storage.StorageTableMeta(
+            name=parameters.name,
+            namespace=parameters.namespace
         )
-        return table
+        DataManager.send_table(
+            output_tables_meta={"table": data_table_meta},
+            download_dir=os.path.abspath(parameters.dir_name)
+        )
+
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/__init__.py` & `fate_flow-2.1.0/fate_flow/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/_base.py` & `fate_flow-2.1.0/fate_flow/entity/_base.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/code/__init__.py` & `fate_flow-2.1.0/fate_flow/entity/code/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/code/_api.py` & `fate_flow-2.1.0/fate_flow/entity/code/_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     class Job:
         PARAMS_ERROR = 1000
         NOT_FOUND = 1001
         CREATE_JOB_FAILED = 1002
         UPDATE_FAILED = 1003
         KILL_FAILED = 1004
         RESOURCE_EXCEPTION = 1005
-        INHERITANCE_FAILED = 1006
+        RESOURCE_LIMIT_EXCEEDED = 1006
+        INHERITANCE_FAILED = 1007
 
     class Task:
         NOT_FOUND = 2000
         START_FAILED = 2001
         UPDATE_FAILED = 2002
         KILL_FAILED = 2003
         RESOURCE_EXCEPTION = 2004
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/code/_process.py` & `fate_flow-2.1.0/fate_flow/entity/code/_process.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/code/_schedule.py` & `fate_flow-2.1.0/fate_flow/entity/code/_schedule.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/__init__.py` & `fate_flow-2.1.0/fate_flow/adapter/bfia/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/__init__.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-from fate_flow.entity.spec.dag._output import ComponentOutputMeta, MetricData
+from fate_flow.entity.spec.dag._output import ComponentOutputMeta, MetricData, OutputArtifactType, OutputArtifactSpec, \
+    OutputArtifacts, IOMeta
 from fate_flow.entity.spec.dag._party import PartySpec
 from fate_flow.entity.spec.dag._job import DAGSchema, DAGSpec, JobConfSpec, TaskConfSpec, TaskSpec, PartyTaskSpec, \
     InheritConfSpec, PartyTaskRefSpec
 from fate_flow.entity.spec.dag._task import TaskConfigSpec, PreTaskConfigSpec, TaskRuntimeConfSpec, \
     TaskCleanupConfigSpec
 from fate_flow.entity.spec.dag._artifact import RuntimeTaskOutputChannelSpec, DataWarehouseChannelSpec, \
-    ModelWarehouseChannelSpec, SourceInputArtifactSpec, RuntimeInputArtifacts, FlowRuntimeInputArtifacts,\
-    ArtifactInputApplySpec, Metadata, RuntimeTaskOutputChannelSpec, \
+    ModelWarehouseChannelSpec, RuntimeInputArtifacts, FlowRuntimeInputArtifacts,\
+    ArtifactInputApplySpec, Metadata, RuntimeTaskOutputChannelSpec, InputArtifactSpec, \
     ArtifactOutputApplySpec, ModelWarehouseChannelSpec, ArtifactOutputSpec, ArtifactSource
-from fate_flow.entity.spec.dag._component import ComponentSpec, ComponentIOArtifactsTypeSpec
+from fate_flow.entity.spec.dag._component import ComponentSpec, ComponentIOArtifactsTypeSpec, ComponentSpecV1
 from fate_flow.entity.spec.dag._computing import EggrollComputingSpec, SparkComputingSpec, StandaloneComputingSpec
 from fate_flow.entity.spec.dag._federation import StandaloneFederationSpec, RollSiteFederationSpec, OSXFederationSpec, \
     PulsarFederationSpec, RabbitMQFederationSpec
 from fate_flow.entity.spec.dag._logger import FlowLogger
 from fate_flow.entity.spec.dag._mlmd import MLMDSpec
-from fate_flow.entity.spec.dag._device import LauncherSpec
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_artifact.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_artifact.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 # see https://www.rfc-editor.org/rfc/rfc3986#appendix-B
 # scheme    = $2
 # authority = $4
 # path      = $5
 # query     = $7
 # fragment  = $9
+from ._party import PartySpec
+
 _uri_regex = re.compile(r"^(([^:/?#]+):)?(//([^/?#]*))?([^?#]*)(\?([^#]*))?(#(.*))?")
 
 
 class ArtifactSource(pydantic.BaseModel):
     task_id: str
     party_task_id: str
     task_name: str
@@ -123,60 +125,52 @@
     def load_uri(cls, engine, address):
         pass
 
 
 class RuntimeTaskOutputChannelSpec(pydantic.BaseModel):
     producer_task: str
     output_artifact_key: str
-    roles: Optional[List[Literal["guest", "host", "arbiter", "local"]]]
+    output_artifact_type_alias: Optional[str]
+    parties: Optional[List[PartySpec]]
 
     class Config:
         extra = "forbid"
 
 
 class DataWarehouseChannelSpec(pydantic.BaseModel):
     job_id: Optional[str]
     producer_task: Optional[str]
     output_artifact_key: Optional[str]
-    roles: Optional[List[Literal["guest", "host", "arbiter", "local"]]]
     namespace: Optional[str]
     name: Optional[str]
+    dataset_id: Optional[str]
+    parties: Optional[List[PartySpec]]
 
     class Config:
         extra = "forbid"
 
 
 class ModelWarehouseChannelSpec(pydantic.BaseModel):
     model_id: Optional[str]
     model_version: Optional[str]
     producer_task: str
     output_artifact_key: str
-    roles: Optional[List[Literal["guest", "host", "arbiter", "local"]]]
+    parties: Optional[List[PartySpec]]
 
     class Config:
         extra = "forbid"
 
 
 InputArtifactSpec = TypeVar("InputArtifactSpec",
                             RuntimeTaskOutputChannelSpec,
                             ModelWarehouseChannelSpec,
                             DataWarehouseChannelSpec)
 
 
-SourceInputArtifactSpec = TypeVar("SourceInputArtifactSpec",
-                                  ModelWarehouseChannelSpec,
-                                  DataWarehouseChannelSpec)
-
-
 class RuntimeInputArtifacts(pydantic.BaseModel):
     data: Optional[Dict[str, Dict[str, Union[List[InputArtifactSpec], InputArtifactSpec]]]]
     model: Optional[Dict[str, Dict[str, Union[List[InputArtifactSpec], InputArtifactSpec]]]]
 
 
-class SourceInputArtifacts(pydantic.BaseModel):
-    data: Optional[Dict[str, Dict[str, Union[SourceInputArtifactSpec, List[SourceInputArtifactSpec]]]]]
-    model: Optional[Dict[str, Dict[str, Union[SourceInputArtifactSpec, List[SourceInputArtifactSpec]]]]]
-
-
 class FlowRuntimeInputArtifacts(pydantic.BaseModel):
     data: Optional[Dict[str, Union[InputArtifactSpec, List[InputArtifactSpec]]]]
     model: Optional[Dict[str, Union[InputArtifactSpec, List[InputArtifactSpec]]]]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_component.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_component.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 #  limitations under the License.
 from typing import Optional, Dict, List, Union, Any, Literal
 from pydantic import BaseModel
 
 
 class ParameterSpec(BaseModel):
     type: str
-    default: Any
+    default: Optional[Any]
     optional: bool
     description: str = ""
     type_meta: dict = {}
 
 
 class ArtifactSpec(BaseModel):
-    type: str
+    types: List[str]
     optional: bool
     stages: Optional[List[str]]
     roles: Optional[List[str]]
     description: str = ""
     is_multi: bool
 
 
@@ -65,15 +65,15 @@
     parameters: Optional[Dict[str, Any]]
     artifacts: Optional[Dict[str, Dict[str, RuntimeOutputChannelSpec]]]
 
 
 class ArtifactTypeSpec(BaseModel):
     type_name: str
     uri_types: List[str]
-    path_type: Literal["file", "directory", "distributed"]
+    path_type: Literal["file", "directory", "distributed", "unresolved"]
 
 
 class ComponentIOArtifactTypeSpec(BaseModel):
     name: str
     is_multi: bool
     optional: bool
     types: List[ArtifactTypeSpec]
@@ -89,7 +89,12 @@
     model: List[ComponentIOArtifactTypeSpec]
     metric: List[ComponentIOArtifactTypeSpec]
 
 
 class ComponentIOArtifactsTypeSpec(BaseModel):
     inputs: ComponentIOInputsArtifactsTypeSpec
     outputs: ComponentIOOutputsArtifactsTypeSpec
+
+
+class ComponentSpecV1(BaseModel):
+    component: ComponentSpec
+    schema_version: str = "v1"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_computing.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_computing.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,37 +11,43 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from typing import Literal, TypeVar
 
 import pydantic
+from pydantic import typing
 
 
 class StandaloneComputingSpec(pydantic.BaseModel):
     class MetadataSpec(pydantic.BaseModel):
         computing_id: str
         options: dict = {}
 
     type: Literal["standalone"]
     metadata: MetadataSpec
 
 
 class EggrollComputingSpec(pydantic.BaseModel):
     class MetadataSpec(pydantic.BaseModel):
         computing_id: str
+        host: typing.Optional[str] = None
+        port: typing.Optional[int] = None
+        config_options: typing.Optional[dict] = None
+        config_properties_file: typing.Optional[str] = None
         options: dict = {}
 
     type: Literal["eggroll"]
     metadata: MetadataSpec
 
 
 class SparkComputingSpec(pydantic.BaseModel):
     class MetadataSpec(pydantic.BaseModel):
         computing_id: str
+        options: dict = {}
 
     type: Literal["spark"]
     metadata: MetadataSpec
 
 
 class CustomComputingSpec(pydantic.BaseModel):
     type: Literal["custom"]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_device.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_device.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,12 +22,7 @@
     type: Literal["CPU"]
     metadata: dict = {}
 
 
 class GPUSpec(pydantic.BaseModel):
     type: Literal["GPU"]
     metadata: dict = {}
-
-
-class LauncherSpec(pydantic.BaseModel):
-    name: str = "default"
-    conf: dict = {}
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_federation.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_federation.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_job.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,52 +9,55 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-from typing import Optional, Union, Literal, Dict, List, Any
+from typing import Optional, Union, Literal, Dict, List, Any, Tuple
 
 from pydantic import BaseModel
 
+from fate_flow.entity.spec.dag._output import OutputArtifacts
 from fate_flow.entity.spec.dag._party import PartySpec
-from fate_flow.entity.spec.dag._artifact import RuntimeInputArtifacts, SourceInputArtifacts
+from fate_flow.entity.spec.dag._artifact import RuntimeInputArtifacts
 
 
 class TaskSpec(BaseModel):
     component_ref: str
     dependent_tasks: Optional[List[str]]
     parameters: Optional[Dict[Any, Any]]
     inputs: Optional[RuntimeInputArtifacts]
+    outputs: Optional[OutputArtifacts]
     parties: Optional[List[PartySpec]]
     conf: Optional[Dict[Any, Any]]
     stage: Optional[Union[Literal["train", "predict", "default", "cross_validation"]]]
 
 
 class PartyTaskRefSpec(BaseModel):
     parameters: Optional[Dict[Any, Any]]
-    inputs: Optional[SourceInputArtifacts]
     conf: Optional[Dict]
 
 
 class PartyTaskSpec(BaseModel):
     parties: Optional[List[PartySpec]]
     tasks: Optional[Dict[str, PartyTaskRefSpec]] = {}
-    conf: Optional[dict]
+    conf: Optional[dict] = {}
 
 
 class EngineRunSpec(BaseModel):
     name: str
     conf: Optional[Dict]
 
 
 class TaskConfSpec(BaseModel):
-    run: Optional[Dict]
+    engine_run: Optional[Dict]
     provider: Optional[str]
+    timeout: Optional[int]
+    launcher_name: Optional[str] = "default"
 
 
 class InheritConfSpec(BaseModel):
     job_id: str
     task_list: List[str]
 
 
@@ -63,29 +66,29 @@
         model_id: str
         model_version: Union[str, int]
     priority: Optional[int]
     scheduler_party_id: Optional[str]
     initiator_party_id: Optional[str]
     inheritance: Optional[InheritConfSpec]
     cores: Optional[int]
-    task_cores: Optional[int]
     computing_partitions: Optional[int]
     sync_type: Optional[Union[Literal["poll", "callback"]]]
     auto_retries: Optional[int]
     model_id: Optional[str]
     model_version: Optional[Union[str, int]]
     model_warehouse: Optional[PipelineModel]
     task: Optional[TaskConfSpec]
-    engine: Optional[EngineRunSpec]
+    extra: Optional[Dict[Any, Any]]
 
 
 class DAGSpec(BaseModel):
     parties: List[PartySpec]
     conf: Optional[JobConfSpec]
     stage: Optional[Union[Literal["train", "predict", "default", "cross_validation"]]]
     tasks: Dict[str, TaskSpec]
     party_tasks: Optional[Dict[str, PartyTaskSpec]]
 
 
 class DAGSchema(BaseModel):
-    dag: DAGSpec
+    dag: Union[DAGSpec, Any]
     schema_version: str
+    kind: str = "fate"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_logger.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,50 +52,69 @@
             "handlers": [],
             "level": level,
         }
         self.disable_existing_loggers = False
 
         # add loggers
         root_logger_dir = os.path.join(log_base_dir, "root")
+        # os.makedirs(root_logger_dir, exist_ok=True)
         self._add_root_loggers(
-            log_base_dir=root_logger_dir, formatter_name="root", delay=delay
+            log_base_dir=root_logger_dir, formatter_name="root", delay=delay, loglevel=level
         )
 
         component_logger_dir = os.path.join(log_base_dir, "component")
+        # os.makedirs(component_logger_dir, exist_ok=True)
         self._add_component_loggers(
             log_base_dir=component_logger_dir,
             formatter_name="component",
             delay=delay,
             loglevel=level,
         )
 
+        # os.makedirs(aggregate_log_base_dir, exist_ok=True)
+        self._add_party_id_loggers(
+            aggregate_log_base_dir=aggregate_log_base_dir, formatter_name="root", delay=delay, loglevel=level
+        )
+
         if aggregate_log_base_dir is not None:
             self._add_aggregate_error_logger(
-                aggregate_log_base_dir, formatter_name="root", delay=delay
+                aggregate_log_base_dir, formatter_name="root", delay=delay,
             )
 
     def build(self):
         return dict(
             version=self.version,
             formatters=self.formatters,
             handlers=self.handlers,
             filters=self.filters,
             loggers=self.loggers,
             root=self.root,
             disable_existing_loggers=self.disable_existing_loggers,
         )
 
-    def _add_root_loggers(self, log_base_dir, formatter_name, delay):
+    def _add_root_loggers(self, log_base_dir, formatter_name, delay, loglevel):
         for level in _LOGGER_LEVELS:
+            if logging.getLevelName(level) < logging.getLevelName(loglevel):
+                continue
             handler_name = f"root_{level.lower()}"
             self.handlers[handler_name] = self._create_file_handler(
                 level, formatter_name, delay, os.path.join(log_base_dir, level)
             )
             self.root["handlers"].append(handler_name)
 
+    def _add_party_id_loggers(self, aggregate_log_base_dir, formatter_name, delay, loglevel):
+        for level in _LOGGER_LEVELS:
+            if logging.getLevelName(level) < logging.getLevelName(loglevel):
+                continue
+            handler_name = f"root_party_{level.lower()}"
+            self.handlers[handler_name] = self._create_file_handler(
+                level, formatter_name, delay, os.path.join(aggregate_log_base_dir, level)
+            )
+            self.root["handlers"].append(handler_name)
+
     def _add_aggregate_error_logger(self, log_base_dir, formatter_name, delay):
         # error from all component
         handler_name = "global_error"
         self.handlers[handler_name] = self._create_file_handler(
             "ERROR", formatter_name, delay, os.path.join(log_base_dir, "ERROR")
         )
         self.root["handlers"].append(handler_name)
@@ -108,14 +127,16 @@
         #   component/
         #       DEBUG
         #       INFO
         #       WARNING
         #       ERROR
         component_handlers_names = []
         for level in _LOGGER_LEVELS:
+            if logging.getLevelName(level) < logging.getLevelName(loglevel):
+                continue
             handler_name = f"component_{level.lower()}"
             self.handlers[handler_name] = self._create_file_handler(
                 level, formatter_name, delay, os.path.join(log_base_dir, level)
             )
             component_handlers_names.append(handler_name)
 
         # add profile logger handler
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_mlmd.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_mlmd.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_output.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_output.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from typing import Literal, Union, List, Dict, Optional
 
 import pydantic
 from pydantic import typing
 
+from ._party import PartySpec
+
 
 class MetricData(pydantic.BaseModel):
     class Group(pydantic.BaseModel):
         name: str
         index: Optional[int]
     name: str
     type: Optional[str]
-    groups: List[Group]
+    groups: List[Group] = []
     step_axis: Optional[str]
     data: Union[List, Dict]
 
 
 class DirectoryDataPool(pydantic.BaseModel):
     class DirectoryDataPoolMetadata(pydantic.BaseModel):
         uri: str
@@ -96,7 +98,31 @@
 
 class ComponentOutputMeta(pydantic.BaseModel):
     class Status(pydantic.BaseModel):
         code: int
         exceptions: typing.Optional[str]
     status: Status
     io_meta: typing.Optional[IOMeta]
+
+
+class OutputArtifactSpec(pydantic.BaseModel):
+    output_artifact_key_alias: str
+    output_artifact_type_alias: str
+    parties: Optional[List[PartySpec]]
+
+
+class OutputArtifacts(pydantic.BaseModel):
+    data: Optional[Dict[str, Union[OutputArtifactSpec, List[OutputArtifactSpec]]]]
+    model: Optional[Dict[str, Union[OutputArtifactSpec, List[OutputArtifactSpec]]]]
+    metric: Optional[Dict[str, Union[OutputArtifactSpec, List[OutputArtifactSpec]]]]
+
+
+class OutputArtifactType(object):
+    DATA = "data"
+    MODEL = "model"
+    METRIC = "metric"
+
+    @classmethod
+    def types(cls):
+        for _type in [cls.DATA, cls.MODEL, cls.METRIC]:
+            yield _type
+
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_party.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_party.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/dag/_task.py` & `fate_flow-2.1.0/fate_flow/entity/spec/dag/_task.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/flow/__init__.py` & `fate_flow-2.1.0/fate_flow/entity/spec/flow/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,10 +12,14 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from ._model import MLModelSpec, Metadata
 from ._storage import FileStorageSpec, MysqlStorageSpec, TencentCosStorageSpec
 from ._provider import ProviderSpec, DockerProviderSpec, K8sProviderSpec, LocalProviderSpec
 from ._scheduler import SchedulerInfoSpec
+from ._protocol import SubmitJobInput, SubmitJobOutput, QueryJobInput, QueryJobOutput, StopJobInput, StopJobOutput, \
+    QueryTaskOutput, QueryTaskInput
 
 __all__ = ["MLModelSpec", "FileStorageSpec", "MysqlStorageSpec", "TencentCosStorageSpec", "ProviderSpec",
-           "DockerProviderSpec", "K8sProviderSpec", "LocalProviderSpec", "SchedulerInfoSpec", "Metadata"]
+           "DockerProviderSpec", "K8sProviderSpec", "LocalProviderSpec", "SchedulerInfoSpec", "Metadata",
+           "SubmitJobInput", "SubmitJobOutput", "QueryJobInput", "QueryJobOutput", "StopJobInput", "StopJobOutput",
+           "QueryTaskInput", "QueryTaskOutput"]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/flow/_model.py` & `fate_flow-2.1.0/fate_flow/entity/spec/flow/_model.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/flow/_provider.py` & `fate_flow-2.1.0/fate_flow/entity/spec/flow/_provider.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/flow/_scheduler.py` & `fate_flow-2.1.0/fate_flow/entity/spec/flow/_scheduler.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/spec/flow/_storage.py` & `fate_flow-2.1.0/fate_flow/entity/spec/flow/_storage.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/__init__.py` & `fate_flow-2.1.0/fate_flow/entity/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_address.py` & `fate_flow-2.1.0/fate_flow/entity/types/_address.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_api.py` & `fate_flow-2.1.0/fate_flow/entity/types/_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,11 +8,16 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-class AppType:
-    SITE = "site"
-    CLIENT = "client"
+class ProviderDevice(object):
+    LOCAL = "local"
+    DOCKER = "docker"
+    K8S = "k8s"
+
+
+class ProviderName(object):
+    FATE = "fate"
+    FATE_FLOW = "fate_flow"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_artificats.py` & `fate_flow-2.1.0/fate_flow/entity/types/_artificats.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_command.py` & `fate_flow-2.1.0/fate_flow/entity/types/_command.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_engine.py` & `fate_flow-2.1.0/fate_flow/entity/types/_engine.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_federation.py` & `fate_flow-2.1.0/fate_flow/entity/types/_federation.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 #  limitations under the License.
 #
 class CoordinationCommunicationProtocol(object):
     HTTP = "http"
     GRPC = "grpc"
 
 
+class OSXMode(object):
+    STREAM = "stream"
+    QUEUE = "queue"
+
+
 class FederatedMode(object):
     SINGLE = "SINGLE"
     MULTIPLE = "MULTIPLE"
 
     def is_single(self, value):
         return value == self.SINGLE
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_input.py` & `fate_flow-2.1.0/fate_flow/entity/types/_input.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_instance.py` & `fate_flow-2.1.0/fate_flow/entity/types/_instance.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_output.py` & `fate_flow-2.1.0/fate_flow/utils/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,29 +8,28 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import Dict, List, Union, Any
+#
+import os
+
+import dotenv
+import typing
 
-from fate_flow.entity import BaseModel
+from fate_flow.runtime.system_settings import VERSION_FILE_PATH
 
 
-class MetricData(BaseModel):
-    namespace: Union[str, None]
-    name: str
-    type: str
-    groups: Dict
-    metadata: Dict
-    data: Union[List, Dict]
+def get_versions() -> typing.Mapping[str, typing.Any]:
+    return dotenv.dotenv_values(
+        dotenv_path=VERSION_FILE_PATH
+    )
 
 
-class ModelStorageEngine(object):
-    FILE = "file"
-    MYSQL = "mysql"
-    TENCENT_COS = "tencent_cos"
+def get_flow_version() -> typing.Optional[str]:
+    return get_versions().get("FATE_FLOW")
 
 
-class ModelFileFormat(object):
-    JSON = "json"
+def get_default_fate_version() -> typing.Optional[str]:
+    return get_versions().get("FATE")
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_permission.py` & `fate_flow-2.1.0/fate_flow/entity/types/_permission.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_provider.py` & `fate_flow-2.1.0/fate_flow/engine/storage/serdes/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-class ProviderDevice(object):
-    LOCAL = "local"
-    DOCKER = "docker"
-    K8S = "k8s"
+#
+
+
+def get_serdes_by_type(serdes_type: int):
+    if serdes_type == 0:
+        from ._unrestricted_serdes import get_unrestricted_serdes
 
+        return get_unrestricted_serdes()
+    elif serdes_type == 1:
+        from ._integer_serdes import get_integer_serdes
 
-class ProviderName(object):
-    FATE = "fate"
-    FATE_FLOW = "fate_flow"
+        return get_integer_serdes()
+    else:
+        raise ValueError(f"serdes type `{serdes_type}` not supported")
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_status.py` & `fate_flow-2.1.0/fate_flow/entity/types/_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     READY = 'ready'
     RUNNING = "running"
     CANCELED = "canceled"
     TIMEOUT = "timeout"
     FAILED = "failed"
     PASS = "pass"
     SUCCESS = "success"
+    FINISHED = "finished"
 
     @classmethod
     def get_level(cls, status):
         return dict(zip(cls.status_list(), range(len(cls.status_list())))).get(status, None)
 
 
 class BaseStateTransitionRule(object):
@@ -51,14 +52,15 @@
             return True
 
 
 class JobStatus(BaseStatus):
     READY = StatusSet.READY
     WAITING = StatusSet.WAITING
     RUNNING = StatusSet.RUNNING
+    FINISHED = StatusSet.FINISHED
     CANCELED = StatusSet.CANCELED
     TIMEOUT = StatusSet.TIMEOUT
     FAILED = StatusSet.FAILED
     SUCCESS = StatusSet.SUCCESS
 
     class StateTransitionRule(BaseStateTransitionRule):
         RULES = {
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entity/types/_work.py` & `fate_flow-2.1.0/ofx/api/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,22 +8,10 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-from fate_flow.entity import CustomEnum
-
-
-class ProcessRole(CustomEnum):
-    DRIVER = "driver"
-    WORKER = "worker"
-
+from ofx.api.models import bfia, fate_flow
 
-class WorkerName(CustomEnum):
-    TASK_ENTRYPOINT = "task_entrypoint"
-    TASK_EXECUTE = "task_execute"
-    COMPONENT_DEFINE = "component_define"
-    TASK_CLEAN = "task_clean"
-    TASK_EXECUTE_CLEAN = "execute_clean"
+__all__ = [bfia, fate_flow]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entrypoint/__init__.py` & `fate_flow-2.1.0/fate_flow/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/entrypoint/cli.py` & `fate_flow-2.1.0/fate_flow/components/entrypoint/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 import json
 import logging
 import os
 import traceback
 
 import click
 
-from fate_flow.components.entrypoint.component import execute_component
-from fate_flow.entity.spec.dag import PreTaskConfigSpec, TaskConfigSpec, TaskCleanupConfigSpec
+from fate_flow.entity.spec.dag import PreTaskConfigSpec, TaskConfigSpec, IOMeta
 from fate_flow.hub.flow_hub import FlowHub
 
+logger = logging.getLogger(__name__)
+
 
 @click.group()
 def component():
     """
     Manipulate components: execute, list, generate describe file
     """
 
 
 @component.command()
 @click.option("--config", required=False, type=click.File(), help="config path")
-@click.option("--env-name", required=False, type=str, help="env name for config")
+@click.option("--env-name", required=True, type=str, help="env name for config", default="CONFIG")
 @click.option("--wraps-module", required=False, type=str, help="component run wraps module")
 def entrypoint(config, env_name, wraps_module):
     # parse config
     configs = {}
     load_config_from_env(configs, env_name)
     load_config_from_file(configs, config)
     task_config = PreTaskConfigSpec.parse_obj(configs)
@@ -82,17 +83,17 @@
     task_config = TaskConfigSpec.parse_obj(configs)
     task_config.conf.logger.install()
     logger = logging.getLogger(__name__)
     logger.debug("logger installed")
     logger.debug(f"task config: {task_config}")
     os.makedirs(os.path.dirname(execution_final_meta_path), exist_ok=True)
     try:
-        execute_component(task_config)
+        io_meta = execute_component(task_config)
         with open(execution_final_meta_path, "w") as fw:
-            json.dump(dict(status=dict(code=0)), fw, indent=4)
+            json.dump(dict(status=dict(code=0), io_meta=io_meta.dict()), fw, indent=4)
     except Exception as e:
         with open(execution_final_meta_path, "w") as fw:
             json.dump(dict(status=dict(code=-1, exceptions=traceback.format_exc())), fw)
         raise e
 
 
 def load_config_from_file(configs, config_file):
@@ -106,7 +107,24 @@
 def load_config_from_env(configs, env_name):
     import os
     from ruamel import yaml
 
     if env_name is not None and os.environ.get(env_name):
         configs.update(yaml.safe_load(os.environ[env_name]))
     return configs
+
+
+def execute_component(config: TaskConfigSpec):
+    component = load_component(config.component)
+    logger.info(f"parameters： {config.parameters}")
+    inputs = IOMeta.InputMeta(data={}, model={})
+    outputs = IOMeta.OutputMeta(data={}, model={}, metric={})
+    component.execute(config, outputs)
+    return IOMeta(inputs=inputs, outputs=outputs)
+
+
+def load_component(cpn_name: str):
+    from fate_flow.components.components import BUILDIN_COMPONENTS
+
+    for cpn in BUILDIN_COMPONENTS:
+        if cpn.name == cpn_name:
+            return cpn
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fate_flow-2.0.0b0/fate_flow/entrypoint/runner.py` & `fate_flow-2.1.0/fate_flow/components/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,26 +9,19 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import argparse
-
-from fate_flow.entity import BaseEntity
-from fate_flow.utils.log import getLogger
-
-
-class Submit:
-    @staticmethod
-    def run():
-        import click
-        from fate_flow.entrypoint.cli import component
-
-        cli = click.Group()
-        cli.add_command(component)
-        cli(prog_name="python -m fate_flow.entrypoint")
 
+"""
+execute with python -m fate.components --config xxx
+"""
 
 if __name__ == "__main__":
-    Submit.run()
+    import click
+    from fate_flow.components.entrypoint.cli import component
+
+    cli = click.Group()
+    cli.add_command(component)
+    cli(prog_name="python -m fate_flow.components")
```

### Comparing `fate_flow-2.0.0b0/fate_flow/errors/__init__.py` & `fate_flow-2.1.0/fate_flow/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/errors/server_error.py` & `fate_flow-2.1.0/fate_flow/errors/server_error.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/errors/zookeeper_error.py` & `fate_flow-2.1.0/fate_flow/errors/zookeeper_error.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/fate_flow_server.py` & `fate_flow-2.1.0/fate_flow/fate_flow_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,59 +16,69 @@
 import os
 import signal
 import sys
 import traceback
 
 import grpc
 from werkzeug.serving import run_simple
+
+if __name__ == '__main__':
+    from fate_flow.db.casbin_models import init_casbin
+    init_casbin()
+
 from fate_flow.apps import app
-from fate_flow.controller.config_manager import ConfigManager
+from fate_flow.manager.service.config_manager import ConfigManager
 from fate_flow.hook import HookManager
 from fate_flow.manager.service.app_manager import AppManager
 from fate_flow.manager.service.provider_manager import ProviderManager
 from fate_flow.manager.service.service_manager import service_db
 from fate_flow.runtime.runtime_config import RuntimeConfig
 from fate_flow.db.base_models import init_database_tables as init_flow_db
-from fate_flow.detection.detector import Detector, FederatedDetector
+from fate_flow.scheduler.detector import Detector, FederatedDetector
 from fate_flow.entity.types import ProcessRole
 from fate_flow.scheduler import init_scheduler
-from fate_flow.scheduler.job_scheduler import DAGScheduler
 from fate_flow.runtime.system_settings import (
     GRPC_PORT, GRPC_SERVER_MAX_WORKERS, HOST, HTTP_PORT , GRPC_OPTIONS, FATE_FLOW_LOG_DIR,
     LOG_LEVEL,
 )
+from fate_flow.scheduler.scheduler import DAGScheduler
 from fate_flow.utils import process_utils
-from fate_flow.utils.grpc_utils import UnaryService, UnaryServiceOSX
+from fate_flow.utils.grpc_utils import UnaryService
 from fate_flow.utils.log import LoggerFactory, getLogger
 from fate_flow.utils.log_utils import schedule_logger
 from fate_flow.utils.version import get_versions
 from fate_flow.utils.xthread import ThreadPoolExecutor
 from fate_flow.proto.rollsite import proxy_pb2_grpc
-from fate_flow.proto.osx import osx_pb2_grpc
 
 detect_logger = getLogger("fate_flow_detect")
 stat_logger = getLogger("fate_flow_stat")
 
 
 def server_init():
     # init logs
     LoggerFactory.set_directory(FATE_FLOW_LOG_DIR)
     LoggerFactory.LEVEL = LOG_LEVEL
 
     # set signal
     if "win" not in sys.platform.lower():
         signal.signal(signal.SIGCHLD, process_utils.wait_child_process)
 
+    # init adapter
+    try:
+        from fate_flow.adapter import init_adapter
+        init_adapter()
+    except Exception as ex:
+        stat_logger.exception(ex)
+
     # init db
     init_flow_db()
 
     # runtime config
     RuntimeConfig.init_env()
     RuntimeConfig.init_config(JOB_SERVER_HOST=HOST, HTTP_PORT=HTTP_PORT)
-    RuntimeConfig.set_process_role(ProcessRole.DRIVER)
     RuntimeConfig.init_config()
     RuntimeConfig.set_service_db(service_db())
     RuntimeConfig.SERVICE_DB.register_flow()
 
     # manager
     ConfigManager.load()
     HookManager.init()
@@ -89,15 +99,14 @@
 def start_server(debug=False):
     # grpc
     thread_pool_executor = ThreadPoolExecutor(max_workers=GRPC_SERVER_MAX_WORKERS)
     stat_logger.info(f"start grpc server thread pool by {thread_pool_executor.max_workers} max workers")
     server = grpc.server(thread_pool=thread_pool_executor,
                          options=GRPC_OPTIONS)
 
-    osx_pb2_grpc.add_PrivateTransferProtocolServicer_to_server(UnaryServiceOSX(), server)
     proxy_pb2_grpc.add_DataTransferServiceServicer_to_server(UnaryService(), server)
     server.add_insecure_port(f"{HOST}:{GRPC_PORT}")
     server.start()
     stat_logger.info("FATE Flow grpc server start successfully")
 
     # http
     stat_logger.info("FATE Flow http server start...")
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hook/__init__.py` & `fate_flow-2.1.0/fate_flow/hook/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/hook/common/__init__.py` & `fate_flow-2.1.0/fate_flow/hook/common/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/hook/common/parameters.py` & `fate_flow-2.1.0/fate_flow/hook/common/parameters.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/hook/flow/__init__.py` & `fate_flow-2.1.0/fate_flow/hook/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/hook/flow/client_authentication.py` & `fate_flow-2.1.0/fate_flow/hook/flow/client_authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fate_flow.controller.app_controller import Authentication, PermissionController
+from fate_flow.controller.permission import Authentication, PermissionController
 from fate_flow.entity.code import ReturnCode
 from fate_flow.errors.server_error import InvalidParameter
 from fate_flow.hook import HookManager
 from fate_flow.hook.common.parameters import AuthenticationReturn, AuthenticationParameters
 
 
 @HookManager.register_client_authentication_hook
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hook/flow/permission.py` & `fate_flow-2.1.0/fate_flow/hook/flow/permission.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from fate_flow.controller.permission_controller import PermissionCheck
+from fate_flow.controller.permission import PermissionCheck
 from fate_flow.entity.code import ReturnCode
 from fate_flow.hook import HookManager
 from fate_flow.hook.common.parameters import PermissionCheckParameters, PermissionReturn
 from fate_flow.runtime.system_settings import LOCAL_PARTY_ID, PARTY_ID
 
 
 @HookManager.register_permission_check_hook
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hook/flow/site_authentication.py` & `fate_flow-2.1.0/fate_flow/hook/flow/site_authentication.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import hashlib
 
-from fate_flow.controller.app_controller import PermissionController, Authentication
+from fate_flow.controller.permission import PermissionController, Authentication
 from fate_flow.entity.code import ReturnCode
 from fate_flow.errors.server_error import NoFoundAppid
 from fate_flow.hook import HookManager
 from fate_flow.hook.common.parameters import SignatureParameters, SignatureReturn, AuthenticationParameters, \
     AuthenticationReturn
 from fate_flow.manager.service.app_manager import AppManager
 from fate_flow.runtime.system_settings import LOCAL_PARTY_ID, PARTY_ID
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/__init__.py` & `fate_flow-2.1.0/fate_flow/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/components_wraps/__init__.py` & `fate_flow-2.1.0/fate_flow/hub/components_wraps/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/components_wraps/fate/__init__.py` & `fate_flow-2.1.0/fate_flow/hub/components_wraps/fate/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/components_wraps/fate/_wraps.py` & `fate_flow-2.1.0/fate_flow/hub/components_wraps/fate/_wraps.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,44 +12,49 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import io
 import json
 import logging
 import os.path
+import sys
 import tarfile
 import traceback
 from typing import List
 
 import yaml
 
 from fate_flow.engine.backend import build_backend
-from fate_flow.engine.storage import StorageEngine
+from fate_flow.engine.storage import StorageEngine, DataType, Session
 from fate_flow.entity.code import ReturnCode
 from fate_flow.entity.spec.dag import PreTaskConfigSpec, DataWarehouseChannelSpec, ComponentIOArtifactsTypeSpec, \
     TaskConfigSpec, ArtifactInputApplySpec, Metadata, RuntimeTaskOutputChannelSpec, \
-    ArtifactOutputApplySpec, ModelWarehouseChannelSpec, ArtifactOutputSpec, ComponentOutputMeta, TaskCleanupConfigSpec
+    ArtifactOutputApplySpec, ModelWarehouseChannelSpec, ArtifactOutputSpec, ComponentOutputMeta, TaskCleanupConfigSpec, \
+    PartySpec
 
 from fate_flow.entity.types import DataframeArtifactType, TableArtifactType, TaskStatus, ComputingEngine, \
-    JsonModelArtifactType
+    JsonModelArtifactType, LauncherType
 
 from fate_flow.hub.components_wraps import WrapsABC
-from fate_flow.manager.data.data_manager import DataManager, DatasetManager
-from fate_flow.runtime.system_settings import STANDALONE_DATA_HOME, DEFAULT_OUTPUT_DATA_PARTITIONS
+from fate_flow.manager.outputs.data import DataManager, DatasetManager
+from fate_flow.runtime.system_settings import STANDALONE_DATA_HOME, DEFAULT_OUTPUT_DATA_PARTITIONS, \
+    DEEPSPEED_MODEL_DIR_PLACEHOLDER, DEEPSPEED_LOGS_DIR_PLACEHOLDER
 from fate_flow.utils import job_utils
+from fate_flow.utils.job_utils import generate_deepspeed_id
 
 logger = logging.getLogger(__name__)
 
 
 class FlowWraps(WrapsABC):
     def __init__(self, config: PreTaskConfigSpec):
         self.config = config
         self.mlmd = self.load_mlmd(config.mlmd)
         self.backend = build_backend(backend_name=self.config.conf.computing.type, launcher_name=self.config.launcher_name)
         self._component_define = None
+        self._destroy_temp_data = []
 
     @property
     def task_info(self):
         return {
             "component": self.config.component,
             "job_id": self.config.job_id,
             "role": self.config.role,
@@ -82,15 +87,18 @@
                 logger.error(exceptions)
         except Exception as e:
             traceback.format_exc()
             code = ReturnCode.Task.TASK_RUN_FAILED
             exceptions = str(e)
             logger.error(e)
         finally:
+            self.destroy(code)
             self.report_status(code, exceptions)
+            if code:
+                sys.exit(code)
 
     def cleanup(self):
         config = TaskCleanupConfigSpec(
             computing=self.config.conf.computing,
             federation=self.config.conf.federation
         )
         return self.backend.cleanup(
@@ -109,14 +117,21 @@
         logger.debug(input_artifacts)
         logger.info(f"PYTHON PATH: {os.environ.get('PYTHONPATH')}")
 
         # output
         logger.info("start generating output artifacts")
         output_artifacts = self._preprocess_output_artifacts()
         logger.info(f"output_artifacts: {output_artifacts}")
+        logger_config = json.dumps(self.config.conf.logger.config)
+        if self.config.launcher_name == LauncherType.DEEPSPEED:
+            logger_config = logger_config.replace(
+                job_utils.get_job_log_directory(self.config.job_id),
+                os.path.join(DEEPSPEED_LOGS_DIR_PLACEHOLDER, self.config.job_id)
+            )
+            self.config.conf.logger.config = json.loads(logger_config)
         config = TaskConfigSpec(
             job_id=self.config.job_id,
             task_id=self.config.task_id,
             party_task_id=self.config.party_task_id,
             component=self.config.component,
             role=self.config.role,
             party_id=self.config.party_id,
@@ -136,38 +151,39 @@
         logger.info("start run task")
         os.makedirs(self.task_input_dir, exist_ok=True)
         os.makedirs(self.task_output_dir, exist_ok=True)
         conf_path = os.path.join(self.task_input_dir, "task_parameters.yaml")
         task_result = os.path.join(self.task_output_dir, "task_result.yaml")
         with open(conf_path, "w") as f:
             yaml.dump(task_parameters, f)
-        self.backend.run(
+        code = self.backend.run(
             provider_name=self.config.provider_name,
             task_info=self.task_info,
             engine_run=self.config.engine_run,
-            launcher_conf=self.config.launcher_conf,
             run_parameters=task_parameters,
             output_path=task_result,
             conf_path=conf_path,
-            session_id=self.config.party_task_id,
+            session_id=generate_deepspeed_id(self.config.party_task_id),
             sync=True
         )
-        logger.info("finish task")
+        logger.info(f"finish task, return code {code}")
         if os.path.exists(task_result):
             with open(task_result, "r") as f:
                 try:
                     result = json.load(f)
                     output_meta = ComponentOutputMeta.parse_obj(result)
-                    logger.debug(output_meta)
-                except:
-                    logger.error(f"Task run failed, you can see the task result file for details: {task_result}")
+                    if code != 0:
+                        output_meta.status.code = code
+                    # logger.debug(output_meta)
+                except Exception as e:
+                    raise RuntimeError(f"Task run failed {e}, you can see the task result file for details: {task_result}.")
         else:
             output_meta = ComponentOutputMeta(status=ComponentOutputMeta.Status(
                 code=ReturnCode.Task.NO_FOUND_RUN_RESULT,
-                exceptions=f"No found task output. Process exit code. "
+                exceptions=f"No found task output."
             ))
         return output_meta
 
     def push_output(self, output_meta: ComponentOutputMeta):
         if self.task_end_with_success(output_meta.status.code):
             # push output data to server
             if not output_meta.io_meta:
@@ -206,33 +222,43 @@
             namespace = output_data.metadata.namespace
             name = output_data.metadata.name
             if not namespace and not name:
                 namespace, name = DatasetManager.get_output_name(output_data.uri)
             logger.info(f"save data tracking to {namespace}, {name}")
             overview = output_data.metadata.data_overview
             source = output_data.metadata.source
+            uri = output_data.uri
+            if output_data.type_name == DataType.DATA_UNRESOLVED:
+                uri = ""
+                # check namespace and name（reader）
+                resp = self.mlmd.query_data_meta(name=name, namespace=namespace)
+                if resp.json().get("code") != 0:
+                    raise ValueError(f"Check failed[{resp.text}]")
             resp = self.mlmd.save_data_tracking(
                 execution_id=self.config.party_task_id,
                 output_key=output_key,
                 meta_data=output_data.metadata.metadata.get("schema", {}),
-                uri=output_data.uri,
+                uri=uri,
                 namespace=namespace,
                 name=name,
                 overview=overview.dict() if overview else {},
                 source=source.dict() if source else {},
                 data_type=output_data.type_name,
                 index=index,
                 partitions=DEFAULT_OUTPUT_DATA_PARTITIONS
             )
             self.log_response(resp, req_info="save data tracking")
 
     def _push_model(self, output_key, output_models: List[ArtifactOutputSpec]):
         logger.info("save model")
         logger.info(f"key[{output_key}] output_models[{output_models}]")
         tar_io = io.BytesIO()
+        if self.config.launcher_name == LauncherType.DEEPSPEED:
+            logger.info("pass")
+            return
         for output_model in output_models:
             engine, address = DataManager.uri_to_address(output_model.uri)
             if engine == StorageEngine.FILE:
                 _path = address.path
                 if os.path.exists(_path):
                     if os.path.isdir(_path):
                         path = _path
@@ -315,31 +341,47 @@
             for _k, _channels in self.config.input_artifacts.data.items():
                 if isinstance(_channels, list):
                     input_artifacts[_k] = []
                     for _channel in _channels:
                         _artifacts = self._intput_data_artifacts(_k, _channel)
                         if _artifacts:
                             input_artifacts[_k].append(_artifacts)
+                elif self._check_is_multi_input_data(_k):
+                    input_artifacts[_k] = [self._intput_data_artifacts(_k, _channels)]
                 else:
                     input_artifacts[_k] = self._intput_data_artifacts(_k, _channels)
                 if not input_artifacts[_k]:
                     input_artifacts.pop(_k)
 
         if self.config.input_artifacts.model:
             for _k, _channels in self.config.input_artifacts.model.items():
                 if isinstance(_channels, list):
                     input_artifacts[_k] = []
                     for _channel in _channels:
                         input_artifacts[_k].append(self._intput_model_artifacts(_k, _channel))
+                elif self._check_is_multi_input_model(_k):
+                    input_artifacts[_k] = [self._intput_model_artifacts(_k, _channels)]
                 else:
                     input_artifacts[_k] = self._intput_model_artifacts(_k, _channels)
                 if not input_artifacts[_k]:
                     input_artifacts.pop(_k)
         return input_artifacts
 
+    def _check_is_multi_input_model(self, key):
+        for define in self.component_define.inputs.model:
+            if define.name == key and define.is_multi:
+                return True
+        return False
+
+    def _check_is_multi_input_data(self, key):
+        for define in self.component_define.inputs.data:
+            if define.name == key and define.is_multi:
+                return True
+        return False
+
     def _preprocess_output_artifacts(self):
         # get component define
         logger.debug("get component define")
         define = self.component_define
         logger.info(f"component define: {define}")
         output_artifacts = {}
         if not define:
@@ -367,16 +409,21 @@
         if type_name in [DataframeArtifactType.type_name, TableArtifactType.type_name]:
             uri = DatasetManager.output_data_uri(self.config.conf.storage, self.config.task_id, is_multi=is_multi)
         else:
             if output_type == "metric":
                 # api path
                 uri = self.mlmd.get_metric_save_url(execution_id=self.config.party_task_id)
             else:
-                # local file path
-                uri = DatasetManager.output_local_uri(task_info=self.task_info, name=name, type_name=type_name, is_multi=is_multi)
+                base_dir = ""
+                if self.config.launcher_name == LauncherType.DEEPSPEED:
+                    base_dir = DEEPSPEED_MODEL_DIR_PLACEHOLDER
+                uri = DatasetManager.output_local_uri(
+                    task_info=self.task_info, name=name, type_name=type_name, is_multi=is_multi,
+                    base_dir=base_dir
+                )
         output_artifacts.uri = uri
         return output_artifacts
 
     @property
     def component_define(self) -> ComponentIOArtifactsTypeSpec:
         if not self._component_define:
             self.set_component_define()
@@ -388,15 +435,15 @@
             task_info=self.task_info,
             stage=self.config.stage
         )
         if define:
             self._component_define = ComponentIOArtifactsTypeSpec(**define)
 
     def _intput_data_artifacts(self, key, channel):
-        if self.config.role not in channel.roles:
+        if not job_utils.check_party_in(self.config.role, self.config.party_id, channel.parties):
             logger.info(f"role {self.config.role} does not require intput data artifacts")
             return
         # data reference conversion
         meta = ArtifactInputApplySpec(
             metadata=Metadata(
                 metadata=dict(options=dict(partitions=self.config.computing_partitions))
             ),
@@ -442,15 +489,18 @@
             raise ValueError(f"Get data artifacts failed: {query_field}, response: {resp.text}")
         resp_data = resp_json.get("data", [])
         logger.info(f"intput data artifacts are ready")
         if len(resp_data) == 1:
             data = resp_data[0]
             schema = data.get("meta", {})
             meta.metadata.metadata.update({"schema": schema})
-
+            meta.type_name = data.get("data_type")
+            if meta.type_name == DataType.TABLE:
+                # destroy table data
+                self._destroy_temp_data.append((data.get("namespace"), data.get("name")))
             meta.uri = data.get("path")
             source = data.get("source", {})
             if source:
                 meta.metadata.source = source
             return meta
         elif len(resp_data) > 1:
             meta_list = []
@@ -464,15 +514,15 @@
                     meta.metadata.source = source
                 meta_list.append(meta)
             return meta_list
         else:
             raise RuntimeError(resp_data)
 
     def _intput_model_artifacts(self, key, channel):
-        if self.config.role not in channel.roles:
+        if not job_utils.check_party_in(self.config.role, self.config.party_id, channel.parties):
             logger.info(f"role {self.config.role} does not require intput model artifacts")
             return
         # model reference conversion
         meta = ArtifactInputApplySpec(metadata=Metadata(metadata={}), uri="")
         query_field = {
             "task_name": channel.producer_task,
             "output_key": channel.output_artifact_key,
@@ -568,14 +618,29 @@
             )
         self.log_response(resp, req_info="report status")
 
     @staticmethod
     def task_end_with_success(code):
         return code == 0
 
+    def destroy(self, code):
+        if self.task_end_with_success(code):
+            for namespace, name in self._destroy_temp_data:
+                try:
+                    logger.info(f"destroy table {namespace}, {name}")
+                    with Session() as sess:
+                        table = sess.get_table(
+                            name=name,
+                            namespace=namespace
+                        )
+                        table.destroy()
+                        logger.info(f"destroy table success")
+                except Exception as e:
+                    logger.error(e)
+
     @staticmethod
     def load_mlmd(mlmd):
         if mlmd.type == "flow":
             from ofx.api.client import FlowSchedulerApi
             client = FlowSchedulerApi(
                 host=mlmd.metadata.get("host"),
                 port=mlmd.metadata.get("port"),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/database/mysql.py` & `fate_flow-2.1.0/fate_flow/hub/database/mysql.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/database/sqlite.py` & `fate_flow-2.1.0/fate_flow/entity/types/_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-from peewee import Insert
+from typing import Dict, List, Union, Any
+
+from fate_flow.entity import BaseModel
+
 
-from fate_flow.runtime.system_settings import SQLITE_PATH
+class ModelStorageEngine(object):
+    FILE = "file"
+    MYSQL = "mysql"
+    TENCENT_COS = "tencent_cos"
 
 
-def get_database_connection(config, decrypt_key):
-    Insert.on_conflict = lambda self, *args, **kwargs: self.on_conflict_replace()
-    from playhouse.apsw_ext import APSWDatabase
-    path = config.get("path")
-    if not path:
-        path = SQLITE_PATH
-    return APSWDatabase(path)
+class ModelFileFormat(object):
+    JSON = "json"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/encrypt/password_encrypt.py` & `fate_flow-2.1.0/fate_flow/hub/encrypt/password_encrypt.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/flow_hub.py` & `fate_flow-2.1.0/fate_flow/hub/flow_hub.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,45 +13,38 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from importlib import import_module
 
 from fate_flow.entity.types import ProviderName, ProviderDevice
 from fate_flow.runtime.component_provider import ComponentProvider
-from fate_flow.runtime.system_settings import DEFAULT_JOB_PARSER_MODULE, DEFAULT_JOB_SCHEDULER_MODULE, \
-    DEFAULT_COMPONENTS_WRAPS_MODULE
+from fate_flow.runtime.system_settings import DEFAULT_COMPONENTS_WRAPS_MODULE
 
 
 class FlowHub:
     @staticmethod
-    def load_job_parser(dag, module_name=DEFAULT_JOB_PARSER_MODULE):
-        class_name = module_name.split(".")[-1]
-        module = ".".join(module_name.split(".")[:-1])
-        return getattr(import_module(module), class_name)(dag)
-
-    @staticmethod
-    def load_job_scheduler(module_name=DEFAULT_JOB_SCHEDULER_MODULE):
-        class_name = module_name.split(".")[-1]
-        module = ".".join(module_name.split(".")[:-1])
-        return getattr(import_module(module), class_name)()
-
-    @staticmethod
     def load_components_wraps(config, module_name=None):
         if not module_name:
             module_name = DEFAULT_COMPONENTS_WRAPS_MODULE
         class_name = module_name.split(".")[-1]
         module = ".".join(module_name.split(".")[:-1])
         return getattr(import_module(module), class_name)(config)
 
     @staticmethod
     def load_provider_entrypoint(provider: ComponentProvider):
         entrypoint = None
         if provider.name == ProviderName.FATE and provider.device == ProviderDevice.LOCAL:
-            from fate_flow.hub.provider.fate import LocalFateEntrypoint
+            from fate_flow.hub.provider.local import LocalFateEntrypoint
             entrypoint = LocalFateEntrypoint(provider)
+        elif provider.name == ProviderName.FATE_FLOW:
+            from fate_flow.hub.provider.local import FATEFLowEntrypoint
+            entrypoint = FATEFLowEntrypoint(provider)
+        elif provider.device == ProviderDevice.DOCKER:
+            from fate_flow.hub.provider.docker import DockerEntrypoint
+            entrypoint = DockerEntrypoint(provider)
         return entrypoint
 
     @staticmethod
     def load_database(engine_name, config, decrypt_key):
         try:
             return getattr(import_module(f"fate_flow.hub.database.{engine_name}"), "get_database_connection")(
                 config, decrypt_key)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/parser/fate/__init__.py` & `fate_flow-2.1.0/fate_flow/proto/rollsite/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,13 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from fate_flow.hub.parser.fate._parser import TaskNodeInfo, JobParser, TaskParser
-
-__all__ = [
-    "TaskNodeInfo", "JobParser", "TaskParser"
-]
-
+import os
+import sys
 
+_pb_path = os.path.abspath(os.path.join(__file__, os.path.pardir))
+if _pb_path not in sys.path:
+    sys.path.append(_pb_path)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/parser/fate/_parser.py` & `fate_flow-2.1.0/fate_flow/controller/parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,43 +9,44 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import copy
+import logging
 import os
 from typing import Dict, Union, List
 
 import networkx as nx
 from pydantic import BaseModel
 
 from fate_flow.entity.spec.dag import DataWarehouseChannelSpec, ModelWarehouseChannelSpec, \
     RuntimeTaskOutputChannelSpec, ComponentSpec, EggrollComputingSpec, SparkComputingSpec, StandaloneComputingSpec, \
     StandaloneFederationSpec, RollSiteFederationSpec, OSXFederationSpec, \
     PulsarFederationSpec, RabbitMQFederationSpec, FlowLogger, MLMDSpec, TaskRuntimeConfSpec, \
-    DAGSchema, DAGSpec, PreTaskConfigSpec, FlowRuntimeInputArtifacts
+    DAGSchema, DAGSpec, PreTaskConfigSpec, FlowRuntimeInputArtifacts, OutputArtifactType, PartySpec
 from fate_flow.entity.types import EngineType, FederationEngine, DataSet, InputArtifactType, ArtifactSourceType, \
-    ComputingEngine
+    ComputingEngine, OSXMode
 from fate_flow.manager.service.provider_manager import ProviderManager
 from fate_flow.runtime.job_default_config import JobDefaultConfig
 from fate_flow.runtime.system_settings import ENGINES, PROXY, FATE_FLOW_CONF_PATH, HOST, HTTP_PORT, PROTOCOL, \
-    API_VERSION
+    API_VERSION, COMPUTING_CONF, LOG_LEVEL
 from fate_flow.utils import job_utils, file_utils
-from .. import TaskParserABC, JobParserABC
 
 
 class TaskNodeInfo(object):
     def __init__(self):
         self._runtime_parameters = None
         self._runtime_parties = None
         self._input_dependencies = None
         self._component_ref = None
         self._component_spec = None
         self._upstream_inputs = dict()
+        self._outputs = dict()
         self._stage = None
         self._conf = None
 
     @property
     def stage(self):
         return self._stage
 
@@ -82,14 +83,22 @@
         return self._upstream_inputs
 
     @upstream_inputs.setter
     def upstream_inputs(self, upstream_inputs):
         self._upstream_inputs = upstream_inputs
 
     @property
+    def outputs(self):
+        return self._outputs
+
+    @outputs.setter
+    def outputs(self, outputs):
+        self._outputs = outputs
+
+    @property
     def component_spec(self):
         return self._component_spec
 
     @component_spec.setter
     def component_spec(self, component_spec):
         self._component_spec = component_spec
 
@@ -110,33 +119,30 @@
         return self._conf
 
     @conf.setter
     def conf(self, conf):
         self._conf = conf
 
 
-class TaskParser(TaskParserABC):
-    def __init__(self, task_node, job_id, task_name, role, party_id, task_id="", execution_id="", model_id="",
-                 model_version="", task_version=None, parties=None, provider=None):
+class TaskParser(object):
+    def __init__(self, task_node, job_id, task_name, role=None, party_id=None, task_id="", execution_id="", model_id="",
+                 model_version="", task_version=None, parties=None, component=None, provider=None, **kwargs):
         self.task_node = task_node
         self.model_id = model_id
         self.model_version = model_version
         self.job_id = job_id
         self.task_name = task_name
         self.role = role
         self.party_id = party_id
         self.task_id = task_id
         self.task_version = task_version
         self.execution_id = execution_id
         self.parties = parties
         self._provider = None
-
-    @property
-    def need_run(self):
-        return (self.role, self.party_id) in [(party.role, party.party_id) for party in self.runtime_parties]
+        self.component = component
 
     @property
     def federation_id(self):
         return job_utils.generate_task_version_id(task_id=self.task_id, task_version=self.task_version)
 
     @property
     def computing_id(self):
@@ -144,15 +150,15 @@
 
     @property
     def runtime_parties(self):
         return self.task_node.runtime_parties
 
     @property
     def component_ref(self):
-        return self.task_node.component_ref
+        return self.component if self.component else self.task_node.component_ref
 
     @property
     def stage(self):
         return self.task_node.stage
 
     @property
     def runtime_parameters(self):
@@ -160,84 +166,96 @@
 
     @property
     def output_definitions(self):
         return self.task_node.output_definitions
 
     @property
     def task_runtime_conf(self):
-        _rc = self.task_node.conf.get(self.role, {}).get(self.party_id, {})
+        _rc = self.task_node.conf
         return _rc if _rc else {}
 
     @property
     def task_runtime_launcher(self):
-        return self.task_runtime_conf.get("launcher", {})
+        return self.task_runtime_conf.get("launcher_name", "default")
+
+    @property
+    def engine_run(self):
+        return self.task_runtime_conf.get("engine_run", {})
 
     @property
     def provider(self):
         if not self._provider:
             provider_name = self.task_runtime_conf.get("provider")
             self._provider = ProviderManager.check_provider_name(provider_name)
         return self._provider
 
     @property
+    def timeout(self):
+        return self.task_runtime_conf.get("timeout", JobDefaultConfig.task_timeout)
+
+    @property
     def provider_name(self):
         return ProviderManager.parser_provider_name(self.provider)[0]
 
     @property
     def input_parameters(self):
-        return self.task_node.runtime_parameters.get(self.role, {}).get(self.party_id, {})
+        return self.task_node.runtime_parameters
 
     @staticmethod
     def generate_mlmd():
         _type = "flow"
         return MLMDSpec(
             type=_type,
             metadata={
                 "host": HOST,
                 "port": HTTP_PORT,
                 "protocol": PROTOCOL,
                 "api_version": API_VERSION
             })
 
     def generate_logger_conf(self):
-        logger_conf = JobDefaultConfig.task_logger
         task_log_dir = job_utils.get_job_log_directory(self.job_id, self.role, self.party_id, self.task_name)
         job_party_log_dir = job_utils.get_job_log_directory(self.job_id, self.role, self.party_id)
-
-        # TODO: fix?
-        level = logger_conf.get("metadata", {}).get("level", "DEBUG")
         delay = True
         formatters = None
         return FlowLogger.create(task_log_dir=task_log_dir,
                                  job_party_log_dir=job_party_log_dir,
-                                 level=level,
+                                 level=logging.getLevelName(LOG_LEVEL),
                                  delay=delay,
                                  formatters=formatters)
 
     @staticmethod
     def generate_device():
         return JobDefaultConfig.task_device
 
     def generate_computing_conf(self):
         if ENGINES.get(EngineType.COMPUTING).lower() == ComputingEngine.STANDALONE:
+            from fate_flow.runtime.system_settings import STANDALONE_DATA_HOME
             return StandaloneComputingSpec(
                 type=ENGINES.get(EngineType.COMPUTING).lower(),
-                metadata={"computing_id": self.computing_id}
+                metadata={"computing_id": self.computing_id, "options": {"data_dir": STANDALONE_DATA_HOME}}
             )
 
         if ENGINES.get(EngineType.COMPUTING).lower() == ComputingEngine.EGGROLL:
             return EggrollComputingSpec(
                 type=ENGINES.get(EngineType.COMPUTING).lower(),
-                metadata={"computing_id": self.computing_id}
+                metadata={
+                    "computing_id": self.computing_id,
+                    "host": COMPUTING_CONF.get(ComputingEngine.EGGROLL).get("host"),
+                    "port": COMPUTING_CONF.get(ComputingEngine.EGGROLL).get("port")
+                }
             )
 
         if ENGINES.get(EngineType.COMPUTING).lower() == ComputingEngine.SPARK:
             return SparkComputingSpec(
                 type=ENGINES.get(EngineType.COMPUTING).lower(),
-                metadata={"computing_id": self.computing_id}
+                metadata={
+                    "computing_id": self.computing_id,
+                    "options": {"home": COMPUTING_CONF.get(ComputingEngine.SPARK).get("home")}
+                }
             )
 
     @staticmethod
     def generate_storage_conf():
         return ENGINES.get(EngineType.STORAGE).lower()
 
     def generate_federation_conf(self):
@@ -246,30 +264,42 @@
             for _party_id in party.party_id:
                 parties_info.append({"role": party.role, "partyid": _party_id})
         parties = {
             "local": {"role": self.role, "partyid": self.party_id},
             "parties": parties_info
         }
         engine_name = ENGINES.get(EngineType.FEDERATION).lower()
-        proxy_conf = PROXY.get(engine_name, {})
+        proxy_conf = copy.deepcopy(PROXY.get(engine_name, {}))
         if engine_name == FederationEngine.STANDALONE:
             spec = StandaloneFederationSpec(type=engine_name, metadata=StandaloneFederationSpec.MetadataSpec(
                 federation_id=self.federation_id, parties=parties))
         elif engine_name == FederationEngine.ROLLSITE:
             spec = RollSiteFederationSpec(type=engine_name, metadata=RollSiteFederationSpec.MetadataSpec(
                 federation_id=self.federation_id,
                 parties=parties,
                 rollsite_config=RollSiteFederationSpec.MetadataSpec.RollSiteConfig(**proxy_conf)
             ))
         elif engine_name == FederationEngine.OSX:
-            spec = OSXFederationSpec(type=engine_name, metadata=OSXFederationSpec.MetadataSpec(
-                federation_id=self.federation_id,
-                parties=parties,
-                osx_config=OSXFederationSpec.MetadataSpec.OSXConfig(**proxy_conf)
-            ))
+            mode = proxy_conf.pop("mode", OSXMode.QUEUE)
+            if mode == OSXMode.QUEUE:
+                spec = OSXFederationSpec(type=engine_name, metadata=OSXFederationSpec.MetadataSpec(
+                    federation_id=self.federation_id,
+                    parties=parties,
+                    osx_config=OSXFederationSpec.MetadataSpec.OSXConfig(**proxy_conf)
+                ))
+            elif mode == OSXMode.STREAM:
+                spec = RollSiteFederationSpec(
+                    type=FederationEngine.ROLLSITE,
+                    metadata=RollSiteFederationSpec.MetadataSpec(
+                        federation_id=self.federation_id,
+                        parties=parties,
+                        rollsite_config=RollSiteFederationSpec.MetadataSpec.RollSiteConfig(**proxy_conf)
+                ))
+            else:
+                raise RuntimeError(f"federation engine {engine_name} mode {mode}is not supported")
         elif engine_name == FederationEngine.PULSAR:
             route_table_path = os.path.join(FATE_FLOW_CONF_PATH, "pulsar_route_table.yaml")
             route_table = file_utils.load_yaml_conf(conf_path=route_table_path)
 
             spec = PulsarFederationSpec(type=engine_name, metadata=PulsarFederationSpec.MetadataSpec(
                 federation_id=self.federation_id,
                 parties=parties,
@@ -316,240 +346,410 @@
             provider_name=self.provider_name,
             party_task_id=self.execution_id,
             component=self.component_ref,
             role=self.role,
             stage=self.stage,
             party_id=self.party_id,
             parameters=self.input_parameters,
-            input_artifacts=self.task_node.upstream_inputs.get(self.role).get(self.party_id),
+            input_artifacts=self.task_node.upstream_inputs,
             conf=self.task_conf,
             mlmd=self.generate_mlmd()
         )
 
 
-class JobParser(JobParserABC):
-    def __init__(self, dag_conf):
-        self._dag = nx.DiGraph()
+class DagParser(object):
+    def __init__(self):
+        self._dag = dict()
+        self._global_dag = nx.DiGraph()
         self._links = dict()
         self._task_parameters = dict()
         self._task_parties = dict()
         self._tasks = dict()
+        self._task_runtime_parties = dict()
         self._conf = dict()
-        self.parse_dag(dag_schema=dag_conf)
 
     def parse_dag(self, dag_schema: DAGSchema, component_specs: Dict[str, ComponentSpec] = None):
         dag_spec = dag_schema.dag
         dag_stage = dag_spec.stage
         tasks = dag_spec.tasks
         if dag_spec.conf:
             self._conf = dag_spec.conf.dict(exclude_defaults=True)
         job_conf = self._conf.get("task", {})
+
+        for party in dag_spec.parties:
+            if party.role not in self._dag:
+                self._dag[party.role] = dict()
+            for party_id in party.party_id:
+                self._dag[party.role][party_id] = nx.DiGraph()
+
         for name, task_spec in tasks.items():
-            self._dag.add_node(name)
+            parties = task_spec.parties if task_spec.parties else dag_spec.parties
             task_stage = dag_stage
             component_ref = task_spec.component_ref
+            if task_spec.stage:
+                task_stage = task_spec.stage
+
+            self._global_dag.add_node(name, component_ref=component_ref)
+
+            self._task_runtime_parties[name] = parties
+
+            for party_spec in parties:
+                if party_spec.role not in self._tasks:
+                    self._tasks[party_spec.role] = dict()
+                for party_id in party_spec.party_id:
+                    self._dag[party_spec.role][party_id].add_node(name)
+                    if party_id not in self._tasks[party_spec.role]:
+                        self._tasks[party_spec.role][party_id] = dict()
+                    self._tasks[party_spec.role][party_id].update({
+                        name: TaskNodeInfo()
+                    })
+                    self._tasks[party_spec.role][party_id][name].stage = task_stage
+                    self._tasks[party_spec.role][party_id][name].component_ref = component_ref
+                    if component_specs:
+                        self._tasks[party_spec.role][party_id][name].component_spec = component_specs[name]
+
+        for name, task_spec in tasks.items():
             if not task_spec.conf:
                 task_conf = copy.deepcopy(job_conf)
             else:
                 task_conf = copy.deepcopy(job_conf)
                 task_conf.update(task_spec.conf)
-            if task_spec.stage:
-                task_stage = task_spec.stage
 
-            self._tasks[name] = TaskNodeInfo()
-            self._tasks[name].stage = task_stage
-            self._tasks[name].component_ref = component_ref
-            if component_specs:
-                self._tasks[name].component_spec = component_specs[name]
             self._init_task_runtime_parameters_and_conf(name, dag_schema, task_conf)
 
             self._init_upstream_inputs(name, dag_schema.dag)
+            self._init_outputs(name, dag_schema.dag)
 
     def _init_upstream_inputs(self, name, dag: DAGSpec):
         task_spec = dag.tasks[name]
-        common_upstream_inputs = dict()
-        if task_spec.inputs:
-            common_upstream_inputs = self._get_upstream_inputs(name, task_spec)
-
         upstream_inputs = dict()
-        role_keys = set([party.role for party in dag.parties])
-        for party in dag.parties:
-            if party.role not in role_keys:
-                continue
-            upstream_inputs[party.role] = dict()
-            for party_id in party.party_id:
-                upstream_inputs[party.role][party_id] = copy.deepcopy(common_upstream_inputs)
 
-        party_tasks = dag.party_tasks
-        if not party_tasks:
-            self._tasks[name].upstream_inputs = upstream_inputs
-            return
+        parties = task_spec.parties if task_spec.parties else dag.parties
+        for party in parties:
+            if party.role not in upstream_inputs:
+                upstream_inputs[party.role] = dict()
+            for party_id in party.party_id:
+                self._tasks[party.role][party_id][name].upstream_inputs = self._get_upstream_inputs(
+                    name, task_spec, party.role, party_id
+                )
 
-        for site_name, party_tasks_spec in party_tasks.items():
-            if not party_tasks_spec.tasks or name not in party_tasks_spec.tasks:
-                continue
-            party_task_spec = party_tasks_spec.tasks[name]
-            if not party_task_spec.inputs:
-                continue
-            party_upstream_inputs = self._get_upstream_inputs(name, party_task_spec)
-            for party in party_tasks_spec.parties:
-                for party_id in party.party_id:
-                    upstream_inputs[party.role][party_id].update(party_upstream_inputs)
+    def _get_upstream_inputs(self, name, task_spec, role, party_id):
+        upstream_inputs = dict()
+        runtime_parties = task_spec.parties
 
-        self._tasks[name].upstream_inputs = upstream_inputs
+        if runtime_parties:
+            runtime_parties_dict = dict((party.role, party.party_id) for party in runtime_parties)
+            if role not in runtime_parties_dict or party_id not in runtime_parties_dict[role]:
+                return upstream_inputs
 
-    def _get_upstream_inputs(self, name, task_spec):
-        upstream_inputs = dict()
-        runtime_roles = self._tasks[name].runtime_roles
         input_artifacts = task_spec.inputs
 
+        if not input_artifacts:
+            return upstream_inputs
+
         for input_type in InputArtifactType.types():
             artifacts = getattr(input_artifacts, input_type)
             if not artifacts:
                 continue
 
-            upstream_inputs[input_type] = dict()
-
             for input_key, output_specs_dict in artifacts.items():
-                upstream_inputs[input_type][input_key] = dict()
                 for artifact_source, channel_spec_list in output_specs_dict.items():
                     if artifact_source == ArtifactSourceType.MODEL_WAREHOUSE:
-                        if isinstance(channel_spec_list, list):
-                            inputs = []
-                            for channel in channel_spec_list:
-                                model_warehouse_channel = ModelWarehouseChannelSpec(
-                                    **channel.dict(exclude_defaults=True))
-                                if model_warehouse_channel.model_id is None:
-                                    model_warehouse_channel.model_id = \
-                                        self._conf.get("model_warehouse", {}).get("model_id", None)
-                                    model_warehouse_channel.model_version = \
-                                        self._conf.get("model_warehouse", {}).get("model_version", None)
-                                inputs.append(model_warehouse_channel)
-                        else:
-                            inputs = ModelWarehouseChannelSpec(**channel_spec_list.dict(exclude_defaults=True))
-                            if inputs.model_id is None:
-                                inputs.model_id = self._conf.get("model_warehouse", {}).get("model_id", None)
-                                inputs.model_version = self._conf.get("model_warehouse", {}).get("model_version", None)
-
-                        upstream_inputs[input_type][input_key] = inputs
-                        continue
+                        is_list = True
+                        if not isinstance(channel_spec_list, list):
+                            is_list = False
+                            channel_spec_list = [channel_spec_list]
+                        inputs = []
+                        for channel in channel_spec_list:
+                            model_warehouse_channel = ModelWarehouseChannelSpec(**channel.dict(exclude_defaults=True))
+                            if model_warehouse_channel.parties and not self.task_can_run(
+                                    role, party_id, runtime_parties=model_warehouse_channel.parties):
+                                continue
+
+                            if model_warehouse_channel.model_id is None:
+                                model_warehouse_channel.model_id = \
+                                    self._conf.get("model_warehouse", {}).get("model_id", None)
+                                model_warehouse_channel.model_version = \
+                                    self._conf.get("model_warehouse", {}).get("model_version", None)
+                            inputs.append(model_warehouse_channel)
+
+                        if not inputs:
+                            continue
+
+                        if input_type not in upstream_inputs:
+                            upstream_inputs[input_type] = dict()
+
+                        if is_list and len(inputs) == 1:
+                            is_list = False
+                        upstream_inputs[input_type][input_key] = inputs if is_list else inputs[0]
+                    elif artifact_source == ArtifactSourceType.DATA_WAREHOUSE:
+                        is_list = True
+                        if not isinstance(channel_spec_list, list):
+                            is_list = False
+                            channel_spec_list = [channel_spec_list]
+                        inputs = []
+                        for channel in channel_spec_list:
+                            if channel.parties and \
+                                    not self.task_can_run(role, party_id, runtime_parties=channel.parties):
+                                continue
+                            inputs.append(DataWarehouseChannelSpec(**channel.dict(exclude_defaults=True)))
+
+                        if not inputs:
+                            continue
+                        if input_type not in upstream_inputs:
+                            upstream_inputs[input_type] = dict()
+
+                        if is_list and len(inputs) == 1:
+                            is_list = False
+                        upstream_inputs[input_type][input_key] = inputs if is_list else inputs[0]
                     else:
-                        if artifact_source == ArtifactSourceType.DATA_WAREHOUSE:
-                            channel_spec = DataWarehouseChannelSpec
-                        else:
-                            channel_spec = RuntimeTaskOutputChannelSpec
-                        if isinstance(channel_spec_list, list):
-                            inputs = [channel_spec(**channel.dict(exclude_defaults=True))
-                                      for channel in channel_spec_list]
+                        if not isinstance(channel_spec_list, list):
+                            channel_spec_list = [channel_spec_list]
+
+                        filter_channel_spec_list = []
+                        for channel_spec in channel_spec_list:
+                            if channel_spec.parties:
+                                parties_dict = dict((party.role, party.party_id) for party in channel_spec.parties)
+                                if role not in parties_dict or party_id not in parties_dict[role]:
+                                    continue
+                            else:
+                                if channel_spec.producer_task not in self._dag[role][party_id].nodes:
+                                    continue
+                            filter_channel_spec_list.append(channel_spec)
+
+                        if not filter_channel_spec_list:
+                            continue
+
+                        if len(filter_channel_spec_list) > 1:
+                            inputs = [RuntimeTaskOutputChannelSpec(**channel.dict(exclude_defaults=True))
+                                      for channel in filter_channel_spec_list]
                         else:
-                            inputs = channel_spec(**channel_spec_list.dict(exclude_defaults=True))
+                            inputs = RuntimeTaskOutputChannelSpec(**filter_channel_spec_list[0].dict(exclude_defaults=True))
 
-                        upstream_inputs[input_type][input_key] = inputs
+                        if not inputs:
+                            continue
 
-                    if not isinstance(channel_spec_list, list):
-                        channel_spec_list = [channel_spec_list]
+                        if input_type not in upstream_inputs:
+                            upstream_inputs[input_type] = dict()
+                        upstream_inputs[input_type][input_key] = inputs
 
-                    for channel_spec in channel_spec_list:
-                        if isinstance(channel_spec, RuntimeTaskOutputChannelSpec):
+                        for channel_spec in filter_channel_spec_list:
                             dependent_task = channel_spec.producer_task
-                            self._add_edge(dependent_task, name)
+                            self._add_edge(dependent_task, name, role, party_id)
+
+        upstream_inputs = self.check_and_add_runtime_party(upstream_inputs, role, party_id, artifact_type="input")
 
-        upstream_inputs = self.check_and_add_runtime_roles(upstream_inputs, runtime_roles)
         return upstream_inputs
 
-    @staticmethod
-    def check_and_add_runtime_roles(upstream_inputs, runtime_roles):
-        correct_inputs = copy.deepcopy(upstream_inputs)
-        for input_type in InputArtifactType.types():
-            if input_type not in upstream_inputs:
+    def _init_outputs(self, name, dag: DAGSpec):
+        task_spec = dag.tasks[name]
+
+        if not task_spec.outputs:
+            return
+
+        parties = task_spec.parties if task_spec.parties else dag.parties
+
+        for output_type, outputs_dict in iter(task_spec.outputs):
+            if not outputs_dict:
                 continue
-            for input_key, channel_list in upstream_inputs[input_type].items():
-                if isinstance(channel_list, list):
-                    for idx, channel in enumerate(channel_list):
-                        if channel.roles is None:
-                            correct_inputs[input_type][input_key][idx].roles = runtime_roles
-                else:
-                    if channel_list.roles is None:
-                        correct_inputs[input_type][input_key].roles = runtime_roles
 
-        return correct_inputs
+            for outputs_key, output_artifact in outputs_dict.items():
+                output_parties = output_artifact.parties if output_artifact.parties else parties
+                for party_spec in output_parties:
+                    for party_id in party_spec.party_id:
+                        if not self.task_can_run(party_spec.role, party_id, runtime_parties=parties):
+                            continue
+
+                        if outputs_key not in self._tasks[party_spec.role][party_id][name].outputs:
+                            self._tasks[party_spec.role][party_id][name].outputs[output_type] = dict()
+
+                        self._tasks[party_spec.role][party_id][name].outputs[output_type][outputs_key] = output_artifact
+
+        for party_spec in parties:
+            for party_id in party_spec.party_id:
+                self._tasks[party_spec.role][party_id][name].outputs = self.check_and_add_runtime_party(
+                    self._tasks[party_spec.role][party_id][name].outputs,
+                    party_spec.role,
+                    party_id,
+                    artifact_type="output"
+                )
 
-    def _add_edge(self, src, dst, attrs=None):
+    def _add_edge(self, src, dst, role, party_id, attrs=None):
         if not attrs:
             attrs = {}
 
-        self._dag.add_edge(src, dst, **attrs)
+        self._dag[role][party_id].add_edge(src, dst, **attrs)
+        self._global_dag.add_edge(src, dst, **attrs)
 
     def _init_task_runtime_parameters_and_conf(self, task_name: str, dag_schema: DAGSchema, global_task_conf):
         dag = dag_schema.dag
-        role_keys = set([party.role for party in dag.parties])
         task_spec = dag.tasks[task_name]
-        if task_spec.parties:
-            task_role_keys = set([party.role for party in task_spec.parties])
-            role_keys = role_keys & task_role_keys
 
         common_parameters = dict()
         if task_spec.parameters:
             common_parameters = task_spec.parameters
 
-        task_parameters = dict()
-        task_conf = dict()
-        task_runtime_parties = []
+        parties = dag.parties if not task_spec.parties else task_spec.parties
 
-        for party in dag.parties:
-            if party.role not in role_keys:
-                continue
-            task_parameters[party.role] = dict()
-            task_conf[party.role] = dict()
+        for party in parties:
             for party_id in party.party_id:
-                task_parameters[party.role][party_id] = copy.deepcopy(common_parameters)
-                task_conf[party.role][party_id] = copy.deepcopy(global_task_conf)
-                task_runtime_parties.append(Party(role=party.role, party_id=party_id))
+                self._tasks[party.role][party_id][task_name].runtime_parameters = copy.deepcopy(common_parameters)
+                self._tasks[party.role][party_id][task_name].conf = copy.deepcopy(global_task_conf)
 
         if dag.party_tasks:
             party_tasks = dag.party_tasks
             for site_name, party_tasks_spec in party_tasks.items():
                 if party_tasks_spec.conf:
                     for party in party_tasks_spec.parties:
-                        if party.role in task_parameters:
-                            for party_id in party.party_id:
-                                task_conf[party.role][party_id].update(party_tasks_spec.conf)
+                        for party_id in party.party_id:
+                            self._tasks[party.role][party_id][task_name].conf.update(party_tasks_spec.conf)
 
                 if not party_tasks_spec.tasks or task_name not in party_tasks_spec.tasks:
                     continue
 
                 party_parties = party_tasks_spec.parties
                 party_task_spec = party_tasks_spec.tasks[task_name]
+
                 if party_task_spec.conf:
                     for party in party_parties:
-                        if party.role in task_parameters:
-                            for party_id in party.party_id:
-                                task_conf[party.role][party_id].update(party_task_spec.conf)
+                        for party_id in party.party_id:
+                            self._tasks[party.role][party_id][task_name].conf.update(party_task_spec.conf)
 
                 parameters = party_task_spec.parameters
 
                 if parameters:
                     for party in party_parties:
-                        if party.role in task_parameters:
-                            for party_id in party.party_id:
-                                task_parameters[party.role][party_id].update(parameters)
-
-        self._tasks[task_name].runtime_parameters = task_parameters
-        self._tasks[task_name].runtime_parties = task_runtime_parties
-        self._tasks[task_name].conf = task_conf
+                        for party_id in party.party_id:
+                            self._tasks[party.role][party_id][task_name].runtime_parameters.update(parameters)
 
-    def get_task_node(self, task_name):
-        return self._tasks[task_name]
+    def get_runtime_roles_on_party(self, task_name, party_id):
+        task_runtime_parties = self._task_runtime_parties[task_name]
 
-    def topological_sort(self):
-        return nx.topological_sort(self._dag)
+        runtime_roles = set()
+        for party_spec in task_runtime_parties:
+            if party_id in party_spec.party_id:
+                runtime_roles.add(party_spec.role)
+
+        return list(runtime_roles)
+
+    def get_task_node(self, role, party_id, task_name):
+        if role not in self._tasks:
+            raise ValueError(f"role={role} does ont exist in dag")
+        if party_id not in self._tasks[role]:
+            raise ValueError(f"role={role}, party_id={party_id} does not exist in dag")
+        if task_name not in self._tasks[role][party_id]:
+            raise ValueError(f"role={role}, party_id={party_id} does not has task {task_name}")
+
+        return self._tasks[role][party_id][task_name]
+
+    def get_need_revisit_tasks(self, visited_tasks, failed_tasks, role, party_id):
+        """
+        visited_tasks: already visited tasks
+        failed_tasks: failed tasks
+
+        this function finds tasks need to rerun, a task need to rerun if is upstreams is failed
+        """
+        invalid_tasks = set(self.party_topological_sort(role, party_id)) - set(visited_tasks)
+        invalid_tasks |= set(failed_tasks)
+
+        revisit_tasks = []
+        for task_to_check in visited_tasks:
+            if task_to_check in invalid_tasks:
+                revisit_tasks.append(task_to_check)
+                continue
+
+            task_valid = True
+            task_stack = {task_to_check}
+            stack = [task_to_check]
+
+            while len(stack) > 0 and task_valid:
+                task = stack.pop()
+                pre_tasks = self.party_predecessors(role, party_id, task)
+
+                for pre_task in pre_tasks:
+                    if pre_task in task_stack:
+                        continue
+                    if pre_task in invalid_tasks:
+                        task_valid = False
+                        break
+
+                    task_stack.add(pre_task)
+                    stack.append(pre_task)
+
+            if not task_valid:
+                revisit_tasks.append(task_to_check)
+
+        return revisit_tasks
+
+    def topological_sort(self, role, party_id):
+        return nx.topological_sort(self._dag[role][party_id])
+
+    def global_topological_sort(self):
+        return nx.topological_sort(self._global_dag)
+
+    def get_component_ref(self, task_name):
+        return self._global_dag.nodes[task_name]["component_ref"]
+
+    def party_topological_sort(self, role, party_id):
+        assert role in self._dag or party_id in self._dag[role], f"role={role}, party_id={party_id} does not exist"
+        return nx.topological_sort(self._dag[role][party_id])
+
+    def party_predecessors(self, role, party_id, task):
+        return set(self._dag[role][party_id].predecessors(task))
+
+    def party_successors(self, role, party_id, task):
+        return self._dag[role][party_id].successors(task)
+
+    def get_edge_attr(self, role, party_id, src, dst):
+        return self._dag[role][party_id].edges[src, dst]
+
+    @classmethod
+    def task_can_run(cls, role, party_id, component_spec: ComponentSpec=None, runtime_parties: List[PartySpec]=None):
+        if component_spec and role not in component_spec.roles:
+            return False
+
+        for party_spec in runtime_parties:
+            if role == party_spec.role and party_id in party_spec.party_id:
+                return True
+
+        return False
+
+    @staticmethod
+    def check_and_add_runtime_party(artifacts, role, party_id, artifact_type):
+        correct_artifacts = copy.deepcopy(artifacts)
+        if artifact_type == "input":
+            types = InputArtifactType.types()
+        else:
+            types = OutputArtifactType.types()
+
+        for t in types:
+            if t not in artifacts:
+                continue
+            for _key, channel_list in artifacts[t].items():
+                if isinstance(channel_list, list):
+                    for idx, channel in enumerate(channel_list):
+                        correct_artifacts[t][_key][idx].parties = [PartySpec(role=role, party_id=[party_id])]
+                else:
+                    correct_artifacts[t][_key].parties = [PartySpec(role=role, party_id=[party_id])]
+
+        return correct_artifacts
+
+    @property
+    def conf(self):
+        return self._conf
+
+    @property
+    def task_runtime_parties(self):
+        return self._task_runtime_parties
+
+    def get_task_runtime_parties(self, task_name):
+        return self._task_runtime_parties[task_name]
 
     @classmethod
     def infer_dependent_tasks(cls, input_artifacts):
-        print(input_artifacts)
         if not input_artifacts:
             return []
 
         dependent_task_list = list()
         for input_type in InputArtifactType.types():
             artifacts = getattr(input_artifacts, input_type)
             if not artifacts:
@@ -562,55 +762,79 @@
                     if not isinstance(channels, list):
                         channels = [channels]
                     for channel in channels:
                         dependent_task_list.append(channel.producer_task)
 
         return dependent_task_list
 
+    @classmethod
+    def translate_dag(cls, src, dst, adapter_map, *args, **kwargs):
+        translate_func = adapter_map[src][dst]
+        return translate_func(*args, **kwargs)
+
+
+class JobParser(object):
+    def __init__(self, dag_conf):
+        self.dag_parser = DagParser()
+        self.dag_parser.parse_dag(dag_conf)
+
+    def get_task_node(self, role, party_id, task_name):
+        return self.dag_parser.get_task_node(role, party_id, task_name)
+
+    def topological_sort(self):
+        return self.dag_parser.global_topological_sort()
+
+    def global_topological_sort(self):
+        return self.dag_parser.global_topological_sort()
+
+    def party_topological_sort(self, role, party_id):
+        return self.dag_parser.party_topological_sort(role, party_id)
+
+    def infer_dependent_tasks(self, input_artifacts):
+        return self.dag_parser.infer_dependent_tasks(input_artifacts)
+
     @property
     def task_parser(self):
         return TaskParser
 
     def component_ref_list(self, role, party_id):
         _list = []
-        for name in self.topological_sort():
-            node = self.get_task_node(name)
+        for name in self.party_topological_sort(role=role, party_id=party_id):
+            node = self.get_task_node(role=role, party_id=party_id, task_name=name)
             if node:
-                if self.task_parser(
-                        task_node=self.get_task_node(task_name=name),
-                        job_id="", task_name=name, role=role, party_id=party_id
-                ).need_run:
-                    _list.append(node.component_ref)
+                _list.append(node.component_ref)
         return _list
 
-    def dataset_list(self, role, party_id) -> List[DataSet]:
-        def append_dataset(datasets, channel):
-            if isinstance(channel, DataWarehouseChannelSpec):
-                if channel.name and channel.namespace:
-                    datasets.append(DataSet(**{
-                        "name": channel.name,
-                        "namespace": channel.namespace
-                    }))
-        _list = []
-        for task_name in self.topological_sort():
-            task_node = self.get_task_node(task_name)
-            input_artifacts = FlowRuntimeInputArtifacts(**task_node.upstream_inputs.get(role, {}).get(party_id, {}))
-            if input_artifacts.data:
-                for _k, _channels in input_artifacts.data.items():
-                    if isinstance(_channels, list):
-                        for _channel in _channels:
-                            append_dataset(_list, _channel)
-                    else:
-                        append_dataset(_list, _channels)
-        return _list
+    def dataset_list(self, role, party_id):
+        data_set = []
+        for task_name in self.party_topological_sort(role=role, party_id=party_id):
+            task_node = self.get_task_node(role=role, party_id=party_id, task_name=task_name)
+            parties = self.get_task_runtime_parties(task_name=task_name)
+            if task_node.component_ref.lower() == "reader" and job_utils.check_party_in(role, party_id, parties):
+                name = task_node.runtime_parameters.get("name")
+                namespace = task_node.runtime_parameters.get("namespace")
+                data_set.append(DataSet(**{"name": name, "namespace": namespace}))
+        return data_set
 
     def role_parameters(self, role, party_id):
         _dict = {}
-        for task_name in self.topological_sort():
-            task_node = self.get_task_node(task_name)
-            _dict[task_node.component_ref] = task_node.runtime_parameters.get(role, {}).get(party_id, {})
+        for task_name in self.party_topological_sort(role=role, party_id=party_id):
+            task_node = self.get_task_node(task_name=task_name, role=role, party_id=party_id)
+            _dict[task_node.component_ref] = task_node.runtime_parameters
         return _dict
 
+    def get_runtime_roles_on_party(self, task_name, party_id):
+        return self.dag_parser.get_runtime_roles_on_party(task_name, party_id)
+
+    def get_task_runtime_parties(self, task_name):
+        try:
+            return self.dag_parser.get_task_runtime_parties(task_name)
+        except:
+            return []
+
+    def get_component_ref(self, task_name):
+        return self.dag_parser.get_component_ref(task_name)
+
 
 class Party(BaseModel):
     role: str
     party_id: Union[str, int]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/provider/__init__.py` & `fate_flow-2.1.0/fate_flow/adapter/bfia/scheduler/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,12 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-import abc
-from typing import Dict
-
+#
+from .detector import BfiaDetector
+from .scheduler import BfiaScheduler
 
-class EntrypointABC:
-    @abc.abstractmethod
-    def component_list(self) -> Dict:
-        ...
+__all__ = [BfiaScheduler, BfiaDetector]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/provider/fate.py` & `fate_flow-2.1.0/fate_flow/hub/provider/local.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,7 +27,25 @@
             sys.path.append(self.provider.python_path)
         from fate.components.core import list_components
         # {'buildin': [], 'thirdparty': []}
         components = list_components()
         _list = components.get('buildin', [])
         _list.extend(components.get("thirdparty", []))
         return _list
+
+    @property
+    def component_description(self):
+        return {}
+
+
+class FATEFLowEntrypoint(EntrypointABC):
+    def __init__(self, provider):
+        self.provider = provider
+
+    @property
+    def component_list(self):
+        from fate_flow.components.components import BUILDIN_COMPONENTS
+        return [component.name for component in BUILDIN_COMPONENTS]
+
+    @property
+    def component_description(self):
+        return {}
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/scheduler/fate/__init__.py` & `fate_flow-2.1.0/fate_flow/utils/db_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,13 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from fate_flow.hub.scheduler.fate._scheduler import DAGScheduler
-
-__all__ = [
-    "DAGScheduler"
-]
+def get_dynamic_db_model(base, job_id):
+    return type(base.model(table_index=get_dynamic_tracking_table_index(job_id=job_id)))
 
 
+def get_dynamic_tracking_table_index(job_id):
+    return job_id[:8]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/hub/scheduler/fate/_scheduler.py` & `fate_flow-2.1.0/fate_flow/scheduler/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,183 +8,71 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-from copy import deepcopy
+import abc
+import os
 
 from pydantic import typing
 
-from fate_flow.controller.job_controller import JobInheritance
-from fate_flow.controller.task_controller import TaskController
+from fate_flow.controller.task import TaskController
 from fate_flow.entity.code import SchedulingStatusCode, FederatedSchedulingStatusCode
-from fate_flow.entity.spec.dag import DAGSchema, JobConfSpec
+from fate_flow.entity.spec.dag import DAGSchema
 from fate_flow.db.schedule_models import ScheduleJob, ScheduleTaskStatus
 from fate_flow.entity.types import StatusSet, JobStatus, TaskStatus, EndStatus, InterruptStatus, ResourceOperation, \
-    FederatedCommunicationType, AutoRerunStatus, ComputingEngine, EngineType
+    FederatedCommunicationType, AutoRerunStatus
 from fate_flow.entity.code import ReturnCode
-from fate_flow.errors.server_error import NoFoundJob, JobParamsError
-from fate_flow.hub.flow_hub import FlowHub
-from fate_flow.hub.scheduler import JobSchedulerABC
-from fate_flow.manager.model.model_meta import ModelMeta
-from fate_flow.operation.job_saver import ScheduleJobSaver
+from fate_flow.errors.server_error import NoFoundJob
+from fate_flow.controller.parser import JobParser
+from fate_flow.manager.operation.job_saver import ScheduleJobSaver, JobSaver
 from fate_flow.runtime.job_default_config import JobDefaultConfig
-from fate_flow.runtime.system_settings import ENGINES, COMPUTING_CONF, IGNORE_RESOURCE_ROLES, PARTY_ID, LOCAL_PARTY_ID
-from fate_flow.scheduler.federated_scheduler import FederatedScheduler
-from fate_flow.utils import job_utils, schedule_utils, wraps_utils
+from fate_flow.controller.federated import FederatedScheduler
+from fate_flow.utils import schedule_utils, wraps_utils, job_utils
 from fate_flow.utils.base_utils import json_dumps
+from fate_flow.utils.cron import Cron
 from fate_flow.utils.log_utils import schedule_logger, exception_to_trace_string
 
 
-class DAGScheduler(JobSchedulerABC):
-    @classmethod
-    def check_job_parameters(cls, dag_schema: DAGSchema, is_local: bool = False):
-        if not dag_schema.dag.conf:
-            dag_schema.dag.conf = JobConfSpec()
-        dag_schema.dag.conf.initiator_party_id = PARTY_ID
-        if not dag_schema.dag.conf.scheduler_party_id:
-            if not is_local:
-                dag_schema.dag.conf.scheduler_party_id = PARTY_ID
-            else:
-                dag_schema.dag.conf.scheduler_party_id = LOCAL_PARTY_ID
-        if not dag_schema.dag.conf.computing_partitions:
-            dag_schema.dag.conf.computing_partitions = JobDefaultConfig.computing_partitions
-
-        # check inheritance
-        JobInheritance.check(dag_schema.dag.conf.inheritance)
-
-        # check model warehouse
-        model_warehouse = dag_schema.dag.conf.model_warehouse
-        if model_warehouse:
-            if not ModelMeta.query(model_id=model_warehouse.model_id, model_version=model_warehouse.model_version):
-                raise JobParamsError(
-                    model_id=model_warehouse.model_id,
-                    model_version=model_warehouse.model_version,
-                    position="dag_schema.dag.conf.model_warehouse"
-                )
+class SchedulerABC(Cron):
+    @abc.abstractmethod
+    def run_do(self):
+        """
+        description：
+            Scheduling various status job, including: waiting、running、ready、rerun、end、etc.
+        """
 
     @classmethod
-    def submit(cls, dag_schema):
-        dag_schema = DAGSchema(**dag_schema)
-        job_id = job_utils.generate_job_id()
-        schedule_logger(job_id).info(
-            f"submit job, dag {dag_schema.dag.dict()}, schema version {dag_schema.schema_version}")
-        submit_result = {
-            "job_id": job_id,
-            "data": {}
-        }
-        try:
-            job = ScheduleJob()
-            job.f_job_id = job_id
-            job.f_parties = [party.dict() for party in dag_schema.dag.parties]
-            job.f_initiator_party_id = dag_schema.dag.conf.initiator_party_id
-            job.f_scheduler_party_id = dag_schema.dag.conf.scheduler_party_id
-            if dag_schema.dag.conf.priority:
-                job.f_priority = dag_schema.dag.conf.priority
-            cls.fill_default_job_parameters(job_id, dag_schema)
-            job.f_dag = dag_schema.dict()
-            submit_result["data"].update({
-                "model_id": dag_schema.dag.conf.model_id,
-                "model_version": dag_schema.dag.conf.model_version
-            })
-            job.f_status = StatusSet.READY
-            ScheduleJobSaver.create_job(job.to_human_model_dict())
-            status_code, response = FederatedScheduler.create_job(
-                job_id, job.f_parties, job.f_initiator_party_id, {"dag_schema": dag_schema.dict(), "job_id": job_id}
-            )
-            if status_code != FederatedSchedulingStatusCode.SUCCESS:
-                job.f_status = JobStatus.FAILED
-                FederatedScheduler.sync_job_status(job_id=job.f_job_id, roles=job.f_parties, job_info={
-                    "job_id": job.f_job_id,
-                    "status": job.f_status
-                })
-                raise Exception("create job failed", response)
-            else:
-                job.f_status = JobStatus.WAITING
-                TaskController.create_schedule_tasks(job, dag_schema)
-                status_code, response = FederatedScheduler.sync_job_status(job_id=job.f_job_id, roles=job.f_parties,
-                                                                           job_info={"job_id": job.f_job_id,
-                                                                                     "status": job.f_status})
-                if status_code != FederatedSchedulingStatusCode.SUCCESS:
-                    raise Exception(f"set job to waiting status failed: {response}")
-                ScheduleJobSaver.update_job_status({"job_id": job.f_job_id, "status": job.f_status})
-            schedule_logger(job_id).info(f"submit job successfully, job id is {job.f_job_id}")
-            result = {
-                "code": ReturnCode.Base.SUCCESS,
-                "message": "success"
-            }
-            submit_result.update(result)
-        except Exception as e:
-            schedule_logger(job_id).exception(e)
-            submit_result["code"] = ReturnCode.Job.CREATE_JOB_FAILED
-            submit_result["message"] = exception_to_trace_string(e)
-        return submit_result
+    def stop_job(cls, job_id: str, stop_status: str):
+        """
+        description：
+            Stop a job to all parties and set the job status to end status
+        :param job_id: job id
+        :param stop_status: In which state to stop the task.
 
-    @classmethod
-    def fill_default_job_parameters(cls, job_id: str, dag_schema: DAGSchema):
-        if not dag_schema.dag.conf.sync_type:
-            dag_schema.dag.conf.sync_type = JobDefaultConfig.sync_type
-        if not dag_schema.dag.conf.model_id or not dag_schema.dag.conf.model_id:
-            dag_schema.dag.conf.model_id, dag_schema.dag.conf.model_version = job_utils.generate_model_info(job_id)
-        if not dag_schema.dag.conf.auto_retries:
-            dag_schema.dag.conf.auto_retries = JobDefaultConfig.auto_retries
+        """
 
     @classmethod
-    def adapt_party_parameters(cls, dag_schema: DAGSchema, role):
-        cores, task_run, task_cores = cls.calculate_resource(dag_schema, role)
-        job_info = {"cores": cores, "remaining_cores": cores}
-        if dag_schema.dag.conf.inheritance:
-            job_info.update({"inheritance": dag_schema.dag.conf.inheritance.dict()})
-        return job_info, task_run, task_cores
+    def rerun_job(cls, job_id: str, auto: bool, tasks=None):
+        """
+        description：
+            rerun a job
+        :param job_id: job id
+        :param auto: Whether the scheduler automatically rerun
+        :param tasks: Specified rerun task list.
+
+        """
+
 
+class DAGScheduler(SchedulerABC):
     @classmethod
-    def calculate_resource(cls, dag_schema: DAGSchema, role):
-        cores = dag_schema.dag.conf.cores if dag_schema.dag.conf.cores else JobDefaultConfig.job_cores
-        if dag_schema.dag.conf.task and dag_schema.dag.conf.task.run:
-            task_run = dag_schema.dag.conf.task.run
-        else:
-            task_run = {}
-        task_cores = cores
-        default_task_run = deepcopy(JobDefaultConfig.task_run.get(ENGINES.get(EngineType.COMPUTING), {}))
-        if ENGINES.get(EngineType.COMPUTING) == ComputingEngine.SPARK:
-            if "num-executors" not in task_run:
-                task_run["num-executors"] = default_task_run.get("num-executors")
-            if "executor-cores" not in task_run:
-                task_run["executor-cores"] = default_task_run.get("executor-cores")
-            if role in IGNORE_RESOURCE_ROLES:
-                task_run["num-executors"] = 1
-                task_run["executor-cores"] = 1
-            task_cores = int(task_run.get("num-executors")) * (task_run.get("executor-cores"))
-            if task_cores > cores:
-                cores = task_cores
-        if ENGINES.get(EngineType.COMPUTING) == ComputingEngine.EGGROLL:
-            if "eggroll.session.processors.per.node" not in task_run:
-                task_run["eggroll.session.processors.per.node"] = \
-                    default_task_run.get("eggroll.session.processors.per.node")
-            task_cores = int(task_run.get("eggroll.session.processors.per.node")) * COMPUTING_CONF.get(
-                ComputingEngine.EGGROLL).get("nodes")
-            if task_cores > cores:
-                cores = task_cores
-            if role in IGNORE_RESOURCE_ROLES:
-                task_run["eggroll.session.processors.per.node"] = 1
-        if ENGINES.get(EngineType.COMPUTING) == ComputingEngine.STANDALONE:
-            if "cores" not in task_run:
-                task_run["cores"] = default_task_run.get("cores")
-            task_cores = int(task_run.get("cores"))
-            if task_cores > cores:
-                cores = task_cores
-            if role in IGNORE_RESOURCE_ROLES:
-                task_run["cores"] = 1
-        if role in IGNORE_RESOURCE_ROLES:
-            cores = 0
-            task_cores = 0
-        return cores, task_run, task_cores
+    def dag_parser(cls, dag):
+        return JobParser(dag)
 
     def run_do(self):
         # waiting
         schedule_logger().info("start schedule waiting jobs")
         # order by create_time and priority
         jobs = ScheduleJobSaver.query_job(
             status=JobStatus.WAITING,
@@ -211,35 +99,22 @@
             try:
                 self.schedule_running_job(job=job, lock=True)
             except Exception as e:
                 schedule_logger(job.f_job_id).exception(e)
                 schedule_logger(job.f_job_id).error("schedule job failed")
         schedule_logger().info("schedule running jobs finished")
 
-        # ready
-        schedule_logger().info("start schedule ready jobs")
-        jobs = ScheduleJobSaver.query_job(ready_signal=True, order_by="create_time", reverse=False)
-        schedule_logger().info(f"have {len(jobs)} ready jobs")
-        for job in jobs:
-            schedule_logger().info(f"schedule ready job {job.f_job_id}")
-            try:
-                pass
-            except Exception as e:
-                schedule_logger(job.f_job_id).exception(e)
-                schedule_logger(job.f_job_id).error(f"schedule ready job failed:\n{e}")
-        schedule_logger().info("schedule ready jobs finished")
-
         # rerun
         schedule_logger().info("start schedule rerun jobs")
         jobs = ScheduleJobSaver.query_job(rerun_signal=True, order_by="create_time", reverse=False)
         schedule_logger().info(f"have {len(jobs)} rerun jobs")
         for job in jobs:
             schedule_logger(job.f_job_id).info(f"schedule rerun job {job.f_job_id}")
             try:
-                self.schedule_rerun_job(job=job)
+                self.schedule_rerun_job(job=job, lock=True)
             except Exception as e:
                 schedule_logger(job.f_job_id).exception(e)
                 schedule_logger(job.f_job_id).error("schedule job failed")
         schedule_logger().info("schedule rerun jobs finished")
 
     @classmethod
     def apply_job_resource(cls, job):
@@ -254,19 +129,24 @@
             cls.rollback_job_resource(job, federated_response)
             return False
 
     @classmethod
     def rollback_job_resource(cls, job, federated_response):
         rollback_party = []
         failed_party = []
+        stop_status = False
         for dest_role in federated_response.keys():
             for dest_party_id in federated_response[dest_role].keys():
                 retcode = federated_response[dest_role][dest_party_id]["code"]
                 if retcode == ReturnCode.Base.SUCCESS:
                     rollback_party.append({"role": dest_role, "party_id": [dest_party_id]})
+                elif retcode == ReturnCode.Job.RESOURCE_LIMIT_EXCEEDED:
+                    # stop job
+                    schedule_logger(job.f_job_id).exception(f"{dest_role} {dest_party_id} resource limit exceeded")
+                    stop_status = True
                 else:
                     failed_party.append({"role": dest_role, "party_id": [dest_party_id]})
         schedule_logger(job.f_job_id).info("job apply resource failed on {}, rollback {}".format(failed_party,
                                                                                                  rollback_party))
         if rollback_party:
             return_status_code, federated_response = FederatedScheduler.resource_for_job(
                 job_id=job.f_job_id,
@@ -274,14 +154,18 @@
                 operation_type=ResourceOperation.RETURN.value
             )
             if return_status_code != FederatedSchedulingStatusCode.SUCCESS:
                 schedule_logger(job.f_job_id).info(f"job return resource failed:\n{federated_response}")
         else:
             schedule_logger(job.f_job_id).info("job no party should be rollback resource")
 
+        if stop_status:
+            cls.stop_job(job.f_job_id, stop_status=JobStatus.FAILED)
+            ScheduleJobSaver.update_job_status({"job_id": job.f_job_id, "status": JobStatus.FAILED})
+
     @classmethod
     @wraps_utils.schedule_lock
     def schedule_waiting_jobs(cls, job: ScheduleJob):
         if job.f_cancel_signal:
             FederatedScheduler.sync_job_status(job_id=job.f_job_id, roles=job.f_parties,
                                                job_info={"job_id": job.f_job_id, "status": JobStatus.CANCELED})
             ScheduleJobSaver.update_job_status({"job_id": job.f_job_id, "status": JobStatus.CANCELED})
@@ -438,15 +322,19 @@
         if not jobs:
             raise RuntimeError(f"can not found job {job_id}")
         job = jobs[0]
         if tasks:
             schedule_logger(job_id).info(f"require {[task.f_task_name for task in tasks]} to rerun")
         else:
             # todo: get_need_revisit_nodes
-            tasks = ScheduleJobSaver.query_task(job_id=job_id, status=TaskStatus.CANCELED, scheduler_status=True)
+            tasks = ScheduleJobSaver.query_task(
+                job_id=job_id,
+                status=[TaskStatus.CANCELED, TaskStatus.FAILED, TaskStatus.TIMEOUT],
+                scheduler_status=True
+            )
         job_can_rerun = any([TaskController.prepare_rerun_task(
             job=job, task=task, auto=auto, force=False,
         ) for task in tasks])
         schedule_logger(job_id).info("job set rerun signal")
         status = schedule_utils.rerun_signal(job_id=job_id, set_or_reset=True)
         schedule_logger(job_id).info(f"job set rerun signal {'successfully' if status else 'failed'}")
         return True
@@ -454,21 +342,92 @@
     @classmethod
     def finish(cls, job, end_status):
         schedule_logger(job.f_job_id).info(f"job finished with {end_status}, do something...")
         cls.stop_job(job_id=job.f_job_id, stop_status=end_status)
         # todo: clean job
         schedule_logger(job.f_job_id).info(f"job finished with {end_status}, done")
 
+    @classmethod
+    def create_all_job(cls, dag, job_id=None):
+        dag_schema = DAGSchema(**dag)
+        if not job_id:
+            job_id = job_utils.generate_job_id()
+        schedule_logger(job_id).info(
+            f"submit job, dag {dag_schema.dag.dict()}, schema version {dag_schema.schema_version}")
+        submit_result = {
+            "job_id": job_id,
+            "data": {}
+        }
+        try:
+            job = ScheduleJob()
+            job.f_job_id = job_id
+            job.f_parties = [party.dict() for party in dag_schema.dag.parties]
+            job.f_initiator_party_id = dag_schema.dag.conf.initiator_party_id
+            job.f_scheduler_party_id = dag_schema.dag.conf.scheduler_party_id
+            if dag_schema.dag.conf.priority:
+                job.f_priority = dag_schema.dag.conf.priority
+            cls.fill_default_job_parameters(job_id, dag_schema)
+            job.f_dag = dag_schema.dict()
+            submit_result["data"].update({
+                "model_id": dag_schema.dag.conf.model_id,
+                "model_version": dag_schema.dag.conf.model_version
+            })
+            job.f_status = StatusSet.READY
+            ScheduleJobSaver.create_job(job.to_human_model_dict())
+            body = dag_schema.dict()
+            body.update({
+                "job_id": job_id
+            })
+            status_code, response = FederatedScheduler.create_job(
+                job_id, job.f_parties, job.f_initiator_party_id, body
+            )
+            if status_code != FederatedSchedulingStatusCode.SUCCESS:
+                job.f_status = JobStatus.FAILED
+                FederatedScheduler.sync_job_status(job_id=job.f_job_id, roles=job.f_parties, job_info={
+                    "job_id": job.f_job_id,
+                    "status": job.f_status
+                })
+                raise Exception("create job failed", response)
+            else:
+                job.f_status = JobStatus.WAITING
+                TaskController.create_schedule_tasks(job, dag_schema)
+                status_code, response = FederatedScheduler.sync_job_status(job_id=job.f_job_id, roles=job.f_parties,
+                                                                           job_info={"job_id": job.f_job_id,
+                                                                                     "status": job.f_status})
+                if status_code != FederatedSchedulingStatusCode.SUCCESS:
+                    raise Exception(f"set job to waiting status failed: {response}")
+                ScheduleJobSaver.update_job_status({"job_id": job.f_job_id, "status": job.f_status})
+            schedule_logger(job_id).info(f"submit job successfully, job id is {job.f_job_id}")
+            result = {
+                "code": ReturnCode.Base.SUCCESS,
+                "message": "success"
+            }
+            submit_result.update(result)
+        except Exception as e:
+            schedule_logger(job_id).exception(e)
+            submit_result["code"] = ReturnCode.Job.CREATE_JOB_FAILED
+            submit_result["message"] = exception_to_trace_string(e)
+        return submit_result
+
+    @classmethod
+    def fill_default_job_parameters(cls, job_id: str, dag_schema: DAGSchema):
+        if not dag_schema.dag.conf.sync_type:
+            dag_schema.dag.conf.sync_type = JobDefaultConfig.sync_type
+        if not dag_schema.dag.conf.model_id or not dag_schema.dag.conf.model_id:
+            dag_schema.dag.conf.model_id, dag_schema.dag.conf.model_version = job_utils.generate_model_info(job_id)
+        if not dag_schema.dag.conf.auto_retries:
+            dag_schema.dag.conf.auto_retries = JobDefaultConfig.auto_retries
+
 
 class TaskScheduler(object):
     @classmethod
     def schedule(cls, job):
         schedule_logger(job.f_job_id).info("scheduling job tasks")
         dag_schema = DAGSchema(**job.f_dag)
-        job_parser = FlowHub.load_job_parser(DAGSchema(**job.f_dag))
+        job_parser = JobParser(DAGSchema(**job.f_dag))
         tasks_group = ScheduleJobSaver.get_status_tasks_asc(job_id=job.f_job_id)
         waiting_tasks = {}
         auto_rerun_tasks = []
         job_interrupt = False
         canceled = job.f_cancel_signal
         for task in tasks_group.values():
             if task.f_sync_type == FederatedCommunicationType.POLL:
@@ -609,14 +568,17 @@
                         "party_status": set_status
                     }
                     ScheduleJobSaver.update_task_status(task_info=tmp_task_info)
 
     @classmethod
     def get_federated_task_status(cls, job_id, task_id, task_version):
         tasks_on_all_party = ScheduleJobSaver.query_task(task_id=task_id, task_version=task_version)
+        if not tasks_on_all_party:
+            schedule_logger(job_id).error(f"task {task_id} {task_version} no found")
+            return TaskStatus.FAILED
         tasks_party_status = [task.f_status for task in tasks_on_all_party]
         status = cls.calculate_multi_party_task_status(tasks_party_status)
         schedule_logger(job_id=job_id).info(
             "task {} {} status is {}, calculate by task party status list: {}".format(task_id, task_version, status,
                                                                                       tasks_party_status))
         return status
 
@@ -634,7 +596,9 @@
                 if status in tmp_status_set:
                     return status
             if TaskStatus.RUNNING in tmp_status_set:
                 return TaskStatus.RUNNING
             if TaskStatus.SUCCESS in tmp_status_set:
                 return TaskStatus.RUNNING
             raise Exception("Calculate task status failed: {}".format(tasks_party_status))
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/__init__.py` & `fate_flow-2.1.0/fate_flow/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/components/__init__.py` & `fate_flow-2.1.0/fate_flow/entity/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/components/base.py` & `fate_flow-2.1.0/fate_flow/manager/components/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,19 @@
         party = PartySpec(role=role, party_id=[party_id])
         dag = DAGSchema(
             schema_version=provider.version,
             dag=DAGSpec(
                 conf=JobConfSpec(task=TaskConfSpec(provider=provider.provider_name)),
                 parties=[party],
                 stage="default",
-                tasks={task_name: TaskSpec(component_ref=component_ref, parties=[party])},
+                tasks={task_name: TaskSpec(
+                    component_ref=component_ref,
+                    parties=[party],
+                    conf=dict(provider=provider.provider_name)
+                )},
                 party_tasks={
                     f"{role}_{party_id}": PartyTaskSpec(
                         parties=[party],
                         tasks={task_name: PartyTaskRefSpec(parameters=parameters)}
                     )}
             ))
         if inputs:
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/container/__init__.py` & `fate_flow-2.1.0/fate_flow/manager/container/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/container/k8s_manager.py` & `fate_flow-2.1.0/fate_flow/manager/container/k8s_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         job_conf = copy.deepcopy(self.job_conf_template)
         metadata = job_conf['metadata']
         metadata['name'] = self.convertname(name + "job-conf")
         metadata['namespace'] = self.namespace
         job_conf['data']['service_conf.yaml'] = service_conf
         return job_conf
 
-    def start(self, name, command, environment):
+    def start(self, name, command, environment, **kwargs):
         # LOGGER.debug(f"command: {type(command)}, {command}")
         job = self.populate_yaml_template(self.convertname(name), command, environment)
         service_conf=yaml.safe_dump(get_base_config(key=None), default_flow_style=False)
         job_conf = self.populate_conf_yaml_template(self.convertname(name), service_conf)
         LOGGER.debug(f"job: {job}")
         LOGGER.debug(f"job_conf: {job}")
         client.CoreV1Api().create_namespaced_config_map(self.namespace, job_conf)
@@ -79,11 +79,14 @@
 
     def is_running(self, name):
         res = client.BatchV1Api().read_namespaced_job_status(self.convertname(name), self.namespace)
         # LOGGER.debug(f"res: {res}")
         if not res:
             return False
         return not (res.status.succeeded or res.status.failed)
+
+    def exit_with_exception(self, name):
+        return False
     
     # convertname: Ensure that name composes the RFC 1123 specification
     def convertname(self, name):
         return name.lower().replace('_','-')
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/data/__init__.py` & `fate_flow-2.1.0/fate_flow/manager/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/data/data_manager.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,31 +10,42 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import json
 import os
-import pickle
 import tarfile
 import uuid
 from tempfile import TemporaryDirectory
+from typing import List
 
 from flask import send_file
 
+from fate_flow.db import TrackingOutputInfo
+from fate_flow.db.base_models import BaseModelOperate
 from fate_flow.engine import storage
 from fate_flow.engine.storage import Session, StorageEngine, DataType
 from fate_flow.entity.types import EggRollAddress, StandaloneAddress, HDFSAddress, PathAddress, ApiAddress
 from fate_flow.errors.server_error import NoFoundTable
-from fate_flow.manager.service.output_manager import OutputDataTracking
 from fate_flow.runtime.system_settings import LOCALFS_DATA_HOME, STANDALONE_DATA_HOME, STORAGE
 from fate_flow.utils import job_utils
 from fate_flow.utils.io_utils import URI
+from fate_flow.utils.wraps_utils import filter_parameters
 
-DELIMITER = '\t'
+
+class OutputDataTracking(BaseModelOperate):
+    @classmethod
+    def create(cls, entity_info):
+        cls._create_entity(TrackingOutputInfo, entity_info)
+
+    @classmethod
+    @filter_parameters()
+    def query(cls, reverse=False, **kwargs) -> List[TrackingOutputInfo]:
+        return cls._query(TrackingOutputInfo, reverse=reverse, order_by="index", **kwargs)
 
 
 class DataManager:
     @classmethod
     def send_table(
             cls,
             output_tables_meta,
@@ -98,15 +109,15 @@
                         write_header = True
                     delimiter = table.meta.get_id_delimiter()
                     if isinstance(v, str):
                         fw.write('{}\n'.format(v))
                     elif isinstance(v, list):
                         fw.write('{}\n'.format(delimiter.join([str(_v) for _v in v])))
                     else:
-                        raise ValueError(type(v))
+                        raise ValueError(f"type={type(v)}, v={v}")
 
     @staticmethod
     def collect_data(table):
         if table.data_type == DataType.DATAFRAME:
             for _, data in table.collect():
                 for v in data:
                     yield v
@@ -119,15 +130,19 @@
     @staticmethod
     def display_data(table_metas):
         datas = {}
         for key, metas in table_metas.items():
             datas[key] = []
             for meta in metas:
                 if meta.data_type in [DataType.DATAFRAME, DataType.TABLE]:
-                    datas[key].append({"data": meta.get_part_of_data(), "metadata": meta.get_data_meta()})
+                    datas[key].append({
+                        "data": meta.get_part_of_data(),
+                        "metadata": meta.get_data_meta(),
+                        "total": meta.get_count()}
+                    )
                 else:
                     continue
         return datas
 
     @classmethod
     def query_output_data_table(cls, **kwargs):
         data_list = OutputDataTracking.query(**kwargs)
@@ -158,18 +173,20 @@
     @classmethod
     def display_output_data(cls, **kwargs):
         outputs = {}
         for key, tables in cls.query_output_data_table(**kwargs).items():
             if key not in outputs:
                 outputs[key] = []
             for table in tables:
-                outputs[key].append(storage.StorageTableMeta(
+                meta = storage.StorageTableMeta(
                     name=table.get("name"),
                     namespace=table.get("namespace")
-                ))
+                )
+                if meta:
+                    outputs[key].append(meta)
         return cls.display_data(outputs)
 
     @staticmethod
     def delete_data(namespace, name):
         with Session() as sess:
             table = sess.get_table(name=name, namespace=namespace)
             if table:
@@ -181,15 +198,18 @@
     def create_data_table(
             namespace, name, uri, partitions, data_meta, data_type, part_of_data=None, count=None, source=None
     ):
         engine, address = DataManager.uri_to_address(uri)
         storage_meta = storage.StorageTableBase(
             namespace=namespace, name=name, address=address,
             partitions=partitions, engine=engine,
-            options=None
+            options=None,
+            key_serdes_type=0,
+            value_serdes_type=0,
+            partitioner_type=0,
         )
         storage_meta.create_meta(
             data_meta=data_meta, part_of_data=part_of_data, count=count, source=source, data_type=data_type
         )
 
     @staticmethod
     def uri_to_address(uri):
@@ -235,23 +255,14 @@
             if isinstance(header, str):
                 header = header.split(delimiter)
         else:
             for field in data_meta.get("schema_meta", {}).get("fields", []):
                 header.append(field.get("name"))
         return header
 
-    @staticmethod
-    def deserialize_data(m):
-        fields = m.partition(DELIMITER)
-        return fields[0], pickle.loads(bytes.fromhex(fields[2]))
-
-    @staticmethod
-    def serialize_data(k, v):
-        return f"{k}{DELIMITER}{pickle.dumps(v).hex()}"
-
 
 class DatasetManager:
     @staticmethod
     def task_output_name(task_id, task_version):
         return f"output_data_{task_id}_{task_version}", uuid.uuid1().hex
 
     @staticmethod
@@ -280,16 +291,16 @@
 
         if is_multi:
             # replace "{index}"
             uri += "_{index}"
         return uri
 
     @classmethod
-    def output_local_uri(cls, name, type_name, task_info, is_multi=False):
-        path = job_utils.get_task_directory(**task_info, output=True)
+    def output_local_uri(cls, name, type_name, task_info, is_multi=False, base_dir=""):
+        path = job_utils.get_task_directory(**task_info, output=True, base_dir=base_dir)
         uri = os.path.join(f"file://{path}", name, type_name)
         if is_multi:
             # replace "{index}"
             uri += "_{index}"
         return uri
 
     @classmethod
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/log/__init__.py` & `fate_flow-2.1.0/fate_flow/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/log/log_manager.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 from fate_flow.runtime.system_settings import LOG_DIR
 from fate_flow.utils.log_utils import replace_ip
 
 JOB = ["schedule_info", "schedule_error"]
 TASK = ["task_error", "task_info", "task_warning", "task_debug"]
 
 
-def parameters_check(log_type, job_id, role, party_id, task_name):
+def parameters_check(log_type, job_id, role, party_id):
     if log_type in JOB:
         if not job_id:
             return False
     if log_type in TASK:
-        if not job_id or not role or not party_id or not task_name:
+        if not job_id or not role or not party_id:
             return False
     return True
 
 
 class LogManager:
     def __init__(self, log_type, job_id, party_id="", role="", task_name="", **kwargs):
         self.log_type = log_type
         self.job_id = job_id
         self.party_id = party_id
         self.role = role
         self.task_name = task_name
 
     @property
     def task_base_path(self):
-        if self.role and self.party_id and self.task_name:
-            return os.path.join(self.job_id, self.role, self.party_id, self.task_name, "root")
-        else:
-            return ""
+        if self.role and self.party_id:
+            path = os.path.join(self.job_id, self.role, self.party_id)
+            if self.task_name:
+                path = os.path.join(path, self.task_name, 'root')
+            return path
+        return ""
 
     @property
     def file_path(self):
-        status = parameters_check(self.log_type, self.job_id, self.role, self.party_id, self.task_name)
+        status = parameters_check(self.log_type, self.job_id, self.role, self.party_id)
         if not status:
             raise Exception(f"job type {self.log_type} Missing parameters")
         type_dict = {
             "schedule_info": os.path.join(self.job_id, "fate_flow_schedule.log"),
             "schedule_error": os.path.join(self.job_id, "fate_flow_schedule_error.log"),
             "task_error": os.path.join(self.task_base_path, "ERROR"),
             "task_warning": os.path.join(self.task_base_path, "WARNING"),
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/metric/__init__.py` & `fate_flow-2.1.0/fate_flow/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/metric/metric_manager.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/metric.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/__init__.py` & `fate_flow-2.1.0/fate_flow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/engine/__init__.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/engine/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from fate_flow.manager.model.engine._tencent_cos import TencentCosStorage
-from fate_flow.manager.model.engine._mysql import MysqlModelStorage
+from fate_flow.manager.outputs.model.engine._mysql import MysqlModelStorage
+from fate_flow.manager.outputs.model.engine._tencent_cos import TencentCosStorage
 
 __all__ = ["MysqlModelStorage", "TencentCosStorage"]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/engine/_mysql.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/engine/_mysql.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/engine/_tencent_cos.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/engine/_tencent_cos.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/handel/__init__.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,13 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from fate_flow.manager.model.handel._base import IOHandle
-from fate_flow.manager.model.handel._file import FileHandle
-from fate_flow.manager.model.handel._mysql import MysqlHandel
-from fate_flow.manager.model.handel._tencent_cos import TencentCosHandel
-
+from fate_flow.manager.outputs.model.handel._base import IOHandle
+from fate_flow.manager.outputs.model.handel._file import FileHandle
+from fate_flow.manager.outputs.model.handel._mysql import MysqlHandel
+from fate_flow.manager.outputs.model.handel._tencent_cos import TencentCosHandel
 
 __all__ = ["IOHandle", "FileHandle", "MysqlHandel", "TencentCosHandel"]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/handel/_base.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-import collections
 import json
 import os.path
 import tarfile
 from typing import Union, List
 
 from ruamel import yaml
 from werkzeug.datastructures import FileStorage
 
 from fate_flow.entity.spec.flow import Metadata
 from fate_flow.errors.server_error import NoFoundModelOutput
-from fate_flow.manager.model.model_meta import ModelMeta
-from fate_flow.operation.job_saver import JobSaver
+from fate_flow.manager.outputs.model.model_meta import ModelMeta
+from fate_flow.manager.operation.job_saver import JobSaver
 
 
 class IOHandle(object):
     @property
     def name(self):
         return self._name
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/handel/_file.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import tarfile
 
 from flask import send_file
 from werkzeug.datastructures import FileStorage
 
 from fate_flow.entity.spec.flow import FileStorageSpec
 from fate_flow.entity.types import ModelStorageEngine
-from fate_flow.manager.model.handel import IOHandle
+from fate_flow.manager.outputs.model.handel import IOHandle
 from fate_flow.runtime.system_settings import MODEL_STORE_PATH
 
 
 class FileHandle(IOHandle):
     def __init__(self, engine_address: FileStorageSpec):
         self.path = engine_address.path if engine_address.path else MODEL_STORE_PATH
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/handel/_mysql.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import io
-import os
 import tarfile
 
 from flask import send_file
 from werkzeug.datastructures import FileStorage
 
 from fate_flow.entity.spec.flow import MysqlStorageSpec
 from fate_flow.entity.types import ModelStorageEngine
-from fate_flow.manager.model.engine import MysqlModelStorage
-from fate_flow.manager.model.handel import IOHandle
+from fate_flow.manager.outputs.model.engine import MysqlModelStorage
+from fate_flow.manager.outputs.model.handel import IOHandle
 
 
 class MysqlHandel(IOHandle):
     def __init__(self, engine_address: MysqlStorageSpec, decrypt_key=None):
         self.engine = MysqlModelStorage(engine_address.dict(), decrypt_key=decrypt_key)
 
     @property
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/handel/_tencent_cos.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/handel/_tencent_cos.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import tarfile
 
 from flask import send_file
 from werkzeug.datastructures import FileStorage
 
 from fate_flow.entity.spec.flow import TencentCosStorageSpec
 from fate_flow.entity.types import ModelStorageEngine
-from fate_flow.manager.model.engine import TencentCosStorage
-from fate_flow.manager.model.handel import IOHandle
+from fate_flow.manager.outputs.model.engine import TencentCosStorage
+from fate_flow.manager.outputs.model.handel import IOHandle
 
 
 class TencentCosHandel(IOHandle):
     def __init__(self, engine_address: TencentCosStorageSpec, decrypt_key: str = None):
         self.engine = TencentCosStorage(engine_address.dict(), decrypt_key)
 
     @property
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/model_manager.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import shutil
 from tempfile import TemporaryDirectory
 
 from werkzeug.datastructures import FileStorage
 
 from fate_flow.entity.spec.flow import FileStorageSpec, MysqlStorageSpec, TencentCosStorageSpec
 from fate_flow.entity.types import ModelStorageEngine
-from fate_flow.manager.model.handel import FileHandle, MysqlHandel, TencentCosHandel
-from fate_flow.manager.model.model_meta import ModelMeta
+from fate_flow.manager.outputs.model.handel import FileHandle, MysqlHandel, TencentCosHandel
+from fate_flow.manager.outputs.model.model_meta import ModelMeta
 from fate_flow.runtime.system_settings import MODEL_STORE
 from fate_flow.errors.server_error import NoFoundModelOutput
 
 
 class PipelinedModel(object):
     engine = MODEL_STORE.get("engine")
     decrypt_key = MODEL_STORE.get("decrypt_key")
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/model/model_meta.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/model_meta.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/service/output_manager.py` & `fate_flow-2.1.0/fate_flow/runtime/reload_config_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,23 +8,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import List
-
-from fate_flow.db.base_models import BaseModelOperate
-from fate_flow.db.db_models import TrackingOutputInfo
-from fate_flow.utils.wraps_utils import filter_parameters
-
-
-class OutputDataTracking(BaseModelOperate):
+#
+class ReloadConfigBase:
     @classmethod
-    def create(cls, entity_info):
-        cls._create_entity(TrackingOutputInfo, entity_info)
+    def get_all(cls):
+        configs = {}
+        for k, v in cls.__dict__.items():
+            if not callable(getattr(cls, k)) and not k.startswith("__") and not k.startswith("_"):
+                configs[k] = v
+        return configs
 
     @classmethod
-    @filter_parameters()
-    def query(cls, reverse=False, **kwargs) -> List[TrackingOutputInfo]:
-        return cls._query(TrackingOutputInfo, reverse=reverse, order_by="index", **kwargs)
+    def get(cls, config_name):
+        return getattr(cls, config_name) if hasattr(cls, config_name) else None
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/service/provider_manager.py` & `fate_flow-2.1.0/fate_flow/manager/service/provider_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 import os
 import sys
 from typing import Union
 
 from fate_flow.db import ProviderInfo, ComponentInfo
 from fate_flow.db.base_models import DB, BaseModelOperate
 from fate_flow.entity.spec.flow import ProviderSpec, LocalProviderSpec, DockerProviderSpec, K8sProviderSpec
-from fate_flow.entity.types import ProviderDevice
+from fate_flow.entity.types import ProviderDevice, PROTOCOL
 from fate_flow.hub.flow_hub import FlowHub
 from fate_flow.hub.provider import EntrypointABC
 from fate_flow.runtime.system_settings import DEFAULT_FATE_PROVIDER_PATH, DEFAULT_PROVIDER, FATE_FLOW_PROVIDER_PATH
 from fate_flow.runtime.component_provider import ComponentProvider
 from fate_flow.utils.log import getLogger
 from fate_flow.utils.version import get_versions, get_default_fate_version, get_flow_version
 from fate_flow.utils.wraps_utils import filter_parameters
 
 stat_logger = getLogger("fate_flow_stat")
 
+
 class ProviderManager(BaseModelOperate):
     @classmethod
     def get_provider_by_provider_name(cls, provider_name) -> ComponentProvider:
         name, version, device = cls.parser_provider_name(provider_name)
         provider_list = [provider_info for provider_info in cls.query_provider(name=name, version=version, device=device)]
         if not provider_list:
             raise ValueError(f"Query provider info failed: {provider_name}")
@@ -52,43 +53,64 @@
             metadata = K8sProviderSpec(check, **metadata)
         else:
             return None
         return ComponentProvider(ProviderSpec(name=name, device=device, version=version, metadata=metadata))
 
     @classmethod
     @DB.connection_context()
-    def register_provider(cls, provider: ComponentProvider):
+    def register_provider(cls, provider: ComponentProvider, components_description=None, protocol=PROTOCOL.FATE_FLOW):
+        if not components_description:
+            components_description = {}
         provider_info = ProviderInfo()
         provider_info.f_provider_name = provider.provider_name
         provider_info.f_name = provider.name
         provider_info.f_device = provider.device
         provider_info.f_version = provider.version
         provider_info.f_metadata = provider.metadata.dict()
         operator_type = cls.safe_save(ProviderInfo, defaults=provider_info.to_dict(),
                                       f_provider_name=provider.provider_name)
-        # todo: load entrypoint、components、params...
-        # load components
-        cls.register_component(provider)
+        cls.register_component(provider, components_description, protocol)
         return operator_type
 
     @classmethod
-    def register_component(cls, provider: ComponentProvider):
-        entrypoint = cls.load_entrypoint(provider)
+    def register_component(cls, provider: ComponentProvider, components_description, protocol):
+        if not protocol:
+            protocol = PROTOCOL.FATE_FLOW
+
+        if not components_description:
+            components_description = {}
+
         component_list = []
-        if entrypoint:
-            component_list = entrypoint.component_list
 
+        if components_description:
+            component_list = components_description.keys()
+        else:
+            entrypoint = cls.load_entrypoint(provider)
+            if entrypoint:
+                component_list = entrypoint.component_list
         for component_name in component_list:
             component = ComponentInfo()
             component.f_provider_name = provider.provider_name
             component.f_name = provider.name
             component.f_device = provider.device
             component.f_version = provider.version
             component.f_component_name = component_name
-            cls.safe_save(ComponentInfo, defaults=component.to_dict(), **component.to_dict())
+            component.f_protocol = protocol
+            component.f_component_description = components_description.get(component_name)
+            cls.safe_save(
+                ComponentInfo, defaults=component.to_dict(),
+                **dict(
+                    f_provider_name=provider.provider_name,
+                    f_name=provider.name,
+                    f_device=provider.device,
+                    f_version=provider.version,
+                    f_component_name=component_name,
+                    f_protocol=protocol
+                )
+            )
 
     @classmethod
     @filter_parameters()
     def query_provider(cls, **kwargs):
         return cls._query(ProviderInfo, **kwargs)
 
     @classmethod
@@ -116,14 +138,27 @@
 
     @classmethod
     def get_all_components(cls):
         component_list = cls._query(ComponentInfo, force=True)
         return list(set([component.f_component_name for component in component_list]))
 
     @classmethod
+    def get_flow_components(cls):
+        component_list = cls._query(ComponentInfo, name="fate_flow", force=True)
+        return list(set([component.f_component_name for component in component_list]))
+
+    @classmethod
+    @filter_parameters()
+    def query_component_description(cls, **kwargs):
+        descriptions = {}
+        for info in cls._query(ComponentInfo, **kwargs):
+            descriptions[info.f_component_name] = info.f_component_description
+        return descriptions
+
+    @classmethod
     def get_fate_flow_provider(cls):
         return cls.get_provider(
             name="fate_flow",
             version=get_flow_version(),
             device=ProviderDevice.LOCAL,
             metadata={
                 "path": FATE_FLOW_PROVIDER_PATH,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/service/resource_manager.py` & `fate_flow-2.1.0/fate_flow/manager/service/resource_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
+from fate_flow.entity.code import ReturnCode
 from pydantic import typing
 
 from fate_flow.db.base_models import DB
 from fate_flow.db.db_models import EngineRegistry, Job, Task
-from fate_flow.entity.types import EngineType, ResourceOperation
+from fate_flow.entity.types import EngineType, ResourceOperation, LauncherType
 from fate_flow.runtime.job_default_config import JobDefaultConfig
 from fate_flow.runtime.system_settings import IGNORE_RESOURCE_ROLES, ENGINES
 from fate_flow.utils import engine_utils, base_utils, job_utils
 from fate_flow.utils.log import getLogger
 from fate_flow.utils.log_utils import schedule_logger
 
 stat_logger = getLogger()
@@ -86,14 +87,17 @@
 
     @classmethod
     @DB.connection_context()
     def resource_for_job(cls, job_id, role, party_id, operation_type: ResourceOperation):
         operate_status = False
         cores, memory = cls.query_job_resource(job_id=job_id, role=role, party_id=party_id)
         engine_name = ENGINES.get(EngineType.COMPUTING)
+        total_cores = EngineRegistry.query(engine_name=engine_name)[0].f_cores
+        if cores > total_cores:
+            raise RuntimeError(ReturnCode.Job.RESOURCE_LIMIT_EXCEEDED, "Resource limit exceeded")
         try:
             with DB.atomic():
                 updates = {
                     Job.f_engine_name: engine_name,
                     Job.f_cores: cores,
                     Job.f_memory: memory,
                 }
@@ -222,17 +226,20 @@
 
     @classmethod
     def query_task_resource(cls, task_info: dict = None):
         cores_per_task = 0
         memory_per_task = 0
         if task_info["role"] in IGNORE_RESOURCE_ROLES:
             return cores_per_task, memory_per_task
-        task_cores, memory = job_utils.get_task_resource_info(
+        task_cores, memory, launcher_name = job_utils.get_task_resource_info(
             task_info["job_id"], task_info["role"], task_info["party_id"], task_info["task_id"], task_info["task_version"]
         )
+        if launcher_name == LauncherType.DEEPSPEED:
+            # todo: apply gpus
+            return 0, 0
         return task_cores, memory
 
     @classmethod
     def update_resource_sql(cls, resource_model: typing.Union[EngineRegistry, Job], cores, memory, operation_type: ResourceOperation):
         if operation_type is ResourceOperation.APPLY:
             filters = [
                 resource_model.f_remaining_cores >= cores,
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/service/service_manager.py` & `fate_flow-2.1.0/fate_flow/manager/service/service_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,38 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import abc
 import atexit
 import json
+import os
 import socket
 import time
 from functools import wraps
 from pathlib import Path
 from queue import Queue
 from threading import Thread
 from urllib import parse
 
+from fate_flow.utils.file_utils import get_fate_flow_directory
 from kazoo.client import KazooClient
 from kazoo.exceptions import NodeExistsError, NoNodeError, ZookeeperError
 from kazoo.security import make_digest_acl
 from shortuuid import ShortUUID
 
 from fate_flow.db import ServiceRegistryInfo, ServerRegistryInfo
 from fate_flow.db.base_models import DB
 from fate_flow.entity.types import FlowInstance
 from fate_flow.errors.zookeeper_error import ServiceNotSupported, ServicesError, ZooKeeperNotConfigured, \
     MissingZooKeeperUsernameOrPassword, ZooKeeperBackendError
 from fate_flow.runtime.reload_config_base import ReloadConfigBase
 from fate_flow.runtime.system_settings import RANDOM_INSTANCE_ID, HOST, HTTP_PORT, GRPC_PORT, ZOOKEEPER_REGISTRY, \
     ZOOKEEPER, USE_REGISTRY, NGINX_HOST, NGINX_HTTP_PORT, FATE_FLOW_MODEL_TRANSFER_ENDPOINT, SERVICE_CONF_NAME
+from fate_flow.settings import DEFAULT_SERVER_CONF_PATH
 from fate_flow.utils import conf_utils, file_utils
 from fate_flow.utils.log import getLogger
 from fate_flow.utils.version import get_flow_version
 
 stat_logger = getLogger("fate_flow_stat")
 
 model_download_endpoint = f'http://{NGINX_HOST}:{NGINX_HTTP_PORT}{FATE_FLOW_MODEL_TRANSFER_ENDPOINT}'
@@ -417,15 +420,16 @@
                 "port": server.f_port,
                 "protocol": server.f_protocol
             }
             setattr(cls, server.f_server_name.upper(), server_info)
 
     @classmethod
     def load_server_info_from_conf(cls):
-        path = Path(file_utils.get_fate_flow_directory()) / 'conf' / SERVICE_CONF_NAME
+        conf_path = DEFAULT_SERVER_CONF_PATH or os.path.join(get_fate_flow_directory(), "conf")
+        path = Path(conf_path) / SERVICE_CONF_NAME
         conf = file_utils.load_yaml_conf(path)
         if not isinstance(conf, dict):
             raise ValueError('invalid config file')
 
         local_path = path.with_name(f'local.{SERVICE_CONF_NAME}')
         if local_path.exists():
             local_conf = file_utils.load_yaml_conf(local_path)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/manager/service/worker_manager.py` & `fate_flow-2.1.0/fate_flow/manager/service/worker_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,54 +9,60 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
+import io
 import logging
 import os
 import subprocess
 import sys
 from uuid import uuid1
 
+from fate_flow.runtime.system_settings import ENGINES
 from ruamel import yaml
 
 from fate_flow.db.base_models import DB, auto_date_timestamp_db_field
 from fate_flow.db.db_models import Task, WorkerInfo
-from fate_flow.entity.types import WorkerName
+from fate_flow.entity.types import WorkerName, EngineType, ComputingEngine
 from fate_flow.runtime.runtime_config import RuntimeConfig
 from fate_flow.utils import job_utils, process_utils
 from fate_flow.utils.base_utils import current_timestamp, json_dumps
 from fate_flow.utils.log_utils import failed_log, schedule_logger, start_log, successful_log
 
 
 class WorkerManager:
     @classmethod
     def start_task_worker(cls, worker_name, task_info, task_parameters=None, executable=None, common_cmd=None,
-                          extra_env: dict = None, record=False, stderr=None, sync=False, **kwargs):
+                          extra_env: dict = None, record=False, stderr=None, sync=False, config_dir=None, std_dir=None,
+                          **kwargs):
         if not extra_env:
             extra_env = {}
         worker_id = uuid1().hex
-        config_dir, std_dir = cls.get_process_dirs(
-            job_id=task_info.get("job_id"),
-            role=task_info.get("role"),
-            party_id=task_info.get("party_id"),
-            task_name=task_info.get("task_name"),
-            task_version=task_info.get("task_version")
-        )
+        if not config_dir or not std_dir:
+            config_dir, std_dir = cls.get_process_dirs(
+                job_id=task_info.get("job_id"),
+                role=task_info.get("role"),
+                party_id=task_info.get("party_id"),
+                task_name=task_info.get("task_name"),
+                task_version=task_info.get("task_version")
+            )
         params_env = {}
         if task_parameters:
             params_env = cls.get_env(task_info.get("job_id"), task_parameters)
         extra_env.update(params_env)
         if executable:
             process_cmd = executable
         else:
             process_cmd = [os.getenv("EXECUTOR_ENV") or sys.executable or "python3"]
         process_cmd.extend(common_cmd)
+        if sync and cls.worker_outerr_with_pipe(worker_name):
+            stderr = subprocess.PIPE
         p = process_utils.run_subprocess(job_id=task_info.get("job_id"), config_dir=config_dir, process_cmd=process_cmd,
                                          added_env=extra_env, std_dir=std_dir, cwd_dir=config_dir,
                                          process_name=worker_name.value, stderr=stderr)
         if record:
             cls.save_worker_info(task_info=task_info, worker_name=worker_name, worker_id=worker_id,
                                  run_ip=RuntimeConfig.JOB_SERVER_HOST, run_pid=p.pid, config=task_parameters,
                                  cmd=process_cmd)
@@ -65,21 +71,35 @@
                 "run_ip": RuntimeConfig.JOB_SERVER_HOST,
                 "worker_id": worker_id,
                 "cmd": process_cmd,
                 "run_port": RuntimeConfig.HTTP_PORT
             }
         else:
             if sync:
+                error_io = io.BytesIO()
+                if cls.worker_outerr_with_pipe(worker_name):
+                    while True:
+                        output = p.stderr.readline()
+                        if output == b'' and p.poll() is not None:
+                            break
+                        if output:
+                            error_io.write(output)
+                error_io.seek(0)
                 _code = p.wait()
-                _e = p.stderr.read() if p.stderr else None
+                _e = error_io.read()
                 if _e and _code:
                     logging.error(f"process {worker_name.value} run error[code:{_code}]\n: {_e.decode()}")
             return p
 
     @classmethod
+    def worker_outerr_with_pipe(cls, worker_name):
+        return worker_name == WorkerName.TASK_EXECUTE and \
+               ENGINES.get(EngineType.COMPUTING) not in [ComputingEngine.SPARK]
+
+    @classmethod
     def get_process_dirs(cls, job_id, role, party_id, task_name, task_version):
         config_dir = job_utils.get_job_directory(job_id, role, party_id, task_name, str(task_version))
         std_dir = job_utils.get_job_log_directory(job_id, role, party_id, task_name, "stdout")
         os.makedirs(config_dir, exist_ok=True)
         return config_dir, std_dir
 
     @classmethod
```

### Comparing `fate_flow-2.0.0b0/fate_flow/operation/__init__.py` & `fate_flow-2.1.0/fate_flow/manager/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/operation/base_saver.py` & `fate_flow-2.1.0/fate_flow/manager/operation/base_saver.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     @classmethod
     def _update_job_status(cls, job_obj, job_info):
         schedule_logger(job_info["job_id"]).info("try to update job status to {}".format(job_info.get("status")))
         update_status = cls._update_status(job_obj, job_info)
         if update_status:
             schedule_logger(job_info["job_id"]).info("update job status successfully")
-            if EndStatus.contains(job_info.get("status")):
+            if cls.end_status_contains(job_info.get("status")):
                 new_job_info = {}
                 # only update tag
                 for k in ["job_id", "role", "party_id", "tag"]:
                     if k in job_info:
                         new_job_info[k] = job_info[k]
                 if not new_job_info.get("tag"):
                     new_job_info["tag"] = "job_end"
@@ -133,38 +133,51 @@
         update_info = {"job_id": entity_info["job_id"]}
 
         for status_field in cls.STATUS_FIELDS:
             if entity_info.get(status_field) and hasattr(entity_model, f"f_{status_field}"):
                 if status_field in ["status", "party_status"]:
                     # update end time
                     if hasattr(obj, "f_start_time") and obj.f_start_time:
-                        update_info["end_time"] = current_timestamp()
-                        update_info['elapsed'] = update_info['end_time'] - obj.f_start_time
+                        if cls.end_status_contains(entity_info.get(status_field)):
+                            update_info["end_time"] = current_timestamp()
+                            update_info['elapsed'] = update_info['end_time'] - obj.f_start_time
                     update_info[status_field] = entity_info[status_field]
                     old_status = getattr(obj, f"f_{status_field}")
                     new_status = update_info[status_field]
                     if_pass = False
                     if isinstance(obj, Task) or isinstance(obj, ScheduleTask) or isinstance(obj, ScheduleTaskStatus):
-                        if TaskStatus.StateTransitionRule.if_pass(src_status=old_status, dest_status=new_status):
+                        if cls.check_task_status(old_status, new_status):
                             if_pass = True
                     elif isinstance(obj, Job) or isinstance(obj, ScheduleJob):
-                        if JobStatus.StateTransitionRule.if_pass(src_status=old_status, dest_status=new_status):
+                        if cls.check_job_status(old_status, new_status):
                             if_pass = True
-                        if EndStatus.contains(new_status) and new_status not in {JobStatus.SUCCESS, JobStatus.CANCELED}:
+                        if cls.end_status_contains(new_status) and new_status not in {JobStatus.SUCCESS, JobStatus.CANCELED}:
                             if isinstance(obj, ScheduleJob):
                                 update_filters.append(ScheduleJob.f_rerun_signal==False)
                     if if_pass:
                         update_filters.append(operator.attrgetter(f"f_{status_field}")(type(obj)) == old_status)
                     else:
                         # not allow update status
                         update_info.pop(status_field)
 
         return cls.execute_update(old_obj=obj, model=entity_model, update_info=update_info, update_filters=update_filters)
 
     @classmethod
+    def check_task_status(cls, old_status, dest_status):
+        return TaskStatus.StateTransitionRule.if_pass(src_status=old_status, dest_status=dest_status)
+
+    @classmethod
+    def check_job_status(cls, old_status, dest_status):
+        return JobStatus.StateTransitionRule.if_pass(src_status=old_status, dest_status=dest_status)
+
+    @classmethod
+    def end_status_contains(cls, status):
+        return EndStatus.contains(status)
+
+    @classmethod
     @DB.connection_context()
     def update_entity_table(cls, entity_model, entity_info, filters: list = None):
         query_filters = []
         primary_keys = entity_model.get_primary_keys_name()
         if not filters:
             for p_k in primary_keys:
                 query_filters.append(operator.attrgetter(p_k)(entity_model) == entity_info[p_k.lstrip("f").lstrip("_")])
```

### Comparing `fate_flow-2.0.0b0/fate_flow/operation/job_saver.py` & `fate_flow-2.1.0/fate_flow/manager/operation/job_saver.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import time
 
 from fate_flow.db.base_models import DB
 from fate_flow.db.db_models import Job, Task
-from fate_flow.entity.code import ReturnCode
+from fate_flow.entity.types import PROTOCOL
 from fate_flow.errors.server_error import NoFoundTask
-from fate_flow.operation.base_saver import BaseSaver
+from fate_flow.manager.operation.base_saver import BaseSaver
 from fate_flow.db.schedule_models import ScheduleJob, ScheduleTask, ScheduleTaskStatus
 
 
 class JobSaver(BaseSaver):
     @classmethod
     def create_job(cls, job_info) -> Job:
         return cls._create_job(Job, job_info)
@@ -33,14 +32,18 @@
         return cls._create_task(Task, task_info)
 
     @classmethod
     def delete_job(cls, job_id):
         return cls._delete_job(Job, job_id)
 
     @classmethod
+    def delete_task(cls, job_id):
+        return cls._delete_job(Task, job_id)
+
+    @classmethod
     def update_job_status(cls, job_info):
         return cls._update_job_status(Job, job_info)
 
     @classmethod
     def query_job(cls, reverse=None, order_by=None, **kwargs):
         return cls._query_job(Job, reverse, order_by, **kwargs)
 
@@ -60,16 +63,23 @@
         return cls._list(Job, limit, offset, query, order_by)
 
     @classmethod
     def list_task(cls, limit, offset, query, order_by):
         return cls._list(Task, limit, offset, query, order_by)
 
     @classmethod
-    def query_task(cls, only_latest=True, reverse=None, order_by=None, **kwargs):
-        return cls._query_task(Task, only_latest=only_latest, reverse=reverse, order_by=order_by, **kwargs)
+    def query_task(
+            cls, only_latest=True, reverse=None, order_by=None, ignore_protocol=False, protocol=PROTOCOL.FATE_FLOW,
+            **kwargs
+    ):
+        if not ignore_protocol:
+            kwargs["protocol"] = protocol
+        return cls._query_task(
+            Task, only_latest=only_latest, reverse=reverse, order_by=order_by, **kwargs
+        )
 
     @classmethod
     def query_task_by_execution_id(cls, execution_id):
         tasks = cls.query_task(execution_id=execution_id)
         if not tasks:
             raise NoFoundTask(execution_id=execution_id)
         return tasks[0]
@@ -105,16 +115,16 @@
         return cls._update_job_status(ScheduleJob, job_info)
 
     @classmethod
     def update_job(cls, job_info):
         return cls._update_job(ScheduleJob, job_info)
 
     @classmethod
-    def query_job(cls, reverse=None, order_by=None, **kwargs):
-        return cls._query_job(ScheduleJob, reverse, order_by, **kwargs)
+    def query_job(cls, reverse=None, order_by=None, protocol=PROTOCOL.FATE_FLOW, **kwargs):
+        return cls._query_job(ScheduleJob, reverse, order_by, protocol=protocol, **kwargs)
 
     @classmethod
     def query_task(cls, only_latest=True, reverse=None, order_by=None, scheduler_status=False, **kwargs):
         if not scheduler_status:
             obj = ScheduleTask
         else:
             obj = ScheduleTaskStatus
```

### Comparing `fate_flow-2.0.0b0/fate_flow/operation/job_tracker.py` & `fate_flow-2.1.0/ofx/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/proto/__init__.py` & `fate_flow-2.1.0/ofx/api/models/bfia/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/proto/osx/__init__.py` & `fate_flow-2.1.0/ofx/api/proto/rollsite/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/proto/rollsite/__init__.py` & `fate_flow-2.1.0/ofx/api/models/bfia/worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,13 +8,19 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-import os
-import sys
+from .resource import BaseAPI
 
-_pb_path = os.path.abspath(os.path.join(__file__, os.path.pardir))
-if _pb_path not in sys.path:
-    sys.path.append(_pb_path)
+
+class Worker(BaseAPI):
+    def report_task_status(self, status, task_id, role):
+        return self.client.post(
+            endpoint="/v1/platform/schedule/task/callback",
+            json={
+                "status": status,
+                "task_id": task_id,
+                "role": role
+            })
```

### Comparing `fate_flow-2.0.0b0/fate_flow/proto/rollsite/basic_meta_pb2.py` & `fate_flow-2.1.0/fate_flow/proto/rollsite/basic_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/proto/rollsite/proxy_pb2.py` & `fate_flow-2.1.0/fate_flow/proto/rollsite/proxy_pb2.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/proto/rollsite/proxy_pb2_grpc.py` & `fate_flow-2.1.0/fate_flow/proto/rollsite/proxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/runtime/__init__.py` & `fate_flow-2.1.0/ofx/api/models/fate_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/runtime/component_provider.py` & `fate_flow-2.1.0/fate_flow/runtime/component_provider.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/runtime/job_default_config.py` & `fate_flow-2.1.0/fate_flow/runtime/job_default_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     federated_command_trys = None
     job_timeout = None
     auto_retries = None
     sync_type = None
 
     task_logger = None
     task_device = None
-    launcher = None
+    task_timeout = None
 
     @classmethod
     def load(cls):
         conf = file_utils.load_yaml_conf(FATE_FLOW_JOB_DEFAULT_CONFIG_PATH)
         if not isinstance(conf, dict):
             raise ValueError("invalid config file")
```

### Comparing `fate_flow-2.0.0b0/fate_flow/runtime/runtime_config.py` & `fate_flow-2.1.0/fate_flow/runtime/runtime_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-from ofx.api.client import FlowSchedulerApi
 from fate_flow.entity.types import ProcessRole
 
 from fate_flow.runtime.reload_config_base import ReloadConfigBase
 from fate_flow.utils.version import get_versions
-from fate_flow.hub.scheduler import JobSchedulerABC
 
 
 class RuntimeConfig(ReloadConfigBase):
     HTTP_PORT = None
     JOB_SERVER_HOST = None
     PROCESS_ROLE = None
-    SCHEDULE_CLIENT: FlowSchedulerApi = None
-    SCHEDULER: JobSchedulerABC = None
+    SCHEDULE_CLIENT = None
     CLIENT_ROLE = list()
     SERVICE_DB = None
+    SESSION_LIST = []
     ENV = dict()
 
     @classmethod
     def init_config(cls, **kwargs):
         for k, v in kwargs.items():
             if hasattr(cls, k):
                 setattr(cls, k, v)
@@ -62,18 +60,14 @@
         cls.PROCESS_ROLE = process_role
 
     @classmethod
     def set_schedule_client(cls, schedule_client):
         cls.SCHEDULE_CLIENT = schedule_client
 
     @classmethod
-    def set_scheduler(cls, scheduler):
-        cls.SCHEDULER = scheduler
-
-    @classmethod
     def set_client_roles(cls, *roles):
         for role in roles:
             if role not in cls.CLIENT_ROLE:
                 cls.CLIENT_ROLE.append(role)
 
     @classmethod
     def set_service_db(cls, service_db):
```

### Comparing `fate_flow-2.0.0b0/fate_flow/runtime/system_settings.py` & `fate_flow-2.1.0/fate_flow/runtime/system_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,30 +23,28 @@
 from fate_flow.utils.conf_utils import get_base_config
 from fate_flow.utils.file_utils import get_fate_flow_directory, get_fate_python_path
 
 from fate_flow.settings import *
 
 # Server
 API_VERSION = "v2"
-INTERCONN_API_VERSION = "v1"
 FATE_FLOW_SERVICE_NAME = "fateflow"
 SERVER_MODULE = "fate_flow_server.py"
 CASBIN_TABLE_NAME = "fate_casbin"
 PERMISSION_TABLE_NAME = "permission_casbin"
 PERMISSION_MANAGER_PAGE = "permission"
 APP_MANAGER_PAGE = "app"
 
 ADMIN_PAGE = [PERMISSION_MANAGER_PAGE, APP_MANAGER_PAGE]
-FATE_FLOW_CONF_PATH = os.path.join(get_fate_flow_directory(), "conf")
+FATE_FLOW_CONF_PATH = DEFAULT_SERVER_CONF_PATH or os.path.join(get_fate_flow_directory(), "conf")
 
 FATE_FLOW_JOB_DEFAULT_CONFIG_PATH = os.path.join(FATE_FLOW_CONF_PATH, "job_default_config.yaml")
 
 SUBPROCESS_STD_LOG_NAME = "std.log"
 
-
 HOST = get_base_config(FATE_FLOW_SERVICE_NAME, {}).get("host", "127.0.0.1")
 HTTP_PORT = get_base_config(FATE_FLOW_SERVICE_NAME, {}).get("http_port")
 GRPC_PORT = get_base_config(FATE_FLOW_SERVICE_NAME, {}).get("grpc_port")
 
 NGINX_HOST = get_base_config(FATE_FLOW_SERVICE_NAME, {}).get("nginx", {}).get("host") or HOST
 NGINX_HTTP_PORT = get_base_config(FATE_FLOW_SERVICE_NAME, {}).get("nginx", {}).get("http_port") or HTTP_PORT
 RANDOM_INSTANCE_ID = get_base_config(FATE_FLOW_SERVICE_NAME, {}).get("random_instance_id", False)
@@ -63,15 +61,14 @@
 DEFAULT_PROVIDER = get_base_config("default_provider", {})
 CASBIN_MODEL_CONF = os.path.join(FATE_FLOW_CONF_PATH, "casbin_model.conf")
 PERMISSION_CASBIN_MODEL_CONF = os.path.join(FATE_FLOW_CONF_PATH, "permission_casbin_model.conf")
 SERVICE_CONF_NAME = "service_conf.yaml"
 
 DATABASE = get_base_config("database", {})
 
-
 IGNORE_RESOURCE_ROLES = {"arbiter"}
 
 SUPPORT_IGNORE_RESOURCE_ENGINES = {
     ComputingEngine.EGGROLL, ComputingEngine.STANDALONE
 }
 DEFAULT_FATE_PROVIDER_PATH = (DEFAULT_FATE_DIR or get_fate_python_path()) if not is_in_virtualenv() else ""
 HEADERS = {
@@ -106,48 +103,49 @@
     (cygrpc.ChannelArgKey.max_send_message_length, -1),
     (cygrpc.ChannelArgKey.max_receive_message_length, -1),
 ]
 
 LOG_DIR = LOG_DIR or get_fate_flow_directory("logs")
 JOB_DIR = JOB_DIR or get_fate_flow_directory("jobs")
 MODEL_STORE_PATH = MODEL_DIR or os.path.join(get_fate_flow_directory(), "model")
-LOCAL_DATA_STORE_PATH = DATA_DIR or os.path.join(get_fate_flow_directory(), "data")
-LOG_LEVEL = LOG_LEVEL or 10
+STANDALONE_DATA_HOME = DATA_DIR or os.path.join(file_utils.get_fate_flow_directory(), "data")
+LOCALFS_DATA_HOME = DATA_DIR or os.path.join(file_utils.get_fate_flow_directory(), "localfs")
+TEMP_DIR = get_fate_flow_directory("temps")
+LOG_LEVEL = int(os.environ.get("LOG_LEVEL") or get_base_config("log_level", 10))
 LOG_SHARE = False
 FATE_FLOW_LOG_DIR = os.path.join(LOG_DIR, "fate_flow")
 WORKERS_DIR = os.path.join(LOG_DIR, "workers")
 
 SQLITE_FILE_DIR = SQLITE_FILE_DIR or get_fate_flow_directory()
 SQLITE_PATH = os.path.join(SQLITE_FILE_DIR, SQLITE_FILE_NAME)
 
-GRPC_SERVER_MAX_WORKERS = GRPC_SERVER_MAX_WORKERS or (os.cpu_count() or 1) * 5
+GRPC_SERVER_MAX_WORKERS = GRPC_SERVER_MAX_WORKERS or (os.cpu_count() or 1) * 20
 
 VERSION_FILE_PATH = os.path.join(get_fate_flow_directory(), "fateflow.env")
 FATE_FLOW_PROVIDER_PATH = get_fate_flow_directory("python")
-FATE_FLOW_CONF_PATH = get_fate_flow_directory()
 
 # Registry
 FATE_FLOW_MODEL_TRANSFER_ENDPOINT = "/v1/model/transfer"
 ZOOKEEPER = get_base_config("zookeeper", {})
 ZOOKEEPER_REGISTRY = {
     # server
     'flow-server': "/FATE-COMPONENTS/fate-flow",
     # model service
     'fateflow': "/FATE-SERVICES/flow/online/transfer/providers",
     'servings': "/FATE-SERVICES/serving/online/publishLoad/providers",
 }
 USE_REGISTRY = get_base_config("use_registry")
 
+DEEPSPEED_LOGS_DIR_PLACEHOLDER = "EGGROLL_DEEPSPEED_LOGS_DIR"
+DEEPSPEED_MODEL_DIR_PLACEHOLDER = "EGGROLL_DEEPSPEED_MODEL_DIR"
+DEEPSPEED_RESULT_PLACEHOLDER = "EGGROLL_DEEPSPEED_RESULT_DIR"
+
 REQUEST_TRY_TIMES = 3
 REQUEST_WAIT_SEC = 2
 REQUEST_MAX_WAIT_SEC = 300
+SESSION_VALID_PERIOD = 7 * 24 * 60 * 60 * 1000
 
 DEFAULT_OUTPUT_DATA_PARTITIONS = 16
 
-STANDALONE_DATA_HOME = os.path.join(file_utils.get_fate_flow_directory(), "data")
-LOCALFS_DATA_HOME = os.path.join(file_utils.get_fate_flow_directory(), "localfs")
-
 # hub module settings
 # define： xxx.class_name
-DEFAULT_JOB_PARSER_MODULE = "fate_flow.hub.parser.fate.JobParser"
-DEFAULT_JOB_SCHEDULER_MODULE = "fate_flow.hub.scheduler.fate.DAGScheduler"
 DEFAULT_COMPONENTS_WRAPS_MODULE = "fate_flow.hub.components_wraps.fate.FlowWraps"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/scheduler/__init__.py` & `fate_flow-2.1.0/fate_flow/scheduler/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,25 +8,33 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from fate_flow.hub.flow_hub import FlowHub
-from ofx.api.client import FlowSchedulerApi
+from fate_flow.scheduler.scheduler import SchedulerABC
 from fate_flow.runtime.runtime_config import RuntimeConfig
 from fate_flow.runtime.system_settings import HOST, HTTP_PORT, PROXY_PROTOCOL, API_VERSION, HTTP_REQUEST_TIMEOUT
 from fate_flow.utils.api_utils import get_federated_proxy_address, generate_headers
+from ofx.api.client import FlowSchedulerApi
 
 
 def init_scheduler():
     remote_host, remote_port, remote_protocol, grpc_channel = get_federated_proxy_address()
 
     protocol = remote_protocol if remote_protocol else PROXY_PROTOCOL
-    RuntimeConfig.set_schedule_client(FlowSchedulerApi(host=HOST, port=HTTP_PORT,
-                                                       api_version=API_VERSION, timeout=HTTP_REQUEST_TIMEOUT,
-                                                       remote_protocol=protocol, remote_host=remote_host,
-                                                       remote_port=remote_port, grpc_channel=grpc_channel,
-                                                       callback=generate_headers))
 
-    RuntimeConfig.set_scheduler(FlowHub.load_job_scheduler())
+    # schedule client
+    RuntimeConfig.set_schedule_client(
+        FlowSchedulerApi(
+            host=HOST,
+            port=HTTP_PORT,
+            api_version=API_VERSION,
+            timeout=HTTP_REQUEST_TIMEOUT,
+            remote_protocol=protocol,
+            remote_host=remote_host,
+            remote_port=remote_port,
+            grpc_channel=grpc_channel,
+            callback=generate_headers)
+    )
+
```

### Comparing `fate_flow-2.0.0b0/fate_flow/scheduler/federated_scheduler.py` & `fate_flow-2.1.0/fate_flow/controller/federated.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from functools import wraps
 
-from fate_flow.entity.code import FederatedSchedulingStatusCode
-from fate_flow.entity.code import ReturnCode
-from fate_flow.operation.job_saver import ScheduleJobSaver
+from fate_flow.entity.code import FederatedSchedulingStatusCode, ReturnCode
+from fate_flow.manager.operation.job_saver import ScheduleJobSaver
 from fate_flow.runtime.runtime_config import RuntimeConfig
 from fate_flow.utils.log_utils import schedule_logger
 
 
 def get_tasks_by_task_id(task_id, roles=None):
     tasks = [{"job_id": task.f_job_id, "role": task.f_role, "party_id": task.f_party_id,
               "component": task.f_component, "task_id": task.f_task_id,
```

### Comparing `fate_flow-2.0.0b0/fate_flow/settings.py` & `fate_flow-2.1.0/fate_flow/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 # GRPC
 GRPC_SERVER_MAX_WORKERS = None  # default: (os.cpu_count() or 1) * 5
 
 # Request
 HTTP_REQUEST_TIMEOUT = 10  # s
 REMOTE_REQUEST_TIMEOUT = 30000  # ms
 
-LOG_LEVEL = 20
 LOG_DIR = ""
 DATA_DIR = ""
 MODEL_DIR = ""
 JOB_DIR = ""
 DEFAULT_FATE_DIR = ""
+DEFAULT_SERVER_CONF_PATH = ""
+UPLOAD_DATA_HOME = ""
 
 # sqlite
 SQLITE_FILE_DIR = ""
 SQLITE_FILE_NAME = "fate_flow_sqlite.db"
 
 
 # Client Manager
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/__init__.py` & `fate_flow-2.1.0/ofx/api/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/api_utils.py` & `fate_flow-2.1.0/fate_flow/utils/api_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -121,33 +121,35 @@
                             return API.Output.json(code=code, message=message)
                 return _wrapper
             return _outer
 
 
 def get_federated_proxy_address():
     # protocol = CoordinationCommunicationProtocol.HTTP
+    proxy_name = PROXY_NAME
     if ENGINES.get("federated_mode") == FederatedMode.SINGLE:
         return HOST, HTTP_PORT, CoordinationCommunicationProtocol.HTTP, PROXY_NAME
-    if PROXY_NAME == CoordinationProxyService.OSX:
-        host = PROXY.get(PROXY_NAME).get("host")
-        port = PROXY.get(PROXY_NAME).get("port")
+    if proxy_name == CoordinationProxyService.OSX:
+        host = PROXY.get(proxy_name).get("host")
+        port = PROXY.get(proxy_name).get("port")
+        proxy_name = CoordinationProxyService.ROLLSITE
         protocol = CoordinationCommunicationProtocol.GRPC
 
-    elif PROXY_NAME == CoordinationProxyService.ROLLSITE:
-        host = PROXY.get(PROXY_NAME).get("host")
-        port = PROXY.get(PROXY_NAME).get("port")
+    elif proxy_name == CoordinationProxyService.ROLLSITE:
+        host = PROXY.get(proxy_name).get("host")
+        port = PROXY.get(proxy_name).get("port")
         protocol = CoordinationCommunicationProtocol.GRPC
 
-    elif PROXY_NAME == CoordinationProxyService.NGINX:
-        protocol = PROXY.get(PROXY_NAME).get("protocol", "http")
-        host = PROXY.get(PROXY_NAME).get(f"host")
-        port = PROXY.get(PROXY_NAME).get(f"{protocol}_port")
+    elif proxy_name == CoordinationProxyService.NGINX:
+        protocol = PROXY.get(proxy_name).get("protocol", "http")
+        host = PROXY.get(proxy_name).get(f"host")
+        port = PROXY.get(proxy_name).get(f"{protocol}_port")
     else:
-        raise RuntimeError(f"can not support coordinate proxy {PROXY_NAME}， all proxy {PROXY.keys()}")
-    return host, port, protocol, PROXY_NAME
+        raise RuntimeError(f"Can not support coordinate proxy {proxy_name}， all proxy {PROXY.keys()}")
+    return host, port, protocol, proxy_name
 
 
 def generate_headers(party_id, body, initiator_party_id=""):
     return HookManager.site_signature(
         SignatureParameters(party_id=party_id, body=body, initiator_party_id=initiator_party_id))
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/base_utils.py` & `fate_flow-2.1.0/fate_flow/utils/base_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import base64
 import datetime
 import json
 import os
-import pickle
 import random
 import socket
 import time
 import uuid
 from enum import Enum, IntEnum
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/cron.py` & `fate_flow-2.1.0/fate_flow/utils/cron.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/db_utils.py` & `fate_flow-2.1.0/fate_flow/entity/types/_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,13 +8,16 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-def get_dynamic_db_model(base, job_id):
-    return type(base.model(table_index=get_dynamic_tracking_table_index(job_id=job_id)))
+#
+class AppType:
+    SITE = "site"
+    CLIENT = "client"
 
 
-def get_dynamic_tracking_table_index(job_id):
-    return job_id[:8]
+class PROTOCOL:
+    FATE_FLOW = "fate"
+    BFIA = "bfia"
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/engine_utils.py` & `fate_flow-2.1.0/fate_flow/utils/engine_utils.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/file_utils.py` & `fate_flow-2.1.0/fate_flow/utils/file_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     if args:
         return os.path.join(PROJECT_BASE, *args)
     return PROJECT_BASE
 
 
 def get_fate_python_path():
     global FATE_PYTHON_PATH
-    if FATE_PYTHON_PATH is None:
+    if not FATE_PYTHON_PATH:
         FATE_PYTHON_PATH = get_project_base_directory("fate", "python")
         if not os.path.exists(FATE_PYTHON_PATH):
             FATE_PYTHON_PATH = get_project_base_directory("python")
             if not os.path.exists(FATE_PYTHON_PATH):
                 return
     return FATE_PYTHON_PATH
 
@@ -86,7 +86,13 @@
         )
 
 
 def rewrite_json_file(filepath, json_data):
     with open(filepath, "w") as f:
         json.dump(json_data, f, indent=4, separators=(",", ": "))
     f.close()
+
+
+def save_file(file, path):
+    with open(path, 'wb') as f:
+        content = file.stream.read()
+        f.write(content)
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/grpc_utils.py` & `fate_flow-2.1.0/fate_flow/utils/grpc_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 from fate_flow.errors.server_error import ResponseException
-from fate_flow.proto.osx import osx_pb2, osx_pb2_grpc
 from fate_flow.proto.rollsite import proxy_pb2_grpc, basic_meta_pb2, proxy_pb2
 
 from fate_flow.runtime.runtime_config import RuntimeConfig
 from fate_flow.runtime.system_settings import FATE_FLOW_SERVICE_NAME, GRPC_PORT, HOST, REMOTE_REQUEST_TIMEOUT
 from fate_flow.utils.base_utils import json_loads, json_dumps
 from fate_flow.utils.log_utils import audit_logger
 from fate_flow.utils.requests_utils import request
@@ -78,48 +77,14 @@
         audit_logger(job_id).info("rpc receive: {} {}".format(get_url(_suffix), param))
         resp = request(method=method, url=get_url(_suffix), json=param_dict, headers=headers)
         audit_logger(job_id).info(f"resp: {resp.text}")
         resp_json = response_json(resp)
         return wrap_grpc_packet(resp_json, method, _suffix, dst.partyId, src.partyId, job_id)
 
 
-class UnaryServiceOSX(osx_pb2_grpc.PrivateTransferProtocolServicer):
-    def invoke(self, _request, context):
-        packet = _request
-        metadata = packet.metadata
-        payload = packet.payload
-        request_info = json_loads(bytes.decode(payload))
-        job_id = metadata.get("JobId")
-        audit_logger(job_id).info(f"rpc receive metadata: {metadata}")
-        audit_logger(job_id).info(f"rpc receive request_info: {request_info}")
-        source_node_id = metadata.get("TargetNodeID")
-        target_node_id = metadata.get("SourceNodeID")
-        _routing_metadata = gen_routing_metadata(src_party_id=source_node_id, dest_party_id=target_node_id)
-        audit_logger(job_id).info(f'start request：{request_info.get("method")}, {get_url(request_info.get("uri"))},'
-                                  f'{request_info.get("json_body")}, {request_info.get("headers")}')
-        resp = request(method=request_info.get("method"), url=get_url(request_info.get("uri")),
-                       json=request_info.get("json_body"), headers=request_info.get("headers", {}))
-        audit_logger(job_id).info(f"resp: {resp.text}")
-        resp_json = response_json(resp)
-        _meta = {
-            "TechProviderCode": metadata.get("TechProviderCode", ""),
-            "SourceInstID": metadata.get("TargetInstID", ""),
-            "TargetInstID": metadata.get("SourceInstID", ""),
-            "SourceNodeID": source_node_id,
-            "TargetNodeID": target_node_id,
-            "TargetComponentName": FATE_FLOW_SERVICE_NAME,
-            "TargetMethod": metadata.get("TargetMethod", ""),
-            "JobId": job_id
-        }
-        _data = bytes(json_dumps(resp_json), 'utf-8')
-        res = osx_pb2.Outbound(metadata=_meta, payload=_data)
-        audit_logger(job_id).info(f"response: {res}")
-        return res
-
-
 def response_json(response):
     try:
         return response.json()
     except:
         audit_logger().exception(response.text)
         e = ResponseException(response=response.text)
         return {"code": e.code, "message": e.message}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/io_utils.py` & `fate_flow-2.1.0/fate_flow/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/log.py` & `fate_flow-2.1.0/fate_flow/utils/log.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/log_utils.py` & `fate_flow-2.1.0/fate_flow/utils/log_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,17 @@
         logger.addHandler(handler)
         logger.addHandler(error_handler)
     with LoggerFactory.lock:
         LoggerFactory.schedule_logger_dict[job_id + log_type] = logger
     return logger
 
 
-def schedule_logger(job_id=None, delete=False):
+def schedule_logger(job_id=None, delete=False, name="fate_flow_schedule"):
     if not job_id:
-        return getLogger("fate_flow_schedule")
+        return getLogger(name)
     else:
         if delete:
             with LoggerFactory.lock:
                 try:
                     for key in LoggerFactory.schedule_logger_dict.keys():
                         if job_id in key:
                             del LoggerFactory.schedule_logger_dict[key]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/object_utils.py` & `fate_flow-2.1.0/fate_flow/utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/password_utils.py` & `fate_flow-2.1.0/fate_flow/utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/permission_utils.py` & `fate_flow-2.1.0/fate_flow/utils/permission_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,26 +9,55 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
+from functools import wraps
+from flask import request as flask_request
+
+from fate_flow.controller.parser import JobParser
+from fate_flow.entity.code import ReturnCode
 from fate_flow.entity.spec.dag import DAGSchema
+from fate_flow.hook import HookManager
 from fate_flow.hook.common.parameters import PermissionCheckParameters
-from fate_flow.hub.flow_hub import FlowHub
+from fate_flow.manager.service.provider_manager import ProviderManager
+from fate_flow.runtime.system_settings import PERMISSION_SWITCH
+from fate_flow.utils.api_utils import API
 
 
 def get_permission_parameters(role, party_id, initiator_party_id, job_info) -> PermissionCheckParameters:
-    dag_schema = DAGSchema(**job_info['dag_schema'])
-    job_parser = FlowHub.load_job_parser(dag_schema)
+    dag_schema = DAGSchema(**job_info)
+    job_parser = JobParser(dag_schema)
     component_list = job_parser.component_ref_list(role, party_id)
+    fate_component_list = set(component_list) - set(ProviderManager.get_flow_components())
     dataset_list = job_parser.dataset_list(role, party_id)
     component_parameters = job_parser.role_parameters(role, party_id)
     return PermissionCheckParameters(
         initiator_party_id=initiator_party_id,
         roles=dag_schema.dag.parties,
-        component_list=component_list,
+        component_list=fate_component_list,
         dataset_list=dataset_list,
         dag_schema=dag_schema.dict(),
         component_parameters=component_parameters
     )
+
+
+def create_job_request_check(func):
+    @wraps(func)
+    def _wrapper(*_args, **_kwargs):
+        party_id = _kwargs.get("party_id")
+        role = _kwargs.get("role")
+        body = flask_request.json
+        headers = flask_request.headers
+        initiator_party_id = headers.get("initiator_party_id")
+
+        # permission check
+        if PERMISSION_SWITCH:
+            permission_return = HookManager.permission_check(get_permission_parameters(
+                role, party_id, initiator_party_id, body
+            ))
+            if permission_return.code != ReturnCode.Base.SUCCESS:
+                return API.Output.fate_flow_exception(permission_return)
+        return func(*_args, **_kwargs)
+    return _wrapper
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/process_utils.py` & `fate_flow-2.1.0/fate_flow/utils/process_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,14 @@
     :param process:
     :return:
     """
     try:
         cmdline = process.cmdline()
     except Exception as e:
         # Not sure whether the process is a task executor process, operations processing is required
-        schedule_logger(task.f_job_id).warning(e)
         return False
     else:
         schedule_logger(task.f_job_id).info(cmdline)
 
     if task.f_worker_id and task.f_worker_id in cmdline:
         return True
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/requests_utils.py` & `fate_flow-2.1.0/fate_flow/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/schedule_utils.py` & `fate_flow-2.1.0/fate_flow/utils/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/version.py` & `fate_flow-2.1.0/fate_flow/engine/storage/serdes/_serdes_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,27 +9,13 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import os
 
-import dotenv
-import typing
+from pickle import loads as p_loads
+from pickle import dumps as p_dumps
+from pickle import Pickler, Unpickler
 
-from fate_flow.runtime.system_settings import VERSION_FILE_PATH
-
-
-def get_versions() -> typing.Mapping[str, typing.Any]:
-    return dotenv.dotenv_values(
-        dotenv_path=VERSION_FILE_PATH
-    )
-
-
-def get_flow_version() -> typing.Optional[str]:
-    return get_versions().get("FATEFlow")
-
-
-def get_default_fate_version() -> typing.Optional[str]:
-    return get_versions().get("FATE")
+__all__ = ["p_dumps", "p_loads", "Pickler", "Unpickler"]
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/wraps_utils.py` & `fate_flow-2.1.0/fate_flow/utils/wraps_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,19 @@
 import threading
 from functools import wraps
 
 from fate_flow.entity.code import ReturnCode
 
 from flask import request as flask_request
 from fate_flow.errors.server_error import NoFoundTask, ResponseException, NoFoundINSTANCE, NoPermission
-from fate_flow.hook import HookManager
-from fate_flow.operation.job_saver import JobSaver
+from fate_flow.manager.operation.job_saver import JobSaver
 from fate_flow.runtime.runtime_config import RuntimeConfig
-from fate_flow.runtime.system_settings import HOST, HTTP_PORT, API_VERSION, PERMISSION_SWITCH
+from fate_flow.runtime.system_settings import HOST, HTTP_PORT, API_VERSION
 from fate_flow.utils.api_utils import API, federated_coordination_on_http
 from fate_flow.utils.log_utils import schedule_logger
-from fate_flow.utils.permission_utils import get_permission_parameters
 from fate_flow.utils.requests_utils import request
 from fate_flow.utils.schedule_utils import schedule_signal
 from fate_flow.db.casbin_models import FATE_CASBIN
 
 
 def filter_parameters(filter_value=None):
     def _inner(func):
@@ -142,45 +140,39 @@
                 _result = func(*args, **kwargs)
             except Exception as e:
                 schedule_logger(job.f_job_id).exception(e)
                 raise e
             finally:
                 schedule_signal(job_id=job.f_job_id, set_or_reset=False)
                 schedule_logger(job.f_job_id).debug(f"release job {job.f_job_id} schedule lock")
-                return _result
+            return _result
         else:
             return func(*args, **kwargs)
     return _wrapper
 
 
 def threading_lock(func):
     @wraps(func)
     def _wrapper(*args, **kwargs):
         with threading.Lock():
             return func(*args, **kwargs)
     return _wrapper
 
 
-def create_job_request_check(func):
+def asynchronous_function(func):
     @wraps(func)
-    def _wrapper(*_args, **_kwargs):
-        party_id = _kwargs.get("party_id")
-        role = _kwargs.get("role")
-        body = flask_request.json
-        headers = flask_request.headers
-        initiator_party_id = headers.get("initiator_party_id")
-
-        # permission check
-        if PERMISSION_SWITCH:
-            permission_return = HookManager.permission_check(get_permission_parameters(
-                role, party_id, initiator_party_id, body
-            ))
-            if permission_return.code != ReturnCode.Base.SUCCESS:
-                return API.Output.fate_flow_exception(permission_return)
-        return func(*_args, **_kwargs)
+    def _wrapper(*args, **kwargs):
+        is_asynchronous = kwargs.pop("is_asynchronous", False)
+        if is_asynchronous:
+            thread = threading.Thread(target=func, args=args, kwargs=kwargs)
+            thread.start()
+            is_asynchronous = True
+            return is_asynchronous
+        else:
+            return func(*args, **kwargs)
     return _wrapper
 
 
 def check_permission(operate=None, types=None):
     def _inner(func):
         @wraps(func)
         def _wrapper(*args, **kwargs):
```

### Comparing `fate_flow-2.0.0b0/fate_flow/utils/xthread.py` & `fate_flow-2.1.0/fate_flow/utils/xthread.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/worker/__init__.py` & `fate_flow-2.1.0/ofx/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/worker/fate_executor.py` & `fate_flow-2.1.0/fate_flow/manager/worker/fate_executor.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/fate_flow/worker/fate_flow_executor.py` & `fate_flow-2.1.0/fate_flow/adapter/bfia/translator/component_spec.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
-import argparse
-import sys
-
-from fate_flow.entity import BaseEntity
-from fate_flow.utils.log import getLogger
-
-
-class FateFlowSubmit:
-    @staticmethod
-    def run():
-        import click
-        from fate_flow.entrypoint.cli import component
-
-        cli = click.Group()
-        cli.add_command(component)
-        cli(prog_name="python -m fate_flow.components")
+from pydantic import BaseModel
+from typing import Optional, Dict, List, Literal
 
 
-if __name__ == "__main__":
-    FateFlowSubmit.run()
+class DataSpec(BaseModel):
+    name: str
+    description: str
+    category: str
+    dataFormat: List[str]
+
+
+class BFIAComponentSpec(BaseModel):
+    componentName: str
+    title: str
+    provider: str
+    version: str
+    description: str
+    roleList: List[Literal["guest", "host", "arbiter", "local"]]
+    desVersion: str
+    storageEngine: List[str]
+    inputParam: Optional[List[Dict]]
+    inputData: Optional[List[DataSpec]]
+    outputData: Optional[List[DataSpec]]
```

### Comparing `fate_flow-2.0.0b0/fate_flow.egg-info/PKG-INFO` & `fate_flow-2.1.0/fate_flow.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 Metadata-Version: 2.1
 Name: fate-flow
-Version: 2.0.0b0
+Version: 2.1.0
+Summary: UNKNOWN
 Home-page: https://fate.fedai.org/
 Author: FederatedAI
 Author-email: contact@FedAI.org
 License: Apache-2.0 License
+Description: [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![CodeStyle](https://img.shields.io/badge/Check%20Style-Google-brightgreen)](https://checkstyle.sourceforge.io/google_style.html) [![Style](https://img.shields.io/badge/Check%20Style-Black-black)](https://checkstyle.sourceforge.io/google_style.html)
+        
+        [中文](./README.zh.md)
+        
+        FATE Flow is a multi-party federated task security scheduling platform for federated learning end-to-end pipeline
+        
+        - [Shared-State Scheduling Architecture](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/41684.pdf)
+        - Secure Multi-Party Communication Across Data Centers
+        
+        Providing production-level service capabilities:
+        
+        - Data Access
+        - Component Registry
+        - Federated Job&Task Scheduling
+        - Multi-Party Resource Coordination
+        - Data Flow Tracking
+        - Real-Time Job Monitoring
+        - Multi-Party Federated Model Registry
+        - Multi-Party Cooperation Authority Management
+        - High Availability
+        - CLI, REST API, Python API
+        
+        ## Deployment
+        
+        Please refer to [FATE](https://github.com/FederatedAI/FATE)
+        
+        ## Documentation
+        
+        The official FATE Flow documentation is here [https://federatedai.github.io/FATE-Flow/latest/](https://federatedai.github.io/FATE-Flow/latest/)
+        
+        ## License
+        [Apache License 2.0](LICENSE)
+        
 Keywords: federated learning scheduler
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rabbitmq
 Provides-Extra: pulsar
 Provides-Extra: spark
 Provides-Extra: eggroll
-Provides-Extra: all
-
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![CodeStyle](https://img.shields.io/badge/Check%20Style-Google-brightgreen)](https://checkstyle.sourceforge.io/google_style.html) [![Style](https://img.shields.io/badge/Check%20Style-Black-black)](https://checkstyle.sourceforge.io/google_style.html)
-
-[中文](./README.zh.md)
-
-FATE Flow is a multi-party federated task security scheduling platform for federated learning end-to-end pipeline
-
-- [Shared-State Scheduling Architecture](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/41684.pdf)
-- Secure Multi-Party Communication Across Data Centers
-
-Providing production-level service capabilities:
-
-- Data Access
-- Component Registry
-- Federated Job&Task Scheduling
-- Multi-Party Resource Coordination
-- Data Flow Tracking
-- Real-Time Job Monitoring
-- Multi-Party Federated Model Registry
-- Multi-Party Cooperation Authority Management
-- High Availability
-- CLI, REST API, Python API
-
-## Deployment
-
-Please refer to [FATE](https://github.com/FederatedAI/FATE)
-
-## Documentation
-
-The official FATE Flow documentation is here [https://federatedai.github.io/FATE-Flow/latest/](https://federatedai.github.io/FATE-Flow/latest/)
-
-## License
-[Apache License 2.0](LICENSE)
+Provides-Extra: fate_flow
```

### Comparing `fate_flow-2.0.0b0/ofx/__init__.py` & `fate_flow-2.1.0/ofx/__init__.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/ofx/api/__init__.py` & `fate_flow-2.1.0/fate_flow/manager/components/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+#
```

### Comparing `fate_flow-2.0.0b0/ofx/api/models/__init__.py` & `fate_flow-2.1.0/fate_flow/adapter/bfia/container/entrypoint/runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,7 +8,22 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+#
+
+class Submit:
+    @staticmethod
+    def run():
+        import click
+        from fate_flow.adapter.bfia.container.entrypoint.cli import component
+
+        cli = click.Group()
+        cli.add_command(component)
+        cli(prog_name="python -m fate_flow.adapter.bfia.container.entrypoint")
+
+
+if __name__ == "__main__":
+    Submit.run()
```

### Comparing `fate_flow-2.0.0b0/ofx/api/models/federated.py` & `fate_flow-2.1.0/ofx/api/models/fate_flow/federated.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/ofx/api/models/resource.py` & `fate_flow-2.1.0/ofx/api/models/fate_flow/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,33 +13,36 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import threading
 
 import json
 import requests
 
-from ..utils.grpc_utils import wrap_osx_grpc_packet, wrap_proxy_grpc_packet
-from ..utils.grpc_utils import gen_routing_metadata, get_osx_channel, get_proxy_channel
+from ...utils.grpc_utils import wrap_proxy_grpc_packet
+from ...utils.grpc_utils import gen_routing_metadata, get_proxy_channel
 
 FEDERATED_ERROR = 104
 
 
 class APIClient(requests.Session):
     def __init__(self, host="127.0.0.1", port=9380, protocol="http", api_version=None, timeout=60,
-                 remote_protocol="http", remote_host=None, remote_port=None, grpc_channel="default"):
+                 remote_protocol="http", remote_host=None, remote_port=None, grpc_channel="default",
+                 provider: str = "FATE", route_table=None):
         super().__init__()
         self.host = host
         self.port = port
         self.protocol = protocol
         self.timeout = timeout
         self.api_version = api_version
         self.remote_protocol = remote_protocol
         self.remote_host = remote_host
         self.remote_port = remote_port
         self.grpc_channel = grpc_channel
+        self.provider = provider
+        self.route_table = route_table
 
     @property
     def base_url(self):
         return f'{self.protocol}://{self.host}:{self.port}'
 
     @property
     def version(self):
@@ -120,18 +123,15 @@
             kwargs.update({
                 "host": self.remote_host,
                 "port": self.remote_port,
             })
             if self.remote_protocol == "http":
                 return self.remote_on_http(**kwargs)
             if self.remote_protocol == "grpc":
-                if self.grpc_channel == "osx":
-                    return self.remote_on_grpc_osx(**kwargs)
-                else:
-                    return self.remote_on_grpc_proxy(**kwargs)
+                return self.remote_on_grpc_proxy(**kwargs)
             else:
                 raise Exception(f'{self.remote_protocol} coordination communication protocol is not supported.')
         else:
             return self.remote_on_http(**kwargs)
 
     def remote_on_http(self, method, endpoint, host=None, port=None, try_times=3, timeout=10,
                        json_body=None, dest_party_id=None, service_name="fateflow", headers=None, **kwargs):
@@ -183,44 +183,14 @@
                 try:
                     return json.loads(bytes.decode(_return.body.value))
                 except Exception:
                     raise RuntimeError(f"{_return}, {_call}")
             finally:
                 channel.close()
 
-    @staticmethod
-    def remote_on_grpc_osx(job_id, method, host, port, endpoint, src_party_id, dest_party_id, json_body,
-                           try_times=3, timeout=10, headers=None, source_host=None, source_port=None, **kwargs):
-        _packet = wrap_osx_grpc_packet(
-            json_body=json_body, http_method=method, url=endpoint,
-            src_party_id=src_party_id, dst_party_id=dest_party_id,
-            job_id=job_id, headers=headers, overall_timeout=timeout,
-            source_host=source_host, source_port=source_port, **kwargs
-        )
-        _routing_metadata = gen_routing_metadata(
-            src_party_id=src_party_id, dest_party_id=dest_party_id,
-        )
-        for t in range(try_times):
-            channel, stub = get_osx_channel(host, port)
-            try:
-                _return, _call = stub.invoke.with_call(
-                    _packet, metadata=_routing_metadata,
-                    timeout=timeout or None,
-                )
-            except Exception as e:
-                if t >= try_times - 1:
-                    raise Exception(str(e))
-            else:
-                try:
-                    return json.loads(bytes.decode(_return.payload))
-                except Exception:
-                    raise RuntimeError(f"{_return}, {_call}")
-            finally:
-                channel.close()
-
 
 class BaseAPI:
     def __init__(self, client: APIClient, callback=None):
         self.client = client
         self.callback = callback
 
     def federated_command(self, job_id, src_role, src_party_id, dest_role, dest_party_id, endpoint, body,
@@ -230,15 +200,15 @@
             headers = {}
             if self.callback:
                 result = self.callback(dest_party_id, body, initiator_party_id=initiator_party_id)
                 if result.code == 0:
                     headers = result.signature if result.signature else {}
                 else:
                     raise Exception(result.code, result.message)
-            headers.update({"initiator_party_id": initiator_party_id})
+            headers.update({"initiator-party-id": initiator_party_id})
             response = self.client.remote(job_id=job_id,
                                           method=method,
                                           endpoint=endpoint,
                                           src_role=src_role,
                                           src_party_id=src_party_id,
                                           dest_party_id=dest_party_id,
                                           json_body=body if body else {},
```

### Comparing `fate_flow-2.0.0b0/ofx/api/models/scheduler.py` & `fate_flow-2.1.0/ofx/api/models/fate_flow/scheduler.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/ofx/api/models/worker.py` & `fate_flow-2.1.0/ofx/api/models/fate_flow/worker.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/ofx/api/proto/__init__.py` & `fate_flow-2.1.0/fate_flow/manager/outputs/model/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,7 +8,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+from fate_flow.manager.outputs.model.model_manager import PipelinedModel
+from fate_flow.manager.outputs.model.model_meta import ModelMeta
+
+__all__ = ["PipelinedModel", "ModelMeta"]
```

### Comparing `fate_flow-2.0.0b0/ofx/api/proto/rollsite/basic_meta_pb2.py` & `fate_flow-2.1.0/ofx/api/proto/rollsite/basic_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/ofx/api/proto/rollsite/proxy_pb2.py` & `fate_flow-2.1.0/ofx/api/proto/rollsite/proxy_pb2.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/ofx/api/proto/rollsite/proxy_pb2_grpc.py` & `fate_flow-2.1.0/ofx/api/proto/rollsite/proxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fate_flow-2.0.0b0/ofx/api/utils/grpc_utils.py` & `fate_flow-2.1.0/ofx/api/utils/grpc_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,34 +12,17 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import json
 
 import grpc
 
-from ..proto.osx import osx_pb2, osx_pb2_grpc
 from ..proto.rollsite import basic_meta_pb2, proxy_pb2, proxy_pb2_grpc
 
 
-def wrap_osx_grpc_packet(job_id, json_body, http_method, url, src_party_id, dst_party_id, headers=None, provider="FATE",
-                         role="fateflow", target_method="UNARY_CALL", **kwargs):
-    _meta = {
-        "TechProviderCode": provider,
-        "SourceNodeID": src_party_id,
-        "TargetNodeID": dst_party_id,
-        "TargetComponentName": role,
-        "TargetMethod": target_method,
-        "JobId": job_id
-    }
-    if not headers:
-        headers = {}
-    _data = bytes(json.dumps(dict(uri=url, json_body=json_body, headers=headers, method=http_method)), 'utf-8')
-    return osx_pb2.Inbound(metadata=_meta, payload=_data)
-
-
 def wrap_proxy_grpc_packet(json_body, http_method, url, src_party_id, dst_party_id, job_id=None, headers=None,
                            overall_timeout=None, role="fateflow", source_host=None, source_port=None):
     if not headers:
         headers = {}
     _src_end_point = basic_meta_pb2.Endpoint(ip=source_host, port=source_port)
     _src = proxy_pb2.Topic(name=job_id, partyId="{}".format(src_party_id), role=role,
                            callback=_src_end_point)
@@ -49,20 +32,14 @@
     _command = proxy_pb2.Command(name=url)
     _conf = proxy_pb2.Conf(overallTimeout=overall_timeout)
     _meta = proxy_pb2.Metadata(src=_src, dst=_dst, task=_task, command=_command, operator=http_method, conf=_conf)
     _data = proxy_pb2.Data(key=url, value=bytes(json.dumps(json_body), 'utf-8'))
     return proxy_pb2.Packet(header=_meta, body=_data)
 
 
-def get_osx_channel(host, port):
-    channel = grpc.insecure_channel(f"{host}:{port}")
-    stub = osx_pb2_grpc.PrivateTransferProtocolStub(channel)
-    return channel, stub
-
-
 def get_proxy_channel(host, port):
     channel = grpc.insecure_channel(f"{host}:{port}")
     stub = proxy_pb2_grpc.DataTransferServiceStub(channel)
     return channel, stub
 
 
 def gen_routing_metadata(src_party_id, dest_party_id):
```

### Comparing `fate_flow-2.0.0b0/setup.py` & `fate_flow-2.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,54 +2,52 @@
 import shutil
 
 import fate_flow
 from setuptools import find_packages, setup, Command
 
 packages = find_packages(".")
 install_requires = [
-    "apsw==3.38.5.post1",
+    "apsw",
     "Flask==2.2.5",
-    "grpcio==1.46.3",
-    "grpcio-tools==1.46.3",
-    "requests<2.26.0",
-    "urllib3==1.26.5",
+    "grpcio==1.59.3",
+    "grpcio-tools==1.59.3",
+    "requests",
+    "urllib3",
     "cachetools",
     "filelock",
-    "pydantic",
+    "pydantic==1.10.12",
     "webargs",
     "peewee",
     "python-dotenv",
     "pyyaml",
     "networkx",
-    "psutil>=5.7.0",
+    "psutil",
     "casbin_peewee_adapter",
     "casbin",
     "pymysql",
     "kazoo",
     "shortuuid",
     "cos-python-sdk-v5",
     "typing-extensions",
-    "ruamel-yaml==0.16",
+    "ruamel.yaml==0.16",
+    "boto3"
 ]
 extras_require = {
     "rabbitmq": ["pika==1.2.1"],
     "pulsar": ["pulsar-client==2.10.2"],
     "spark": ["pyspark"],
     "eggroll": [
-        "grpcio==1.46.3",
-        "grpcio-tools==1.46.3",
-        "numba==0.56.4",
-        "protobuf==3.19.6",
-        "pyarrow==6.0.1",
-        "mmh3==3.0.0",
-        "cachetools>=3.0.0",
-        "cloudpickle==2.1.0",
-        "psutil>=5.7.0",
+        "cloudpickle",
+        "lmdb",
+        "protobuf",
+        "grpcio",
+        "grpcio-tools",
+        "protobuf",
     ],
-    "all": ["fate_flow[rabbitmq,pulsar,spark,eggroll]"],
+    "fate_flow": ["fate_flow[rabbitmq,pulsar,spark,eggroll]"],
 }
 
 
 CONF_NAME = "conf"
 PACKAGE_NAME = "fate_flow"
 ENV_NAME = "fateflow.env"
 HOME = os.path.abspath("../")
```

