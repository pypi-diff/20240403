# Comparing `tmp/amazon_sagemaker_jupyter_scheduler-3.0.7.tar.gz` & `tmp/amazon_sagemaker_jupyter_scheduler-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_sagemaker_jupyter_scheduler-3.0.7.tar", last modified: Fri Feb  9 23:00:12 2024, max compression
+gzip compressed data, was "amazon_sagemaker_jupyter_scheduler-3.0.9.tar", last modified: Mon Mar 25 11:31:27 2024, max compression
```

## Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7.tar` & `amazon_sagemaker_jupyter_scheduler-3.0.9.tar`

### file list

```diff
@@ -1,227 +1,224 @@
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.278284 amazon_sagemaker_jupyter_scheduler-3.0.7/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/.eslintignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1026 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/.eslintrc.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1707 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/.gitignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/.prettierignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/.prettierrc
--rw-r--r--   0 p4admin  (12569) amazon     (100)      794 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/Config
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5383 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/DEVELOPMENT.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)    11358 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/LICENSE
--rw-r--r--   0 p4admin  (12569) amazon     (100)      686 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/MANIFEST.in
--rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/NOTICE
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1217 2024-02-09 23:00:12.278284 amazon_sagemaker_jupyter_scheduler-3.0.7/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)      347 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/README.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2046 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/RELEASE.md
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.258285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      455 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/_version.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.258285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/advanced_environments/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/advanced_environments/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      163 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/advanced_environments/base_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6333 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    15692 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2541 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      465 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/aws_config.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.250285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/botocore_model/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.250285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.258285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/
--rw-r--r--   0 p4admin  (12569) amazon     (100)  1378776 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)    20768 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4732 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/cron_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2060 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/deletable_resource.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1816 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/environment_detector.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3981 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3729 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      716 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/extension.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4553 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/file_download_manager.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5757 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/file_uploader.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4262 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    57996 2024-02-09 22:59:58.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1646 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.262285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5410 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.250285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/schemas/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.250285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.262285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1301 2024-02-09 23:00:04.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5294 2024-02-09 23:00:04.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.262285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/
--rw-r--r--   0 p4admin  (12569) amazon     (100)    29540 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/240.145b0024b0b19e6c54a7.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/240.145b0024b0b19e6c54a7.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    14905 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/543.3b5f882f510e08e43423.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/673.1543875757f3fa999f79.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    59089 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/75.454a593e3b6ddf9464fb.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   197056 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/827.56fabfcc2be29102ab30.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      490 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/827.56fabfcc2be29102ab30.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7892 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.7e06320a8ba69020b115.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2024-02-09 23:00:04.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    38076 2024-02-09 23:00:11.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6649 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/logging.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    30833 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/model_converter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4106 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/models.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.266285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1015 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4756 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/jupyterlab_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      679 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/revenue.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9468 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6056 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5916 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/tags.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3114 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      498 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/s3_uri.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    43586 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/scheduler.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      840 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/stack_trace_filter.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.266285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/__init__.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.266285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/helpers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/helpers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      913 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.266285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/providers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/providers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12941 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    10827 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    20446 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3180 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1439 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    17404 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3695 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2149 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1895 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1058 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2339 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6823 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2280 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3519 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6058 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    29711 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2133 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    32683 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2200 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_stack_trace_filter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      427 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.266285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/util/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/util/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      672 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/util/constants.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2805 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.258285 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler.egg-info/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1217 2024-02-09 23:00:12.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9109 2024-02-09 23:00:12.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-02-09 23:00:12.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-02-09 23:00:12.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 p4admin  (12569) amazon     (100)      202 2024-02-09 23:00:12.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler.egg-info/requires.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-02-09 23:00:12.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler.egg-info/top_level.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)      261 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/babel.config.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)       73 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/custom.d.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2181 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/host_region_mapping.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      866 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/jest.config.base.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      669 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/jest.config.js
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.266285 amazon_sagemaker_jupyter_scheduler-3.0.7/jupyter-config/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.266285 amazon_sagemaker_jupyter_scheduler-3.0.7/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      109 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/jupyter-config/jupyter_server_config.d/amazon_sagemaker_jupyter_scheduler.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      466 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/jupyter-config/jupyter_server_config.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)   744363 2024-02-09 23:00:03.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/package-lock.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5294 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/package.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      127 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/pyproject.toml
--rw-r--r--   0 p4admin  (12569) amazon     (100)      128 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/requirements.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2024-02-09 23:00:12.278284 amazon_sagemaker_jupyter_scheduler-3.0.7/setup.cfg
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3109 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/setup.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.266285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.266285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/__mocks__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/__mocks__/fileMock.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/__tests__/
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    12462 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/__tests__/CreateNotebookJobForm.spec.tsx
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)     4348 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/__tests__/VpcCheckbox.spec.tsx
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    13449 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/__tests__/initalValueHelpers.spec.ts
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    11135 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/__tests__/validationHelpers.spec.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.250285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1093 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/Link.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      823 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/RouterLink.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/__test__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1186 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/__test__/Link.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1011 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/__test__/RouterLink.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      184 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/selectinput/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1583 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/selectinput/SelectInput.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       56 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/selectinput/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      967 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/selectinput/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1585 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/TextInput.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1934 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/__tests__/TextInput.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       54 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2789 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      206 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/tooltip/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1364 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/tooltip/Tooltip.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/tooltip/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      851 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/tooltip/__tests__/Tooltip.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/tooltip/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      587 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/tooltip/styles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/constants/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8431 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/constants/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       53 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/constants/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       99 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/constants/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      146 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/plugins/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1715 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/plugins/ScheduleNotebookPlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7216 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/plugins/SchedulerTelemetryPlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       85 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/plugins/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3328 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/themeProvider.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.270285 amazon_sagemaker_jupyter_scheduler-3.0.7/src/types/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      420 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/types/images.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       82 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/types/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      141 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/types/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/types/sagemaker.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.274284 amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2399 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/PluginEnvironmentProvider.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.274284 amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1761 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1530 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/images.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      108 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1205 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1017 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/rendering.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.274284 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4733 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJob.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.274284 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.274284 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/
--rw-r--r--   0 p4admin  (12569) amazon     (100)    17828 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.274284 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3914 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3226 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1094 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.274284 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3531 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       55 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      285 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5596 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    15139 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1229 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/InputContainer.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.274284 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2737 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      918 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5244 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/JupyterLabJobEnvironment.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      162 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1280 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3138 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1561 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-02-09 23:00:12.278284 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1645 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6050 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      552 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12185 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    64113 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      781 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1305 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       41 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8199 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1727 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2216 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/mockResponses.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2815 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9486 2024-02-09 22:58:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.7/tsconfig.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.181599 amazon_sagemaker_jupyter_scheduler-3.0.9/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/.eslintignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1026 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/.eslintrc.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1707 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/.gitignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/.prettierignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/.prettierrc
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      794 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/Config
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5383 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/DEVELOPMENT.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    11358 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/LICENSE
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      616 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/MANIFEST.in
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/NOTICE
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1217 2024-03-25 11:31:27.181599 amazon_sagemaker_jupyter_scheduler-3.0.9/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      347 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/README.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2046 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/RELEASE.md
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.161599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      455 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/_version.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.161599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/advanced_environments/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/advanced_environments/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      163 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/advanced_environments/base_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6333 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    15692 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2781 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      465 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/aws_config.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    20103 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4732 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/cron_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2060 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/deletable_resource.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1816 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/environment_detector.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3981 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3729 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      716 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/extension.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4553 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/file_download_manager.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5757 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/file_uploader.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4262 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    57996 2024-03-25 11:31:14.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1646 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.161599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5410 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.153599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/schemas/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.153599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.161599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1301 2024-03-25 11:31:19.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5294 2024-03-25 11:31:19.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.165599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    29540 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/240.145b0024b0b19e6c54a7.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/240.145b0024b0b19e6c54a7.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    14905 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/543.3b5f882f510e08e43423.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/673.1543875757f3fa999f79.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    59089 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/75.454a593e3b6ddf9464fb.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   197056 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/827.56fabfcc2be29102ab30.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      490 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/827.56fabfcc2be29102ab30.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7892 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.5393ffde93b2d5747094.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2024-03-25 11:31:19.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    38076 2024-03-25 11:31:26.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6649 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/logging.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    30833 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/model_converter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4106 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/models.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.165599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1015 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5239 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/jupyterlab_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      679 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/revenue.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9468 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6056 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6642 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/tags.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3114 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      498 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/s3_uri.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    43897 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/scheduler.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      840 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/stack_trace_filter.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/__init__.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/helpers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/helpers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      913 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/providers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/providers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12941 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    10827 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    20446 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3180 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1439 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    17404 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3695 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2149 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1895 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1058 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2339 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6823 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2280 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3519 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    24239 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_jupyterlab_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6058 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    29711 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2133 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    32944 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2200 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_stack_trace_filter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      427 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/util/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/util/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      672 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/util/constants.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2805 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.161599 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler.egg-info/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1217 2024-03-25 11:31:27.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9098 2024-03-25 11:31:27.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-03-25 11:31:27.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2024-03-25 11:31:27.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      202 2024-03-25 11:31:27.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler.egg-info/requires.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-03-25 11:31:27.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      261 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/babel.config.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       73 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/custom.d.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2181 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/host_region_mapping.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      866 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/jest.config.base.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      669 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/jest.config.js
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/jupyter-config/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      109 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/jupyter-config/jupyter_server_config.d/amazon_sagemaker_jupyter_scheduler.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      466 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/jupyter-config/jupyter_server_config.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   744363 2024-03-25 11:31:18.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/package-lock.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5294 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/package.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      127 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/pyproject.toml
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      128 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/requirements.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2024-03-25 11:31:27.181599 amazon_sagemaker_jupyter_scheduler-3.0.9/setup.cfg
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3109 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/setup.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/__mocks__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/__mocks__/fileMock.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/__tests__/
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    12462 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/__tests__/CreateNotebookJobForm.spec.tsx
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)     4348 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/__tests__/VpcCheckbox.spec.tsx
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    13449 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/__tests__/initalValueHelpers.spec.ts
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    11135 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/__tests__/validationHelpers.spec.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.153599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.169599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1093 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/Link.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      823 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/RouterLink.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/__test__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1186 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/__test__/Link.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1011 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/__test__/RouterLink.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      184 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/selectinput/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1583 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/selectinput/SelectInput.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       56 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/selectinput/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      967 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/selectinput/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1585 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/TextInput.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1934 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/__tests__/TextInput.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       54 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2789 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      206 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/tooltip/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1364 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/tooltip/Tooltip.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/tooltip/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      851 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/tooltip/__tests__/Tooltip.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/tooltip/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      587 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/tooltip/styles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/constants/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8431 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/constants/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       53 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/constants/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       99 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/constants/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      146 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/plugins/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1715 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/plugins/ScheduleNotebookPlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     7216 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/plugins/SchedulerTelemetryPlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       85 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/plugins/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3328 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/themeProvider.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/types/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      420 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/types/images.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       82 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/types/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      141 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/types/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/types/sagemaker.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2399 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/PluginEnvironmentProvider.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.173599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1761 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1530 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/images.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      108 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1205 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1017 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/rendering.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.177599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4733 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJob.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.177599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.177599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    17828 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.177599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3914 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3226 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1094 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.177599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3531 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       55 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      285 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5596 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    15139 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1229 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/InputContainer.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.177599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2737 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      918 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5244 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/JupyterLabJobEnvironment.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      162 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1280 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3138 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1561 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:31:27.181599 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1645 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6050 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      552 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12185 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    64113 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      781 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1305 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       41 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8199 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1727 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2216 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/mockResponses.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2815 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9486 2024-03-25 11:28:49.000000 amazon_sagemaker_jupyter_scheduler-3.0.9/tsconfig.json
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/.eslintrc.js` & `amazon_sagemaker_jupyter_scheduler-3.0.9/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/.gitignore` & `amazon_sagemaker_jupyter_scheduler-3.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/Config` & `amazon_sagemaker_jupyter_scheduler-3.0.9/Config`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/DEVELOPMENT.md` & `amazon_sagemaker_jupyter_scheduler-3.0.9/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/LICENSE` & `amazon_sagemaker_jupyter_scheduler-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/MANIFEST.in` & `amazon_sagemaker_jupyter_scheduler-3.0.9/MANIFEST.in`

 * *Files 7% similar despite different names*

```diff
@@ -19,9 +19,8 @@
 # Patterns to exclude from any directory
 global-exclude *~
 global-exclude *.pyc
 global-exclude *.pyo
 global-exclude .git
 global-exclude .ipynb_checkpoints
 
-recursive-include amazon_sagemaker_jupyter_scheduler/botocore_model *
 include amazon_sagemaker_jupyter_scheduler/host_region_mapping.json *
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/PKG-INFO` & `amazon_sagemaker_jupyter_scheduler-3.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_sagemaker_jupyter_scheduler
-Version: 3.0.7
+Version: 3.0.9
 Summary: Amazon SageMaker Jupyter Scheduler based on the https://pypi.org/project/jupyter-scheduler/
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Scheduling Notebooks,Notebooks,Amazon Sagemaker
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/RELEASE.md` & `amazon_sagemaker_jupyter_scheduler-3.0.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/__init__.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/app_metadata.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/app_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,14 +62,26 @@
     return _get_app_metadata_file().get("SpaceName", "")
 
 
 def get_domain_id():
     return _get_app_metadata_file().get("DomainId")
 
 
+def get_space_name():
+    return _get_app_metadata_file().get("SpaceName", "")
+
+
+def get_app_type():
+    return _get_app_metadata_file().get("AppType", "")
+
+
+def get_app_name():
+    return _get_app_metadata_file().get("ResourceName", "")
+
+
 def get_user_details():
     user_details = None
 
     user_profile_name = get_user_profile_name()
     if user_profile_name:
         user_details = UserDetails(
             user_id_key=UserTypes.PROFILE_USER, user_id_value=user_profile_name
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/clients.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/clients.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,29 +29,15 @@
             # TODO: Refine these values (currently copied from LooseLeafNb2Kg)
             connect_timeout=60,
             read_timeout=60,
             retries={"max_attempts": 4},
         )
         self.partition = partition
         self.region_name = region_name
-
-        # aiobotocore is pinned to botocore 1.23 but our training changes are very recent.
-        # copied the latest model file from botocore https://github.com/boto/botocore/blob/develop/botocore/data/sagemaker/2017-07-24/service-2.json
-        # This env should cause botocore to load this model - https://botocore.amazonaws.com/v1/documentation/api/latest/reference/loaders.html
-        # and not affect any other clients running in the environment
-        PACKAGE_ROOT = os.path.abspath(os.path.dirname(__file__))
-        os.environ["SCHEDULING_DATA_PATH"] = os.path.join(
-            PACKAGE_ROOT, "botocore_model"
-        )
-        # we want to modify the default search path for service models
-        # https://github.com/boto/botocore/blob/develop/botocore/configprovider.py#L53
-        # TODO: Find a way to upgrade aiobotocore and remove this hack
-        self.sess = get_session(
-            {"data_path": ("data_path", "SCHEDULING_DATA_PATH", None, None)}
-        )
+        self.sess = get_session()
 
 
 class SageMakerAsyncBoto3Client(BaseAsyncBotoClient):
     def _create_sagemaker_client(self):
         # based on the Studio domain stage, we want to choose the sagemaker endpoint
         # rest of the services will use prod stages for non prod stages
         stage = InternalMetadataAdapter().get_stage()
@@ -157,14 +143,18 @@
                 DomainId=domain_id, UserProfileName=user_profile_name
             )
 
     async def describe_space(self, domain_id: str, space_name: str) -> Dict:
         async with self._create_sagemaker_client() as sm:
             return await sm.describe_space(DomainId=domain_id, SpaceName=space_name)
 
+    async def describe_app(self, domain_id: str, space_name: str, app_type: str, app_name: str) -> Dict:
+        async with self._create_sagemaker_client() as sm:
+            return await sm.describe_app(DomainId=domain_id, SpaceName=space_name, AppType=app_type, AppName=app_name)
+
     async def create_pipeline(
         self,
         pipeline_name: str,
         pipeline_display_name: str,
         pipeline_description: str,
         pipeline_definition: str,
         role_arn: str,
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/cron_util.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/cron_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/deletable_resource.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/deletable_resource.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/environment_detector.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/environment_detector.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/environments.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/error_util.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/error_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/extension.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/extension.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/file_download_manager.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/file_download_manager.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/file_uploader.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/file_uploader.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/handlers.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
 {
-    "ap-southeast-7": [
+    "us-isof-east-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -68,15 +68,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-southeast-6": [
+    "il-central-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -141,15 +141,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "af-south-1": [
+    "sa-east-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -212,18 +212,17 @@
         "ml.trn1.2xlarge",
         "ml.trn1.32xlarge",
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
-        "ml.c5n.18xlarge",
-        "ml.m4.8xlarge"
+        "ml.c5n.18xlarge"
     ],
-    "mx-central-1": [
+    "eu-central-2": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -288,15 +287,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-southeast-5": [
+    "us-east-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -361,15 +360,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-east-2": [
+    "ap-east-2": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -434,15 +433,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "eusc-de-east-1": [
+    "us-isob-east-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -507,15 +506,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "me-south-1": [
+    "ca-central-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -580,15 +579,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ca-west-1": [
+    "af-south-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -652,21 +651,17 @@
         "ml.trn1.32xlarge",
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge",
-        "ml.c5.large",
-        "ml.c5.12xlarge",
-        "ml.c5.24xlarge",
-        "ml.m5.8xlarge",
-        "ml.m5.16xlarge"
+        "ml.m4.8xlarge"
     ],
-    "ap-south-1": [
+    "ap-southeast-5": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -731,15 +726,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "eu-west-1": [
+    "eusc-de-east-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -804,15 +799,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-gov-west-1": [
+    "us-west-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -877,15 +872,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "eu-south-2": [
+    "eu-west-3": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -950,15 +945,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-southeast-4": [
+    "us-iso-east-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1023,15 +1018,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "eu-west-2": [
+    "eu-north-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1096,15 +1091,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-west-1": [
+    "us-gov-west-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1169,15 +1164,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-northeast-1": [
+    "cn-north-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1242,15 +1237,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-northeast-1": [
+    "ap-southeast-2": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1315,15 +1310,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "eu-north-1": [
+    "me-central-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1388,15 +1383,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "sa-east-1": [
+    "cn-northwest-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1461,15 +1456,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-east-1": [
+    "ap-northeast-2": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1534,15 +1529,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "il-central-1": [
+    "us-gov-east-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1607,15 +1602,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "eu-west-3": [
+    "ap-east-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1680,15 +1675,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-isof-east-1": [
+    "ap-southeast-4": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1753,15 +1748,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "cn-north-1": [
+    "ap-south-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1826,15 +1821,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "eu-central-1": [
+    "us-east-2": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1899,15 +1894,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-isob-east-1": [
+    "us-isob-west-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -1972,15 +1967,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-southeast-3": [
+    "ap-northeast-3": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2043,17 +2038,18 @@
         "ml.trn1.2xlarge",
         "ml.trn1.32xlarge",
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
-        "ml.c5n.18xlarge"
+        "ml.c5n.18xlarge",
+        "ml.m4.8xlarge"
     ],
-    "us-west-2": [
+    "eu-west-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2118,15 +2114,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "cn-northwest-1": [
+    "ap-southeast-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2191,15 +2187,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-isof-south-1": [
+    "eu-south-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2262,17 +2258,18 @@
         "ml.trn1.2xlarge",
         "ml.trn1.32xlarge",
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
-        "ml.c5n.18xlarge"
+        "ml.c5n.18xlarge",
+        "ml.m4.8xlarge"
     ],
-    "us-gov-east-1": [
+    "eu-south-2": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2337,15 +2334,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "eu-central-2": [
+    "eu-central-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2410,15 +2407,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-southeast-1": [
+    "ap-southeast-3": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2483,15 +2480,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-east-2": [
+    "ap-southeast-7": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2556,15 +2553,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-northeast-2": [
+    "us-isof-south-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2629,15 +2626,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-south-2": [
+    "ca-west-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2700,17 +2697,22 @@
         "ml.trn1.2xlarge",
         "ml.trn1.32xlarge",
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
-        "ml.c5n.18xlarge"
+        "ml.c5n.18xlarge",
+        "ml.c5.large",
+        "ml.c5.12xlarge",
+        "ml.c5.24xlarge",
+        "ml.m5.8xlarge",
+        "ml.m5.16xlarge"
     ],
-    "ca-central-1": [
+    "ap-northeast-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2775,15 +2777,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "eu-south-1": [
+    "us-west-2": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2846,18 +2848,17 @@
         "ml.trn1.2xlarge",
         "ml.trn1.32xlarge",
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
-        "ml.c5n.18xlarge",
-        "ml.m4.8xlarge"
+        "ml.c5n.18xlarge"
     ],
-    "ap-northeast-3": [
+    "mx-central-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2920,18 +2921,17 @@
         "ml.trn1.2xlarge",
         "ml.trn1.32xlarge",
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
-        "ml.c5n.18xlarge",
-        "ml.m4.8xlarge"
+        "ml.c5n.18xlarge"
     ],
-    "me-central-1": [
+    "us-northeast-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -2996,15 +2996,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-southeast-2": [
+    "ap-south-2": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -3069,15 +3069,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-iso-east-1": [
+    "ap-southeast-6": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -3142,15 +3142,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "us-isob-west-1": [
+    "me-south-1": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
@@ -3215,15 +3215,15 @@
         "ml.trn1n.32xlarge",
         "ml.c5n.xlarge",
         "ml.c5n.2xlarge",
         "ml.c5n.4xlarge",
         "ml.c5n.9xlarge",
         "ml.c5n.18xlarge"
     ],
-    "ap-east-1": [
+    "eu-west-2": [
         "ml.m4.xlarge",
         "ml.m4.2xlarge",
         "ml.m4.4xlarge",
         "ml.m4.10xlarge",
         "ml.m4.16xlarge",
         "ml.m5.large",
         "ml.m5.xlarge",
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/package.json` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.961111111111111%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'3.0.9'"}*

```diff
@@ -61,18 +61,14 @@
     "files": [
         "dist/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.7e06320a8ba69020b115.js"
-        },
         "disabledExtensions": [
             "@jupyterlab/scheduler:IAdvancedOptions",
             "@jupyterlab/scheduler:TelemetryHandler"
         ],
         "extension": true,
         "outputDir": "amazon_sagemaker_jupyter_scheduler/labextension",
         "schemaDir": "schema",
@@ -127,9 +123,9 @@
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "3.0.7"
+    "version": "3.0.9"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig` & `amazon_sagemaker_jupyter_scheduler-3.0.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'3.0.9'"}*

```diff
@@ -123,9 +123,9 @@
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "3.0.7"
+    "version": "3.0.9"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/240.145b0024b0b19e6c54a7.js` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/240.145b0024b0b19e6c54a7.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/543.3b5f882f510e08e43423.js` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/543.3b5f882f510e08e43423.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/673.1543875757f3fa999f79.js` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/673.1543875757f3fa999f79.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/75.454a593e3b6ddf9464fb.js` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/75.454a593e3b6ddf9464fb.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/827.56fabfcc2be29102ab30.js` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/827.56fabfcc2be29102ab30.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.7e06320a8ba69020b115.js` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.5393ffde93b2d5747094.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, i, u, l, s, f, d, c, p, h, m, v, b, g, y, w, j = {
-            2344: (e, r, t) => {
+            8761: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(827), t.e(271), t.e(75)]).then((() => () => t(2372))),
                         "./extension": () => Promise.all([t.e(827), t.e(271), t.e(75)]).then((() => () => t(2372)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -113,15 +113,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("@amzn/sagemaker-jupyter-scheduler", "3.0.7", (() => Promise.all([S.e(827), S.e(271), S.e(75)]).then((() => () => S(2372))))), u("@emotion/css", "11.11.2", (() => S.e(543).then((() => () => S(4543))))), u("react-router-dom", "5.3.4", (() => Promise.all([S.e(240), S.e(271), S.e(673)]).then((() => () => S(7240)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@amzn/sagemaker-jupyter-scheduler", "3.0.9", (() => Promise.all([S.e(827), S.e(271), S.e(75)]).then((() => () => S(2372))))), u("@emotion/css", "11.11.2", (() => S.e(543).then((() => () => S(4543))))), u("react-router-dom", "5.3.4", (() => Promise.all([S.e(240), S.e(271), S.e(673)]).then((() => () => S(7240)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -293,10 +293,10 @@
                     u && u(S)
                 }
                 for (r && r(t); l < o.length; l++) n = o[l], S.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyter_scheduler = self.webpackChunk_amzn_sagemaker_jupyter_scheduler || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var P = S(2344);
+    var P = S(8761);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyter-scheduler"] = P
 })();
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/logging.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/logging.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/model_converter.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/model_converter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/models.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/models.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/jupyterlab_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/jupyterlab_image_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import asyncio
 
 from async_lru import alru_cache
 from jupyter_scheduler.exceptions import SchedulerError
 
 from amazon_sagemaker_jupyter_scheduler.app_metadata import (
     get_domain_id,
-    get_shared_space_name,
+    get_space_name,
+    get_app_type,
+    get_app_name,
 )
 from amazon_sagemaker_jupyter_scheduler.clients import get_sagemaker_client
 from amazon_sagemaker_jupyter_scheduler.models import ImageMetadata
 
 
 IMAGE_OWNER_ENV_VAR_KEY = "AWS_INTERNAL_IMAGE_OWNER"
 IMAGE_URI_ENV_VAR_KEY = "SAGEMAKER_INTERNAL_IMAGE_URI"
@@ -41,15 +43,15 @@
 async def _fetch_custom_images(sm_client):
     DEFAULT_USER_SETTINGS_KEY = "DefaultUserSettings"
     USER_SETTINGS_KEY = "UserSettings"
     api_calls = [sm_client.describe_domain(get_domain_id())]
 
     # For JupyterLab apps, we will get user profile ARN from 'DescribeSpace' API calls
     space_details = await sm_client.describe_space(
-        get_domain_id(), get_shared_space_name()
+        get_domain_id(), get_space_name()
     )
     user_profile_name = space_details.get("OwnershipSettings", {}).get("OwnerUserProfileName", None)
 
     if user_profile_name:
         api_calls.append(
             sm_client.describe_user_profile(
                 get_domain_id(), user_profile_name
@@ -65,19 +67,33 @@
     ).get("CustomImages", []) + user_details.get(USER_SETTINGS_KEY, {}).get(
         "JupyterLabAppSettings", {}
     ).get(
         "CustomImages", []
     )
 
 
+async def get_image_or_version_arn(sm_client):
+    app_details = await sm_client.describe_app(
+        get_domain_id(), get_space_name(), get_app_type(), get_app_name()
+    )
+    resource_spec = app_details.get("ResourceSpec", {})
+
+    app_image_version_arn = resource_spec.get("SageMakerImageVersionArn", None)
+    
+    if not app_image_version_arn:
+        return resource_spec.get("SageMakerImageArn", None)
+    return app_image_version_arn
+
+
 async def get_third_party_image() -> ImageMetadata:
-    image_arn = get_image_or_version_arn_from_metadata()
     sagemaker_client = get_sagemaker_client()
+    image_arn = await get_image_or_version_arn(sagemaker_client)
     image_name = None
     image_version_number = None
+
     if ":image/" in image_arn:
         image_name = image_arn.split(":image/")[1]
     elif ":image-version/" in image_arn:
         [
             image_arn_prefix,
             image_name,
             image_version_number,
@@ -109,23 +125,24 @@
 
     return ImageMetadata(
         image_arn=image_version.get("ImageArn"),
         image_display_name=image_details.get("DisplayName"),
         ecr_uri=image_version.get("BaseImage"),
         # default values from here - https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAppImageConfig.html
         mount_path=file_system_config.get("MountPath", "/home/sagemaker-user"),
-        uid=str(file_system_config.get("DefaultUid", 0)),
-        gid=str(file_system_config.get("DefaultGid", 0)),
+        uid=str(file_system_config.get("DefaultUid", 1000)),
+        gid=str(file_system_config.get("DefaultGid", 100)),
     )
 
 
 @alru_cache(maxsize=1)
 async def get_image_metadata_jupyterlab() -> ImageMetadata:
     # For JupyterLab apps, we will always use the same image customer use to start JupyterLap
     # apps for notebook jobs
+
     if is_custom_image():
         try:
             return await get_third_party_image()
         except:
             raise SchedulerError(
                 f"Unable to find metadata for current JupyterLab app"
             )
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/revenue.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/revenue.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/providers/tags.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/providers/tags.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,32 +22,48 @@
         tags += [
             {
                 "Key": f"sagemaker:{user_details.user_id_key}-name",
                 "Value": user_details.user_id_value,
             }
         ]
         sm_client = get_sagemaker_client()
-        user_arn = ""
+        user_arns = []
         if user_details.user_id_key == UserTypes.SHARED_SPACE_USER:
             space_details = await sm_client.describe_space(
                 domain_id=get_domain_id(), space_name=user_details.user_id_value
             )
-            user_arn = space_details["SpaceArn"]
+            user_arns.append(space_details["SpaceArn"])
+
+            owner_user_profile_name = space_details.get("OwnershipSettings", {}).get("OwnerUserProfileName", None)
+            if owner_user_profile_name:
+                tags += [
+                    {
+                        "Key": f"sagemaker:{UserTypes.PROFILE_USER}-name",
+                        "Value": owner_user_profile_name,
+                    }
+                ]
+                owner_user_profile_details = await sm_client.describe_user_profile(
+                    domain_id=get_domain_id(), user_profile_name=owner_user_profile_name
+                )
+                user_arns.append(owner_user_profile_details["UserProfileArn"])
         else:
             user_profile = await sm_client.describe_user_profile(
                 domain_id=get_domain_id(), user_profile_name=user_details.user_id_value
             )
-            user_arn = user_profile["UserProfileArn"]
+            user_arns.append(user_profile["UserProfileArn"])
 
-        user_tags = await sm_client.list_tags(resource_arn=user_arn)
+        user_tags = []
+        for user_arn in user_arns:
+          user_tags += (await sm_client.list_tags(resource_arn=user_arn))["Tags"]
         logger.info(f"user profile tags retrieved - {user_tags}")
+
         # filter any "aws:" internal tags, this is needed because Looseleaf adds aws: tags for beta & gamma stacks
         # this change will also protect us from any future internal aws: tags added by Sagemaker
         sanitized_tags = [
-            tag for tag in user_tags["Tags"] if not tag["Key"].startswith("aws:")
+            tag for tag in user_tags if not tag["Key"].startswith("aws:")
         ]
         logger.info(f"sanitized user profile tags - {sanitized_tags}")
     return tags + sanitized_tags
 
 
 def _get_base_tags(
     job_name: str, notebook_name: str, headless_driver_version: str
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/scheduler.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,14 +364,20 @@
     async def list_jobs(
         self, query: ListJobsQuery, metrics: MetricsContext
     ) -> ListJobsResponse:
         """Returns list of all jobs filtered by query"""
 
         self.log.info("Calling SageMaker Search...")
 
+        # max_items has default value and if it's overridden as 0, return empty list without calling
+        # search API. Max_items as 0 is used by a contract from OSS side to detect the
+        # scheduler extension availability.
+        if query.max_items == 0:
+            return ListJobsResponse(jobs=[])
+
         try:
             training_job_list_response = await self.sagemaker_client().search(
                 self.converter.to_training_job_search_input(query)
             )
         except Exception as error:
             self.handle_aws_client_error(
                 error, f"Error when calling SageMaker Search: {error}"
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/stack_trace_filter.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/stack_trace_filter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -823,14 +823,24 @@
         actual_filters,
         expected_common_filters,
         key_name="Name",
     )
 
 
 @pytest.mark.asyncio
+async def test_list_job_with_max_items_as_zero():
+    scheduler = create_scheduler_with_mocked_dependencies()
+    query = MagicMock()
+    query.max_items = 0
+
+    response = await scheduler.list_jobs(query)
+    assert response.jobs == []
+
+
+@pytest.mark.asyncio
 async def test_prepare_job_artifacts_region_check_same_bucket():
     BUCKET_REGION = "us-west-2"
     AWS_REGION = "us-east-1"
     scheduler = create_scheduler_with_mocked_dependencies()
     mock_runtime_envs = MagicMock()
     TEST_S3_BUCKET_NAME = "customer-bucket"
     TEST_S3_INPUT = f"s3://{TEST_S3_BUCKET_NAME}/scheduling"
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/tests/test_stack_trace_filter.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/tests/test_stack_trace_filter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/util/constants.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/util/constants.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler/utils.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-sagemaker-jupyter-scheduler
-Version: 3.0.7
+Version: 3.0.9
 Summary: Amazon SageMaker Jupyter Scheduler based on the https://pypi.org/project/jupyter-scheduler/
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Scheduling Notebooks,Notebooks,Amazon Sagemaker
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,26 +51,25 @@
 amazon_sagemaker_jupyter_scheduler.egg-info/not-zip-safe
 amazon_sagemaker_jupyter_scheduler.egg-info/requires.txt
 amazon_sagemaker_jupyter_scheduler.egg-info/top_level.txt
 amazon_sagemaker_jupyter_scheduler/advanced_environments/__init__.py
 amazon_sagemaker_jupyter_scheduler/advanced_environments/base_advanced_environments.py
 amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py
 amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py
-amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json
 amazon_sagemaker_jupyter_scheduler/labextension/package.json
 amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
 amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
 amazon_sagemaker_jupyter_scheduler/labextension/static/240.145b0024b0b19e6c54a7.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/240.145b0024b0b19e6c54a7.js.LICENSE.txt
 amazon_sagemaker_jupyter_scheduler/labextension/static/543.3b5f882f510e08e43423.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/673.1543875757f3fa999f79.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/75.454a593e3b6ddf9464fb.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/827.56fabfcc2be29102ab30.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/827.56fabfcc2be29102ab30.js.LICENSE.txt
-amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.7e06320a8ba69020b115.js
+amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.5393ffde93b2d5747094.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
 amazon_sagemaker_jupyter_scheduler/providers/__init__.py
 amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
 amazon_sagemaker_jupyter_scheduler/providers/jupyterlab_image_metadata.py
 amazon_sagemaker_jupyter_scheduler/providers/revenue.py
 amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
@@ -85,14 +84,15 @@
 amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py
 amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py
 amazon_sagemaker_jupyter_scheduler/tests/test_environments.py
 amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py
 amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py
 amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py
 amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py
+amazon_sagemaker_jupyter_scheduler/tests/test_jupyterlab_image_metadata.py
 amazon_sagemaker_jupyter_scheduler/tests/test_logging.py
 amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py
 amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py
 amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py
 amazon_sagemaker_jupyter_scheduler/tests/test_stack_trace_filter.py
 amazon_sagemaker_jupyter_scheduler/tests/test_utils.py
 amazon_sagemaker_jupyter_scheduler/tests/helpers/__init__.py
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/host_region_mapping.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/host_region_mapping.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/jest.config.base.js` & `amazon_sagemaker_jupyter_scheduler-3.0.9/jest.config.base.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/jest.config.js` & `amazon_sagemaker_jupyter_scheduler-3.0.9/jest.config.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/package-lock.json` & `amazon_sagemaker_jupyter_scheduler-3.0.9/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166626055880442%*

 * *Differences: {"'packages'": "{'': {'version': '3.0.9'}}", "'version'": "'3.0.9'"}*

```diff
@@ -8878,15 +8878,15 @@
                 "jest-environment-jsdom": "^29.7.0",
                 "npm-run-all": "^4.1.5",
                 "ts-jest": "29.1.1",
                 "typescript": "^4.9.5"
             },
             "license": "Apache 2.0",
             "name": "@amzn/sagemaker-jupyter-scheduler",
-            "version": "3.0.7"
+            "version": "3.0.9"
         },
         "node_modules/@adobe/css-tools": {
             "dev": true,
             "integrity": "sha512-/62yikz7NLScCGAAST5SHdnjaDJQBDq0M2muyRTpf2VQhw6StBg2ALiu73zSJQ4fMVLA+0uBhBHAle7Wg+2kSg==",
             "license": "MIT",
             "version": "4.3.1"
         },
@@ -21812,9 +21812,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "license": "MIT",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "3.0.7"
+    "version": "3.0.9"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/package.json` & `amazon_sagemaker_jupyter_scheduler-3.0.9/amazon_sagemaker_jupyter_scheduler/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.961111111111111%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.5393ffde93b2d5747094.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'version'": "'3.0.9'"}*

```diff
@@ -61,14 +61,18 @@
     "files": [
         "dist/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.5393ffde93b2d5747094.js"
+        },
         "disabledExtensions": [
             "@jupyterlab/scheduler:IAdvancedOptions",
             "@jupyterlab/scheduler:TelemetryHandler"
         ],
         "extension": true,
         "outputDir": "amazon_sagemaker_jupyter_scheduler/labextension",
         "schemaDir": "schema",
@@ -123,9 +127,9 @@
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "test:watch": "jest --watch",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "3.0.7"
+    "version": "3.0.9"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/setup.py` & `amazon_sagemaker_jupyter_scheduler-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/__tests__/CreateNotebookJobForm.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/__tests__/CreateNotebookJobForm.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/__tests__/VpcCheckbox.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/__tests__/VpcCheckbox.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/__tests__/initalValueHelpers.spec.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/__tests__/initalValueHelpers.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/__tests__/validationHelpers.spec.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/__tests__/validationHelpers.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/Link.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/Link.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/RouterLink.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/RouterLink.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/__test__/Link.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/__test__/Link.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/link/__test__/RouterLink.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/link/__test__/RouterLink.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/selectinput/SelectInput.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/selectinput/SelectInput.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/selectinput/types.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/selectinput/types.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/TextInput.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/TextInput.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/__tests__/TextInput.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/__tests__/TextInput.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/textinput/styles.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/textinput/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/tooltip/Tooltip.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/tooltip/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/tooltip/__tests__/Tooltip.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/tooltip/__tests__/Tooltip.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/components/tooltip/styles.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/components/tooltip/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/constants/common.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/constants/common.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/plugins/ScheduleNotebookPlugin.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/plugins/ScheduleNotebookPlugin.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/plugins/SchedulerTelemetryPlugin.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/plugins/SchedulerTelemetryPlugin.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/themeProvider.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/themeProvider.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/PluginEnvironmentProvider.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/PluginEnvironmentProvider.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/images.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/images.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/kernels.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/kernels.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/utils/rendering.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/utils/rendering.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJob.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJob.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/InputContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/InputContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/JupyterLabJobEnvironment.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/JupyterLabJobEnvironment.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/CreateNotebookJobForm/styles.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/CreateNotebookJobForm/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/mockResponses.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/mockResponses.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/src/widgets/styles.ts` & `amazon_sagemaker_jupyter_scheduler-3.0.9/src/widgets/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-3.0.7/tsconfig.json` & `amazon_sagemaker_jupyter_scheduler-3.0.9/tsconfig.json`

 * *Files identical despite different names*

