# Comparing `tmp/osml-model-runner-2.0.0.tar.gz` & `tmp/osml-model-runner-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osml-model-runner-2.0.0.tar", last modified: Thu Feb 29 18:07:16 2024, max compression
+gzip compressed data, was "osml-model-runner-2.1.0.tar", last modified: Tue Apr  2 22:15:20 2024, max compression
```

## Comparing `osml-model-runner-2.0.0.tar` & `osml-model-runner-2.1.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.102810 osml-model-runner-2.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)      946 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-02-29 18:07:16.102810 osml-model-runner-2.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     6569 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      547 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2318 2024-02-29 18:07:16.102810 osml-model-runner-2.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.090809 osml-model-runner-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.086809 osml-model-runner-2.0.0/src/aws/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.086809 osml-model-runner-2.0.0/src/aws/osml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.090809 osml-model-runner-2.0.0/src/aws/osml/model_runner/
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.090809 osml-model-runner-2.0.0/src/aws/osml/model_runner/api/
--rwxr-xr-x   0 runner    (1001) docker     (127)      526 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/api/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9711 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/api/image_request.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/api/inference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2379 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/api/region_request.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1879 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/api/request_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/api/sink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53376 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5201 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/app_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.094809 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1457 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      216 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/auto_string_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      901 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/credentials_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3616 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/endpoint_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      191 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/log_context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/metrics_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7539 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/mr_post_processing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4416 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/security_classification.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2618 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/common/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.094809 osml-model-runner-2.0.0/src/aws/osml/model_runner/database/
--rwxr-xr-x   0 runner    (1001) docker     (127)      779 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/database/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10578 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/database/ddb_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4482 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/database/endpoint_statistics_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      706 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/database/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11060 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/database/feature_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9197 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/database/job_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6210 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/database/region_request_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.098810 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/
--rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1457 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/endpoint_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/endpoint_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9508 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/feature_selection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11914 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/http_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/sm_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.098810 osml-model-runner-2.0.0/src/aws/osml/model_runner/queue/
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/queue/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/queue/request_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.098810 osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/
--rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4507 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/kinesis_sink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3583 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/s3_sink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1171 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/sink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1854 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/sink_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.098810 osml-model-runner-2.0.0/src/aws/osml/model_runner/status/
--rwxr-xr-x   0 runner    (1001) docker     (127)      409 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/status/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/status/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1805 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/status/image_request_status.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/status/sns_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3827 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/status/status_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.102810 osml-model-runner-2.0.0/src/aws/osml/model_runner/tile_worker/
--rwxr-xr-x   0 runner    (1001) docker     (127)      322 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/tile_worker/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      184 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/tile_worker/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9897 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/tile_worker/tile_worker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13472 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/src/aws/osml/model_runner/tile_worker/tile_worker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.102810 osml-model-runner-2.0.0/src/osml_model_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-02-29 18:07:16.000000 osml-model-runner-2.0.0/src/osml_model_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-02-29 18:07:16.000000 osml-model-runner-2.0.0/src/osml_model_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 18:07:16.000000 osml-model-runner-2.0.0/src/osml_model_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 18:07:15.000000 osml-model-runner-2.0.0/src/osml_model_runner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-29 18:07:16.000000 osml-model-runner-2.0.0/src/osml_model_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-29 18:07:16.000000 osml-model-runner-2.0.0/src/osml_model_runner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:07:16.102810 osml-model-runner-2.0.0/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12846 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/test/test_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30059 2024-02-29 18:07:11.000000 osml-model-runner-2.0.0/test/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      946 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6895 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      547 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2318 2024-04-02 22:15:20.905538 osml-model-runner-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.889538 osml-model-runner-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.889538 osml-model-runner-2.1.0/src/aws/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.889538 osml-model-runner-2.1.0/src/aws/osml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.889538 osml-model-runner-2.1.0/src/aws/osml/model_runner/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      209 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.893538 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      531 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9708 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/image_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/region_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1884 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/request_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/api/sink.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53228 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5206 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.893538 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1462 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/auto_string_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      906 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/credentials_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3621 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/endpoint_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      196 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/log_context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/metrics_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7544 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/mr_post_processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4421 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/security_classification.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2623 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1518 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/common/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.893538 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      784 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10583 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/ddb_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4487 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/endpoint_statistics_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      711 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11027 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/feature_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9202 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/job_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6210 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/database/region_request_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.897538 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      493 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1462 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/endpoint_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/endpoint_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9513 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/feature_selection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11901 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/http_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/sm_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.897538 osml-model-runner-2.1.0/src/aws/osml/model_runner/queue/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      250 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/queue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3553 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/queue/request_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.897538 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4404 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/kinesis_sink.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3522 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/s3_sink.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/sink.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1859 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/sink_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1810 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/image_request_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2244 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/sns_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3772 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/status/status_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      327 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9898 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/tile_worker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13353 2024-04-02 22:15:10.000000 osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/tile_worker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 22:15:20.000000 osml-model-runner-2.1.0/src/osml_model_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:15:20.901538 osml-model-runner-2.1.0/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12851 2024-04-02 22:15:11.000000 osml-model-runner-2.1.0/test/test_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30059 2024-04-02 22:15:11.000000 osml-model-runner-2.1.0/test/test_app.py
```

### Comparing `osml-model-runner-2.0.0/LICENSE` & `osml-model-runner-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.0.0/PKG-INFO` & `osml-model-runner-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-model-runner
-Version: 2.0.0
+Version: 2.1.0
 Summary: Application to run large scale imagery against AI/ML models
 Author: Amazon Web Services
 Author-email: aws-osml-admin@amazon.com
 License: 
         MIT No Attribution
         
         Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
@@ -116,14 +116,20 @@
 features of interest would fall on the tile boundaries and therefore be missed by the ML models because they are only
 seeing a fractional object. This application mitigates that by allowing requests to specify an overlap region size that
 should be tuned to the expected size of the objects. Each tile sent to the ML model will be cut from the full image
 overlapping the previous by the specified amount. Then the results from each tile are aggregated with the aid of a
 Non-Maximal Suppression algorithm used to eliminate duplicates in cases where an object in an overlap region was picked
 up by multiple model runs.
 
+### Metrics and Logs
+
+As the application runs key performance metrics and detailed logging information are output to [CloudWatch](https://aws.amazon.com/cloudwatch/).
+A detailed description of what information is tracked along with example dashboards can be found in
+[METRICS_AND_DASHBOARDS.md](./METRICS_AND_DASHBOARDS.md).
+
 ### Package Layout
 
 * **/src**: This is the Python implementation of this application.
 * **/test**: Unit tests have been implemented using [pytest](https://docs.pytest.org).
 * **/bin**: The entry point for the containerized application.
 * **/scripts**: Utility scripts that are not part of the main application frequently used in development / testing.
```

### Comparing `osml-model-runner-2.0.0/README.md` & `osml-model-runner-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,20 @@
 features of interest would fall on the tile boundaries and therefore be missed by the ML models because they are only
 seeing a fractional object. This application mitigates that by allowing requests to specify an overlap region size that
 should be tuned to the expected size of the objects. Each tile sent to the ML model will be cut from the full image
 overlapping the previous by the specified amount. Then the results from each tile are aggregated with the aid of a
 Non-Maximal Suppression algorithm used to eliminate duplicates in cases where an object in an overlap region was picked
 up by multiple model runs.
 
+### Metrics and Logs
+
+As the application runs key performance metrics and detailed logging information are output to [CloudWatch](https://aws.amazon.com/cloudwatch/).
+A detailed description of what information is tracked along with example dashboards can be found in
+[METRICS_AND_DASHBOARDS.md](./METRICS_AND_DASHBOARDS.md).
+
 ### Package Layout
 
 * **/src**: This is the Python implementation of this application.
 * **/test**: Unit tests have been implemented using [pytest](https://docs.pytest.org).
 * **/bin**: The entry point for the containerized application.
 * **/scripts**: Utility scripts that are not part of the main application frequently used in development / testing.
```

### Comparing `osml-model-runner-2.0.0/pyproject.toml` & `osml-model-runner-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.0.0/setup.cfg` & `osml-model-runner-2.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osml-model-runner
-version = 2.0.0
+version = 2.1.0
 description = Application to run large scale imagery against AI/ML models
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Amazon Web Services
 author_email = aws-osml-admin@amazon.com
 license = 
 	MIT No Attribution
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/api/__init__.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 # Telling flake8 to not flag errors in this file. It is normal that these classes are imported but not used in an
 # __init__.py file.
 # flake8: noqa
 
 from .exceptions import InvalidImageRequestException, InvalidS3ObjectException
 from .image_request import ImageRequest
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/api/image_request.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 from json import dumps, loads
 from typing import Any, Dict, List, Optional
 
 import boto3
 import shapely.geometry
@@ -155,15 +155,15 @@
 
         if not self.job_arn or not self.job_id or not self.outputs:
             logger.error("Missing job arn, job id, or outputs properties in ImageRequest")
             return False
 
         num_feature_detection_options = len(self.get_feature_distillation_option())
         if num_feature_detection_options > 1:
-            logger.error("{} feature distillation options in ImageRequest".format(num_feature_detection_options))
+            logger.error(f"{num_feature_detection_options} feature distillation options in ImageRequest")
             return False
 
         return True
 
     def get_shared_values(self) -> Dict[str, Any]:
         """
         Returns a formatted dict that contains the properties of an image
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/api/region_request.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/region_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from typing import Any, Dict
 
 from aws.osml.model_runner.common import ImageCompression, ImageDimensions, ImageFormats, ImageRegion
 
 from .inference import ModelInvokeMode
 from .request_utils import shared_properties_are_valid
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/api/request_utils.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/request_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from aws.osml.model_runner.common import VALID_IMAGE_COMPRESSION, VALID_IMAGE_FORMATS
 
 from .inference import VALID_MODEL_HOSTING_OPTIONS
 
 
 def shared_properties_are_valid(request) -> bool:
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/api/sink.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/api/sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from enum import auto
 
 from aws.osml.model_runner.common import AutoStringEnum
 
 
 class SinkMode(str, AutoStringEnum):
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/app.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import ast
 import functools
 import json
 import logging
 import math
 from dataclasses import asdict
@@ -174,16 +174,17 @@
                                 image_id=region_request.image_id,
                                 job_id=region_request.job_id,
                                 region_pixel_bounds=region_pixel_bounds,
                                 region_id=region_request.region_id,
                             )
                             self.region_request_table.start_region_request(region_request_item)
                             logging.info(
-                                "Adding region request: imageid: {0} - regionid: {1}".format(
-                                    region_request_item.image_id, region_request_item.region_id
+                                (
+                                    f"Adding region request: image id: {region_request_item.image_id} - "
+                                    f"region id: {region_request_item.region_id}"
                                 )
                             )
 
                         # Process our region request
                         image_request_item = self.process_region_request(
                             region_request, region_request_item, raster_dataset, sensor_model
                         )
@@ -199,15 +200,15 @@
                         self.region_request_queue.reset_request(receipt_handle, visibility_timeout=0)
                     except SelfThrottledRegionException:
                         self.region_request_queue.reset_request(
                             receipt_handle,
                             visibility_timeout=int(ServiceConfig.throttling_retry_timeout),
                         )
                     except Exception as err:
-                        logger.error("There was a problem processing the region request: {}".format(err))
+                        logger.error(f"There was a problem processing the region request: {err}")
                         self.region_request_queue.finish_request(receipt_handle)
                 else:
                     logger.debug("Checking work queue for images to process ...")
                     (receipt_handle, image_request_message) = next(self.image_requests_iter)
 
                     # If we found a request on the queue
                     if image_request_message is not None:
@@ -215,27 +216,27 @@
                         try:
                             # Parse the message into a working ImageRequest
                             image_request = ImageRequest.from_external_message(image_request_message)
                             ThreadingLocalContextFilter.set_context(image_request.__dict__)
 
                             # Check that our image request looks good
                             if not image_request.is_valid():
-                                error = "Invalid image request: {}".format(image_request_message)
+                                error = f"Invalid image request: {image_request_message}"
                                 logger.exception(error)
                                 raise InvalidImageRequestException(error)
 
                             # Process the request
                             self.process_image_request(image_request)
 
                             # Update the queue
                             self.image_request_queue.finish_request(receipt_handle)
                         except RetryableJobException:
                             self.image_request_queue.reset_request(receipt_handle, visibility_timeout=0)
                         except Exception as err:
-                            logger.error("There was a problem processing the image request: {}".format(err))
+                            logger.error(f"There was a problem processing the image request: {err}")
                             min_image_id = image_request.image_id if image_request and image_request.image_id else ""
                             min_job_id = image_request.job_id if image_request and image_request.job_id else ""
                             min_job_arn = image_request.job_arn if image_request and image_request.job_arn else ""
                             minimal_job_item = JobItem(
                                 image_id=min_image_id,
                                 job_id=min_job_id,
                                 job_arn=min_job_arn,
@@ -265,15 +266,15 @@
                 max_regions = self.endpoint_utils.calculate_max_regions(
                     image_request.model_name, image_request.model_invocation_role
                 )
                 # Add entry to the endpoint statistics table
                 self.endpoint_statistics_table.upsert_endpoint(image_request.model_name, max_regions)
 
             # Update the image status to started and include relevant image meta-data
-            logger.info("Starting processing of {}".format(image_request.image_url))
+            logger.info(f"Starting processing of {image_request.image_url}")
             image_request_item = JobItem(
                 image_id=image_request.image_id,
                 job_id=image_request.job_id,
                 job_arn=image_request.job_arn,
                 tile_size=str(image_request.tile_size),
                 tile_overlap=str(image_request.tile_overlap),
                 model_name=image_request.model_name,
@@ -299,17 +300,15 @@
             # Load the relevant image meta data into memory
             image_extension, raster_dataset, sensor_model, all_regions = self.load_image_request(
                 image_request_item, image_request.roi
             )
 
             if sensor_model is None:
                 logging.warning(
-                    "Dataset {} did not have a geo transform. Results are not geo-referenced.".format(
-                        image_request_item.image_id
-                    )
+                    f"Dataset {image_request_item.image_id} did not have a geo transform. Results are not geo-referenced."
                 )
 
             # If we got valid outputs
             if raster_dataset and all_regions and image_extension:
                 image_request_item.region_count = Decimal(len(all_regions))
                 image_request_item.width = Decimal(raster_dataset.RasterXSize)
                 image_request_item.height = Decimal(raster_dataset.RasterYSize)
@@ -374,15 +373,15 @@
         :param sensor_model: Optional[SensorModel] = the sensor model for this raster dataset
 
         :return None
         """
         # Set aside the first region
         first_region = all_regions.pop(0)
         for region in all_regions:
-            logger.info("Queueing region: {}".format(region))
+            logger.info(f"Queueing region: {region}")
 
             region_pixel_bounds = f"{region[0]}{region[1]}"
             region_id = f"{region_pixel_bounds}-{token_hex(16)}"
             region_request = RegionRequest(
                 image_request.get_shared_values(), region_bounds=region, region_id=region_id, image_extension=image_extension
             )
 
@@ -391,24 +390,25 @@
                 image_id=image_request.image_id,
                 job_id=image_request.job_id,
                 region_pixel_bounds=region_pixel_bounds,
                 region_id=region_id,
             )
             self.region_request_table.start_region_request(region_request_item)
             logging.info(
-                "Adding region request: imageid: {0} - regionid: {1}".format(
-                    region_request_item.image_id, region_request_item.region_id
+                (
+                    f"Adding region request: image id: {region_request_item.image_id} - "
+                    f"region id: {region_request_item.region_id}"
                 )
             )
 
             # Send the attributes of the region request as the message.
             self.region_request_queue.send_request(region_request.__dict__)
 
         # Go ahead and process the first region
-        logger.info("Processing first region {}: {}".format(0, first_region))
+        logger.info(f"Processing first region {0}: {first_region}")
 
         region_pixel_bounds = f"{first_region[0]}{first_region[1]}"
         region_id = f"{region_pixel_bounds}-{token_hex(16)}"
         first_region_request = RegionRequest(
             image_request.get_shared_values(),
             region_bounds=first_region,
             region_id=region_id,
@@ -420,17 +420,15 @@
             image_id=image_request.image_id,
             job_id=image_request.job_id,
             region_pixel_bounds=region_pixel_bounds,
             region_id=region_id,
         )
         self.region_request_table.start_region_request(region_request_item)
         logging.info(
-            "Adding region request: imageid: {0} - regionid: {1}".format(
-                region_request_item.image_id, region_request_item.region_id
-            )
+            f"Adding region request: imageid: {region_request_item.image_id} - regionid: {region_request_item.region_id}"
         )
 
         # Processes our region request and return the updated item
         image_request_item = self.process_region_request(
             first_region_request, region_request_item, raster_dataset, sensor_model
         )
 
@@ -461,15 +459,15 @@
 
         :return: None
         """
         if isinstance(metrics, MetricsLogger):
             metrics.set_dimensions()
 
         if not region_request.is_valid():
-            logger.error("Invalid Region Request! {}".format(region_request.__dict__))
+            logger.error(f"Invalid Region Request! {region_request.__dict__}")
             raise ValueError("Invalid Region Request")
 
         if isinstance(metrics, MetricsLogger):
             image_format = str(raster_dataset.GetDriver().ShortName).upper()
             metrics.put_dimensions(
                 {
                     MetricLabels.OPERATION_DIMENSION: MetricLabels.REGION_PROCESSING_OPERATION,
@@ -485,23 +483,23 @@
             # Add entry to the endpoint statistics table
             self.endpoint_statistics_table.upsert_endpoint(region_request.model_name, max_regions)
             in_progress = self.endpoint_statistics_table.current_in_progress_regions(region_request.model_name)
 
             if in_progress >= max_regions:
                 if isinstance(metrics, MetricsLogger):
                     metrics.put_metric(MetricLabels.THROTTLES, 1, str(Unit.COUNT.value))
-                logger.info("Throttling region request. (Max: {} In-progress: {}".format(max_regions, in_progress))
+                logger.info(f"Throttling region request. (Max: {max_regions} In-progress: {in_progress}")
                 raise SelfThrottledRegionException
 
             # Increment the endpoint region counter
             self.endpoint_statistics_table.increment_region_count(region_request.model_name)
 
         try:
             with Timer(
-                task_str="Processing region {} {}".format(region_request.image_url, region_request.region_bounds),
+                task_str=f"Processing region {region_request.image_url} {region_request.region_bounds}",
                 metric_name=MetricLabels.DURATION,
                 logger=logger,
                 metrics_logger=metrics,
             ):
                 # Set up our threaded tile worker pool
                 tile_queue, tile_workers = setup_tile_workers(region_request, sensor_model, self.elevation_model)
 
@@ -527,17 +525,18 @@
                 # TODO: Consider adding the +1 invocation to timer
                 metrics.put_metric(MetricLabels.INVOCATIONS, 1, str(Unit.COUNT.value))
 
             # Return the updated item
             return image_request_item
 
         except Exception as err:
-            logger.error("Failed to process image region: {}".format(err))
+            failed_msg = f"Failed to process image region: {err}"
+            logger.error(failed_msg)
             # update the table to take in that exception
-            region_request_item.message = "Failed to process image region: {0}".format(err)
+            region_request_item.message = failed_msg
             return self.fail_region_request(region_request_item, metrics)
 
         finally:
             # Decrement the endpoint region counter
             if ServiceConfig.self_throttling:
                 self.endpoint_statistics_table.decrement_region_count(region_request.model_name)
 
@@ -620,15 +619,15 @@
         Updates failed metrics and update the status monitor accordingly
 
         :param image_request_item: JobItem = the image request that failed.
         :param err: Exception = the exception that caused the failure
 
         :return: None
         """
-        logger.exception("Failed to start image processing!: {}".format(err))
+        logger.exception(f"Failed to start image processing!: {err}")
         self.status_monitor.process_event(image_request_item, ImageRequestStatus.FAILED, str(err))
 
     def complete_image_request(self, region_request: RegionRequest, image_format: str) -> None:
         """
         Runs after every region has completed processing to check if that was the last region and run required
         completion logic for the associated ImageRequest.
 
@@ -947,15 +946,15 @@
             tracking_output_sinks = {
                 "S3": False,
                 "Kinesis": False,
             }  # format: job_id = {"s3": true, "kinesis": true}
 
             # Ensure we have outputs defined for where to dump our features
             if image_request_item.outputs:
-                logging.info("Writing aggregate feature for job '{}'".format(image_request_item.job_id))
+                logging.info(f"Writing aggregate feature for job '{image_request_item.job_id}'")
                 for sink in SinkFactory.outputs_to_sinks(json.loads(image_request_item.outputs)):
                     if sink.mode == SinkMode.AGGREGATE and image_request_item.job_id:
                         is_write_output_succeeded = sink.write(image_request_item.job_id, features)
                         tracking_output_sinks[sink.name()] = is_write_output_succeeded
 
                 # Log them let them know if both written to both outputs (S3 and Kinesis) or one in another
                 # If both couldn't write to either stream because both were down, return False. Otherwise True
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/app_config.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/app_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import os
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional
 
 from botocore.config import Config
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/common/__init__.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 # Telling flake8 to not flag errors in this file. It is normal that these classes are imported but not used in an
 # __init__.py file.
 # flake8: noqa
 
 from .auto_string_enum import AutoStringEnum
 from .credentials_utils import get_credentials_for_assumed_role
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/common/credentials_utils.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/credentials_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from typing import Dict
 
 import boto3
 
 from aws.osml.model_runner.app_config import BotoConfig
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/common/endpoint_utils.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/endpoint_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import math
 import operator
 from typing import Optional
 
 import boto3
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/common/feature_utils.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/feature_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from typing import Optional, Tuple
 
 import geojson
 
 from aws.osml.features import ImagedFeaturePropertyAccessor
 
 property_accessor = ImagedFeaturePropertyAccessor()
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/common/log_context.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/log_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 import threading
 from typing import List, Optional
 
 _LOG_CONTEXT = threading.local()
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/common/mr_post_processing.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/mr_post_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from abc import ABC, ABCMeta, abstractmethod
 from dataclasses import dataclass, field
 from enum import Enum, EnumMeta, auto
 from typing import Dict, List
 
 from .auto_string_enum import AutoStringEnum
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/common/security_classification.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/security_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from dataclasses import dataclass, field
 from enum import auto
 from inspect import signature
 from typing import Any, Dict, List, Optional, Tuple
 
 from osgeo import gdal
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/common/timer.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import time
 from typing import Optional
 
 from aws_embedded_metrics.logger.metrics_logger import MetricsLogger
 from aws_embedded_metrics.unit import Unit
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/common/typing.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/common/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from enum import Enum, auto
 from typing import Tuple
 
 from aws.osml.model_runner.common import AutoStringEnum
 
 # Pixel coordinate (row, column)
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/database/__init__.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 # Telling flake8 to not flag errors in this file. It is normal that these classes are imported but not used in an
 # __init__.py file.
 # flake8: noqa
 
 from .ddb_helper import DDBHelper, DDBItem, DDBKey
 from .endpoint_statistics_table import EndpointStatisticsTable
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/database/ddb_helper.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/ddb_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import random
 import time
 from dataclasses import asdict, dataclass, field, fields
 from typing import Any, Dict, List, Optional, Tuple
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/database/endpoint_statistics_table.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/endpoint_statistics_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 from dataclasses import dataclass
 from decimal import Decimal
 
 from boto3.dynamodb.conditions import Attr
 from botocore.exceptions import ClientError
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/database/exceptions.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 
 # Database Exceptions
 class AddFeaturesException(Exception):
     pass
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/database/feature_table.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/feature_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import random
 import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from dataclasses import dataclass
 from secrets import token_hex
@@ -261,10 +261,8 @@
         min_y_offset = int(bbox[1]) % stride_y
 
         if min_x_offset < self.overlap[0] and min_x_index > 0:
             min_x_index -= 1
         if min_y_offset < self.overlap[1] and min_y_index > 0:
             min_y_index -= 1
 
-        return "{}-region-{}:{}:{}:{}".format(
-            feature["properties"]["image_id"], min_x_index, max_x_index, min_y_index, max_y_index
-        )
+        return f"{feature['properties']['image_id']}-region-{min_x_index}:{max_x_index}:{min_y_index}:{max_y_index}"
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/database/job_table.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/job_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import time
 from dataclasses import dataclass
 from decimal import Decimal
 from typing import Optional
 
 from dacite import from_dict
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/database/region_request_table.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/database/region_request_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import time
 from dataclasses import dataclass
 from decimal import Decimal
 from typing import Optional
 
@@ -143,10 +143,10 @@
         """
         try:
             # Retrieve job item from our table and set to expected RegionRequestItem class
             return from_dict(
                 RegionRequestItem,
                 self.get_ddb_item(RegionRequestItem(region_id=region_id, image_id=image_id)),
             )
-        except Exception as e:
-            logger.warning(GetRegionRequestItemException("Failed to get RegionRequestItem! {0}".format(e)))
+        except Exception as err:
+            logger.warning(GetRegionRequestItemException(f"Failed to get RegionRequestItem! {err}"))
             return None
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/exceptions.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 
 # ModelRunner Exceptions
 class RetryableJobException(Exception):
     pass
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/detector.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import abc
 from io import BufferedReader
 
 from aws_embedded_metrics.logger.metrics_logger import MetricsLogger
 from aws_embedded_metrics.metric_scope import metric_scope
 from geojson import FeatureCollection
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/endpoint_builder.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/endpoint_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from abc import ABC, abstractmethod
 from typing import Optional
 
 from .detector import Detector
 
 
 class FeatureEndpointBuilder(ABC):
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/endpoint_factory.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/endpoint_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 from typing import Dict, Optional
 
 from aws.osml.model_runner.api import ModelInvokeMode
 
 from .detector import Detector
 from .http_detector import HTTPDetectorBuilder
 from .sm_detector import SMDetectorBuilder
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/feature_selection.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/feature_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from collections import OrderedDict
 from typing import List, Tuple
 
 from ensemble_boxes import nms, soft_nms
 from geojson import Feature
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/feature_utils.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/feature_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 from datetime import datetime
 from io import BufferedReader
 from json import dumps
 from math import radians
 from secrets import token_hex
@@ -250,12 +250,12 @@
                         "classification": source_classification_str,
                     }
                 ]
             }
 
             return source_property
         except Exception as err:
-            logging.warning("Source metadata not available for {} image extension! {}".format(image_extension, err))
+            logging.warning(f"Source metadata not available for {image_extension} image extension! {err}")
             return None
     else:
-        logging.warning("Source metadata not available for {} image extension!".format(image_extension))
+        logging.warning(f"Source metadata not available for {image_extension} image extension!")
         return None
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/http_detector.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/http_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
+
 import logging
 from io import BufferedReader
 from json import JSONDecodeError
 from typing import Optional
 
 import geojson
 import urllib3
@@ -104,15 +106,15 @@
         Query the established endpoint mode to find features based on a payload
 
         :param payload: BufferedReader object that holds the data that will be sent to the feature generator
         :param metrics: Metrics logger object to capture the log data on the system
 
         :return: GeoJSON FeatureCollection containing the center point of a tile
         """
-        logger.info("Invoking Model: {}".format(self.name))
+        logger.info(f"Invoking Model: {self.name}")
         if isinstance(metrics, MetricsLogger):
             metrics.set_dimensions()
             metrics.put_dimensions(
                 {
                     MetricLabels.OPERATION_DIMENSION: MetricLabels.MODEL_INVOCATION_OPERATION,
                     MetricLabels.MODEL_NAME_DIMENSION: self.name,
                 }
@@ -145,29 +147,30 @@
                     if isinstance(metrics, MetricsLogger):
                         metrics.put_metric(MetricLabels.RETRIES, retry_count, str(Unit.COUNT.value))
                     return geojson.loads(response.data.decode("utf-8"))
         except RetryError as err:
             self.error_count += 1
             if isinstance(metrics, MetricsLogger):
                 metrics.put_metric(MetricLabels.ERRORS, 1, str(Unit.COUNT.value))
-            logger.error("Retry failed - failed due to {}".format(err))
+            logger.error(f"Retry failed - failed due to {err}")
             logger.exception(err)
         except MaxRetryError as err:
             self.error_count += 1
             if isinstance(metrics, MetricsLogger):
                 metrics.put_metric(MetricLabels.ERRORS, 1, str(Unit.COUNT.value))
-            logger.error("Max retries reached - failed due to {}".format(err.reason))
+            logger.error(f"Max retries reached - failed due to {err.reason}")
             logger.exception(err)
         except JSONDecodeError as err:
             self.error_count += 1
             if isinstance(metrics, MetricsLogger):
                 metrics.put_metric(MetricLabels.ERRORS, 1, str(Unit.COUNT.value))
             logger.error(
-                "Unable to decode response from model. URL: {}, Status: {}, Headers: {}, Response: {}".format(
-                    self.endpoint, response.status, response.info(), response.data
+                (
+                    f"Unable to decode response from model. URL: {self.endpoint}, Status: {response.status}, "
+                    f"Headers: {response.info()}, Response: {response.data}"
                 )
             )
             logger.exception(err)
 
         # Return an empty feature collection if the process errored out
         return FeatureCollection([])
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/inference/sm_detector.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/inference/sm_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
-
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 from io import BufferedReader
 from json import JSONDecodeError
 from typing import Dict, Optional
 
 import boto3
@@ -66,15 +64,15 @@
 
         :param payload: BufferedReader = the BufferedReader object that holds the
                                     data that will be sent to the feature generator
         :param metrics: MetricsLogger = the metrics logger object to capture the log data on the system
 
         :return: FeatureCollection = a feature collection containing the center point of a tile
         """
-        logger.info("Invoking Model: {}".format(self.endpoint))
+        logger.info(f"Invoking Model: {self.endpoint}")
         if isinstance(metrics, MetricsLogger):
             metrics.set_dimensions()
             metrics.put_dimensions(
                 {
                     MetricLabels.OPERATION_DIMENSION: MetricLabels.MODEL_INVOCATION_OPERATION,
                     MetricLabels.MODEL_NAME_DIMENSION: self.endpoint,
                 }
@@ -111,17 +109,15 @@
         except ClientError as ce:
             self.error_count += 1
             error_code = ce.response.get("Error", {}).get("Code")
             http_status_code = ce.response.get("ResponseMetadata", {}).get("HTTPStatusCode")
             if isinstance(metrics, MetricsLogger):
                 metrics.put_metric(MetricLabels.ERRORS, 1, str(Unit.COUNT.value))
             logger.error(
-                "Unable to get detections from model - HTTP Status Code: {}, Error Code: {}".format(
-                    http_status_code, error_code
-                )
+                f"Unable to get detections from model - HTTP Status Code: {http_status_code}, Error Code: {error_code}"
             )
             logger.exception(ce)
         # If there was an error parsing the models output
         except JSONDecodeError as de:
             self.error_count += 1
             if isinstance(metrics, MetricsLogger):
                 metrics.put_metric(MetricLabels.ERRORS, 1, str(Unit.COUNT.value))
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/queue/request_queue.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/queue/request_queue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import json
 import logging
 from typing import Dict
 
 import boto3
-import botocore
+from botocore.exceptions import ClientError
 
 from aws.osml.model_runner.app_config import BotoConfig
 
 
 class RequestQueue:
     def __init__(
         self,
@@ -29,49 +29,49 @@
                     QueueUrl=self.queue_url,
                     AttributeNames=["All"],
                     MessageAttributeNames=["All"],
                     MaxNumberOfMessages=self.num_messages,
                     WaitTimeSeconds=self.wait_seconds,
                 )
 
-                logging.debug("Dequeued processing request {}".format(str(queue_response)))
+                logging.debug(f"Dequeued processing request {queue_response}")
 
                 if "Messages" in queue_response:
                     for message in queue_response["Messages"]:
                         message_body = message["Body"]
-                        logging.debug("Message Body {}".format(message_body))
+                        logging.debug(f"Message Body {message_body}")
 
                         try:
                             work_request = json.loads(message_body)
 
                             yield message["ReceiptHandle"], work_request
 
                         except json.JSONDecodeError:
-                            logging.warning("Skipping message that is not valid JSON: {}".format(message_body))
+                            logging.warning(f"Skipping message that is not valid JSON: {message_body}")
                             yield None, None
                 else:
                     yield None, None
 
-            except botocore.exceptions.ClientError as error:
-                logging.error("Unable to retrieve message from queue: {}".format(error))
+            except ClientError as err:
+                logging.error(f"Unable to retrieve message from queue: {err}")
                 yield None, None
 
     def finish_request(self, receipt_handle: str) -> None:
         """
         Delete the message from the SQS
 
         :param receipt_handle: str = unique identifier of a message
 
         :return: None
         """
         try:
             # Remove the message from the queue since it has been successfully processed
             self.sqs_client.delete_message(QueueUrl=self.queue_url, ReceiptHandle=receipt_handle)
-        except botocore.exceptions.ClientError as error:
-            logging.error("Unable to remove message from queue: {}".format(error))
+        except ClientError as err:
+            logging.error(f"Unable to remove message from queue: {err}")
 
     def reset_request(self, receipt_handle: str, visibility_timeout: int = 0) -> None:
         """
         Reset the message in SQS
 
         :param receipt_handle: str = unique identifier of a message
         :param visibility_timeout: int = period of time which SQS prevents other consumers from receiving
@@ -81,22 +81,22 @@
         """
         try:
             self.sqs_client.change_message_visibility(
                 QueueUrl=self.queue_url,
                 ReceiptHandle=receipt_handle,
                 VisibilityTimeout=visibility_timeout,
             )
-        except botocore.exceptions.ClientError as error:
-            logging.error("Unable to reset message visibility: {}".format(error))
+        except ClientError as err:
+            logging.error(f"Unable to reset message visibility: {err}")
 
     def send_request(self, request: Dict) -> None:
         """
         Send the message via SQS
 
         :param request: Dict = unique identifier of a message
 
         :return: None
         """
         try:
             self.sqs_client.send_message(QueueUrl=self.queue_url, MessageBody=json.dumps(request))
-        except botocore.exceptions.ClientError as error:
-            logging.error("Unable to send message visibility: {}".format(error))
+        except ClientError as err:
+            logging.error(f"Unable to send message visibility: {err}")
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/kinesis_sink.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/kinesis_sink.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import sys
 from typing import List, Optional
 
 import boto3
 import geojson
@@ -73,20 +73,18 @@
 
                     pending_features.append(feature)
                     pending_features_size += feature_size
 
             # Flush any remaining features
             if pending_features:
                 self._flush_stream(job_id, pending_features)
-            logger.info("Wrote {} features for job '{}' to Kinesis Stream '{}'".format(len(features), job_id, self.stream))
+            logger.info(f"Wrote {len(features)} features for job '{job_id}' to Kinesis Stream '{self.stream}'")
             return True
         else:
-            logger.error(
-                "Cannot write {} features for job '{}' to Kinesis Stream '{}'".format(len(features), job_id, self.stream)
-            )
+            logger.error(f"Cannot write {len(features)} features for job '{job_id}' to Kinesis Stream '{self.stream}'")
             return False
 
     def validate_kinesis_stream(self) -> bool:
         """
         Ensure output Kinesis stream exists/can be written to
 
         :return: bool = True if kinesis stream exist and can be read/written to it
@@ -96,18 +94,16 @@
 
             # check if Stream is ACTIVE
             stream_status = describe_stream_response["StreamDescription"]["StreamStatus"]
             if stream_status == "ACTIVE" or stream_status == "UPDATING":
                 # reason to include UPDATING is that Kinesis Stream functions during these operations
                 return True
             else:
-                logging.error(
-                    "{} current status is: {}. It is not in ACTIVE or UPDATING state.".format(self.stream, stream_status)
-                )
+                logging.error(f"{self.stream} current status is: {stream_status}. It is not in ACTIVE or UPDATING state.")
                 return False
-        except Exception as e:
-            logger.error("Failed to fetch Kinesis stream - {}. {}".format(self.stream, e))
+        except Exception as err:
+            logger.error(f"Failed to fetch Kinesis stream - {self.stream}. {err}")
             return False
 
     @staticmethod
     def name() -> str:
         return str(SinkType.KINESIS.value)
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/s3_sink.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/s3_sink.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import os
 from typing import List, Optional
 
 import boto3
 import geojson
@@ -59,17 +59,15 @@
             # as a GeoJSON output.
             self.s3_client.put_object(
                 Body=str(geojson.dumps(features_collection)),
                 Bucket=self.bucket,
                 Key=object_key,
                 ACL="bucket-owner-full-control",
             )
-            logger.info(
-                "Wrote aggregate feature collection for Image '{}' to s3://{}/{}".format(image_id, self.bucket, object_key)
-            )
+            logger.info(f"Wrote aggregate feature collection for Image '{image_id}' to s3://{self.bucket}/{object_key}")
             return True
         else:
             return False
 
     def validate_s3_bucket(self) -> bool:
         """
         Check if Output S3 bucket exists and can be read/written to it
@@ -77,16 +75,16 @@
         :return: bool = True if bucket exist and can be read/written to it
         """
         try:
             self.s3_client.head_bucket(Bucket=self.bucket)
             return True
         except ClientError as err:
             if err.response["Error"]["Code"] == "404":  # Does not exist
-                logging.error("This S3 Bucket({}) does not exist".format(self.bucket))
+                logging.error(f"This S3 Bucket({self.bucket}) does not exist")
             elif err.response["Error"]["Code"] == "403":  # Forbidden access
-                logging.error("Do not have permission to read/write this S3 Bucket({})".format(self.bucket))
-            logging.error("Cannot read/write S3 Bucket ({})".format(self.bucket))
+                logging.error(f"Do not have permission to read/write this S3 Bucket({self.bucket})")
+            logging.error(f"Cannot read/write S3 Bucket ({self.bucket})")
             return False
 
     @staticmethod
     def name() -> str:
         return str(SinkType.S3.value)
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/sink.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import abc
 from typing import List
 
 from geojson import Feature
 
 from aws.osml.model_runner.api import SinkMode
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/sink/sink_factory.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/sink/sink_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 from typing import Any, Dict, List
 
 from aws.osml.model_runner.api import InvalidImageRequestException
 from aws.osml.model_runner.sink import KinesisSink, S3Sink, Sink
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/status/image_request_status.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/status/image_request_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from dataclasses import dataclass, field, fields
 from decimal import Decimal
 from enum import Enum
 from typing import Dict, List, Optional
 
 from shapely.geometry.base import BaseGeometry
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/status/sns_helper.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/status/sns_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 from typing import Any, Dict, Optional, Union
 
 import boto3
 
 from aws.osml.model_runner.app_config import BotoConfig
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/status/status_monitor.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/status/status_monitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 
 from aws.osml.model_runner.app_config import ServiceConfig
 from aws.osml.model_runner.common import ImageRequestStatus
 from aws.osml.model_runner.database.job_table import JobItem
 
@@ -52,19 +52,17 @@
 
                 status_message = f"StatusMonitor update: {status} {image_request_item.job_id}: {message}"
                 self.image_status_sns.publish_message(
                     status_message,
                     sns_message_attributes.asdict_str_values(),
                 )
             except Exception as err:
-                raise StatusMonitorException(
-                    "StatusMonitor failed: {} {}: {}".format(status, image_request_item.job_id, err)
-                )
+                raise StatusMonitorException(f"StatusMonitor failed: {status} {image_request_item.job_id}: {err}")
         else:
-            raise StatusMonitorException("StatusMonitor failed: {} {}".format(status, image_request_item.job_id))
+            raise StatusMonitorException(f"StatusMonitor failed: {status} {image_request_item.job_id}")
 
     @staticmethod
     def get_image_request_status(image_request_item: JobItem) -> ImageRequestStatus:
         """
         Produce a image request status from a given image request
 
         :param image_request_item: JobItem = the image request item
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/tile_worker/tile_worker.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/tile_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import asyncio
 import logging
 from datetime import datetime, timezone
 from queue import Queue
 from threading import Thread
 from typing import Dict, List, Optional
@@ -43,16 +43,17 @@
         while True:
             image_info: Dict = self.in_queue.get()
             ThreadingLocalContextFilter.set_context(image_info)
 
             if image_info is None:
                 logging.info("All images processed. Stopping tile worker.")
                 logging.info(
-                    "Feature Detector Stats: {} requests with {} errors".format(
-                        self.feature_detector.request_count, self.feature_detector.error_count
+                    (
+                        f"Feature Detector Stats: {self.feature_detector.request_count} requests "
+                        f"with {self.feature_detector.error_count} errors"
                     )
                 )
                 break
 
             try:
                 self.process_tile(image_info)
             finally:
@@ -135,15 +136,15 @@
             if isinstance(metrics, MetricsLogger):
                 metrics.put_metric(MetricLabels.INVOCATIONS, 1, str(Unit.COUNT.value))
 
             features = []
             ulx = image_info["region"][0][1]
             uly = image_info["region"][0][0]
             if isinstance(feature_collection, dict) and "features" in feature_collection:
-                logging.info("SM Model returned {} features".format(len(feature_collection["features"])))
+                logging.info(f"SM Model returned {len(feature_collection['features'])} features")
                 for feature in feature_collection["features"]:
                     # Check to see if there is a bbox defined in image coordinates. If so, update it to
                     # use full image coordinates and store the updated value in the feature properties.
                     tiled_image_bbox = self.property_accessor.get_image_bbox(feature)
                     if tiled_image_bbox is not None:
                         full_image_bbox = translate(tiled_image_bbox, xoff=ulx, yoff=uly)
                         self.property_accessor.set_image_bbox(feature, full_image_bbox)
@@ -172,21 +173,21 @@
 
                     # This conversion only happens here so the rest of the system can depend on a standard
                     # set of properties. Eventually this call should be removed once the old properties are
                     # no longer used by CV models.
                     TileWorker.convert_deprecated_feature_properties(feature)
 
                     features.append(feature)
-            logging.info("# Features Created: {}".format(len(features)))
+            logging.info(f"# Features Created: {len(features)}")
             if len(features) > 0:
                 if self.geolocator is not None:
                     # Create a geometry for each feature in the result. The geographic coordinates of these
                     # features are computed using the sensor model provided in the image metadata
                     self.geolocator.geolocate_features(features)
-                    logging.info("Created Geographic Coordinates for {} features".format(len(features)))
+                    logging.info(f"Created Geographic Coordinates for {len(features)} features")
 
         return features
 
     @staticmethod
     def convert_deprecated_feature_properties(feature: geojson.Feature) -> None:
         """
         This function converts the legacy properties produced by CV models into the feature properties used
```

### Comparing `osml-model-runner-2.0.0/src/aws/osml/model_runner/tile_worker/tile_worker_utils.py` & `osml-model-runner-2.1.0/src/aws/osml/model_runner/tile_worker/tile_worker_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 import logging
 import tempfile
 from pathlib import Path
 from queue import Queue
 from secrets import token_hex
 from typing import List, Optional, Tuple
@@ -71,19 +71,19 @@
             if sensor_model is not None:
                 geolocator = Geolocator(ImagedFeaturePropertyAccessor(), sensor_model, elevation_model=elevation_model)
 
             worker = TileWorker(tile_queue, feature_detector, geolocator, feature_table)
             worker.start()
             tile_workers.append(worker)
 
-        logger.info("Setup pool of {} tile workers".format(len(tile_workers)))
+        logger.info(f"Setup pool of {len(tile_workers)} tile workers")
 
         return tile_queue, tile_workers
     except Exception as err:
-        logger.exception("Failed to setup tile workers!: {}".format(err))
+        logger.exception(f"Failed to setup tile workers!: {err}")
         raise SetupTileWorkersException("Failed to setup tile workers!") from err
 
 
 def process_tiles(
     region_request: RegionRequest,
     tile_queue: Queue,
     tile_workers: List[TileWorker],
@@ -130,21 +130,17 @@
                 # image region request at the start of this function would have failed
                 for tile_bounds in generate_crops(
                     region_request.region_bounds,  # type: ignore[arg-type]
                     region_request.tile_size,
                     region_request.tile_overlap,
                 ):
                     # Create a temp file name for the encoded region
-                    region_image_filename = "{}-region-{}-{}-{}-{}.{}".format(
-                        token_hex(16),
-                        tile_bounds[0][0],
-                        tile_bounds[0][1],
-                        tile_bounds[1][0],
-                        tile_bounds[1][1],
-                        region_request.tile_format,
+                    region_image_filename = (
+                        f"{token_hex(16)}-region-{tile_bounds[0][0]}-{tile_bounds[0][1]}-"
+                        f"{tile_bounds[1][0]}-{tile_bounds[1][1]}.{region_request.tile_format}"
                     )
 
                     # Set a path for the tmp image
                     tmp_image_path = Path(tmp, region_image_filename)
 
                     # Generate an encoded tile of the requested image region
                     absolute_tile_path = _create_tile(gdal_tile_factory, tile_bounds, tmp_image_path)
@@ -175,20 +171,21 @@
                 # Wait for all the workers to finish gracefully before we clean up the temp directory
                 tile_error_count = 0
                 for worker in tile_workers:
                     worker.join()
                     tile_error_count += worker.feature_detector.error_count
 
         logger.info(
-            "Model Runner Stats Processed {} image tiles for region {}. {} tile errors.".format(
-                total_tile_count, region_request.region_bounds, tile_error_count
+            (
+                f"Model Runner Stats Processed {total_tile_count} image tiles for "
+                f"region {region_request.region_bounds}. {tile_error_count} tile errors."
             )
         )
     except Exception as err:
-        logger.exception("File processing tiles: {}", err)
+        logger.exception(f"File processing tiles: {err}")
         raise ProcessTilesException("Failed to process tiles!") from err
 
     return total_tile_count, tile_error_count
 
 
 @metric_scope
 def _create_tile(gdal_tile_factory, tile_bounds, tmp_image_path, metrics: MetricsLogger = None) -> Optional[str]:
@@ -209,15 +206,15 @@
                 MetricLabels.INPUT_FORMAT_DIMENSION: str(gdal_tile_factory.raster_dataset.GetDriver().ShortName).upper(),
             }
         )
 
     # Use GDAL to create an encoded tile of the image region
     absolute_tile_path = tmp_image_path.absolute()
     with Timer(
-        task_str="Creating image tile: {}".format(absolute_tile_path),
+        task_str=f"Creating image tile: {absolute_tile_path}",
         metric_name=MetricLabels.DURATION,
         logger=logger,
         metrics_logger=metrics,
     ):
         if isinstance(metrics, MetricsLogger):
             metrics.put_metric(MetricLabels.INVOCATIONS, 1, str(Unit.COUNT.value))
```

### Comparing `osml-model-runner-2.0.0/src/osml_model_runner.egg-info/PKG-INFO` & `osml-model-runner-2.1.0/src/osml_model_runner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osml-model-runner
-Version: 2.0.0
+Version: 2.1.0
 Summary: Application to run large scale imagery against AI/ML models
 Author: Amazon Web Services
 Author-email: aws-osml-admin@amazon.com
 License: 
         MIT No Attribution
         
         Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
@@ -116,14 +116,20 @@
 features of interest would fall on the tile boundaries and therefore be missed by the ML models because they are only
 seeing a fractional object. This application mitigates that by allowing requests to specify an overlap region size that
 should be tuned to the expected size of the objects. Each tile sent to the ML model will be cut from the full image
 overlapping the previous by the specified amount. Then the results from each tile are aggregated with the aid of a
 Non-Maximal Suppression algorithm used to eliminate duplicates in cases where an object in an overlap region was picked
 up by multiple model runs.
 
+### Metrics and Logs
+
+As the application runs key performance metrics and detailed logging information are output to [CloudWatch](https://aws.amazon.com/cloudwatch/).
+A detailed description of what information is tracked along with example dashboards can be found in
+[METRICS_AND_DASHBOARDS.md](./METRICS_AND_DASHBOARDS.md).
+
 ### Package Layout
 
 * **/src**: This is the Python implementation of this application.
 * **/test**: Unit tests have been implemented using [pytest](https://docs.pytest.org).
 * **/bin**: The entry point for the containerized application.
 * **/scripts**: Utility scripts that are not part of the main application frequently used in development / testing.
```

### Comparing `osml-model-runner-2.0.0/src/osml_model_runner.egg-info/SOURCES.txt` & `osml-model-runner-2.1.0/src/osml_model_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osml-model-runner-2.0.0/test/test_api.py` & `osml-model-runner-2.1.0/test/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Amazon.com, Inc. or its affiliates.
+#  Copyright 2023-2024 Amazon.com, Inc. or its affiliates.
 
 from typing import Any, Dict
 from unittest import TestCase, main
 from unittest.mock import patch
 
 import boto3
 import pytest
```

### Comparing `osml-model-runner-2.0.0/test/test_app.py` & `osml-model-runner-2.1.0/test/test_app.py`

 * *Files identical despite different names*

