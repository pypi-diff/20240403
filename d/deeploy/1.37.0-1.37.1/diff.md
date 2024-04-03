# Comparing `tmp/deeploy-1.37.0.tar.gz` & `tmp/deeploy-1.37.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeploy-1.37.0.tar", last modified: Fri Mar 29 10:00:12 2024, max compression
+gzip compressed data, was "deeploy-1.37.1.tar", last modified: Wed Apr  3 13:41:30 2024, max compression
```

## Comparing `deeploy-1.37.0.tar` & `deeploy-1.37.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.761710 deeploy-1.37.0/
--rw-rw-rw-   0 root         (0) root         (0)    11346 2024-03-29 09:57:27.000000 deeploy-1.37.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      926 2024-03-29 10:00:12.761710 deeploy-1.37.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1900 2024-03-29 09:57:27.000000 deeploy-1.37.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.753710 deeploy-1.37.0/deeploy/
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.753710 deeploy-1.37.0/deeploy/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.753710 deeploy-1.37.0/deeploy/cli/custom_instances/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/custom_instances/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3608 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/custom_instances/explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/custom_instances/model.py
--rw-rw-rw-   0 root         (0) root         (0)      864 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/custom_instances/model_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1878 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/custom_instances/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     7147 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/deeploycli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/cli/deploy_instances/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/deploy_instances/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3137 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/deploy_instances/deeploy_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     3732 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/deploy_instances/deeploy_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1885 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/deploy_instances/deeploy_transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     4894 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/cli/parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/parsers/parser_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/parsers/parser_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/parsers/parser_transformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/cli/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/cli/templates/explainer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/templates/explainer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/cli/templates/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/templates/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/cli/templates/transformer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/templates/transformer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/cli/wrappers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/wrappers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/wrappers/explainer_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/wrappers/model_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1748 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/cli/wrappers/transformer_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)    20741 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/common/
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/common/constants/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/common/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/common/constants/pytorch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/common/functions/
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/common/functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/common/functions/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/deepfair/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/deepfair/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6402 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/deepfair/fair.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.757710 deeploy-1.37.0/deeploy/enums/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/enums/algo.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/enums/auth_type.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/enums/explainer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/enums/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/enums/prediction_version.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/enums/qf.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/enums/query_param.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/enums/transformer_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.761710 deeploy-1.37.0/deeploy/fairsd/
--rw-rw-rw-   0 root         (0) root         (0)      275 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/fairsd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29012 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/fairsd/algorithms.py
--rw-rw-rw-   0 root         (0) root         (0)    12988 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/fairsd/discretization.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/fairsd/qualitymeasures.py
--rw-rw-rw-   0 root         (0) root         (0)     8018 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/fairsd/searchspace.py
--rw-rw-rw-   0 root         (0) root         (0)     7340 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/fairsd/sgdescription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.761710 deeploy-1.37.0/deeploy/models/
--rw-rw-rw-   0 root         (0) root         (0)     1543 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/actual_response.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/client_options.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_actuals.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_azure_ml_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     6087 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_deployment_base.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_explainer_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     2295 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_model_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_sagemaker_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/create_transformer_reference.py
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/feature.py
--rw-rw-rw-   0 root         (0) root         (0)     3455 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/get_prediction_logs_options.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/metadata_json.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/prediction_log.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/reference_json.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/update_azure_ml_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     6286 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/update_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/update_deployment_base.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/update_deployment_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/update_sagemaker_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/models/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.761710 deeploy-1.37.0/deeploy/services/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16781 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/deeploy_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4727 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/explainer_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.761710 deeploy-1.37.0/deeploy/services/explainers/
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/explainers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1292 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/explainers/alibi.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/explainers/base_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1382 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/explainers/omni_tabular.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/explainers/shap.py
--rw-rw-rw-   0 root         (0) root         (0)     3432 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/file_service.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/git_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3369 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/model_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.761710 deeploy-1.37.0/deeploy/services/models/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/models/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/models/onnx.py
--rw-rw-rw-   0 root         (0) root         (0)     3161 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/models/pytorch.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/models/sklearn.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/models/tensorflow.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/models/triton.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2024-03-29 09:57:27.000000 deeploy-1.37.0/deeploy/services/models/xgboost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.753710 deeploy-1.37.0/deeploy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      926 2024-03-29 10:00:12.000000 deeploy-1.37.0/deeploy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3647 2024-03-29 10:00:12.000000 deeploy-1.37.0/deeploy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 10:00:12.000000 deeploy-1.37.0/deeploy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-03-29 10:00:12.000000 deeploy-1.37.0/deeploy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      279 2024-03-29 10:00:12.000000 deeploy-1.37.0/deeploy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-29 10:00:12.000000 deeploy-1.37.0/deeploy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-29 10:00:12.761710 deeploy-1.37.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1929 2024-03-29 09:57:27.000000 deeploy-1.37.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 10:00:12.761710 deeploy-1.37.0/test/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-29 09:57:27.000000 deeploy-1.37.0/test/test_deeploy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.552092 deeploy-1.37.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11346 2024-04-03 13:31:52.000000 deeploy-1.37.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      926 2024-04-03 13:41:30.552092 deeploy-1.37.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2024-04-03 13:31:52.000000 deeploy-1.37.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.528092 deeploy-1.37.1/deeploy/
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.532092 deeploy-1.37.1/deeploy/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.532092 deeploy-1.37.1/deeploy/cli/custom_instances/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/model_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/custom_instances/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7147 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deeploycli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.532092 deeploy-1.37.1/deeploy/cli/deploy_instances/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deploy_instances/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3137 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4894 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/parsers/parser_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/parsers/parser_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/parsers/parser_transformer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/templates/explainer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/templates/explainer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/templates/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/templates/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/templates/transformer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/templates/transformer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/cli/wrappers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/wrappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/wrappers/explainer_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/wrappers/model_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/cli/wrappers/transformer_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)    20741 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/common/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/common/constants/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/constants/pytorch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.536092 deeploy-1.37.1/deeploy/common/functions/
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/common/functions/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.540092 deeploy-1.37.1/deeploy/deepfair/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/deepfair/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6549 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/deepfair/fair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.540092 deeploy-1.37.1/deeploy/enums/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/algo.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/auth_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/explainer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/prediction_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/qf.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/query_param.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/enums/transformer_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.544092 deeploy-1.37.1/deeploy/fairsd/
+-rw-rw-rw-   0 root         (0) root         (0)      275 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30522 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/algorithms.py
+-rw-rw-rw-   0 root         (0) root         (0)    13196 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/discretization.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/qualitymeasures.py
+-rw-rw-rw-   0 root         (0) root         (0)     8381 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/searchspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     7701 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/fairsd/sgdescription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.548092 deeploy-1.37.1/deeploy/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/actual_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/client_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      714 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_actuals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_azure_ml_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     6088 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_deployment_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_explainer_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2295 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_model_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_sagemaker_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/create_transformer_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/get_prediction_logs_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/metadata_json.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)      781 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/prediction_log.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/reference_json.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_azure_ml_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     6287 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_deployment_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_deployment_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/update_sagemaker_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/models/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.548092 deeploy-1.37.1/deeploy/services/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16781 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/deeploy_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainer_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.548092 deeploy-1.37.1/deeploy/services/explainers/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/alibi.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/base_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1382 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/omni_tabular.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/explainers/shap.py
+-rw-rw-rw-   0 root         (0) root         (0)     3432 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/file_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/git_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3369 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/model_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.552092 deeploy-1.37.1/deeploy/services/models/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/onnx.py
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/pytorch.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/sklearn.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/tensorflow.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/triton.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-04-03 13:31:52.000000 deeploy-1.37.1/deeploy/services/models/xgboost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.528092 deeploy-1.37.1/deeploy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      926 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3647 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 13:41:30.000000 deeploy-1.37.1/deeploy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 13:41:30.552092 deeploy-1.37.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2024-04-03 13:31:52.000000 deeploy-1.37.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:30.552092 deeploy-1.37.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-03 13:31:52.000000 deeploy-1.37.1/test/test_deeploy.py
```

### Comparing `deeploy-1.37.0/LICENSE` & `deeploy-1.37.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/PKG-INFO` & `deeploy-1.37.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeploy
-Version: 1.37.0
+Version: 1.37.1
 Summary: The official Deeploy client for Python
 Home-page: https://gitlab.com/deeploy-ml/deeploy-python-client
 Author: Tim Kleinloog
 Author-email: opensource@deeploy.ml
 License: UNKNOWN
 Project-URL: Documentation, https://deeploy-ml.gitlab.io/deeploy-python-client/
 Project-URL: Deeploy website, https://deeploy.ml
```

### Comparing `deeploy-1.37.0/README.md` & `deeploy-1.37.1/README.md`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/__init__.py` & `deeploy-1.37.1/deeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/custom_instances/explainer.py` & `deeploy-1.37.1/deeploy/cli/custom_instances/explainer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/custom_instances/model.py` & `deeploy-1.37.1/deeploy/cli/custom_instances/model.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/custom_instances/model_repository.py` & `deeploy-1.37.1/deeploy/cli/custom_instances/model_repository.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/custom_instances/transformer.py` & `deeploy-1.37.1/deeploy/cli/custom_instances/transformer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/deeploycli.py` & `deeploy-1.37.1/deeploy/cli/deeploycli.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/deploy_instances/deeploy_explainer.py` & `deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_explainer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/deploy_instances/deeploy_model.py` & `deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_model.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/deploy_instances/deeploy_transformer.py` & `deeploy-1.37.1/deeploy/cli/deploy_instances/deeploy_transformer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/interface.py` & `deeploy-1.37.1/deeploy/cli/interface.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/parsers/parser_explainer.py` & `deeploy-1.37.1/deeploy/cli/parsers/parser_explainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,18 +139,15 @@
         "--verbose_every",
         type=int,
         action=GroupedAction,
         dest="explainer.verbose_every",
         default=argparse.SUPPRESS,
     )
     parser.add_argument(
-        "--transformer",
-        help="Transformer present",
-        default=argparse.SUPPRESS,
-        type=str2bool
+        "--transformer", help="Transformer present", default=argparse.SUPPRESS, type=str2bool
     )
 
 
 def parse_args_explainer(sys_args):
     parser = argparse.ArgumentParser(parents=[kserve.model_server.parser])
     parser.add_argument(
         "--storage_uri",
@@ -158,23 +155,16 @@
         default=os.environ.get(ENV_STORAGE_URI),
     )
     parser.add_argument(
         "--model_name",
         default=DEFAULT_EXPLAINER_NAME,
         help="The name of model explainer.",
     )
-    parser.add_argument(
-        "--predictor_host", help="The host for the predictor", required=True
-    )
-    parser.add_argument(
-        "--transformer",
-        help="Transformer present",
-        default=False,
-        type=str2bool
-    )
+    parser.add_argument("--predictor_host", help="The host for the predictor", required=True)
+    parser.add_argument("--transformer", help="Transformer present", default=False, type=str2bool)
 
     args, _ = parser.parse_known_args(sys_args)
 
     argdDict = vars(args).copy()
     if "explainer" in argdDict:
         extra = vars(args.explainer)
     else:
```

### Comparing `deeploy-1.37.0/deeploy/cli/parsers/parser_model.py` & `deeploy-1.37.1/deeploy/cli/parsers/parser_model.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/parsers/parser_transformer.py` & `deeploy-1.37.1/deeploy/cli/parsers/parser_transformer.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/utils.py` & `deeploy-1.37.1/deeploy/cli/utils.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/wrappers/explainer_wrapper.py` & `deeploy-1.37.1/deeploy/cli/wrappers/explainer_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/wrappers/model_wrapper.py` & `deeploy-1.37.1/deeploy/cli/wrappers/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/cli/wrappers/transformer_wrapper.py` & `deeploy-1.37.1/deeploy/cli/wrappers/transformer_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/client.py` & `deeploy-1.37.1/deeploy/client.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/common/constants/pytorch.py` & `deeploy-1.37.1/deeploy/common/constants/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/common/functions/functions.py` & `deeploy-1.37.1/deeploy/common/functions/functions.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/deepfair/fair.py` & `deeploy-1.37.1/deeploy/deepfair/fair.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         X: Union[pd.DataFrame, np.array],
         y_true: Union[pd.DataFrame, np.array],
         y_pred: Union[pd.DataFrame, np.array],
         feature_names: list[str] = None,
         sensitive_features: list[str] = None,
         nominal_features: list[str] = None,
         numeric_features: list[str] = None,
-        ignore_features: list[str] =  None
+        ignore_features: list[str] = None,
     ):
         """
         X : pandas dataframe or numpy array
         y_true : numpy array, pandas dataframe, or pandas Series
             represent the ground truth
         y_pred : numpy array, pandas dataframe, or pandas Series
             contain the predicted values
@@ -47,35 +47,40 @@
         self.y_pred = y_pred
         self.feature_names = feature_names
         self.sensitive_features = sensitive_features
         self.nominal_features = nominal_features
         self.numeric_features = numeric_features
         if ignore_features:
             if sensitive_features:
-                self.ignore_features = list(set(ignore_features)^set(sensitive_features))
+                self.ignore_features = list(set(ignore_features) ^ set(sensitive_features))
             else:
                 self.ignore_features = ignore_features
             if len(ignore_features) > len(self.ignore_features):
-                raise Exception("Sensitive features found in ignore features list. Cannot ignore provided sensitive features")
+                raise Exception(
+                    "Sensitive features found in ignore features list. Cannot ignore provided sensitive features"
+                )
             if self.ignore_features:
                 self.X = self.X.drop(self.ignore_features, axis=1)
                 if self.nominal_features:
-                    self.nominal_features = list(set(self.nominal_features)^set(self.ignore_features))
+                    self.nominal_features = list(
+                        set(self.nominal_features) ^ set(self.ignore_features)
+                    )
                 if self.numeric_features:
-                    self.numeric_features = list(set(self.numeric_features)^set(self.ignore_features))
-
+                    self.numeric_features = list(
+                        set(self.numeric_features) ^ set(self.ignore_features)
+                    )
 
     def find_sub_groups(
         self,
         quality_factor: QualityFactor,
         algorithm: SearchAlgorithm = SearchAlgorithm.dssd,
         beam_width: int = 20,
         a: float = 0.9,
-        result_set_size:int = 5,
-        **kwargs
+        result_set_size: int = 5,
+        **kwargs,
     ) -> ResultSet:
         """
         :param quality_factor: QualityFactor this parameter corresponds to the choice of quality factor
         :param algorithm: SearchAlgorithm this parameter corresponds to the choice of search algorithm to utilize to obtain sub groups
         :param beam_width: int
         :param a: float this parameter correspond to the alpha parameter. the more a is high, the less the subgroups redundancy is taken into account.
         """
@@ -85,65 +90,63 @@
             self.y_true,
             self.y_pred,
             qf=str(quality_factor),
             feature_names=self.feature_names,
             sensitive_features=self.sensitive_features,
             nominal_features=self.nominal_features,
             numeric_features=self.numeric_features,
-            result_set_size = result_set_size
+            result_set_size=result_set_size,
         )
 
         if algorithm == SearchAlgorithm.beam_search:
             result_set = fsd.BeamSearch(beam_width=beam_width).execute(task)
         elif algorithm == SearchAlgorithm.dssd:
             result_set = fsd.DSSD(beam_width=beam_width, a=a).execute(task)
 
         self.result_set = result_set
         return result_set
 
     def get_subgroup_mask(self, index: int = 0) -> list[bool]:
         """
-        This method generate and return the feature of the subgroup with index = sg_index in the current object. 
-            The result is indeed a boolean array of the same length of the dataset X. 
+        This method generate and return the feature of the subgroup with index = sg_index in the current object.
+            The result is indeed a boolean array of the same length of the dataset X.
             Each i-th element of this array is true iff the i-th tuple of X belong to the subgroup with index sg_index.
-        :param index: int subgroup_index 
+        :param index: int subgroup_index
         :return boolean: mapping for subgroup wrt to original dataset
         """
         sg_feature = self.result_set.sg_feature(sg_index=index, X=self.X)
         return sg_feature
-    
+
     def get_subgroup_description(self, index: int = 0) -> Description:
         """
         This method returns description of subgroup at provided index from resultset
-        :param index: int subgroup_index 
+        :param index: int subgroup_index
         """
         return self.result_set.get_description(index)
-    
-    def get_user_defined_subgroup(self, multi_condition_func) ->  pd.DataFrame:
-        return self.X.apply(multi_condition_func, axis=1).astype('bool')
-    
+
+    def get_user_defined_subgroup(self, multi_condition_func) -> pd.DataFrame:
+        return self.X.apply(multi_condition_func, axis=1).astype("bool")
+
     def get_all_metrics_for_user_defined_subgroup(self, multi_condition_func):
         """
-        multi_condition_func: lambda function condition on row for defining subgroup. 
+        multi_condition_func: lambda function condition on row for defining subgroup.
             eg. lambda row: ((row['age'] > 35) & (row['sex'] in ['Male', 'Nonbinary']) )
         """
         defined_subgroup = self.get_user_defined_subgroup(multi_condition_func)
-        demographic_parity_difference_val =  demographic_parity_difference(y_true = self.y_true, y_pred = self.y_pred, sensitive_features = defined_subgroup)
-        demographic_parity_ratio_val = demographic_parity_ratio(y_true = self.y_true, y_pred = self.y_pred, sensitive_features = defined_subgroup)
-        equalized_odds_difference_val = equalized_odds_difference(y_true = self.y_true, y_pred = self.y_pred, sensitive_features = defined_subgroup)
-        equalized_odds_ratio_val = equalized_odds_ratio(y_true = self.y_true, y_pred = self.y_pred, sensitive_features = defined_subgroup)
+        demographic_parity_difference_val = demographic_parity_difference(
+            y_true=self.y_true, y_pred=self.y_pred, sensitive_features=defined_subgroup
+        )
+        demographic_parity_ratio_val = demographic_parity_ratio(
+            y_true=self.y_true, y_pred=self.y_pred, sensitive_features=defined_subgroup
+        )
+        equalized_odds_difference_val = equalized_odds_difference(
+            y_true=self.y_true, y_pred=self.y_pred, sensitive_features=defined_subgroup
+        )
+        equalized_odds_ratio_val = equalized_odds_ratio(
+            y_true=self.y_true, y_pred=self.y_pred, sensitive_features=defined_subgroup
+        )
         return (
-           ("demographic_parity_difference", demographic_parity_difference_val),
-           ("demographic_parity_ratio", demographic_parity_ratio_val),
-           ("equalized_odds_difference", equalized_odds_difference_val),
-           ("equalized_odds_ratio", equalized_odds_ratio_val),
+            ("demographic_parity_difference", demographic_parity_difference_val),
+            ("demographic_parity_ratio", demographic_parity_ratio_val),
+            ("equalized_odds_difference", equalized_odds_difference_val),
+            ("equalized_odds_ratio", equalized_odds_ratio_val),
         )
-        
-    
-
-    
-
-    
-    
-
-    
-
```

### Comparing `deeploy-1.37.0/deeploy/fairsd/algorithms.py` & `deeploy-1.37.1/deeploy/fairsd/algorithms.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,50 +10,47 @@
 from deeploy.fairsd.sgdescription import Description
 
 """
 The class SubgroupDiscoveryTask is an adaptation of the homonymous class of the pysubgroup library.
 """
 
 quality_function_options = [
-    'equalized_odds_difference',
-    'equalized_odds_ratio',
-    'demographic_parity_difference',
-    'demographic_parity_ratio'
+    "equalized_odds_difference",
+    "equalized_odds_ratio",
+    "demographic_parity_difference",
+    "demographic_parity_ratio",
 ]
 
-quality_function_parameters = [
-    'y_true',
-    'y_pred',
-    'sensitive_features'
-]
+quality_function_parameters = ["y_true", "y_pred", "sensitive_features"]
 
 
 class SubgroupDiscoveryTask:
-    """This is an interface class and will contain all the parameters useful for the sg discovery algorithms.
-    """
-    def __init__(self,
-            X, # pandas dataframe or numpy array with features
-            y_true, # numpy array, pandas dataframe, or pandas Series with ground truth labels
-            y_pred = None, # numpy array, pandas dataframe, or pandas Series with classifier's predicted labels
-            feature_names=None, # optional, list with column names in case users supply a numpy array X
-            sensitive_features = None, #list of sensitive features names (str)
-            nominal_features = None, #optional, list of nominal features
-            numeric_features = None, #optional, list of nominal features
-            qf='equalized_odds_difference', # str or callable object
-            discretizer='equalfreq', # str
-            num_bins = 6,
-            dynamic_discretization=True, #boolean
-            result_set_size=5, # int
-            depth=3, # int
-            min_quality=0, # float
-            min_support=200, #int
-            min_support_ratio=0.1, #float
-            max_support_ratio=0.5, #float
-            logging_level=logging.INFO
-        ):
+    """This is an interface class and will contain all the parameters useful for the sg discovery algorithms."""
+
+    def __init__(
+        self,
+        X,  # pandas dataframe or numpy array with features
+        y_true,  # numpy array, pandas dataframe, or pandas Series with ground truth labels
+        y_pred=None,  # numpy array, pandas dataframe, or pandas Series with classifier's predicted labels
+        feature_names=None,  # optional, list with column names in case users supply a numpy array X
+        sensitive_features=None,  # list of sensitive features names (str)
+        nominal_features=None,  # optional, list of nominal features
+        numeric_features=None,  # optional, list of nominal features
+        qf="equalized_odds_difference",  # str or callable object
+        discretizer="equalfreq",  # str
+        num_bins=6,
+        dynamic_discretization=True,  # boolean
+        result_set_size=5,  # int
+        depth=3,  # int
+        min_quality=0,  # float
+        min_support=200,  # int
+        min_support_ratio=0.1,  # float
+        max_support_ratio=0.5,  # float
+        logging_level=logging.INFO,
+    ):
         """
         Parameters
         ----------
         X : pandas dataframe or numpy array
         y_true : numpy array, pandas dataframe, or pandas Series
             represent the ground truth
         y_pred : numpy array, pandas dataframe, or pandas Series
@@ -82,182 +79,225 @@
             minimum proportion of a subgroup compared to the whole dataset size
         max_support_ratio : float
             maximum proportion of a subgroup compared to the whole dataset size
         logging_level : int
             logging level
         """
         logging.basicConfig(level=logging_level)
-        self.inputChecking(X, y_true, y_pred, feature_names, sensitive_features, nominal_features, numeric_features,
-                           discretizer, dynamic_discretization, result_set_size, depth, min_quality, min_support, min_support_ratio)
+        self.inputChecking(
+            X,
+            y_true,
+            y_pred,
+            feature_names,
+            sensitive_features,
+            nominal_features,
+            numeric_features,
+            discretizer,
+            dynamic_discretization,
+            result_set_size,
+            depth,
+            min_quality,
+            min_support,
+            min_support_ratio,
+        )
         if isinstance(X, np.ndarray):
             self.data = pd.DataFrame(X, columns=feature_names)
         else:
             self.data = X.copy()
 
-        self.data['y_true'] = y_true
+        self.data["y_true"] = y_true
         if y_pred is not None:
-            self.data['y_pred'] = y_pred
-            self.there_is_y_pred =True
+            self.data["y_pred"] = y_pred
+            self.there_is_y_pred = True
         else:
             self.there_is_y_pred = False
-        self.sensitive_features=sensitive_features
-        self.discretizer = Discretizer(discretization_type=discretizer, target='y_true', num_bins=num_bins)
-        self.search_space = SearchSpace(self.data, ['y_true', 'y_pred'], nominal_features, numeric_features,
-                                        dynamic_discretization, self.discretizer, sensitive_features)
-
+        self.sensitive_features = sensitive_features
+        self.discretizer = Discretizer(
+            discretization_type=discretizer, target="y_true", num_bins=num_bins
+        )
+        self.search_space = SearchSpace(
+            self.data,
+            ["y_true", "y_pred"],
+            nominal_features,
+            numeric_features,
+            dynamic_discretization,
+            self.discretizer,
+            sensitive_features,
+        )
 
-        self.qf=self.set_qualityfuntion(qf)
+        self.qf = self.set_qualityfuntion(qf)
 
         self.result_set_size = result_set_size
         self.depth = depth
         self.min_quality = min_quality
         self.min_support = min_support
         self.min_support_ratio = min_support_ratio
         self.max_support_ratio = max_support_ratio
 
-
     def set_qualityfuntion(self, qf):
         if isinstance(qf, str):
             if qf not in quality_function_options:
-                raise ValueError('Quality function not known')
+                raise ValueError("Quality function not known")
             else:
                 return getattr(flm, qf)
 
         if not callable(qf):
-            RuntimeError('Supplied metric object must be callable or string')
+            RuntimeError("Supplied metric object must be callable or string")
         sig = inspect.signature(qf).parameters
         for par in quality_function_parameters:
             if par not in sig:
-                raise ValueError("Please use the functions in the fairlearn.metrics package as quality functions or "
-                                 "other fuctions with the same interface")
+                raise ValueError(
+                    "Please use the functions in the fairlearn.metrics package as quality functions or "
+                    "other fuctions with the same interface"
+                )
         return qf
 
-    def inputChecking(self,
-              X,  # pandas dataframe or numpy array
-              y_true,  # numpy array, pandas dataframe, or pandas Series with ground truth labels
-              y_pred,  # numpy array, pandas dataframe, or pandas Series with classifier's predicted labels
-              feature_names,  # optional, list with column names in case users supply a numpy array X
-              sensitive_features,
-              nominal_features,  # optional, list of nominal features
-              numeric_features,  # optional, list of nominal features
-              discretizer,  # str
-              dynamic_discretization,  # boolean
-              result_set_size,  # int
-              depth,  # int
-              min_quality,  # float
-              min_support,  # int
-              min_support_ratio # float
-        ):
+    def inputChecking(
+        self,
+        X,  # pandas dataframe or numpy array
+        y_true,  # numpy array, pandas dataframe, or pandas Series with ground truth labels
+        y_pred,  # numpy array, pandas dataframe, or pandas Series with classifier's predicted labels
+        feature_names,  # optional, list with column names in case users supply a numpy array X
+        sensitive_features,
+        nominal_features,  # optional, list of nominal features
+        numeric_features,  # optional, list of nominal features
+        discretizer,  # str
+        dynamic_discretization,  # boolean
+        result_set_size,  # int
+        depth,  # int
+        min_quality,  # float
+        min_support,  # int
+        min_support_ratio,  # float
+    ):
         if not (isinstance(X, pd.DataFrame) or isinstance(X, np.ndarray)):
             raise TypeError("X must be of type numpy.ndarray or pandas.DataFrame")
-        if not (isinstance(y_true, pd.DataFrame) or isinstance(y_true, np.ndarray) or isinstance(y_true, pd.Series)):
-            raise TypeError("y_true must be of type numpy.ndarray, pandas.Series or pandas.DataFrame")
+        if not (
+            isinstance(y_true, pd.DataFrame)
+            or isinstance(y_true, np.ndarray)
+            or isinstance(y_true, pd.Series)
+        ):
+            raise TypeError(
+                "y_true must be of type numpy.ndarray, pandas.Series or pandas.DataFrame"
+            )
         if X.shape[0] != y_true.size:
             raise RuntimeError("X and y_true have two different dimensions")
         if y_pred is not None:
-            if not (isinstance(y_pred, pd.DataFrame) or isinstance(y_pred, np.ndarray) or isinstance(y_pred, pd.Series)):
-                raise TypeError("y_pred must be of type numpy.ndarray, pandas.Series or pandas.DataFrame")
+            if not (
+                isinstance(y_pred, pd.DataFrame)
+                or isinstance(y_pred, np.ndarray)
+                or isinstance(y_pred, pd.Series)
+            ):
+                raise TypeError(
+                    "y_pred must be of type numpy.ndarray, pandas.Series or pandas.DataFrame"
+                )
             if y_pred.size != y_true.size:
                 raise RuntimeError("y_pred and y_true have two different dimensions")
         if isinstance(X, np.ndarray):
             if (not isinstance(feature_names, list)) or len(feature_names) != X.shape[1]:
-                raise RuntimeError("If X is a numpy.ndarray, feature_names must contain the names of the colums")
+                raise RuntimeError(
+                    "If X is a numpy.ndarray, feature_names must contain the names of the colums"
+                )
         if sensitive_features is not None and not isinstance(sensitive_features, list):
             raise RuntimeError("sensitive_features input must be of list type or None")
         if nominal_features is not None and not isinstance(nominal_features, list):
             raise RuntimeError("nominal_features input must be of list type or None")
         if numeric_features is not None and not isinstance(nominal_features, list):
             raise RuntimeError("numeric_features input must be of list type or None")
         if not isinstance(discretizer, str):
             raise TypeError("discretizer input must be of string type")
         if discretizer == "mdlp":
             t = pd.DataFrame(y_true).iloc[:, 0].unique()
-            if not (t ==[1,0]).all() and not (t ==[0,1]).all():
+            if not (t == [1, 0]).all() and not (t == [0, 1]).all():
                 raise RuntimeError("MDLP discretization supports only binary target")
         if not isinstance(dynamic_discretization, bool):
             raise TypeError("dynamic_discretization input must be of bool type")
         if not isinstance(dynamic_discretization, bool):
             raise TypeError("dynamic_discretization input must be of bool type")
-        if not isinstance(result_set_size, int) or result_set_size<1:
+        if not isinstance(result_set_size, int) or result_set_size < 1:
             raise RuntimeError("result_set_size input must be greater than 0")
         if not isinstance(depth, int):
             raise RuntimeError("depth input must be greater than 0")
         if not isinstance(min_support, int):
             raise RuntimeError("min_support input must be greater than 0")
         if not isinstance(min_support_ratio, float):
             raise RuntimeError("min_support_ratio input must be of float type")
-        if min_quality>1 or min_quality<0:
+        if min_quality > 1 or min_quality < 0:
             raise RuntimeError("min_quality input must be between 0 and 1")
 
 
 class ResultSet:
     """
     This class is used to represent the subgroup set found by one of the
     subgroup discovery algorithms implemented in this package.
     """
+
     def __init__(self, descriptions_list, x_size):
         """
         :param descriptions_list: list of Description objects
         :param x_size: int, size of the dataset
         """
-        self.descriptions_list=descriptions_list
+        self.descriptions_list = descriptions_list
         self.X_size = x_size
 
     def to_dataframe(self):
-        """ Convert the result set into a dataframe
+        """Convert the result set into a dataframe
 
         :return: pandas.Dataframe
         """
-        lod=list()
+        lod = list()
         for d in self.descriptions_list:
-            row = [d.quality, d.__repr__(), d.support, d.support/self.X_size]
+            row = [d.quality, d.__repr__(), d.support, d.support / self.X_size]
             lod.append(row)
-        columns = ['quality', 'description', 'size', 'proportion']
+        columns = ["quality", "description", "size", "proportion"]
         index = [str(x) for x in range(len(self.descriptions_list))]
         return pd.DataFrame(lod, index=index, columns=columns)
 
     def get_description(self, sg_index):
-        if (sg_index >= len(self.descriptions_list) or sg_index < 0):
+        if sg_index >= len(self.descriptions_list) or sg_index < 0:
             raise RuntimeError("The requested subgroup doesn't exists")
         return self.descriptions_list[sg_index]
 
-    def sg_feature(self,sg_index, X):
+    def sg_feature(self, sg_index, X):
         """
         This method generate and return the feature of the subgroup with index = sg_index in the current object.
         The result is indeed a boolean array of the same length of the dataset X. Each i-th element of this
         array is true iff the i-th tuple of X belong to the subgroup with index sg_index.
 
         :param sg_index: int, number of the subgroup in the current object
         :param X: pandas DataFrame or numpy array
         :return: boolean list
         """
-        if(sg_index>=len(self.descriptions_list) or sg_index<0):
+        if sg_index >= len(self.descriptions_list) or sg_index < 0:
             raise RuntimeError("The requested subgroup doesn't exists")
-        return pd.Series(self.descriptions_list[sg_index].to_boolean_array(X), name=str("sg"+str(sg_index)))
+        return pd.Series(
+            self.descriptions_list[sg_index].to_boolean_array(X),
+            name=str("sg" + str(sg_index)),
+        )
 
     def __repr__(self):
-        res=""
+        res = ""
         for desc in self.descriptions_list:
-            res+= desc.__repr__() + "\n"
+            res += desc.__repr__() + "\n"
         return res
 
     def print(self):
         print(self.__repr__())
 
     def to_string(self):
         return self.__repr__()
 
 
 class BeamSearch:
     """This class is used to execute the Beam Search Algorithm."""
+
     def __init__(self, beam_width=20):
         """
         :param beam_width : int
         """
-        if beam_width<1:
+        if beam_width < 1:
             raise RuntimeError("beam_width must be greater than 0")
         self.beam_width = beam_width
 
     def execute(self, task):
         """
         This method execute the Beam Search
 
@@ -266,96 +306,111 @@
 
         Notes
         -----
         The list_of_beam variable is: a list of list of descriptions. The i-th element of list_of_beam, at the end,
         will contain the most interesting descriptions formed by i descriptors.
         """
         if self.beam_width < task.result_set_size:
-            raise RuntimeError('Beam width is smaller than the result set size!')
+            raise RuntimeError("Beam width is smaller than the result set size!")
 
-        list_of_beam=list()
+        list_of_beam = list()
         list_of_beam.append(list())
-        list_of_beam[0] =[Description()]
+        list_of_beam[0] = [Description()]
 
         depth = 0
         while depth < task.depth:
             list_of_beam.append(list())
-            #print(depth)
+            # print(depth)
             current_min_quality = 1
             for last_sg in list_of_beam[depth]:
-                ss = task.search_space.extract_search_space(task.data, task.discretizer, current_description=last_sg)
+                ss = task.search_space.extract_search_space(
+                    task.data, task.discretizer, current_description=last_sg
+                )
                 for sel in ss:
                     new_Descriptors = list(last_sg.Descriptors)
                     new_Descriptors.append(sel)
-                    new_description=Description(new_Descriptors)
+                    new_description = Description(new_Descriptors)
 
                     # check for duplicates
                     if new_description.is_present_in(list_of_beam[depth + 1]):
                         continue
 
-                    sg_belonging_feature = new_description.to_boolean_array(task.data, set_attributes=True)
+                    sg_belonging_feature = new_description.to_boolean_array(
+                        task.data, set_attributes=True
+                    )
                     # check min support
-                    if new_description.size(task.data)<task.min_support \
-                        or new_description.size(task.data)<task.min_support_ratio*task.data.shape[0] \
-                            or new_description.size(task.data)>task.max_support_ratio*task.data.shape[0]:
+                    if (
+                        new_description.size(task.data) < task.min_support
+                        or new_description.size(task.data)
+                        < task.min_support_ratio * task.data.shape[0]
+                        or new_description.size(task.data)
+                        > task.max_support_ratio * task.data.shape[0]
+                    ):
                         continue
                     # evaluate subgroup
                     if task.there_is_y_pred:
-                        quality=task.qf(y_true = task.data['y_true'], y_pred = task.data['y_pred'],
-                                        sensitive_features =sg_belonging_feature)
+                        quality = task.qf(
+                            y_true=task.data["y_true"],
+                            y_pred=task.data["y_pred"],
+                            sensitive_features=sg_belonging_feature,
+                        )
                     else:
-                        quality = task.qf(y_true=task.data['y_true'], sensitive_features=sg_belonging_feature)
+                        quality = task.qf(
+                            y_true=task.data["y_true"],
+                            sensitive_features=sg_belonging_feature,
+                        )
                     if quality < task.min_quality:
                         continue
                     new_description.set_quality(quality)
 
                     if len(list_of_beam[depth + 1]) < self.beam_width:
                         list_of_beam[depth + 1].append(new_description)
                         if current_min_quality > quality:
                             current_min_quality = quality
                     elif quality > current_min_quality:
-                        i=0
+                        i = 0
                         while list_of_beam[depth + 1][i].quality != current_min_quality:
                             i = i + 1
                         list_of_beam[depth + 1][i] = new_description
                         current_min_quality = 1
                         for d in list_of_beam[depth + 1]:
                             if d.quality < current_min_quality:
                                 current_min_quality = d.quality
-            depth +=1
+            depth += 1
 
-        subgroups=list()
+        subgroups = list()
         for beam in list_of_beam[1:]:
             subgroups.extend(beam)
         subgroups.sort(reverse=True)
-        return ResultSet(subgroups[:task.result_set_size], task.data.shape[0])
+        return ResultSet(subgroups[: task.result_set_size], task.data.shape[0])
 
 
 class DSSD:
     """
     This class implements the Diverse Subgroup Set Discovery algorithm (DSSD).
     This algorithm is a variant of the Beam Search Algorithm that also take into account
     the redundancy of the generated subgroups.
     In this implementation a cover-based redundancy definition is used: roughly, the more tuples two subgroups
     have in common, the more they are considered redundant.
     This algorithm is described in details in the Van Leeuwen and Knobbe's paper "Diverse Subgroup Set Discovery".
     """
+
     def __init__(self, beam_width=20, a=0.9):
         """
         :param beam_width: int
         :param a: float
             this parameter correspond to the alpha parameter.
             the more a is high, the less the subgroups redundancy is taken into account.
         """
-        if beam_width<1:
+        if beam_width < 1:
             raise RuntimeError("beam_width must be greater than 0")
-        if a<0 or a>1:
+        if a < 0 or a > 1:
             raise RuntimeError("a-parameter must be between 0 and 1")
-        self.beam_width=beam_width
-        self.a= 1-a # for future calculations it is more practical to memorize 1-a
+        self.beam_width = beam_width
+        self.a = 1 - a  # for future calculations it is more practical to memorize 1-a
 
     def execute(self, task):
         """
         :param task: SubgroupDiscoveryTask object
         :return: ResultSet object
 
         Notes
@@ -363,27 +418,27 @@
         The algorithm is divided in three phases:
         Phase 1: a modified beam search algorithm is performed to find a first non-redundant subset
         Phase 2: Dominance Pruning - the algorithm try to generalize the subgroups finded in the previous phase
         Phase 3: The subgroups to return are chosen among the sg-set resulting from the previous phase. Again, the
             subgroups to put in the result set are chosen by taking into account both quality and diversity.
         """
         if self.beam_width < task.result_set_size:
-            raise RuntimeError('Beam width is smaller than the result set size!')
+            raise RuntimeError("Beam width is smaller than the result set size!")
 
         # PHASE 1 - MODIFIED BEAM SEARCH
         list_of_beam = list()
         self.redundancy_aware_beam_search(list_of_beam, task)
 
         # PHASE 2 - DOMINANCE PRUNING
         subgroups = list()
         subgroups.extend(list_of_beam[1])
-        if len(list_of_beam)>2:
+        if len(list_of_beam) > 2:
             for beam in list_of_beam[2:]:
                 self.dominance_pruning(beam, subgroups, task)
-        if len(subgroups)<task.result_set_size:
+        if len(subgroups) < task.result_set_size:
             subgroups.sort(reverse=True)
             return ResultSet(subgroups, task.data.shape[0])
 
         # PHASE 3 - SUBGROUP SELECTION
         tuples_sg_matrix = []
         quality_array = []
         support_array = list()
@@ -391,15 +446,22 @@
             tuples_sg_matrix.append(descr.to_boolean_array(task.data))
             quality_array.append(descr.get_quality())
             support_array.append(descr.support)
         support_array = np.array(support_array)
         quality_array = np.array(quality_array)
         tuples_sg_matrix = np.array(tuples_sg_matrix)
         final_sgs = []
-        self.beam_creation(tuples_sg_matrix, support_array, quality_array, subgroups, final_sgs, task.result_set_size)
+        self.beam_creation(
+            tuples_sg_matrix,
+            support_array,
+            quality_array,
+            subgroups,
+            final_sgs,
+            task.result_set_size,
+        )
 
         final_sgs.sort(reverse=True)
         return ResultSet(final_sgs, task.data.shape[0])
 
     def redundancy_aware_beam_search(self, list_of_beam, task):
         """
         Parameters
@@ -419,95 +481,118 @@
         list_of_beam[0] = [Description()]
 
         depth = 0
         while depth < task.depth:
             # Generation of the beam with number of descriptors = depth+1
 
             list_of_beam.append(list())
-            logging.debug("DEPTH: "+str(depth+1))
+            logging.debug("DEPTH: " + str(depth + 1))
 
-            tuples_sg_matrix = [] # boolean matrix where rows are candidates subgroups and columns are tuples of the dataset
-                                  # tuples_sg_matrix[i][j] == true iff subgroup i contain tuple j
+            tuples_sg_matrix = []  # boolean matrix where rows are candidates subgroups and columns are tuples of the dataset
+            # tuples_sg_matrix[i][j] == true iff subgroup i contain tuple j
             quality_array = []  # will contain the quality of each candidate subgroup
             support_array = []  # will contain the support of each candidate subgroup
-            decriptions_list = list()  # will contain the description object of each candidate subgroup
+            decriptions_list = (
+                list()
+            )  # will contain the description object of each candidate subgroup
 
             # generation of candidates subgroups
             for last_sg in list_of_beam[depth]:  # for each subgroup in the previous beam
-                ss = task.search_space.extract_search_space(task.data, task.discretizer, current_description=last_sg)
+                ss = task.search_space.extract_search_space(
+                    task.data, task.discretizer, current_description=last_sg
+                )
 
                 # generation of all the possible extensions of the description last_sg
                 for sel in ss:
                     new_Descriptors = list(last_sg.Descriptors)
                     new_Descriptors.append(sel)
                     new_description = Description(new_Descriptors)
 
                     # check for duplicates
                     if new_description.is_present_in(decriptions_list):
                         continue
 
-                    sg_belonging_feature = new_description.to_boolean_array(task.data, set_attributes=True)
+                    sg_belonging_feature = new_description.to_boolean_array(
+                        task.data, set_attributes=True
+                    )
                     support = new_description.support
                     # check min support
-                    if support < task.min_support \
-                        or support < task.min_support_ratio * task.data.shape[0] \
-                            or support > task.max_support_ratio * task.data.shape[0]:
+                    if (
+                        support < task.min_support
+                        or support < task.min_support_ratio * task.data.shape[0]
+                        or support > task.max_support_ratio * task.data.shape[0]
+                    ):
                         continue
                     # comparison with new descriptor alone
                     sel_feature = Description([sel]).to_boolean_array(task.data)
                     # evaluate subgroup
                     if task.there_is_y_pred:
-                        quality = task.qf(y_true=task.data['y_true'], y_pred=task.data['y_pred'],
-                                          sensitive_features=sg_belonging_feature)
+                        quality = task.qf(
+                            y_true=task.data["y_true"],
+                            y_pred=task.data["y_pred"],
+                            sensitive_features=sg_belonging_feature,
+                        )
                         ### to evaluate
-                        sel_quality = task.qf(y_true=task.data['y_true'], y_pred=task.data['y_pred'],
-                                          sensitive_features=sel_feature)
+                        sel_quality = task.qf(
+                            y_true=task.data["y_true"],
+                            y_pred=task.data["y_pred"],
+                            sensitive_features=sel_feature,
+                        )
                     else:
-                        quality = task.qf(y_true=task.data['y_true'], sensitive_features=sg_belonging_feature)
+                        quality = task.qf(
+                            y_true=task.data["y_true"],
+                            sensitive_features=sg_belonging_feature,
+                        )
                         ### to evaluate
-                        sel_quality = task.qf(y_true=task.data['y_true'], sensitive_features=sel_feature)
+                        sel_quality = task.qf(
+                            y_true=task.data["y_true"], sensitive_features=sel_feature
+                        )
 
                     # if the quality of the new descriptor has deteriorated by merging the new descriptor
                     # with the current description, we do not add the new descriptor
                     ### to evaluate
                     if quality < task.min_quality or quality < sel_quality:
                         continue
-                    '''
+                    """
                     # This is for allowing descriptions with negative quality in the first beam
                     if depth>0 and (quality < task.min_quality or quality < sel_quality):
                         continue
-                    '''
+                    """
 
                     # This code is for apriori discard those descriptions dominated by another descriptions not containing sensitive features
                     pruned_des = []
                     new_description.set_quality(quality)
                     self.dominance_pruning([new_description], pruned_des, task)
                     pruned_des.sort(reverse=True)
                     pruned_attr = pruned_des[0].get_attributes()
                     if task.sensitive_features is not None:
                         any_in = any(i in task.sensitive_features for i in pruned_attr)
                         if not any_in:
                             continue
 
-
                     # insert current subgroup in the candidates
                     tuples_sg_matrix.append(sg_belonging_feature)
                     support_array.append(support)
                     quality_array.append(quality)
                     decriptions_list.append(new_description)
 
             if len(decriptions_list) == 0:
                 break
             # CREATION OF THE BEAM
             support_array = np.array(support_array)
             quality_array = np.array(quality_array)
             tuples_sg_matrix = np.array(tuples_sg_matrix)
-            self.beam_creation(tuples_sg_matrix, support_array, quality_array, decriptions_list,
-                               list_of_beam[depth + 1], self.beam_width)
-
+            self.beam_creation(
+                tuples_sg_matrix,
+                support_array,
+                quality_array,
+                decriptions_list,
+                list_of_beam[depth + 1],
+                self.beam_width,
+            )
 
             for d in list_of_beam[depth + 1]:
                 logging.debug(d)
             logging.debug(" ")
             depth += 1
 
     def dominance_pruning(self, subgroups, pruned_sgs, task):
@@ -522,40 +607,53 @@
         """
 
         for desc in subgroups:
             Descriptors = desc.get_Descriptors()
 
             generalizable = False
             for i in range(len(Descriptors)):
-
-                #creation of a generalized description by excluding the i-th descriptor
+                # creation of a generalized description by excluding the i-th descriptor
                 new_sel_list = []
                 for j in range(len(Descriptors)):
                     if i != j:
                         new_sel_list.append(Descriptors[j])
                 new_des = Description(new_sel_list)
 
                 sg_belonging_feature = new_des.to_boolean_array(task.data, set_attributes=True)
                 if task.there_is_y_pred:
-                    quality = task.qf(y_true=task.data['y_true'], y_pred=task.data['y_pred'],
-                                      sensitive_features=sg_belonging_feature)
+                    quality = task.qf(
+                        y_true=task.data["y_true"],
+                        y_pred=task.data["y_pred"],
+                        sensitive_features=sg_belonging_feature,
+                    )
                 else:
-                    quality = task.qf(y_true=task.data['y_true'], sensitive_features=sg_belonging_feature)
+                    quality = task.qf(
+                        y_true=task.data["y_true"],
+                        sensitive_features=sg_belonging_feature,
+                    )
 
                 if quality >= desc.get_quality():
-                    generalizable=True
+                    generalizable = True
                     if new_des.is_present_in(pruned_sgs):
                         continue
                     new_des.set_quality(quality)
                     pruned_sgs.append(new_des)
 
             if generalizable is False:
                 pruned_sgs.append(desc)
 
-    def beam_creation(self, tuples_sg_matrix, support_array, quality_array, decriptions_list, beam, beam_width):
+    def beam_creation(
+        self,
+        tuples_sg_matrix,
+        support_array,
+        quality_array,
+        decriptions_list,
+        beam,
+        beam_width,
+    ):
         """
         Parameters
         ----------
         tuples_sg_matrix : numpy array
             this is a boolean matrix. The rows are candidate subgroups and the columns are the istances of the dataset
         support_array :  numpy array
             contains the support of each candidate subgroup
@@ -594,16 +692,18 @@
         decriptions_list.sort(key=lambda x: x.support, reverse=True)
 
         # selection of the sg with highest quality
         index_of_max = np.argmax(quality_array)
         descr = decriptions_list[index_of_max]
         descr.set_quality(quality_array[index_of_max])
         beam.append(descr)
-        quality_array[index_of_max] = 0 # the quality of the selected sg is set to 0 in the quality_array,
-                                        # in this way this subgroup will never be choosen again
+        quality_array[index_of_max] = (
+            0  # the quality of the selected sg is set to 0 in the quality_array,
+        )
+        # in this way this subgroup will never be choosen again
 
         a_tothe_c_array = np.ones(tuples_sg_matrix.shape[1])
 
         num_iterations = min(beam_width, support_array.size)
         i = 1
         while i < num_iterations:
             # a_tothe_c updating
@@ -620,8 +720,8 @@
             weighted_quality_array = np.multiply(quality_array, weights)
             index_of_max = np.argmax(weighted_quality_array)
             descr = decriptions_list[index_of_max]
             descr.set_quality(quality_array[index_of_max])
             # isertion of the description in the beam
             beam.append(descr)
             quality_array[index_of_max] = 0
-            i+=1
+            i += 1
```

### Comparing `deeploy-1.37.0/deeploy/fairsd/discretization.py` & `deeploy-1.37.1/deeploy/fairsd/discretization.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     This parameter is interpret as an hard constraint: only cut points that produce buckets larger than
     min_groupSize will be returned.
     Another parameter that is possible to set is "force". If this parameter is setted to True the findCutPoints
     method will retur at list one cut point. This unless even a cut point can be found which produces two subgroups
     with a size greater than min_groupSize and with class partition entropy less than the entropy of the entire set.
 
     """
-    def __init__(self, min_groupsize = 1, force=False):
+
+    def __init__(self, min_groupsize=1, force=False):
         """
         :param min_groupsize: int
         :param force: boolean
         """
         self.min_groupsize = min_groupsize
         self.force = force
 
@@ -30,21 +31,21 @@
         :param x: list, numpy array or pandas Series that contains the values of the numeric feature to discretize
         :param y: list, numpy array or pandas Series that contains binary values (0 or 1) representing the class label
 
         :return: list of (ascending) ordered cut points
             if the function returns the cut points [c1, c2, ..., cn], with c1<c2<...<cn, the feature can be discretized
             by creating n+1 buckets: (-infinite, c1], (c1, c2], ..., (cn-1, cn], (cn, +infinite)
         """
-        df = pd.DataFrame({'x':x, 'y':y})
+        df = pd.DataFrame({"x": x, "y": y})
         total_size = df.shape[0]
 
-        df=df.groupby('x')['y'].agg(['sum','count'])
+        df = df.groupby("x")["y"].agg(["sum", "count"])
         df.reset_index(inplace=True)
-        total_sum=df['sum'].sum()
-        df['prop'] = df['sum'] / df['count']
+        total_sum = df["sum"].sum()
+        df["prop"] = df["sum"] / df["count"]
 
         cut_points = self.find_partitions(df, total_size, total_sum, self.force)
         cut_points.sort()
         return cut_points
 
     def find_partitions(self, df, total_size, total_sum, force=False):
         """
@@ -73,21 +74,24 @@
         count = 0
         min_cpe = total_size  # Class Partition Entropy (CPE)
         partition_index = 0
         partition_x = 0
         partition_sum = 0
         partition_count = 0
 
-        #find best candidate cut point
+        # find best candidate cut point
         for i in range(0, df.shape[0] - 1):
             loc = df.iloc[i]
-            sum += loc['sum']
-            count += loc['count']
-            if loc['prop'] == df.iloc[i + 1]['prop'] or count < self.min_groupsize or (
-                    total_size - count) < self.min_groupsize:
+            sum += loc["sum"]
+            count += loc["count"]
+            if (
+                loc["prop"] == df.iloc[i + 1]["prop"]
+                or count < self.min_groupsize
+                or (total_size - count) < self.min_groupsize
+            ):
                 continue
 
             # cakculate CPE cut point
             pc1s0 = sum / count  # probability of class 1 in subgroup 0
             pc0s0 = 1 - pc1s0
             pc1s0_ = pc1s0 if pc1s0 != 0 else 1
             pc0s0_ = pc0s0 if pc0s0 != 0 else 1
@@ -100,54 +104,61 @@
             entS1 = -(pc1s1 * math.log2(pc1s1_) + pc0s1 * math.log2(pc0s1_))
 
             cpe = (count / total_size) * entS0 + ((total_size - count) / total_size) * entS1
 
             if cpe < min_cpe:
                 min_cpe = cpe
                 partition_index = i
-                partition_x = loc['x']
+                partition_x = loc["x"]
                 partition_sum = sum
                 partition_count = count
                 partition_entS0 = entS0
                 partition_entS1 = entS1
         if min_cpe == total_size:
             return []
 
-        #test MDLP condition
+        # test MDLP condition
         pc1 = total_sum / total_size
         pc0 = 1 - pc1
         pc1_ = pc1 if pc1 != 0 else 1
         pc0_ = pc0 if pc0 != 0 else 1
         entS = -(pc1 * math.log2(pc1_) + pc0 * math.log2(pc0_))
         gain = entS - min_cpe
 
         remained_pos = total_sum - partition_sum
         total_rem = total_size - partition_count
         c0 = 2 if (partition_sum == 0 or partition_sum == partition_count) else 1
         c1 = 2 if (remained_pos == 0 or remained_pos == total_rem) else 1
         delta = math.log2(9) - c0 * partition_entS0 - c1 * partition_entS1
 
-        delta = math.log2(7) -( 2*entS -c0 * partition_entS0 - c1 * partition_entS1)
+        delta = math.log2(7) - (2 * entS - c0 * partition_entS0 - c1 * partition_entS1)
 
-        if (gain <= ((math.log2(total_size - 1) + delta) / total_size)):
+        if gain <= ((math.log2(total_size - 1) + delta) / total_size):
             if force:
                 return [partition_x]
             return []
 
-        #recoursive splitting
-        left_partitions = self.find_partitions(df.iloc[:(partition_index+1)], partition_count, partition_sum)
-        right_partitions= self.find_partitions(df.iloc[(partition_index+1):], (total_size-partition_count), (total_sum-partition_sum))
-        a= [partition_x]+ left_partitions + right_partitions
+        # recoursive splitting
+        left_partitions = self.find_partitions(
+            df.iloc[: (partition_index + 1)], partition_count, partition_sum
+        )
+        right_partitions = self.find_partitions(
+            df.iloc[(partition_index + 1) :],
+            (total_size - partition_count),
+            (total_sum - partition_sum),
+        )
+        a = [partition_x] + left_partitions + right_partitions
         return a
 
 
 class EqualFrequency:
     """
     This class find the cut points to discretize a numerical feature using an approximate equal frequency discretization.
     """
+
     def __init__(self, min_bin_size=1, num_bins=0):
         """
         Parameters
         __________
         num_bins : int
             this number is to interpret as the maximum number of bins that will be generated.
             If this parameter is not specified (0 by deafault), it will be automatically determined
@@ -168,141 +179,143 @@
         self.num_bins = num_bins
 
     def findCutPoints(self, x):
         """
         :param x: numpy array or pandas series
         :return: list of (ascending) ordered cut points
         """
-        #determination of the number of bins
-        if self.num_bins >1:
-            num_bins = min(self.num_bins, int(x.size/(self.min_group_size*1.2)))
+        # determination of the number of bins
+        if self.num_bins > 1:
+            num_bins = min(self.num_bins, int(x.size / (self.min_group_size * 1.2)))
         else:
-            num_bins = int(x.size/(self.min_group_size*1.2))
+            num_bins = int(x.size / (self.min_group_size * 1.2))
         if num_bins < 2:
             return []
 
         avg_group_size = x.size / num_bins
 
         if isinstance(x, pd.Series):
             x = x.to_numpy()
         val, counts = np.unique(x, return_counts=True)
 
-        quantiles = [] #actually this array will contains quantiles * x.size
-        sum =0
+        quantiles = []  # actually this array will contains quantiles * x.size
+        sum = 0
         for c in counts:
-            sum = sum+c
+            sum = sum + c
             quantiles.append(sum)
 
         up_index = 0
         low_index = 0
-        current_quantile=avg_group_size #again, is quantile * x.size
+        current_quantile = avg_group_size  # again, is quantile * x.size
 
         cut_indexes = []
-        #for each expected quantile, find his approximation
-        while current_quantile < (sum-avg_group_size/2): # sum is equal to x.size
-            up_index, low_index = self.findApproximationIndexex(up_index, low_index, current_quantile, quantiles)
-            '''
+        # for each expected quantile, find his approximation
+        while current_quantile < (sum - avg_group_size / 2):  # sum is equal to x.size
+            up_index, low_index = self.findApproximationIndexex(
+                up_index, low_index, current_quantile, quantiles
+            )
+            """
             # this commented code use the cut point that best approximates the expected quantile
             num_up = quantiles[up_index] - current_quantile
             num_low = current_quantile - quantiles[low_index]
 
             if num_up < num_low:
                 if up_index not in cut_indexes:
                     cut_indexes.append(up_index)
             else:
                 if low_index not in cut_indexes:
                     cut_indexes.append(low_index)
-            '''
+            """
 
             ### here we always choose an approximation by excess of the expected quantile.
             # This consistency can help create more similarly sized bins
             if up_index not in cut_indexes:
                 cut_indexes.append(up_index)
             current_quantile += avg_group_size
             ###
 
         cut_points = []
         bins_size = []
         last_quantile = 0
         for i in cut_indexes:
             cut_points.append(val[i])
-            bins_size.append(quantiles[i]-last_quantile)
+            bins_size.append(quantiles[i] - last_quantile)
             last_quantile = quantiles[i]
         bins_size.append(sum - last_quantile)
 
         # The bins with size <= min_group_size will be merged with one of the other adiacent bins
         self.mergeSmallBins(cut_points, bins_size)
         return cut_points
 
-    def findApproximationIndexex(self,up_index, low_index, current_quantile, quantiles):
+    def findApproximationIndexex(self, up_index, low_index, current_quantile, quantiles):
         """
         :param up_index: int
         :param low_index: int
         :param current_quantile: float
         :param quantiles: list of float
 
         :return: (int, int)
         """
 
         new_up_i = up_index
         while new_up_i < len(quantiles):
             if quantiles[new_up_i] < current_quantile:
-                new_up_i+=1
+                new_up_i += 1
             else:
                 break
         new_low_i = low_index
         if new_up_i > up_index:
-            new_low_i= new_up_i-1
+            new_low_i = new_up_i - 1
         return new_up_i, new_low_i
 
-
     def mergeSmallBins(self, cut_points, bins_size):
         """
         :param cut_points: list
         :param bins_size: list
         :return: void
         """
         # find the smallest bin
         min_smallbin = self.min_group_size
         min_index = 0
         for i in range(len(bins_size)):
-            if bins_size[i]<min_smallbin:
+            if bins_size[i] < min_smallbin:
                 min_smallbin = bins_size[i]
                 min_index = i
 
         # check if the smallest bin finded has size lower than the min_group_size
         if min_smallbin == self.min_group_size:
             return
 
         previous_size = 0
         next_size = 0
         if min_index > 0:
             previous_size = bins_size[min_index - 1]
-        if min_index < (len(bins_size)-1):
+        if min_index < (len(bins_size) - 1):
             next_size = bins_size[min_index + 1]
 
-        if previous_size == 0 and next_size ==0:
+        if previous_size == 0 and next_size == 0:
             return
 
         if (previous_size == 0) or (next_size > 0 and next_size < previous_size):
-            bins_size[min_index+1] = bins_size[min_index+1]+bins_size[min_index]
+            bins_size[min_index + 1] = bins_size[min_index + 1] + bins_size[min_index]
             cut_points.pop(min_index)
             bins_size.pop(min_index)
         else:
             bins_size[min_index - 1] = bins_size[min_index - 1] + bins_size[min_index]
-            cut_points.pop(min_index-1)
+            cut_points.pop(min_index - 1)
             bins_size.pop(min_index)
 
         self.mergeSmallBins(cut_points, bins_size)
 
 
 class EqualWidth:
     """
-        This class find the cut points to discretize a numerical feature using the equal width discretization.
-        """
+    This class find the cut points to discretize a numerical feature using the equal width discretization.
+    """
+
     def __init__(self, min_bins_size=1, num_bins=0):
         """
         Parameters
         __________
         num_bins : int
             this number is to interpret as the maximum number of bins that will be generated.
             If this parameter is not specified (0 by deafault), it will be automatically determined.
@@ -327,16 +340,16 @@
             num_bins = int(x.size / (self.min_group_size * 1.2))
         if num_bins < 2:
             return []
 
         if isinstance(x, pd.Series):
             x = x.to_numpy()
         minim = x.min()
-        bin_width = (x.max() - minim)/num_bins
+        bin_width = (x.max() - minim) / num_bins
         cut_points = []
         current_cut = minim + bin_width
         i = 1
         while i < num_bins:
             cut_points.append(current_cut)
             current_cut = current_cut + bin_width
-            i+=1
+            i += 1
         return cut_points
```

### Comparing `deeploy-1.37.0/deeploy/fairsd/qualitymeasures.py` & `deeploy-1.37.1/deeploy/fairsd/qualitymeasures.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 
 class QualityFunction(ABC):
     """Abstract class.
 
     If the user wants to create a customized quality function, it is recommended to extend this class
     """
+
     @abstractmethod
     def evaluate(self, y_true, y_pred, sensitive_features):
         """Evaluate the quality of a description.
 
         Parameters
         ----------
         y_true : list, pandas.series or numpy array
@@ -29,8 +30,8 @@
     def evaluate(self, y_true, y_pred, sensitive_features):
         s0y_true = (y_true & ~sensitive_features).sum()
         s0y_true = 1 if s0y_true == 0 else s0y_true
         p_s0 = (y_true & y_pred & ~sensitive_features).sum() / s0y_true
         s1y_true = (y_true & sensitive_features).sum()
         s1y_true = 1 if s1y_true == 0 else s1y_true
         p_s1 = (y_true & y_pred & sensitive_features).sum() / s1y_true
-        return p_s0-p_s1
+        return p_s0 - p_s1
```

### Comparing `deeploy-1.37.0/deeploy/fairsd/searchspace.py` & `deeploy-1.37.1/deeploy/fairsd/searchspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,24 @@
     ----------
     nominal_Descriptors : list of Descriptor(s)
         will contain all possible non numeric Descriptors.
     numeric_Descriptors : list of Descriptor(s)
         will contain all possible  numeric Descriptors.
     """
 
-    def __init__(self, dataset, ignore=None, nominal_features=None, numeric_features=None, dynamic_discretization=False, discretizer=None, sensitiive_features=None):
+    def __init__(
+        self,
+        dataset,
+        ignore=None,
+        nominal_features=None,
+        numeric_features=None,
+        dynamic_discretization=False,
+        discretizer=None,
+        sensitiive_features=None,
+    ):
         """
         :param dataset : pandas.DataFrame
         :param ignore : list of String(s)
             list the attributes to not take into consideration for creating the search space.
         :param nominal_features : list of Strings that contain a subgroup of nominal features
         :param numeric_features : list of Strings that contain a subgroup of numeric features
         :param dynamic_discretization: boolean
@@ -38,45 +47,53 @@
         if nominal_features is None:
             nominal_features = []
         if numeric_features is None:
             numeric_features = []
         self.nominal_Descriptors = []
         self.numeric_Descriptors = []
         # create nominal Descriptors
-        #nominal features with explicit type phassed
+        # nominal features with explicit type phassed
         for col in nominal_features:
             if col not in ignore:
                 values = dataset[col].unique()
                 for x in values:
                     self.nominal_Descriptors.append(Descriptor(col, attribute_value=x))
-        #nominal features without explicit type phassed
-        dtypes_subs = dataset.select_dtypes(exclude=['number'])
+        # nominal features without explicit type phassed
+        dtypes_subs = dataset.select_dtypes(exclude=["number"])
         for col in dtypes_subs.columns:
             if col not in ignore + nominal_features + numeric_features:
                 values = dataset[col].unique()
                 for x in values:
                     self.nominal_Descriptors.append(Descriptor(col, attribute_value=x))
 
         # numerical Descriptors
         if dynamic_discretization:
             for col in numeric_features:
                 if col not in ignore:
-                    self.numeric_Descriptors.append(Descriptor(col, to_discretize=True, is_numeric=True))
-            dtypes_subs = dataset.select_dtypes(include=['number'])
+                    self.numeric_Descriptors.append(
+                        Descriptor(col, to_discretize=True, is_numeric=True)
+                    )
+            dtypes_subs = dataset.select_dtypes(include=["number"])
             for col in dtypes_subs.columns:
                 if col not in ignore + nominal_features + numeric_features:
-                    self.numeric_Descriptors.append(Descriptor(col, to_discretize=True, is_numeric=True))
+                    self.numeric_Descriptors.append(
+                        Descriptor(col, to_discretize=True, is_numeric=True)
+                    )
         else:
             for col in numeric_features:
                 if col not in ignore:
-                    self.numeric_Descriptors.extend(discretizer.discretize(dataset, Description(), col))
-            dtypes_subs = dataset.select_dtypes(include=['number'])
+                    self.numeric_Descriptors.extend(
+                        discretizer.discretize(dataset, Description(), col)
+                    )
+            dtypes_subs = dataset.select_dtypes(include=["number"])
             for col in dtypes_subs.columns:
                 if col not in ignore + nominal_features + numeric_features:
-                    self.numeric_Descriptors.extend(discretizer.discretize(dataset, Description(), col))
+                    self.numeric_Descriptors.extend(
+                        discretizer.discretize(dataset, Description(), col)
+                    )
 
     def extract_search_space(self, dataset, discretizer, current_description=None):
         """This method return the subset of the search space to explore
          for expanding the description "current_description".
 
         All descriptors containing attributes present in the current_description will be removed
         from the returned search space subset.
@@ -105,48 +122,52 @@
         Descriptors = []
         for Descriptor in self.nominal_Descriptors:
             if Descriptor.attribute_name not in to_exclude:
                 Descriptors.append(Descriptor)
         for Descriptor in self.numeric_Descriptors:
             if Descriptor.attribute_name not in to_exclude:
                 if Descriptor.is_to_discretize():
-                    Descriptors.extend(discretizer.discretize(dataset, current_description, Descriptor.get_attribute_name()))
-                else :
+                    Descriptors.extend(
+                        discretizer.discretize(
+                            dataset, current_description, Descriptor.get_attribute_name()
+                        )
+                    )
+                else:
                     Descriptors.append(Descriptor)
         return Descriptors
 
 
 class Discretizer:
     """Class for the discretization of the numeric attributes."""
 
-    def __init__(self, discretization_type, target=None, min_groupsize=1, num_bins = 6):
+    def __init__(self, discretization_type, target=None, min_groupsize=1, num_bins=6):
         """
 
         :param discretization_type : enumerated
             can be "mdlp" or "equalfreq" or "equalwidth"
         :param target: String, optional
             this parameter is needed only for supervised discretizations (mdlp)
         :param min_groupsize: int, optional
             discretize() method will create only subgroups with size >= min_groupsize.
         """
         self.discretization_type = discretization_type
-        if discretization_type =='mdlp':
+        if discretization_type == "mdlp":
             self.supervised = True
             self.discretizer = MDLP(min_groupsize, force=True)
             self.target = target
-        elif discretization_type =='equalfreq':
+        elif discretization_type == "equalfreq":
             self.supervised = False
             self.discretizer = EqualFrequency(min_groupsize, num_bins)
-        elif discretization_type =='equalwidth':
+        elif discretization_type == "equalwidth":
             self.supervised = False
             self.discretizer = EqualWidth(min_groupsize, num_bins)
         else:
             raise RuntimeError('discretization_type must be "mdlp" OR "equalfreq" OR "equalwidth"')
 
-    def discretize(self, data, description, feature): #### to test
+    def discretize(self, data, description, feature):  #### to test
         """
         Parameters
         ----------
         data: pandas.DataFrame
             The dataset.
         description: Description
             The discretization will be based only on those tuples of the dataset that match the description.
@@ -154,24 +175,24 @@
             Is the name of the numeric attribute of the dataset to discretize.
 
         Returns
         -------
         list of Descriptor(s)
             Will be created and returned (in a list) one Descriptor for each bin created in the discretization phase.
         """
-        subset= data[description.to_boolean_array(data)]
+        subset = data[description.to_boolean_array(data)]
         x = subset[feature]
         if self.supervised:
             y = subset[self.target]
-            cut_points=self.discretizer.findCutPoints(x, y)
+            cut_points = self.discretizer.findCutPoints(x, y)
         else:
             cut_points = self.discretizer.findCutPoints(x)
 
         Descriptors = []
         if len(cut_points) < 1:
             return Descriptors
 
         Descriptors.append(Descriptor(feature, low_bound=None, up_bound=None, is_numeric=True))
         for cp in cut_points:
-            Descriptors[-1].up_bound=cp
+            Descriptors[-1].up_bound = cp
             Descriptors.append(Descriptor(feature, low_bound=cp, up_bound=None, is_numeric=True))
         return Descriptors
```

### Comparing `deeploy-1.37.0/deeploy/fairsd/sgdescription.py` & `deeploy-1.37.1/deeploy/fairsd/sgdescription.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,92 +5,109 @@
 
 class Descriptor:
     """
     Thi object is formed by an attribute name and an attribute value (or a lower bound plus an upper bound
     if the Descriptor is numeric).
     """
 
-    def __init__(self, attribute_name, attribute_value=None, up_bound=None, low_bound=None, to_discretize=False, is_numeric=False):
-        """
-        Parameters
-        ----------
-        attribute_name : string
-        attribute_value : string or bool, default None
-            To set only if the Descriptor is not numeric.
-        up_bound : double or int, default None
-             To set iff the Descriptor is numeric and already discretized.
-         low_bound : double or int, default None
-             To set iff the Descriptor is numeric and already discretized.
-       to_discretize : bool, default False
-            To set at True iff the Descriptor is numeric and not still discretized. In this case
-            the up_bound and low_bound attributes will be meaningless
-        is_numeric : bool, default False
-            To set at true iff the descriptor is numeric
+    def __init__(
+        self,
+        attribute_name,
+        attribute_value=None,
+        up_bound=None,
+        low_bound=None,
+        to_discretize=False,
+        is_numeric=False,
+    ):
+        """
+         Parameters
+         ----------
+         attribute_name : string
+         attribute_value : string or bool, default None
+             To set only if the Descriptor is not numeric.
+         up_bound : double or int, default None
+              To set iff the Descriptor is numeric and already discretized.
+          low_bound : double or int, default None
+              To set iff the Descriptor is numeric and already discretized.
+        to_discretize : bool, default False
+             To set at True iff the Descriptor is numeric and not still discretized. In this case
+             the up_bound and low_bound attributes will be meaningless
+         is_numeric : bool, default False
+             To set at true iff the descriptor is numeric
         """
 
         self.attribute_name = attribute_name
         self.is_numeric = is_numeric
         if is_numeric:
             self.up_bound = up_bound
             self.low_bound = low_bound
         else:
             self.attribute_value = attribute_value
-        self.to_discretize = to_discretize # The current implementation could work also without this parameter
+        self.to_discretize = (
+            to_discretize  # The current implementation could work also without this parameter
+        )
 
     def get_attribute_name(self):
         return self.attribute_name
+
     def is_to_discretize(self):
         return self.to_discretize
+
     def is_present_in(self, other_descriptors):
         """
         :param: other_descriptors: list of Descriptors
         :return: bool
         """
         for other in other_descriptors:
-            if self.attribute_name == other.attribute_name and self.is_numeric== other.is_numeric:
-                if self.is_numeric and self.up_bound==other.up_bound and self.low_bound==other.low_bound:
+            if self.attribute_name == other.attribute_name and self.is_numeric == other.is_numeric:
+                if (
+                    self.is_numeric
+                    and self.up_bound == other.up_bound
+                    and self.low_bound == other.low_bound
+                ):
                     return True
-                elif self.is_numeric is False and self.attribute_value==other.attribute_value:
+                elif self.is_numeric is False and self.attribute_value == other.attribute_value:
                     return True
         return False
 
 
 class Description:
     """List of Descriptors plus other description attributes.
 
     Semantically it is to be interpreted as the conjunction of all the Descriptors contained in the list:
     a dataset record will match the description if each single Descriptor of the description will match with this record.
     """
+
     def __init__(self, Descriptors=None):
         """
         :param Descriptors : list of Descriptor
         """
         if Descriptors is None:
-            self.Descriptors=[]
+            self.Descriptors = []
         else:
-            self.Descriptors=Descriptors
+            self.Descriptors = Descriptors
         self.support = None
 
     def __repr__(self, opposite=False):
         """Represent the description as a string.
 
         :return : String
         """
-        descr=""
+        descr = ""
         if opposite:
             descr = descr + "NOT ("
         for s in self.Descriptors:
             # If the descriptor is numeric, the string will be formed by the attribute name and the lower and upper bound
             if s.is_numeric:
                 low = str(s.low_bound) if s.low_bound is not None else "-infinite"
                 up = str(s.up_bound) if s.up_bound is not None else "+infinite"
-                descr = descr + s.attribute_name + " = (" + low +", "+ up +"] AND "
+                descr = descr + s.attribute_name + " = (" + low + ", " + up + "] AND "
             # If the descriptor is not numeric, the string will be formed by the attribute name and the attribute value
             else:
-                descr = descr+ s.attribute_name+' = "'+str(s.attribute_value)+'" AND '
+                descr = descr + s.attribute_name + ' = "' + str(s.attribute_value) + '" AND '
         if descr != "":
             descr = descr[:-4]
         if opposite:
             descr = descr + ")"
         return descr
 
     def to_string(self, opposite=False):
@@ -125,34 +142,41 @@
             If a description is empty, the returned array will have all elements equal to True.
         """
         s = np.full(dataset.shape[0], True)
         s = pd.Series(s)
         for i in range(0, len(self.Descriptors)):
             if self.Descriptors[i].is_numeric:
                 if self.Descriptors[i].low_bound is not None:
-                    s = s & (dataset[self.Descriptors[i].attribute_name] > self.Descriptors[i].low_bound)
+                    s = s & (
+                        dataset[self.Descriptors[i].attribute_name] > self.Descriptors[i].low_bound
+                    )
                 if self.Descriptors[i].up_bound is not None:
-                    s = s & (dataset[self.Descriptors[i].attribute_name] <= self.Descriptors[i].up_bound)
+                    s = s & (
+                        dataset[self.Descriptors[i].attribute_name] <= self.Descriptors[i].up_bound
+                    )
             else:
-                s =( (s) & (dataset[self.Descriptors[i].attribute_name] == self.Descriptors[i].attribute_value))
+                s = (s) & (
+                    dataset[self.Descriptors[i].attribute_name]
+                    == self.Descriptors[i].attribute_value
+                )
 
         if set_attributes:
-            #set size, relative size and target share
-            self.support=sum(s)
+            # set size, relative size and target share
+            self.support = sum(s)
         return s
 
     def size(self, dataset=None):
-        """ Return the support of the description and set the support in case this parameters was not set.
+        """Return the support of the description and set the support in case this parameters was not set.
 
         :param dataset: pandas.DataFrame
         :return: int
         """
         if self.support is None:
             if dataset is None:
-                raise RuntimeError ("dataset argument required in Description.size()")
+                raise RuntimeError("dataset argument required in Description.size()")
             self.to_boolean_array(dataset, set_attributes=True)
         return self.support
 
     def get_attributes(self):
         """Return the list of the attribute names in the description.
 
         :return: list of String
@@ -172,21 +196,21 @@
         :return: bool
             True if the current description (self) is present in the list (beam).
             Return true iff the current object (Description) have the same parameters of at list another object
             present in the beam.
 
         """
         for descr in beam:
-            equals=True
+            equals = True
             for sel in self.Descriptors:
                 if sel.is_present_in(descr.Descriptors) is False:
                     equals = False
                     break
             if equals:
                 return True
         return False
 
     def set_quality(self, q):
-        self.quality=q
+        self.quality = q
 
     def get_quality(self):
         return self.quality
```

### Comparing `deeploy-1.37.0/deeploy/models/__init__.py` & `deeploy-1.37.1/deeploy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/client_options.py` & `deeploy-1.37.1/deeploy/models/client_options.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/create_actuals.py` & `deeploy-1.37.1/deeploy/models/create_actuals.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/create_azure_ml_deployment.py` & `deeploy-1.37.1/deeploy/models/create_azure_ml_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/create_deployment.py` & `deeploy-1.37.1/deeploy/models/create_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,9 +95,9 @@
             "transformerInstanceType": self.transformer_instance_type,
             "transformerMemRequest": self.transformer_mem_request,
             "transformerMemLimit": self.transformer_mem_limit,
             "transformerCpuRequest": self.transformer_cpu_request,
             "transformerCpuLimit": self.transformer_cpu_limit,
             "transformerGpuRequest": self.transformer_gpu_request,
             "transformerEnv": self.transformer_env,
-            "transformerArgs": self.transformer_args
+            "transformerArgs": self.transformer_args,
         }
```

### Comparing `deeploy-1.37.0/deeploy/models/create_deployment_base.py` & `deeploy-1.37.1/deeploy/models/create_deployment_base.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/create_evaluation.py` & `deeploy-1.37.1/deeploy/models/create_evaluation.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/create_explainer_reference.py` & `deeploy-1.37.1/deeploy/models/create_explainer_reference.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/create_metadata.py` & `deeploy-1.37.1/deeploy/models/create_metadata.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/create_model_reference.py` & `deeploy-1.37.1/deeploy/models/create_model_reference.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/create_sagemaker_deployment.py` & `deeploy-1.37.1/deeploy/models/create_sagemaker_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/create_transformer_reference.py` & `deeploy-1.37.1/deeploy/models/create_transformer_reference.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/deployment.py` & `deeploy-1.37.1/deeploy/models/deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/get_prediction_logs_options.py` & `deeploy-1.37.1/deeploy/models/get_prediction_logs_options.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/prediction_log.py` & `deeploy-1.37.1/deeploy/models/prediction_log.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/reference_json.py` & `deeploy-1.37.1/deeploy/models/reference_json.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/update_azure_ml_deployment.py` & `deeploy-1.37.1/deeploy/models/update_azure_ml_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/update_deployment.py` & `deeploy-1.37.1/deeploy/models/update_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,11 +95,11 @@
             "transformerInstanceType": self.transformer_instance_type,
             "transformerMemRequest": self.transformer_mem_request,
             "transformerMemLimit": self.transformer_mem_limit,
             "transformerCpuRequest": self.transformer_cpu_request,
             "transformerCpuLimit": self.transformer_cpu_limit,
             "transformerGpuRequest": self.transformer_gpu_request,
             "transformerEnv": self.transformer_env,
-            "transformerArgs": self.transformer_args
+            "transformerArgs": self.transformer_args,
         }
         request_body = {k: v for k, v in request_body.items() if v is not None}
         return {k: v for k, v in request_body.items() if v is not None and v != {}}
```

### Comparing `deeploy-1.37.0/deeploy/models/update_deployment_base.py` & `deeploy-1.37.1/deeploy/models/update_deployment_base.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/update_deployment_description.py` & `deeploy-1.37.1/deeploy/models/update_deployment_description.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/models/update_sagemaker_deployment.py` & `deeploy-1.37.1/deeploy/models/update_sagemaker_deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/services/deeploy_service.py` & `deeploy-1.37.1/deeploy/services/deeploy_service.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/services/explainer_wrapper.py` & `deeploy-1.37.1/deeploy/services/explainer_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/services/explainers/alibi.py` & `deeploy-1.37.1/deeploy/services/explainers/alibi.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/services/explainers/omni_tabular.py` & `deeploy-1.37.1/deeploy/services/explainers/omni_tabular.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/services/explainers/shap.py` & `deeploy-1.37.1/deeploy/services/explainers/shap.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/services/file_service.py` & `deeploy-1.37.1/deeploy/services/file_service.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/services/git_service.py` & `deeploy-1.37.1/deeploy/services/git_service.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/services/model_wrapper.py` & `deeploy-1.37.1/deeploy/services/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/deeploy/services/models/sklearn.py` & `deeploy-1.37.1/deeploy/services/models/sklearn.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,13 @@
     __sklearn_model: BaseEstimator
 
     def __init__(self, model_object: Any, **kwargs) -> None:
         if not issubclass(type(model_object), BaseEstimator):
             raise Exception("Not a valid SKLearn class")
 
         self.__sklearn_model = model_object
-        return
 
     def save(self, local_folder_path: str) -> None:
         dump(self.__sklearn_model, join(local_folder_path, "model.joblib"))
-        return
 
     def get_model_type(self) -> ModelType:
         return ModelType.SKLEARN
```

### Comparing `deeploy-1.37.0/deeploy/services/models/tensorflow.py` & `deeploy-1.37.1/deeploy/services/models/tensorflow.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 
 class TensorFlowModel(BaseModel):
     __tensorflow_model: Module
 
     def __init__(self, model_object: Any, **kwargs) -> None:
         if not issubclass(type(model_object), Module):
             raise Exception("Not a valid TensorFlow class")
-
         self.__tensorflow_model = model_object
-        return
 
     def save(self, local_folder_path: str) -> None:
         self.__tensorflow_model.save(join(local_folder_path, "1"))
-        return
 
     def get_model_type(self) -> ModelType:
         return ModelType.TENSORFLOW
```

### Comparing `deeploy-1.37.0/deeploy/services/models/xgboost.py` & `deeploy-1.37.1/deeploy/services/models/xgboost.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,13 @@
     def __init__(self, model_object: Any, **kwargs) -> None:
         if not issubclass(type(model_object), XGBClassifier) and not issubclass(
             type(model_object), Booster
         ):
             raise Exception("Not a valid XGBoost class")
 
         self.__xgboost_model = model_object
-        return
 
     def save(self, local_folder_path: str) -> None:
         self.__xgboost_model.save_model(join(local_folder_path, "model.bst"))
-        return
 
     def get_model_type(self) -> ModelType:
         return ModelType.XGBOOST
```

### Comparing `deeploy-1.37.0/deeploy.egg-info/PKG-INFO` & `deeploy-1.37.1/deeploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeploy
-Version: 1.37.0
+Version: 1.37.1
 Summary: The official Deeploy client for Python
 Home-page: https://gitlab.com/deeploy-ml/deeploy-python-client
 Author: Tim Kleinloog
 Author-email: opensource@deeploy.ml
 License: UNKNOWN
 Project-URL: Documentation, https://deeploy-ml.gitlab.io/deeploy-python-client/
 Project-URL: Deeploy website, https://deeploy.ml
```

### Comparing `deeploy-1.37.0/deeploy.egg-info/SOURCES.txt` & `deeploy-1.37.1/deeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeploy-1.37.0/setup.py` & `deeploy-1.37.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,36 +28,31 @@
     url="https://gitlab.com/deeploy-ml/deeploy-python-client",
     project_urls={
         "Documentation": "https://deeploy-ml.gitlab.io/deeploy-python-client/",
         "Deeploy website": "https://deeploy.ml",
     },
     install_requires=[
         "pydantic<2.0.0",
-        "gitpython==3.1.23",
         "requests>=2.26.0",
         "joblib==1.3.2",
         "dill==0.3.6",
-        "ipython>=7.26.0",
-        "nbconvert>=6.0.7",
-        "torch-model-archiver==0.3.1",
         "click",
         "Jinja2",
     ],
-
     extras_require={
         "fair": [
             "numpy>=1.17.2",
             "pandas>=0.25.1",
             "scikit-learn>=0.22.1",
             "fairlearn>=0.5.0",
         ],
         "docker": [
             "kserve[storage]==0.11.0",
             "nest-asyncio~=1.4.0",
-        ]
+        ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7, <3.11",
```

