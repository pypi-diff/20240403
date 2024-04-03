# Comparing `tmp/fiddler-client-3.0.0.dev8.tar.gz` & `tmp/fiddler-client-3.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-3.0.0.dev8.tar", last modified: Mon Feb 26 12:59:01 2024, max compression
+gzip compressed data, was "fiddler-client-3.0.0.dev9.tar", last modified: Tue Mar  5 11:53:54 2024, max compression
```

## Comparing `fiddler-client-3.0.0.dev8.tar` & `fiddler-client-3.0.0.dev9.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.657079 fiddler-client-3.0.0.dev8/
--rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/LICENSE.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-02-26 12:59:01.657079 fiddler-client-3.0.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)    19978 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/PUBLIC.md
--rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.637079 fiddler-client-3.0.0.dev8/fiddler/
--rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/VERSION
--rw-r--r--   0 runner    (1001) runner    (1001)     3378 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      258 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/configs.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5760 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/connection.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.637079 fiddler-client-3.0.0.dev8/fiddler/constants/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      321 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/common.py
--rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/constants/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/decorators.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.647079 fiddler-client-3.0.0.dev8/fiddler/entities/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11908 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8157 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6802 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4712 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4370 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4894 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)    16499 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5514 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3757 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4595 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3059 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3798 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20232 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/entities/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/exceptions.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.647079 fiddler-client-3.0.0.dev8/fiddler/libs/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/libs/json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/libs/semver.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.647079 fiddler-client-3.0.0.dev8/fiddler/packtools/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10467 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/packtools/template_model.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.647079 fiddler-client-3.0.0.dev8/fiddler/schemas/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1222 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)      923 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5382 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/custom_features.py
--rw-r--r--   0 runner    (1001) runner    (1001)      475 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/filter_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1361 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/model_schema.py
--rw-r--r--   0 runner    (1001) runner    (1001)      642 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/model_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/model_task_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/server_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/schemas/xai_params.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.647079 fiddler-client-3.0.0.dev8/fiddler/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.647079 fiddler-client-3.0.0.dev8/fiddler/tests/apis/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11197 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7580 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8942 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4765 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4510 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_files.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4970 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_generate_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2453 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_mixin.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14512 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2441 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_model_surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6440 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28537 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      857 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/conftest.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1081 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/constants.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/test_connection.py
--rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/test_logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/test_utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/tests/utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.647079 fiddler-client-3.0.0.dev8/fiddler/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/utils/helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/utils/logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/utils/model_generator.py
--rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/utils/validations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/utils/version.py
--rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/fiddler/version.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-26 12:59:01.657079 fiddler-client-3.0.0.dev8/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-02-26 12:59:01.000000 fiddler-client-3.0.0.dev8/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     3278 2024-02-26 12:59:01.000000 fiddler-client-3.0.0.dev8/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-02-26 12:59:01.000000 fiddler-client-3.0.0.dev8/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-02-26 12:59:01.000000 fiddler-client-3.0.0.dev8/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-02-26 12:59:01.000000 fiddler-client-3.0.0.dev8/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-02-26 12:59:01.657079 fiddler-client-3.0.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-02-26 12:58:56.000000 fiddler-client-3.0.0.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/
+-rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)    19978 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/PUBLIC.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.292116 fiddler-client-3.0.0.dev9/fiddler/
+-rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/VERSION
+-rw-r--r--   0 runner    (1001) runner    (1001)     3382 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/configs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5760 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/connection.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.292116 fiddler-client-3.0.0.dev9/fiddler/constants/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      321 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/common.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/decorators.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.292116 fiddler-client-3.0.0.dev9/fiddler/entities/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11557 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8028 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6827 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4661 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4370 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    16723 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5514 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3757 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3059 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3798 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20232 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/exceptions.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.292116 fiddler-client-3.0.0.dev9/fiddler/libs/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/libs/json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/libs/semver.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/packtools/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10467 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/template_model.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/schemas/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1222 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      923 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      844 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5382 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/custom_features.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/filter_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1361 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model_schema.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      642 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model_task_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/server_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/xai_params.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/tests/apis/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11231 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7650 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8442 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_custom_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4835 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4510 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_files.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4970 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_generate_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2453 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_mixin.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14652 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2441 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8038 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_segment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6440 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28537 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      857 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/conftest.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1081 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/constants.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/model_generator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/validations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/version.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/version.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/setup.py
```

### Comparing `fiddler-client-3.0.0.dev8/LICENSE.txt` & `fiddler-client-3.0.0.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/PKG-INFO` & `fiddler-client-3.0.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.0.0.dev8
+Version: 3.0.0.dev9
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
```

### Comparing `fiddler-client-3.0.0.dev8/PUBLIC.md` & `fiddler-client-3.0.0.dev9/PUBLIC.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/README.md` & `fiddler-client-3.0.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/__init__.py` & `fiddler-client-3.0.0.dev9/fiddler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ModelTask,
 )
 from fiddler.constants.model_deployment import ArtifactType, DeploymentType  # noqa
 from fiddler.constants.xai import ExplainMethod  # noqa
 from fiddler.entities.alert_record import AlertRecord  # noqa
 from fiddler.entities.alert_rule import AlertRule  # noqa
 from fiddler.entities.baseline import Baseline  # noqa
-from fiddler.entities.custom_metric import CustomMetric, Segment  # noqa
+from fiddler.entities.custom_expression import CustomMetric, Segment  # noqa
 from fiddler.entities.dataset import Dataset  # noqa
 from fiddler.entities.file import File  # noqa
 from fiddler.entities.job import Job  # noqa
 from fiddler.entities.model import Model  # noqa
 from fiddler.entities.model_deployment import ModelDeployment  # noqa
 from fiddler.entities.project import Project  # noqa
 from fiddler.entities.webhook import Webhook  # noqa
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/connection.py` & `fiddler-client-3.0.0.dev9/fiddler/connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/constants/alert_rule.py` & `fiddler-client-3.0.0.dev9/fiddler/constants/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/constants/model.py` & `fiddler-client-3.0.0.dev9/fiddler/constants/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/decorators.py` & `fiddler-client-3.0.0.dev9/fiddler/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/alert_record.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/alert_rule.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/alert_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,45 +136,35 @@
         response = cls._client().get(url=cls._get_url(id_=id_))
         return cls._from_response(response=response)
 
     @classmethod
     @handle_api_error
     def list(  # pylint: disable=too-many-arguments
         cls,
-        model_id: UUID | None = None,
-        project_id: UUID | None = None,
+        model_id: UUID | str,
         metric_id: UUID | str | None = None,
         columns: list[str] | None = None,
-        baseline_id: UUID | None = None,
+        baseline_id: UUID | str | None = None,
         ordering: list[str] | None = None,
     ) -> Iterator[AlertRule]:
         """
         Get a list of all alert rules in the organization.
 
         :param model_id: list from the specified model
-        :param project_id: list from the specified project
         :param metric_id: list rules set on the specified metric id
         :param columns: list rules set on the specified list of columns
         :param baseline_id: list rules set on the specified baseline_id
         :param ordering: order result as per list of fields. ["-field_name"] for descending
 
         :return: paginated list of alert rules for the specified filters
         """
-        rules: list[QueryRule | QueryCondition] = []
+        rules: list[QueryRule | QueryCondition] = [
+            QueryRule(field='model_id', operator=OperatorType.EQUAL, value=model_id)
+        ]
 
-        if model_id:
-            rules.append(
-                QueryRule(field='model_id', operator=OperatorType.EQUAL, value=model_id)
-            )
-        if project_id:
-            rules.append(
-                QueryRule(
-                    field='project_id', operator=OperatorType.EQUAL, value=project_id
-                )
-            )
         if baseline_id:
             rules.append(
                 QueryRule(
                     field='baseline_id', operator=OperatorType.EQUAL, value=baseline_id
                 )
             )
         if metric_id:
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/base.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/base.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/baseline.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/baseline.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,26 +168,22 @@
 
         return cls._from_dict(data=response.json()['data']['items'][0])
 
     @classmethod
     @handle_api_error
     def list(
         cls,
-        model_id: UUID | None = None,
+        model_id: UUID | str,
         type_: str | None = None,
         environment: EnvType | None = None,
     ) -> Iterator[Baseline]:
-        """Get a list of all baselines in the organization."""
+        """Get a list of all baselines of a model."""
 
         rules: list[QueryRule | QueryCondition] = []
 
-        if model_id:
-            rules.append(
-                QueryRule(field='model_id', operator=OperatorType.EQUAL, value=model_id)
-            )
         if type_:
             rules.append(
                 QueryRule(field='type', operator=OperatorType.EQUAL, value=type_)
             )
         if environment:
             rules.append(
                 QueryRule(
@@ -196,15 +192,16 @@
                     value=environment,
                 )
             )
 
         _filter = QueryCondition(rules=rules)
         params: dict[str, Any] = {'filter': _filter.json()}
 
-        for baseline in cls._paginate(url=cls._get_url(), params=params):
+        url = f'/v3/models/{model_id}/baselines'
+        for baseline in cls._paginate(url=url, params=params):
             yield cls._from_dict(data=baseline)
 
     @handle_api_error
     def create(self) -> Baseline:
         """Create a new baseline."""
         payload = {
             'name': self.name,
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/custom_metric.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/custom_expression.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from abc import abstractmethod
 from datetime import datetime
 from typing import Any, Iterator
 from uuid import UUID
 
 from fiddler.decorators import handle_api_error
 from fiddler.entities.base import BaseEntity
-from fiddler.entities.model import Model
-from fiddler.schemas.custom_metric import (
+from fiddler.entities.model import ModelCompactMixin
+from fiddler.entities.project import ProjectCompactMixin
+from fiddler.schemas.custom_expression import (
     CustomExpressionResp,
     CustomMetricResp,
     SegmentResp,
 )
 from fiddler.schemas.filter_query import OperatorType, QueryCondition, QueryRule
 from fiddler.utils.helpers import raise_not_found
 
 
-class CustomExpression(BaseEntity):
+class CustomExpression(BaseEntity, ModelCompactMixin, ProjectCompactMixin):
     def __init__(
         self,
         name: str,
         model_id: UUID,
         definition: str,
         description: str | None = None,
     ) -> None:
@@ -33,18 +34,29 @@
 
         self.id: UUID | None = None
         self.created_at: datetime | None = None
 
         # Deserialized response object
         self._resp: CustomExpressionResp | None = None
 
+    @classmethod
+    def _get_url(cls, id_: UUID | str | None = None) -> str:
+        """Get custom expression resource/item url."""
+        url = f'/v3/{cls._get_url_path()}'
+        return url if not id_ else f'{url}/{id_}'
+
     @staticmethod
     @abstractmethod
-    def _get_url(id_: UUID | str | None = None) -> str:
-        """Get custom expression resource/item url."""
+    def _get_url_path() -> str:
+        """Get custom expression resource path"""
+
+    @staticmethod
+    @abstractmethod
+    def _get_display_name() -> str:
+        """Get custom expression display name"""
 
     def _refresh(self, data: dict) -> None:
         """Refresh the fields of this instance from the given response dictionary"""
         # Deserialize the response
         resp_obj = CustomMetricResp(**data)
         assert self.model_id
         fields = [
@@ -61,22 +73,19 @@
 
     @classmethod
     def _from_dict(cls, data: dict) -> CustomExpression:
         """Build entity object from the given dictionary."""
 
         # Deserialize the response
         resp_obj = CustomMetricResp(**data)
-        model = Model.from_name(
-            name=resp_obj.model_name, project_name=resp_obj.project_name
-        )
-        assert model.id
+
         # Initialize
         instance = cls(
             name=resp_obj.name,
-            model_id=model.id,
+            model_id=resp_obj.model.id,
             definition=resp_obj.definition,
             description=resp_obj.description,
         )
 
         # Add remaining fields
         fields = [
             'id',
@@ -115,62 +124,58 @@
 
         :return: CustomMetric instance for the provided params
         """
 
         _filter = QueryCondition(
             rules=[
                 QueryRule(field='name', operator=OperatorType.EQUAL, value=name),
+                QueryRule(
+                    field='model_name', operator=OperatorType.EQUAL, value=model_name
+                ),
+                QueryRule(
+                    field='project_name',
+                    operator=OperatorType.EQUAL,
+                    value=project_name,
+                ),
             ]
         )
         params: dict[str, Any] = {
             'filter': _filter.json(),
-            'organization_name': cls.get_organization_name(),
-            'project_name': project_name,
-            'model_name': model_name,
         }
 
         response = cls._client().get(
             url=cls._get_url(),
             params=params,
         )
         if response.json()['data']['total'] == 0:
-            raise_not_found('Custom metric not found for the given identifier')
+            raise_not_found(
+                f'{cls._get_display_name()} not found for the given identifier'
+            )
 
         return cls._from_dict(data=response.json()['data']['items'][0])
 
     @classmethod
     @handle_api_error
     def list(
         cls,
         model_id: UUID,
     ) -> Iterator[CustomExpression]:
         """Get a list of all custom metrics in the organization."""
 
-        model = Model.get(id_=model_id)
-        params: dict[str, Any] = {
-            'organization_name': cls.get_organization_name(),
-            'project_name': model.project.name,
-            'model_name': model.name,
-        }
+        url = f'/v3/models/{model_id}/{cls._get_url_path()}'
 
-        for custom_metric in cls._paginate(
-            url=cls._get_url(),
-            params=params,
-        ):
-            yield cls._from_dict(data=custom_metric)
+        for item in cls._paginate(url=url):
+            yield cls._from_dict(data=item)
 
     @handle_api_error
     def create(self) -> CustomExpression:
         """Create a new custom metric."""
-        model = Model.get(id_=self.model_id)
         payload = {
+            'model_id': self.model_id,
             'name': self.name,
-            'organization_name': self.get_organization_name(),
-            'project_name': model.project.name,
-            'model_name': model.name,
             'definition': self.definition,
         }
 
         if self.description:
             payload['description'] = self.description
 
         response = self._client().post(
@@ -195,28 +200,32 @@
         """Construct a custom metric instance."""
         super().__init__(name, model_id, definition, description)
 
         # Deserialized response object
         self._resp: CustomMetricResp | None = None
 
     @staticmethod
-    def _get_url(id_: UUID | str | None = None) -> str:
-        """Get custom metric resource/item url."""
-        url = '/v2/custom-metrics'
-        return url if not id_ else f'{url}/{id_}'
+    def _get_url_path() -> str:
+        return 'custom-metrics'
+
+    @staticmethod
+    def _get_display_name() -> str:
+        return 'Custom metric'
 
 
 class Segment(CustomExpression):
     def __init__(
         self, name: str, model_id: UUID, definition: str, description: str | None = None
     ) -> None:
         """Construct a segment instance."""
         super().__init__(name, model_id, definition, description)
 
         # Deserialized response object
         self._resp: SegmentResp | None = None
 
     @staticmethod
-    def _get_url(id_: UUID | str | None = None) -> str:
-        """Get segment resource/item url."""
-        url = '/v2/segments'
-        return url if not id_ else f'{url}/{id_}'
+    def _get_url_path() -> str:
+        return 'segments'
+
+    @staticmethod
+    def _get_display_name() -> str:
+        return 'Segment'
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/dataset.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,26 +104,24 @@
         if response.json()['data']['total'] == 0:
             raise_not_found('Dataset not found for the given identifier')
 
         return cls._from_dict(data=response.json()['data']['items'][0])
 
     @classmethod
     @handle_api_error
-    def list(cls, model_id: UUID | str | None = None) -> Iterator[Dataset]:
+    def list(cls, model_id: UUID | str) -> Iterator[Dataset]:
         """
-        Get a list of all datasets in the organization.
+        Get a list of all datasets of a model.
 
         :param model_id: unique uuid format identifier for model
         :return: Iterator of datasets
         """
         params: dict[str, Any] = {'type': EnvType.PRE_PRODUCTION.value}
-        if model_id:
-            params['model_id'] = str(model_id)
-
-        for dataset in cls._paginate(url=cls._get_url(), params=params):
+        url = f'/v3/models/{model_id}/environments'
+        for dataset in cls._paginate(url=url, params=params):
             yield cls._from_dict(data=dataset)
 
 
 @dataclass
 class DatasetCompact:
     id: UUID
     name: str
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/events.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/file.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,31 +61,28 @@
 
     @handle_api_error
     def upload(
         self,
         chunk_size: int = MULTI_PART_CHUNK_SIZE,
     ) -> File:
         """Upload file. Single or multipart upload depends on file size"""
-        print(f'file size = {os.path.getsize(self.path)}, chunk_size = {chunk_size}')
         if os.path.getsize(self.path) < chunk_size:
             return self.single_upload()
 
         return self.multipart_upload(chunk_size=chunk_size)
 
     @handle_api_error
     def single_upload(self) -> File:
         """Single part file upload"""
-        with open(self.path, 'rb') as f:
-            response = self._client().post(
-                url='/v3/files/upload',
-                files={
-                    'file': (self.name, io.BytesIO(f.read())),
-                },
-                headers={CONTENT_TYPE_HEADER_KEY: None},
-            )
+
+        response = self._client().post(
+            url='/v3/files/upload',
+            files={'file': (self.name, open(self.path, 'rb'))},
+            headers={CONTENT_TYPE_HEADER_KEY: None},
+        )
 
         self._refresh_from_response(response)
         return self
 
     @handle_api_error
     def multipart_upload(
         self,
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/job.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/model.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,45 +247,55 @@
         response = self._client().patch(url=self._get_url(id_=self.id), data=body)
         self._refresh_from_response(response=response)
 
     @classmethod
     @handle_api_error
     def list(
         cls,
-        project_id: UUID | None = None,
+        project_id: UUID,
     ) -> Iterator[ModelCompact]:
         """
         Get a list of all models with the given filters
 
         :param project_id: Project identifier
         :return: ModelCompact iterator
         """
-        params = {}
-        if project_id:
-            params['project_id'] = project_id
+        _filter = QueryCondition(
+            rules=[
+                QueryRule(
+                    field='project_id', operator=OperatorType.EQUAL, value=project_id
+                ),
+            ]
+        )
+
+        params = {'filter': _filter.json()}
 
         for model in cls._paginate(url=cls._get_url(), params=params):
             yield ModelCompact(id=model['id'], name=model['name'])
 
     @property
     def datasets(self) -> Iterator[Dataset]:
         """Fetch all the datasets of this model"""
         from fiddler.entities.dataset import (  # pylint: disable=import-outside-toplevel
             Dataset,
         )
 
+        assert self.id is not None
+
         yield from Dataset.list(model_id=self.id)
 
     @property
     def baselines(self) -> Iterator[Baseline]:
         """Fetch all the baselines of this model"""
         from fiddler.entities.baseline import (  # pylint: disable=import-outside-toplevel
             Baseline,
         )
 
+        assert self.id is not None
+
         yield from Baseline.list(model_id=self.id)
 
     @cached_property
     @handle_api_error
     def deployment(self) -> ModelDeployment:
         """Fetch model deployment instance of this model"""
         assert self.id is not None
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/model_artifact.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/model_deployment.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/organization.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/organization.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/project.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,16 @@
     @property
     def models(self) -> Iterator[ModelCompact]:
         """Fetch all the models of this project"""
         from fiddler.entities.model import (  # pylint: disable=import-outside-toplevel
             Model,
         )
 
+        assert self.id is not None
+
         yield from Model.list(project_id=self.id)
 
 
 @dataclass
 class ProjectCompact:
     id: UUID
     name: str
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/surrogate.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/user.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/user.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/webhook.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/entities/xai.py` & `fiddler-client-3.0.0.dev9/fiddler/entities/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/exceptions.py` & `fiddler-client-3.0.0.dev9/fiddler/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/libs/http_client.py` & `fiddler-client-3.0.0.dev9/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/libs/json_encoder.py` & `fiddler-client-3.0.0.dev9/fiddler/libs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/libs/semver.py` & `fiddler-client-3.0.0.dev9/fiddler/libs/semver.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/packtools/gem.py` & `fiddler-client-3.0.0.dev9/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-3.0.0.dev9/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-3.0.0.dev9/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/packtools/template_model.py` & `fiddler-client-3.0.0.dev9/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/alert_record.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/alert_rule.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/baseline.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/custom_features.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/custom_features.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/dataset.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/filter_query.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/filter_query.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/model.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/model_deployment.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/model_schema.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/model_schema.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/model_spec.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/model_spec.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/model_task_params.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/model_task_params.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/response.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/response.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/schemas/xai.py` & `fiddler-client-3.0.0.dev9/fiddler/schemas/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_alert_record.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_alert_rule.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_alert_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,27 +193,27 @@
 
 @responses.activate
 def test_alert_rule_list_success() -> None:
     responses.get(
         url=f'{URL}/v2/alert-configs',
         json=LIST_API_RESPONSE,
     )
-    for rule in AlertRule.list():
+    for rule in AlertRule.list(model_id=MODEL_ID):
         assert isinstance(rule, AlertRule)
 
 
 @responses.activate
 def test_alert_rule_list_empty() -> None:
 
     responses.get(
         url=f'{URL}/v2/alert-configs',
         json=LIST_API_RESPONSE_EMPTY,
     )
 
-    assert len(list(AlertRule.list())) == 0
+    assert len(list(AlertRule.list(model_id=MODEL_ID))) == 0
 
 
 @responses.activate
 def test_delete_alert_rule() -> None:
     responses.get(
         url=f'{URL}/v2/alert-configs/{ALERT_RULE_ID}',
         json=API_RESPONSE_200,
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_baseline.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_baseline.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,33 +199,33 @@
             project_name=PROJECT_NAME,
         )
 
 
 @responses.activate
 def test_baseline_list_success() -> None:
     responses.get(
-        url=f'{URL}/v3/baselines',
+        url=f'{URL}/v3/models/{MODEL_ID}/baselines',
         json=LIST_API_RESPONSE,
     )
-    for baseline in Baseline.list():
+    for baseline in Baseline.list(model_id=MODEL_ID):
         assert isinstance(baseline, Baseline)
 
 
 @responses.activate
 def test_baseline_list_empty() -> None:
     resp = API_RESPONSE_FROM_NAME.copy()
     resp['data']['total'] = 0
     resp['data']['item_count'] = 0
     resp['data']['items'] = []
 
     responses.get(
-        url=f'{URL}/v3/baselines',
+        url=f'{URL}/v3/models/{MODEL_ID}/baselines',
         json=resp,
     )
-    assert len(list(Baseline.list())) == 0
+    assert len(list(Baseline.list(model_id=MODEL_ID))) == 0
 
 
 @responses.activate
 def test_add_baseline_success() -> None:
     responses.post(
         url=f'{URL}/v3/baselines',
         json=API_RESPONSE_200,
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_custom_metric.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_custom_metric.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,80 @@
 from http import HTTPStatus
 from uuid import UUID
 
 import pytest
 import responses
 from responses import matchers
 
-from fiddler.entities.custom_metric import CustomMetric
+from fiddler.entities.custom_expression import CustomMetric
 from fiddler.exceptions import Conflict, NotFound
-from fiddler.tests.apis.test_model import API_RESPONSE_200 as MODEL_API_RESPONSE_200
-from fiddler.tests.apis.test_model import (
-    API_RESPONSE_FROM_NAME as MODEL_API_RESPONSE_FROM_NAME,
+from fiddler.tests.constants import (
+    MODEL_ID,
+    MODEL_NAME,
+    ORG_ID,
+    ORG_NAME,
+    PROJECT_ID,
+    PROJECT_NAME,
+    URL,
+    USER_EMAIL,
+    USER_ID,
+    USER_NAME,
 )
-from fiddler.tests.constants import MODEL_ID, MODEL_NAME, ORG_NAME, PROJECT_NAME, URL
 
 CUSTOM_METRIC_ID = '7057867c-6dd8-4915-89f2-a5f253dd4a3a'
 CUSTOM_METRIC_NAME = 'xyzabc'
 
 API_RESPONSE_200 = {
     'data': {
-        'description': 'meh',
+        'id': CUSTOM_METRIC_ID,
+        'name': CUSTOM_METRIC_NAME,
         'definition': "average(\"Age\")",
+        'description': 'average age',
+        'project': {
+            'id': PROJECT_ID,
+            'name': PROJECT_NAME,
+        },
+        'organization': {
+            'id': ORG_ID,
+            'name': ORG_NAME,
+        },
+        'model': {
+            'id': MODEL_ID,
+            'name': MODEL_NAME,
+        },
         'created_by': {
-            'id': 2,
-            'full_name': 'Nikhil Singh',
-            'email': 'nikhil@fiddler.ai',
+            'id': USER_ID,
+            'full_name': USER_NAME,
+            'email': USER_EMAIL,
+        },
+        'updated_by': {
+            'id': USER_ID,
+            'full_name': USER_NAME,
+            'email': USER_EMAIL,
         },
-        'name': CUSTOM_METRIC_NAME,
-        'id': CUSTOM_METRIC_ID,
-        'organization_name': ORG_NAME,
-        'model_name': MODEL_NAME,
-        'project_name': PROJECT_NAME,
         'created_at': '2024-02-13T07:56:04.275549+00:00',
+        'updated_at': '2024-02-13T07:56:04.275549+00:00',
     },
-    'api_version': '2.0',
+    'api_version': '3.0',
     'kind': 'NORMAL',
 }
 
 API_RESPONSE_404 = {
     'error': {
         'code': 404,
-        'message': "CustomMetric({'uuid': UUID('7057867c-6dd8-4915-89f2-a5f253dd4a3a')}) not found",
+        'message': 'CustomMetric not found',
         'errors': [
             {
                 'reason': 'ObjectNotFound',
-                'message': "CustomMetric({'uuid': UUID('7057867c-6dd8-4915-89f2-a5f253dd4a3a')}) not found",
+                'message': 'CustomMetric not found',
                 'help': '',
             }
         ],
     },
-    'api_version': '2.0',
+    'api_version': '3.0',
     'kind': 'ERROR',
 }
 
 API_RESPONSE_FROM_NAME = {
     'data': {
         'page_size': 100,
         'total': 1,
@@ -83,27 +105,42 @@
         'item_count': 2,
         'page_count': 1,
         'page_index': 1,
         'offset': 0,
         'items': [
             API_RESPONSE_200['data'],
             {
-                'description': 'meh',
+                'id': 'a509c450-c00b-4b5c-9a96-89c43e287e5a',
+                'name': 'avg age 2',
                 'definition': "average(\"Age\")",
+                'description': 'average age 2',
+                'project': {
+                    'id': PROJECT_ID,
+                    'name': PROJECT_NAME,
+                },
+                'organization': {
+                    'id': ORG_ID,
+                    'name': ORG_NAME,
+                },
+                'model': {
+                    'id': MODEL_ID,
+                    'name': MODEL_NAME,
+                },
                 'created_by': {
-                    'id': 2,
-                    'full_name': 'Nikhil Singh',
-                    'email': 'nikhil@fiddler.ai',
+                    'id': USER_ID,
+                    'full_name': USER_NAME,
+                    'email': USER_EMAIL,
                 },
-                'name': 'abcxyz',
-                'id': 'a509c450-c00b-4b5c-9a96-89c43e287e5a',
-                'organization_name': ORG_NAME,
-                'model_name': MODEL_NAME,
-                'project_name': PROJECT_NAME,
-                'created_at': '2024-02-12T07:56:04.275549+00:00',
+                'updated_by': {
+                    'id': USER_ID,
+                    'full_name': USER_NAME,
+                    'email': USER_EMAIL,
+                },
+                'created_at': '2024-02-13T07:56:04.275549+00:00',
+                'updated_at': '2024-02-13T07:56:04.275549+00:00',
             },
         ],
     }
 }
 
 API_RESPONSE_409 = {
     'error': {
@@ -113,240 +150,170 @@
             {
                 'reason': 'Conflict',
                 'message': 'Custom metric with the same name already exists for this model',
                 'help': '',
             }
         ],
     },
-    'api_version': '2.0',
+    'api_version': '3.0',
     'kind': 'ERROR',
 }
 
 
 @responses.activate
 def test_get_custom_metric() -> None:
     responses.get(
-        url=f'{URL}/v2/custom-metrics/{CUSTOM_METRIC_ID}',
+        url=f'{URL}/v3/custom-metrics/{CUSTOM_METRIC_ID}',
         json=API_RESPONSE_200,
     )
 
-    responses.get(
-        url=f'{URL}/v3/models',
-        json=MODEL_API_RESPONSE_FROM_NAME,
-    )
-
-    responses.get(
-        url=f'{URL}/v3/models/{MODEL_ID}',
-        json=MODEL_API_RESPONSE_200,
-    )
-
-    cm = CustomMetric.get(id_=CUSTOM_METRIC_ID)
-    assert isinstance(cm, CustomMetric)
+    custom_metric = CustomMetric.get(id_=CUSTOM_METRIC_ID)
+    assert isinstance(custom_metric, CustomMetric)
+    assert custom_metric.model.id == UUID(MODEL_ID)
+    assert custom_metric.project.id == UUID(PROJECT_ID)
 
 
 @responses.activate
-def test_get_cm_not_found() -> None:
+def test_get_not_found() -> None:
     responses.get(
-        url=f'{URL}/v2/custom-metrics/{CUSTOM_METRIC_ID}',
+        url=f'{URL}/v3/custom-metrics/{CUSTOM_METRIC_ID}',
         json=API_RESPONSE_404,
         status=HTTPStatus.NOT_FOUND,
     )
 
     with pytest.raises(NotFound):
         CustomMetric.get(id_=CUSTOM_METRIC_ID)
 
 
 @responses.activate
-def test_cm_from_name() -> None:
+def test_from_name() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "xyzabc"}]}',
-        'model_name': 'bank_churn',
-        'organization_name': 'fiddler_dev',
-        'project_name': 'bank_churn',
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "xyzabc"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}]}'
     }
 
     responses.get(
-        url=f'{URL}/v2/custom-metrics',
+        url=f'{URL}/v3/custom-metrics',
         json=API_RESPONSE_FROM_NAME,
         match=[matchers.query_param_matcher(params)],
     )
-    responses.get(
-        url=f'{URL}/v3/models',
-        json=MODEL_API_RESPONSE_FROM_NAME,
-    )
-
-    responses.get(
-        url=f'{URL}/v3/models/{MODEL_ID}',
-        json=MODEL_API_RESPONSE_200,
-    )
-    cm = CustomMetric.from_name(
+    custom_metric = CustomMetric.from_name(
         name=CUSTOM_METRIC_NAME,
         model_name=MODEL_NAME,
         project_name=PROJECT_NAME,
     )
-    assert isinstance(cm, CustomMetric)
+    assert isinstance(custom_metric, CustomMetric)
 
 
 @responses.activate
-def test_cm_from_name_not_found() -> None:
+def test_from_name_not_found() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "xyzabc"}]}',
-        'model_name': 'bank_churn',
-        'organization_name': 'fiddler_dev',
-        'project_name': 'bank_churn',
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "xyzabc"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}]}'
     }
     responses.get(
-        url=f'{URL}/v2/custom-metrics',
+        url=f'{URL}/v3/custom-metrics',
         json=EMPTY_LIST_API_RESPONSE,
         match=[matchers.query_param_matcher(params)],
     )
     with pytest.raises(NotFound):
         CustomMetric.from_name(
             name=CUSTOM_METRIC_NAME,
             model_name=MODEL_NAME,
             project_name=PROJECT_NAME,
         )
 
 
 @responses.activate
-def test_cm_list_empty() -> None:
+def test_custom_metric_list_empty() -> None:
     responses.get(
-        url=f'{URL}/v2/custom-metrics',
+        url=f'{URL}/v3/models/{MODEL_ID}/custom-metrics',
         json=EMPTY_LIST_API_RESPONSE,
     )
 
-    responses.get(
-        url=f'{URL}/v3/models/{MODEL_ID}',
-        json=MODEL_API_RESPONSE_200,
-    )
-
     assert len(list(CustomMetric.list(model_id=MODEL_ID))) == 0
 
 
 @responses.activate
-def test_cm_list_success() -> None:
+def test_custom_metric_list_success() -> None:
     params = {
-        'organization_name': ORG_NAME,
-        'project_name': PROJECT_NAME,
-        'model_name': MODEL_NAME,
         'limit': 50,
         'offset': 0,
     }
 
     responses.get(
-        url=f'{URL}/v2/custom-metrics',
+        url=f'{URL}/v3/models/{MODEL_ID}/custom-metrics',
         json=LIST_API_RESPONSE,
         match=[matchers.query_param_matcher(params)],
     )
 
-    responses.get(
-        url=f'{URL}/v3/models',
-        json=MODEL_API_RESPONSE_FROM_NAME,
-    )
-
-    responses.get(
-        url=f'{URL}/v3/models/{MODEL_ID}',
-        json=MODEL_API_RESPONSE_200,
-    )
-
-    for cm in CustomMetric.list(model_id=MODEL_ID):
-        assert isinstance(cm, CustomMetric)
+    for custom_metric in CustomMetric.list(model_id=MODEL_ID):
+        assert isinstance(custom_metric, CustomMetric)
 
 
 @responses.activate
-def test_cm_create() -> None:
+def test_custom_metric_create() -> None:
     responses.post(
-        url=f'{URL}/v2/custom-metrics',
+        url=f'{URL}/v3/custom-metrics',
         json=API_RESPONSE_200,
     )
 
-    responses.get(
-        url=f'{URL}/v3/models/{MODEL_ID}',
-        json=MODEL_API_RESPONSE_200,
-    )
-
     custom_metric = CustomMetric(
         name=CUSTOM_METRIC_NAME,
         model_id=MODEL_ID,
         definition="average(\"Age\")",
-        description='meh',
+        description='average age',
     ).create()
 
     assert isinstance(custom_metric, CustomMetric)
     assert custom_metric.id == UUID(CUSTOM_METRIC_ID)
     assert custom_metric.name == CUSTOM_METRIC_NAME
     assert custom_metric.model_id
 
 
 @responses.activate
-def test_cm_create_conflict() -> None:
+def test_custom_metric_create_conflict() -> None:
     responses.post(
-        url=f'{URL}/v2/custom-metrics',
+        url=f'{URL}/v3/custom-metrics',
         json=API_RESPONSE_409,
         status=HTTPStatus.CONFLICT,
     )
 
-    responses.get(
-        url=f'{URL}/v3/models/{MODEL_ID}',
-        json=MODEL_API_RESPONSE_200,
-    )
-
     with pytest.raises(Conflict):
         CustomMetric(
             name=CUSTOM_METRIC_NAME,
             model_id=MODEL_ID,
             definition="average(\"Age\")",
-            description='meh',
+            description='average age',
         ).create()
 
 
 @responses.activate
-def test_delete_cm() -> None:
+def test_delete_custom_metric() -> None:
     responses.get(
-        url=f'{URL}/v2/custom-metrics/{CUSTOM_METRIC_ID}',
+        url=f'{URL}/v3/custom-metrics/{CUSTOM_METRIC_ID}',
         json=API_RESPONSE_200,
     )
-
-    responses.get(
-        url=f'{URL}/v3/models',
-        json=MODEL_API_RESPONSE_FROM_NAME,
-    )
-
-    responses.get(
-        url=f'{URL}/v3/models/{MODEL_ID}',
-        json=MODEL_API_RESPONSE_200,
-    )
     custom_metric = CustomMetric.get(id_=CUSTOM_METRIC_ID)
 
     responses.delete(
-        url=f'{URL}/v2/custom-metrics/{CUSTOM_METRIC_ID}',
+        url=f'{URL}/v3/custom-metrics/{CUSTOM_METRIC_ID}',
     )
 
     custom_metric.delete()
 
 
 @responses.activate
-def test_delete_cm_not_found() -> None:
+def test_delete_custom_metric_not_found() -> None:
     responses.get(
-        url=f'{URL}/v2/custom-metrics/{CUSTOM_METRIC_ID}',
+        url=f'{URL}/v3/custom-metrics/{CUSTOM_METRIC_ID}',
         json=API_RESPONSE_200,
     )
 
-    responses.get(
-        url=f'{URL}/v3/models',
-        json=MODEL_API_RESPONSE_FROM_NAME,
-    )
-
-    responses.get(
-        url=f'{URL}/v3/models/{MODEL_ID}',
-        json=MODEL_API_RESPONSE_200,
-    )
     custom_metric = CustomMetric.get(id_=CUSTOM_METRIC_ID)
 
     responses.delete(
-        url=f'{URL}/v2/custom-metrics/{CUSTOM_METRIC_ID}',
+        url=f'{URL}/v3/custom-metrics/{CUSTOM_METRIC_ID}',
         json=API_RESPONSE_404,
         status=HTTPStatus.NOT_FOUND,
     )
 
     with pytest.raises(NotFound):
         custom_metric.delete()
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_dataset.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,26 +148,26 @@
             project_name=PROJECT_NAME,
         )
 
 
 @responses.activate
 def test_dataset_list_success() -> None:
     responses.get(
-        url=f'{URL}/v3/environments',
+        url=f'{URL}/v3/models/{MODEL_ID}/environments',
         json=LIST_API_RESPONSE,
     )
-    for dataset in Dataset.list():
+    for dataset in Dataset.list(model_id=MODEL_ID):
         assert isinstance(dataset, Dataset)
 
 
 @responses.activate
 def test_dataset_list_empty() -> None:
     resp = API_RESPONSE_FROM_NAME.copy()
     resp['data']['total'] = 0
     resp['data']['item_count'] = 0
     resp['data']['items'] = []
 
     responses.get(
-        url=f'{URL}/v3/environments',
+        url=f'{URL}/v3/models/{MODEL_ID}/environments',
         json=resp,
     )
-    assert len(list(Dataset.list())) == 0
+    assert len(list(Dataset.list(model_id=MODEL_ID))) == 0
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_events.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_files.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_files.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_generate_model.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_generate_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_job.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_mixin.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_model.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,19 @@
     models = Model.list(project_id=PROJECT_ID)
     for model in models:
         assert isinstance(model, ModelCompact)
 
 
 @responses.activate
 def test_model_list_success() -> None:
-    params = {'project_id': str(PROJECT_ID), 'limit': 50, 'offset': 0}
+    params = {
+        'filter': '{"condition": "AND", "rules": [{"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}]}',
+        'limit': 50,
+        'offset': 0,
+    }
     responses.get(
         url=f'{URL}/v3/models',
         json=LIST_API_RESPONSE,
         match=[matchers.query_param_matcher(params)],
     )
     models = Model.list(project_id=PROJECT_ID)
     for model in models:
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_model_artifact.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_model_deployment.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_model_surrogate.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_project.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_webhook.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/apis/test_xai.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/conftest.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/constants.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/test_connection.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/test_json_encoder.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/tests/test_utils.py` & `fiddler-client-3.0.0.dev9/fiddler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/utils/helpers.py` & `fiddler-client-3.0.0.dev9/fiddler/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/utils/logger.py` & `fiddler-client-3.0.0.dev9/fiddler/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/utils/model_generator.py` & `fiddler-client-3.0.0.dev9/fiddler/utils/model_generator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler/utils/version.py` & `fiddler-client-3.0.0.dev9/fiddler/utils/version.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev8/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-3.0.0.dev9/fiddler_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.0.0.dev8
+Version: 3.0.0.dev9
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
```

### Comparing `fiddler-client-3.0.0.dev8/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-3.0.0.dev9/fiddler_client.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 fiddler/constants/model_deployment.py
 fiddler/constants/xai.py
 fiddler/entities/__init__.py
 fiddler/entities/alert_record.py
 fiddler/entities/alert_rule.py
 fiddler/entities/base.py
 fiddler/entities/baseline.py
-fiddler/entities/custom_metric.py
+fiddler/entities/custom_expression.py
 fiddler/entities/dataset.py
 fiddler/entities/events.py
 fiddler/entities/file.py
 fiddler/entities/job.py
 fiddler/entities/model.py
 fiddler/entities/model_artifact.py
 fiddler/entities/model_deployment.py
@@ -49,16 +49,16 @@
 fiddler/packtools/project_attributions_helpers.py
 fiddler/packtools/template_model.py
 fiddler/schemas/__init__.py
 fiddler/schemas/alert_record.py
 fiddler/schemas/alert_rule.py
 fiddler/schemas/base.py
 fiddler/schemas/baseline.py
+fiddler/schemas/custom_expression.py
 fiddler/schemas/custom_features.py
-fiddler/schemas/custom_metric.py
 fiddler/schemas/dataset.py
 fiddler/schemas/events.py
 fiddler/schemas/file.py
 fiddler/schemas/filter_query.py
 fiddler/schemas/job.py
 fiddler/schemas/model.py
 fiddler/schemas/model_deployment.py
@@ -93,14 +93,15 @@
 fiddler/tests/apis/test_job.py
 fiddler/tests/apis/test_mixin.py
 fiddler/tests/apis/test_model.py
 fiddler/tests/apis/test_model_artifact.py
 fiddler/tests/apis/test_model_deployment.py
 fiddler/tests/apis/test_model_surrogate.py
 fiddler/tests/apis/test_project.py
+fiddler/tests/apis/test_segment.py
 fiddler/tests/apis/test_webhook.py
 fiddler/tests/apis/test_xai.py
 fiddler/utils/__init__.py
 fiddler/utils/helpers.py
 fiddler/utils/logger.py
 fiddler/utils/model_generator.py
 fiddler/utils/validations.py
```

### Comparing `fiddler-client-3.0.0.dev8/setup.py` & `fiddler-client-3.0.0.dev9/setup.py`

 * *Files identical despite different names*

