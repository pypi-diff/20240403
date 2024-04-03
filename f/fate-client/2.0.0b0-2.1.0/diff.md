# Comparing `tmp/fate-client-2.0.0b0.tar.gz` & `tmp/fate-client-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fate-client-2.0.0b0.tar", last modified: Tue Sep 19 06:31:17 2023, max compression
+gzip compressed data, was "fate-client-2.1.0.tar", last modified: Wed Apr  3 07:27:09 2024, max compression
```

## Comparing `fate-client-2.0.0b0.tar` & `fate-client-2.1.0.tar`

### file list

```diff
@@ -1,150 +1,174 @@
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.225884 fate-client-2.0.0b0/
--rw-r--r--   0 sage       (501) staff       (20)      121 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/MANIFEST.in
--rw-r--r--   0 sage       (501) staff       (20)      685 2023-09-19 06:31:17.225693 fate-client-2.0.0b0/PKG-INFO
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.210070 fate-client-2.0.0b0/fate_client/
--rw-r--r--   0 sage       (501) staff       (20)      642 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/__init__.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.211303 fate-client-2.0.0b0/fate_client/flow_cli/
--rw-r--r--   0 sage       (501) staff       (20)      616 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/__init__.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.212942 fate-client-2.0.0b0/fate_client/flow_cli/commands/
--rw-r--r--   0 sage       (501) staff       (20)      616 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     4196 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/client.py
--rw-r--r--   0 sage       (501) staff       (20)     2825 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/data.py
--rw-r--r--   0 sage       (501) staff       (20)     4829 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/job.py
--rw-r--r--   0 sage       (501) staff       (20)     1868 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/log.py
--rw-r--r--   0 sage       (501) staff       (20)     2365 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/model.py
--rw-r--r--   0 sage       (501) staff       (20)     5089 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/output.py
--rw-r--r--   0 sage       (501) staff       (20)     3294 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/permission.py
--rw-r--r--   0 sage       (501) staff       (20)     2083 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/provider.py
--rw-r--r--   0 sage       (501) staff       (20)     1213 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/server.py
--rw-r--r--   0 sage       (501) staff       (20)     1147 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/site.py
--rw-r--r--   0 sage       (501) staff       (20)     1671 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/table.py
--rw-r--r--   0 sage       (501) staff       (20)     1856 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/task.py
--rw-r--r--   0 sage       (501) staff       (20)     2418 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/commands/test.py
--rw-r--r--   0 sage       (501) staff       (20)     5736 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/flow.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.213381 fate-client-2.0.0b0/fate_client/flow_cli/utils/
--rw-r--r--   0 sage       (501) staff       (20)      616 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/utils/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     3700 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/utils/args_desc.py
--rw-r--r--   0 sage       (501) staff       (20)     7103 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/utils/cli_args.py
--rw-r--r--   0 sage       (501) staff       (20)     2077 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_cli/utils/cli_utils.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.213612 fate-client-2.0.0b0/fate_client/flow_sdk/
--rw-r--r--   0 sage       (501) staff       (20)      646 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     1353 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/_client.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.215116 fate-client-2.0.0b0/fate_client/flow_sdk/api/
--rw-r--r--   0 sage       (501) staff       (20)      949 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     4373 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/client.py
--rw-r--r--   0 sage       (501) staff       (20)     2964 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/data.py
--rw-r--r--   0 sage       (501) staff       (20)     6432 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/job.py
--rw-r--r--   0 sage       (501) staff       (20)     1941 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/log.py
--rw-r--r--   0 sage       (501) staff       (20)     2731 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/model.py
--rw-r--r--   0 sage       (501) staff       (20)     5305 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/output.py
--rw-r--r--   0 sage       (501) staff       (20)     3210 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/permission.py
--rw-r--r--   0 sage       (501) staff       (20)     2089 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/provider.py
--rw-r--r--   0 sage       (501) staff       (20)      916 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/service.py
--rw-r--r--   0 sage       (501) staff       (20)     1014 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/site.py
--rw-r--r--   0 sage       (501) staff       (20)     1470 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/table.py
--rw-r--r--   0 sage       (501) staff       (20)     2496 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/task.py
--rw-r--r--   0 sage       (501) staff       (20)     2666 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/api/test.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.215532 fate-client-2.0.0b0/fate_client/flow_sdk/utils/
--rw-r--r--   0 sage       (501) staff       (20)        0 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/utils/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     4868 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/utils/base_utils.py
--rw-r--r--   0 sage       (501) staff       (20)     2335 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/utils/io_utils.py
--rw-r--r--   0 sage       (501) staff       (20)      863 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/flow_sdk/utils/params_utils.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.215954 fate-client-2.0.0b0/fate_client/pipeline/
--rw-r--r--   0 sage       (501) staff       (20)      691 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/__init__.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.216069 fate-client-2.0.0b0/fate_client/pipeline/component_define/
--rw-r--r--   0 sage       (501) staff       (20)      614 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/__init__.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.218295 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/
--rw-r--r--   0 sage       (501) staff       (20)      614 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     9261 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/coordinated_linr.yaml
--rw-r--r--   0 sage       (501) staff       (20)     9518 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/coordinated_lr.yaml
--rw-r--r--   0 sage       (501) staff       (20)     4815 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/data_split.yaml
--rw-r--r--   0 sage       (501) staff       (20)     1904 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/dataframe_io_test.yaml
--rw-r--r--   0 sage       (501) staff       (20)     1875 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/dataframe_transformer.yaml
--rw-r--r--   0 sage       (501) staff       (20)     2128 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/evaluation.yaml
--rw-r--r--   0 sage       (501) staff       (20)     4562 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/feature_scale.yaml
--rw-r--r--   0 sage       (501) staff       (20)     7956 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/hetero_feature_binning.yaml
--rw-r--r--   0 sage       (501) staff       (20)     7511 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/hetero_feature_selection.yaml
--rw-r--r--   0 sage       (501) staff       (20)     6557 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/hetero_sbt.yaml
--rw-r--r--   0 sage       (501) staff       (20)     6556 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/homo_lr.yaml
--rw-r--r--   0 sage       (501) staff       (20)     3251 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/homo_nn.yaml
--rw-r--r--   0 sage       (501) staff       (20)     1334 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/psi.yaml
--rw-r--r--   0 sage       (501) staff       (20)     2841 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/reader.yaml
--rw-r--r--   0 sage       (501) staff       (20)     3782 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/sample.yaml
--rw-r--r--   0 sage       (501) staff       (20)     3734 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/statistics.yaml
--rw-r--r--   0 sage       (501) staff       (20)      932 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/union.yaml
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.218552 fate-client-2.0.0b0/fate_client/pipeline/components/
--rw-r--r--   0 sage       (501) staff       (20)      729 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)    15360 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/component_base.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.220834 fate-client-2.0.0b0/fate_client/pipeline/components/fate/
--rw-r--r--   0 sage       (501) staff       (20)     1353 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     2543 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/coordinated_linr.py
--rw-r--r--   0 sage       (501) staff       (20)     2604 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/coordinated_lr.py
--rw-r--r--   0 sage       (501) staff       (20)     1698 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/data_split.py
--rw-r--r--   0 sage       (501) staff       (20)     1278 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/dataframe_io_test.py
--rw-r--r--   0 sage       (501) staff       (20)     1484 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/dataframe_transformer.py
--rw-r--r--   0 sage       (501) staff       (20)     1624 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/evaluation.py
--rw-r--r--   0 sage       (501) staff       (20)     1865 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/feature_scale.py
--rw-r--r--   0 sage       (501) staff       (20)     2484 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/hetero_feature_binning.py
--rw-r--r--   0 sage       (501) staff       (20)     2047 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/hetero_feature_selection.py
--rw-r--r--   0 sage       (501) staff       (20)     2908 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/hetero_sbt.py
--rw-r--r--   0 sage       (501) staff       (20)     2309 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/homo_lr.py
--rw-r--r--   0 sage       (501) staff       (20)     5658 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/homo_nn.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.221303 fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/
--rw-r--r--   0 sage       (501) staff       (20)      614 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     2927 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/algo_params.py
--rw-r--r--   0 sage       (501) staff       (20)     5097 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/loader.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.221902 fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/torch/
--rw-r--r--   0 sage       (501) staff       (20)      615 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/torch/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     2849 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/torch/base.py
--rw-r--r--   0 sage       (501) staff       (20)    77164 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/torch/nn.py
--rw-r--r--   0 sage       (501) staff       (20)    13688 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/torch/optim.py
--rw-r--r--   0 sage       (501) staff       (20)     1347 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/psi.py
--rw-r--r--   0 sage       (501) staff       (20)     1678 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/reader.py
--rw-r--r--   0 sage       (501) staff       (20)     1532 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/sample.py
--rw-r--r--   0 sage       (501) staff       (20)     1597 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/statistics.py
--rw-r--r--   0 sage       (501) staff       (20)     1225 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/components/fate/union.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.222432 fate-client-2.0.0b0/fate_client/pipeline/conf/
--rw-r--r--   0 sage       (501) staff       (20)      614 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/conf/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     1816 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/conf/env_config.py
--rw-r--r--   0 sage       (501) staff       (20)     1030 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/conf/job_configuration.py
--rw-r--r--   0 sage       (501) staff       (20)     2062 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/conf/types.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.223549 fate-client-2.0.0b0/fate_client/pipeline/entity/
--rw-r--r--   0 sage       (501) staff       (20)      726 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/entity/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     3932 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/entity/component_structures.py
--rw-r--r--   0 sage       (501) staff       (20)     4328 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/entity/dag.py
--rw-r--r--   0 sage       (501) staff       (20)     4417 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/entity/dag_structures.py
--rw-r--r--   0 sage       (501) staff       (20)     1348 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/entity/model_info.py
--rw-r--r--   0 sage       (501) staff       (20)     1417 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/entity/model_structure.py
--rw-r--r--   0 sage       (501) staff       (20)     2300 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/entity/runtime_entity.py
--rw-r--r--   0 sage       (501) staff       (20)     2344 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/entity/task_info.py
--rw-r--r--   0 sage       (501) staff       (20)     2169 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/entity/task_structure.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.223806 fate-client-2.0.0b0/fate_client/pipeline/executor/
--rw-r--r--   0 sage       (501) staff       (20)      697 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/executor/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     4448 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/executor/task_executor.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.224047 fate-client-2.0.0b0/fate_client/pipeline/interface/
--rw-r--r--   0 sage       (501) staff       (20)      819 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/interface/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     4383 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/interface/channel.py
--rw-r--r--   0 sage       (501) staff       (20)    11550 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/pipeline.py
--rw-r--r--   0 sage       (501) staff       (20)     3793 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/pipeline_cli.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.224400 fate-client-2.0.0b0/fate_client/pipeline/scheduler/
--rw-r--r--   0 sage       (501) staff       (20)      614 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/scheduler/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)     2460 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/scheduler/component_stage.py
--rw-r--r--   0 sage       (501) staff       (20)    30319 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/scheduler/dag_parser.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.224799 fate-client-2.0.0b0/fate_client/pipeline/utils/
--rw-r--r--   0 sage       (501) staff       (20)      614 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/utils/__init__.py
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.225255 fate-client-2.0.0b0/fate_client/pipeline/utils/fateflow/
--rw-r--r--   0 sage       (501) staff       (20)      614 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/utils/fateflow/__init__.py
--rw-r--r--   0 sage       (501) staff       (20)    10357 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/utils/fateflow/fate_flow_job_invoker.py
--rw-r--r--   0 sage       (501) staff       (20)     4420 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/utils/fateflow/flow_client.py
--rw-r--r--   0 sage       (501) staff       (20)      764 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/utils/file_utils.py
--rw-r--r--   0 sage       (501) staff       (20)     3249 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/pipeline/utils/test_utils.py
--rw-r--r--   0 sage       (501) staff       (20)      197 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/fate_client/settings.yaml
-drwxr-xr-x   0 sage       (501) staff       (20)        0 2023-09-19 06:31:17.210912 fate-client-2.0.0b0/fate_client.egg-info/
--rw-r--r--   0 sage       (501) staff       (20)      685 2023-09-19 06:31:17.000000 fate-client-2.0.0b0/fate_client.egg-info/PKG-INFO
--rw-r--r--   0 sage       (501) staff       (20)     5571 2023-09-19 06:31:17.000000 fate-client-2.0.0b0/fate_client.egg-info/SOURCES.txt
--rw-r--r--   0 sage       (501) staff       (20)        1 2023-09-19 06:31:17.000000 fate-client-2.0.0b0/fate_client.egg-info/dependency_links.txt
--rw-r--r--   0 sage       (501) staff       (20)      120 2023-09-19 06:31:17.000000 fate-client-2.0.0b0/fate_client.egg-info/entry_points.txt
--rw-r--r--   0 sage       (501) staff       (20)      144 2023-09-19 06:31:17.000000 fate-client-2.0.0b0/fate_client.egg-info/requires.txt
--rw-r--r--   0 sage       (501) staff       (20)       12 2023-09-19 06:31:17.000000 fate-client-2.0.0b0/fate_client.egg-info/top_level.txt
--rw-r--r--   0 sage       (501) staff       (20)       38 2023-09-19 06:31:17.225937 fate-client-2.0.0b0/setup.cfg
--rw-r--r--   0 sage       (501) staff       (20)     1888 2023-09-19 06:30:50.000000 fate-client-2.0.0b0/setup.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.188646 fate-client-2.1.0/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      176 2024-04-03 07:26:03.000000 fate-client-2.1.0/MANIFEST.in
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      679 2024-04-03 07:27:09.187993 fate-client-2.1.0/PKG-INFO
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.142634 fate-client-2.1.0/fate_client/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      637 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/__init__.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.146067 fate-client-2.1.0/fate_client/flow_cli/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      616 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/__init__.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.152336 fate-client-2.1.0/fate_client/flow_cli/commands/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      616 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4196 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/client.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3237 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/data.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4829 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/job.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1868 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/log.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2365 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/model.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     5089 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/output.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3294 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/permission.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2083 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/provider.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1213 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/server.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1147 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/site.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2065 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/table.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1856 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/task.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2604 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/commands/test.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     5736 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/flow.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.153608 fate-client-2.1.0/fate_client/flow_cli/utils/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      616 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/utils/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3749 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/utils/args_desc.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     7271 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/utils/cli_args.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2077 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_cli/utils/cli_utils.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.154166 fate-client-2.1.0/fate_client/flow_sdk/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      646 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1353 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/_client.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.160525 fate-client-2.1.0/fate_client/flow_sdk/api/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      949 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4429 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/client.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4224 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/data.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     6432 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/job.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2451 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/log.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3433 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/model.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     6161 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/output.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3708 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/permission.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2379 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/provider.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      916 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/service.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1040 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/site.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1973 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/table.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2503 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/task.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2666 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/api/test.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.162164 fate-client-2.1.0/fate_client/flow_sdk/utils/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/utils/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4868 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/utils/base_utils.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2335 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/utils/io_utils.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      863 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/flow_sdk/utils/params_utils.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.162950 fate-client-2.1.0/fate_client/pipeline/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      691 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/__init__.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.163177 fate-client-2.1.0/fate_client/pipeline/adapters/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1340 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/adapters/__init__.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.163408 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      615 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/__init__.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.164760 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      616 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1166 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/component_spec.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3611 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/component_translator.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1975 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/dag_spec.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)    21800 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/dsl_translator.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.165268 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/utils/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      616 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/utils/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1005 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/utils/types.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.165496 fate-client-2.1.0/fate_client/pipeline/component_define/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      614 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/__init__.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.171413 fate-client-2.1.0/fate_client/pipeline/component_define/fate/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      614 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     9254 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/coordinated_linr.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     9511 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/coordinated_lr.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4808 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/data_split.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1551 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/dataframe_transformer.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2139 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/evaluation.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2339 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/feature_correlation.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4555 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/feature_scale.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     7949 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/hetero_feature_binning.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     7500 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/hetero_feature_selection.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3304 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/hetero_nn.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     9749 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/hetero_secureboost.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     6665 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/homo_lr.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3314 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/homo_nn.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1331 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/psi.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1139 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/reader.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3775 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/sample.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     7121 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/sshe_linr.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     7119 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/sshe_lr.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3727 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/statistics.yaml
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      920 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/component_define/fate/union.yaml
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.171920 fate-client-2.1.0/fate_client/pipeline/components/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      729 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)    16000 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/component_base.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.177343 fate-client-2.1.0/fate_client/pipeline/components/fate/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1493 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2544 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/coordinated_linr.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2605 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/coordinated_lr.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1699 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/data_split.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1420 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/dataframe_transformer.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1628 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/evaluation.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1588 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/feature_correlation.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1866 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/feature_scale.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2485 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/hetero_feature_binning.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2048 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/hetero_feature_selection.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4943 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/hetero_nn.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3419 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/hetero_secureboost.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2283 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/homo_lr.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     5819 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/homo_nn.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.178611 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      614 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     9607 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/algo_params.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2977 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/common_utils.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     6283 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/loader.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)       13 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/source.yaml
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.179686 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/torch/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      615 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/torch/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2849 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/torch/base.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)    77164 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/torch/nn.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)    13688 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/nn/torch/optim.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1324 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/psi.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1217 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/reader.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1533 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/sample.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2562 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/sshe_linr.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2556 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/sshe_lr.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1598 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/statistics.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1218 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/components/fate/union.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.180631 fate-client-2.1.0/fate_client/pipeline/conf/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      614 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/conf/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1816 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/conf/env_config.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1030 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/conf/job_configuration.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2062 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/conf/types.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.182988 fate-client-2.1.0/fate_client/pipeline/entity/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      726 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/entity/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3932 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/entity/component_structures.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     6230 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/entity/dag.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4409 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/entity/dag_structures.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1348 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/entity/model_info.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1417 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/entity/model_structure.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3576 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/entity/runtime_entity.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2344 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/entity/task_info.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2169 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/entity/task_structure.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.183502 fate-client-2.1.0/fate_client/pipeline/executor/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      697 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/executor/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4644 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/executor/task_executor.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.183967 fate-client-2.1.0/fate_client/pipeline/interface/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      819 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/interface/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4382 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/interface/channel.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)    15191 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/pipeline.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3793 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/pipeline_cli.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.184677 fate-client-2.1.0/fate_client/pipeline/scheduler/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      614 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/scheduler/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     2460 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/scheduler/component_stage.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)    39472 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/scheduler/dag_parser.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.185545 fate-client-2.1.0/fate_client/pipeline/utils/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      614 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/utils/__init__.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.186070 fate-client-2.1.0/fate_client/pipeline/utils/callbacks/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      790 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/utils/callbacks/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4749 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/utils/callbacks/_callback.py
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.186791 fate-client-2.1.0/fate_client/pipeline/utils/fateflow/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      614 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/utils/fateflow/__init__.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)    10066 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/utils/fateflow/fate_flow_job_invoker.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     4420 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/utils/fateflow/flow_client.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      764 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/utils/file_utils.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     3202 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/pipeline/utils/test_utils.py
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      197 2024-04-03 07:26:03.000000 fate-client-2.1.0/fate_client/settings.yaml
+drwxr-xr-x   0 maguoqiang   (501) staff       (20)        0 2024-04-03 07:27:09.187098 fate-client-2.1.0/fate_client.egg-info/
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      679 2024-04-03 07:27:09.000000 fate-client-2.1.0/fate_client.egg-info/PKG-INFO
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     6646 2024-04-03 07:27:09.000000 fate-client-2.1.0/fate_client.egg-info/SOURCES.txt
+-rw-r--r--   0 maguoqiang   (501) staff       (20)        1 2024-04-03 07:27:09.000000 fate-client-2.1.0/fate_client.egg-info/dependency_links.txt
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      120 2024-04-03 07:27:09.000000 fate-client-2.1.0/fate_client.egg-info/entry_points.txt
+-rw-r--r--   0 maguoqiang   (501) staff       (20)      140 2024-04-03 07:27:09.000000 fate-client-2.1.0/fate_client.egg-info/requires.txt
+-rw-r--r--   0 maguoqiang   (501) staff       (20)       12 2024-04-03 07:27:09.000000 fate-client-2.1.0/fate_client.egg-info/top_level.txt
+-rw-r--r--   0 maguoqiang   (501) staff       (20)       38 2024-04-03 07:27:09.188777 fate-client-2.1.0/setup.cfg
+-rw-r--r--   0 maguoqiang   (501) staff       (20)     1884 2024-04-03 07:26:03.000000 fate-client-2.1.0/setup.py
```

### Comparing `fate-client-2.0.0b0/PKG-INFO` & `fate-client-2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fate-client
-Version: 2.0.0b0
+Version: 2.1.0
 Summary: Clients for FATE, supply pipeline this version
 Home-page: https://fate.fedai.org/
 Author: FederatedAI
 Author-email: contact@FedAI.org
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click
@@ -13,12 +13,12 @@
 Requires-Dist: requests
 Requires-Dist: requests_toolbelt
 Requires-Dist: ruamel.yaml
 Requires-Dist: setuptools
 Requires-Dist: networkx
 Requires-Dist: pydantic
 Provides-Extra: fate
-Requires-Dist: pyfate==2.0.0b0; extra == "fate"
+Requires-Dist: pyfate==2.1.0; extra == "fate"
 Provides-Extra: fate-flow
-Requires-Dist: fate_flow==2.0.0b0; extra == "fate-flow"
+Requires-Dist: fate_flow==2.1.0; extra == "fate-flow"
 
 Clients for FATE, supply pipeline this version
```

### Comparing `fate-client-2.0.0b0/fate_client/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/utils/file_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,9 +8,14 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+from ruamel import yaml
 
-__version__ = "2.0.0-beta"
+
+def load_yaml_file(path: str):
+    with open(path, "r") as fin:
+        buf = fin.read()
+        return yaml.safe_load(buf)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/__init__.py` & `fate-client-2.1.0/fate_client/flow_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/__init__.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/client.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/client.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/data.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,31 @@
     """
     config_data = preprocess(**kwargs)
     client: FlowClient = ctx.obj["client"]
     response = client.data.upload(**config_data)
     prettify(response)
 
 
+@data.command("upload-file")
+@cli_args.CONF_PATH
+@click.pass_context
+def upload_file(ctx, **kwargs):
+    """
+    \b
+    -description: Upload file to storage engine.
+
+    \b
+    -usage: flow data upload-file -c examples/upload/upload_guest.csv
+    """
+    config_data = preprocess(**kwargs)
+    client: FlowClient = ctx.obj["client"]
+    response = client.data.upload_file(**config_data)
+    prettify(response)
+
+
 @data.command("download-component")
 @cli_args.NAME_REQUIRED
 @cli_args.NAMESPACE_REQUIRED
 @cli_args.PATH_REQUIRED
 @click.pass_context
 def download_component(ctx, **kwargs):
     """
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/job.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/job.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/log.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/log.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/model.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/model.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/output.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/output.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/permission.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/permission.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/provider.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/provider.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/server.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/server.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/site.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/site.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/table.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/table.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,7 +60,24 @@
     \b
     -usage: flow table delete --name xxx --namespace xxx
     """
     client: FlowClient = ctx.obj["client"]
     response = client.table.delete(**kwargs)
     prettify(response)
 
+
+@table.command("bind")
+@cli_args.NAMESPACE_REQUIRED
+@cli_args.NAME_REQUIRED
+@cli_args.PATH_REQUIRED
+@click.pass_context
+def bind(ctx, **kwargs):
+    """
+    \b
+    -description: Bind data table.
+
+    \b
+    -usage: flow table bind --name xxx --namespace xxx -o /data/xxx
+    """
+    client: FlowClient = ctx.obj["client"]
+    response = client.table.bind_path(**kwargs)
+    prettify(response)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/task.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/task.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/commands/test.py` & `fate-client-2.1.0/fate_client/flow_cli/commands/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,19 @@
     """
     flow_sdk = FlowClient(ip=ctx.obj["ip"], port=ctx.obj["http_port"], version=ctx.obj["api_version"],
                           app_id=ctx.obj.get("app_id"), app_token=ctx.obj.get("app_token"))
     submit_result = flow_sdk.test.toy(**kwargs)
     if submit_result["code"] == 0:
         job_id = submit_result["job_id"]
         for t in range(kwargs["timeout"]):
-            r = flow_sdk.job.query(job_id=job_id, role="guest", party_id=kwargs["guest_party_id"])
+            party_id = kwargs["guest_party_id"]
+            info = flow_sdk.site.info()
+            if info.get("code") == 0:
+                party_id = info.get("data", {}).get("party_id", kwargs["guest_party_id"])
+            r = flow_sdk.job.query(job_id=job_id, party_id=party_id)
             if r["code"] == 0 and len(r["data"]):
                 job_status = r["data"][0]["status"]
                 print(f"toy test job {job_id} is {job_status}")
                 if job_status in {"failed", "canceled"}:
                     warn_print(job_id)
                     break
                 if job_status in {"success"}:
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/flow.py` & `fate-client-2.1.0/fate_client/flow_cli/flow.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/utils/__init__.py` & `fate-client-2.1.0/fate_client/flow_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/utils/args_desc.py` & `fate-client-2.1.0/fate_client/flow_cli/utils/args_desc.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,10 +98,11 @@
 APP_ID_DESC = "App ID for the client"
 SITE_APP_ID_DESC = "App ID for the site"
 SITE_APP_TOKEN_DESC = "App token for the site"
 
 
 GUEST_PARTY_ID_DESC = "Site ID of the guest"
 HOST_PARTY_ID_DESC = "Site ID of the host"
+ARBITER_PARTY_ID_DESC = "Site ID of the arbiter"
 CLIENT_PATH_DESC = "Directory or file path on the client"
 TIMEOUT_DESC = "Timeout limit"
 TASK_CORES_DESC = "Task cores"
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/utils/cli_args.py` & `fate-client-2.1.0/fate_client/flow_cli/utils/cli_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 import click
 
 from fate_client.flow_cli.utils.args_desc import CONF_PATH_DESC, LIMIT_DESC, JOB_ID_DESC, ROLE_DESC, \
     PERMISSION_ROLE_DESC, PARTY_ID_DESC, APP_ID_DESC, APP_NAME_DESC, SITE_APP_TOKEN_DESC, GUEST_PARTY_ID_DESC, \
     HOST_PARTY_ID_DESC, TASK_NAME_DESC, TASK_ID_DESC, TASK_VERSION_DESC, STATUS_DESC, CLIENT_PATH_DESC, NAME_DESC, \
     NAMESPACE_DESC, DISPLAY_DESC, MODEL_ID_DESC, MODEL_VERSION_DESC, SERVICE_NAME_DESC, SERVER_NAME_DESC, TIMEOUT_DESC, \
     TASK_CORES_DESC, LOG_TYPE_DESC, INSTANCE_ID_DESC, OUTPUT_KEY_DESC, DEVICE_DESC, VERSION_DESC, URI_DESC, METHOD_DESC, \
-    PARAMS_DESC, DATA_DESC, PROTOCOL_DESC, PROVIDER_NAME_DESC, HOST_DESC, PORT_DESC, NODES_DESC, TYPES_DESC
+    PARAMS_DESC, DATA_DESC, PROTOCOL_DESC, PROVIDER_NAME_DESC, HOST_DESC, PORT_DESC, NODES_DESC, TYPES_DESC, \
+    ARBITER_PARTY_ID_DESC
 
 role_ide_list = ["guest", "host", "arbiter", "local"]
 role_choices_list = ["site", "client", "super_client"]
 status_choices_list = ["success", "failed", "running", "waiting", "timeout", "canceled", "partial", "deleted"]
 
 CONF_PATH = click.option("-c", "--conf-path", type=click.Path(exists=True), required=True, help=CONF_PATH_DESC)
 LIMIT = click.option("-l", "--limit", type=click.INT, default=10, help=LIMIT_DESC)
@@ -45,14 +46,18 @@
 APP_TOKEN_REQUIRED = click.option("--app-token", type=click.STRING, required=True, help=SITE_APP_TOKEN_DESC)
 GUEST_PARTYID_REQUIRED = click.option(
     "-gid", "--guest-party-id", type=click.STRING, required=True, help=GUEST_PARTY_ID_DESC
 )
 HOST_PARTYID_REQUIRED = click.option(
     "-hid", "--host-party-id", type=click.STRING, required=True, help=HOST_PARTY_ID_DESC
 )
+
+ARBITER_PARTYID_REQUIRED = click.option(
+    "-aid", "--arbiter-party-id", type=click.STRING, required=True, help=ARBITER_PARTY_ID_DESC
+)
 TASK_NAME = click.option("-tn", "--task-name", type=click.STRING, help=TASK_NAME_DESC)
 TASK_NAME_REQUIRED = click.option("-tn", "--task-name", type=click.STRING, help=TASK_NAME_DESC, required=True,)
 TASK_ID = click.option("-tid", "--task-id", type=click.STRING, help=TASK_ID_DESC)
 TASK_ID_REQUIRED = click.option("-tid", "--task-id", type=click.STRING, help=TASK_ID_DESC, required=True,)
 TASK_VERSION = click.option("-tv", "--task-version", type=click.STRING, help=TASK_VERSION_DESC)
 STATUS = click.option("-s", "--status", type=click.Choice(status_choices_list), metavar="TEXT", help=STATUS_DESC)
 OUTPUT_PATH = click.option("-o", "--output-path", type=click.Path(exists=False), help=CLIENT_PATH_DESC)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_cli/utils/cli_utils.py` & `fate-client-2.1.0/fate_client/flow_cli/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/__init__.py` & `fate-client-2.1.0/fate_client/flow_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/_client.py` & `fate-client-2.1.0/fate_client/flow_sdk/_client.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/__init__.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/client.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         Query client
 
         Args:
             app_id: app_id.
             app_name: app_name.
 
         Returns:
-        {"code":0,"data":{"xxx":"xxx",},"message":"success"}
+        {"code":0,"data":{"app_id":"xxx","app_name":"xxx","app_token":"xxx","app_type":"xxx"},"message":"success"}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._get(url='/app/client/query', params=params)
 
     def create_site(self, party_id: str = None):
         """
@@ -119,29 +119,29 @@
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/app/partner/create', json=params)
 
     def delete_partner(self, party_id: str = None):
         """
-        Delete client
+        Delete partner
 
         Args:
             party_id: party_id.
 
         Returns:
         {"code":0,"data":{"status":"xxx"},"message":"success"}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/app/partner/delete', json=params)
 
     def query_partner(self, party_id: str = None):
         """
-        Query client
+        Query partner
 
         Args:
             party_id: party_id.
 
         Returns:
         {"code":0,"data":{"xxx":"xxx",},"message":"success"}
         """
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/data.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/table.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,88 +9,58 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
-import os
 from ..utils.base_utils import BaseFlowAPI
 from ..utils.params_utils import filter_invalid_params
-from ..utils.io_utils import download_from_request
 
 
-class Data(BaseFlowAPI):
-    def upload(self, file: str, head: bool, partitions: int, meta: dict, namespace: str = None, name: str = None,
-               extend_sid: bool = None, role: str = None, party_id: str = None):
+class Table(BaseFlowAPI):
+    def query(self, namespace: str = None, name: str = None, display: bool = False):
         """
-        upload data
-
+        query table
         Args:
-            file: file
-            head:
-            namespace:
-            name:
-            partitions:
-            extend_sid:
-            meta:
-            role:
-            party_id:
-
-
+            namespace: namespace
+            name: name
+            display: bool
 
         Returns:
-        {'code': 0, 'message': 'success','data':{...}]}
+        {'code': 0, 'message': 'success','data':{...}}
         """
         kwargs = locals()
-        if not os.path.exists(file):
-            raise Exception(f"{file} is not exist, please check the file path")
         params = filter_invalid_params(**kwargs)
-        return self._post(url='/data/component/upload', json=params)
+        return self._get(url='/table/query', params=params)
 
-    def dataframe_transformer(self, namespace: str, name: str, data_warehouse: dict, drop: bool = True,
-                              site_name: str = None):
+    def delete(self, namespace: str = None, name: str = None):
         """
+        delete table
         Args:
-            namespace:
-            name:
-            data_warehouse: {"namespace": xxx, "name": xxx}
-            drop: destroy table if the table exist
-            site_name: site name
+            namespace: namespace
+            name: name
 
         Returns:
-        {'code': 0, 'message': 'success','data':{...}]}
+        {'code': 0, 'message': 'success','data':{...}}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
-        return self._post(url='/data/component/dataframe/transformer', json=params)
+        return self._post(url='/table/delete', json=params)
 
-    def download(self, namespace: str = None, name: str = None, path: str = None):
+    def bind_path(self, namespace: str, name: str, path: str):
         """
-        download data
-
+        bind path
         Args:
-            namespace:
-            name:
+            namespace: namespace
+            name: name
+            path: path, /data/xxx
 
         Returns:
-
+        {'code': 0, 'message': 'success'}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
-        resp = self._get(url='/data/download', params=params, handle_result=False)
-        return download_from_request(resp, path)
-
-    def download_component(self, namespace: str = None, name: str = None, path: str = None):
-        """
-        download
+        return self._post(url='/table/bind/path', json=params)
 
-        Args:
-            namespace:
-            name:
 
-        Returns:
 
-        """
-        kwargs = locals()
-        params = filter_invalid_params(**kwargs)
-        return self._post(url='/data/component/download', json=params)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/job.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/job.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/log.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/log.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,41 +20,41 @@
 class Log(BaseFlowAPI):
     def count(self, log_type: str = None, job_id: bool = None, role: str = None, party_id: str = None,
               task_name: int = None, instance_id: str = None):
         """
         get log file count
 
         Args:
-            log_type:
-            job_id:
-            role:
-            party_id:
-            task_name:
-            instance_id:
+            log_type: log type such as: "task_error","task_warning","task_error","task_debug","fate_flow_schedule","fate_flow_schedule_error".
+            job_id: job id.
+            role: role, such as: "guest", "host".
+            party_id: party id, such as: "9999", "10000".
+            task_name: task name, such as:'psi_0...'
+            instance_id: instance id.
 
         Returns:
         {'code': 0, 'message': 'success','data':num]}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._get(url='/log/count', params=params)
 
     def query(self, log_type: str = None, job_id: bool = None, role: str = None, party_id: str = None,
               task_name: int = None, begin: int = None, end: int = None, instance_id: str = None):
         """
         query log
 
         Args:
-            log_type:
-            job_id:
-            role:
-            party_id:
-            task_name:
-            begin:
-            end:
-            instance_id:
+            log_type: log type such as: "info","warning","error","debug","fate_flow_schedule","fate_flow_schedule_error".
+            job_id: job id.
+            role: role, such as: "guest", "host".
+            party_id: party id, such as: "9999", "10000".
+            task_name: task name, such as:'psi_0',...
+            begin: num, starting line number.
+            end: num, ending line number.
+            instance_id: instance id.
         Returns:
-            {'code': 0, 'message': 'success','data':num]}
+            {'code': 0, 'message': 'success','data':[]}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._get(url='/log/query', params=params)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/model.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,43 +43,54 @@
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/model/migrate', params=params)
 
     def export(self, role: str, model_id: str, model_version: str, party_id: str, path: str):
         """
-
+        export model data
         Args:
-
+            role: role.
+            model_id: model_id.
+            model_version: model_version.
+            party_id: party_id.
+            path: path, /data/xxx
         Returns:
-
+            {"code":0,"data":{"status":"xxx"},"message":"success"}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/model/export', json=params)
 
     def import_model(self, model_id: str, model_version: str, path: str):
         """
-
+        import model data
         Args:
-
+            model_id: model_id.
+            model_version: model_version.
+            path: path, /data/xxx.
         Returns:
 
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         files = {'file': open(path, 'rb')}
         return self._post(url='/model/import', data=params, files=files, handle_result=False)
 
     def delete_model(self, model_id: str, model_version: str, role: str = None,
                      party_id: str = None, task_name: str = None, output_key: str = None):
         """
-
+        delete model
         Args:
-
+            model_id: model_id
+            model_version: model_version
+            role: role, such as: "guest", "host"
+            party_id: party id, such as: "9999", "10000"
+            task_name: task name
+            output_key: output key, Primary key for output data or model of the task
         Returns:
 
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/model/delete', json=params)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/permission.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/permission.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,45 +19,45 @@
 
 class Permission(BaseFlowAPI):
     def grant(self, app_id: str = None, role: str = None):
         """
         add role to user
 
         Args:
-            app_id:
-            role:
+            app_id: app id.
+            role: role,such as: "site", "client", "super_client".
 
         Returns:
         {'code': 0, 'message': 'success','data':None}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/permission/grant', json=params)
 
     def delete(self, app_id: str = None, role: str = None):
         """
         delete role to user
 
         Args:
-            app_id:
-            role:
+            app_id: app id
+            role: role,such as: "site", "client", "super_client".
 
         Returns:
         {'code': 0, 'message': 'success','data':None}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/permission/delete', json=params)
 
     def query(self, app_id: str = None):
         """
         query user permission
 
         Args:
-            app_id:
+            app_id: app id.
 
         Returns:
         {'code': 0, 'message': 'success','data':{...}}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._get(url='/permission/query', params=params)
@@ -71,34 +71,46 @@
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._get(url='/permission/role/query', params=params)
 
     def grant_resource(self, party_id: str, component: str = None, dataset: dict = None):
         """
         grant resource
+        Args:
+            party_id: party id.
+            component: component.
+            dataset: {'name':xxx,'namespace':xxx}.
+
         Returns:
         {'code': 0, 'message': 'success','data':[...]}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/permission/resource/grant', json=params)
 
     def delete_resource(self, party_id: str, component: str = None, dataset: dict = None):
         """
         delete resource
+        Args:
+            party_id: party id.
+            component: component.
+            dataset: {'name':xxx,'namespace':xxx}.
         Returns:
         {'code': 0, 'message': 'success','data':[...]}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/permission/resource/delete', json=params)
 
     def query_resource(self, party_id: str, component: str = None, dataset: dict = None):
         """
-        delete resource
+        query resource
+            party_id: party id.
+            component: component.
+            dataset: {'name':xxx,'namespace':xxx}.
         Returns:
         {'code': 0, 'message': 'success','data':[...]}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._get(url='/permission/resource/query', params=params)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/provider.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,54 +14,57 @@
 #  limitations under the License.
 #
 from ..utils.base_utils import BaseFlowAPI
 from ..utils.params_utils import filter_invalid_params
 
 
 class Provider(BaseFlowAPI):
-    def register(self, name: str = None, device: str = None, version: str = None, metadata: dict = None):
+    def register(self, name: str = None, device: str = None, version: str = None, metadata: dict = None,
+                 protocol: str = None, components_description: dict = None):
         """
 
         Args:
-            name:
-            device:
-            version:
-            metadata:
+            name: name.
+            device: device.
+            version: version.
+            metadata: metadata.
+            protocol: protocol, such as:fate,bfia...
+            components_description: components description.
 
         Returns:
         {'code': 0, 'message': 'device success','data':None}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/provider/register', json=params)
 
     def query(self, name: str = None, device: str = None, version: str = None, provider_name: str = None):
         """
 
         Args:
-            name:
-            device:
-            version:
-            provider_name:
+            name: name
+            device: device
+            version: version
+            provider_name: provider name
 
         Returns:
         {'code': 0, 'message': 'success','data':[{...},{...}]}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._get(url='/provider/query', params=params)
 
     def delete(self, name: str = None, device: str = None, version: str = None, provider_name: str = None):
         """
 
         Args:
-            name:
-            device:
-            version:
-            provider_name:
+            name: name
+            device: device
+            version: version
+            provider_name: provider name
 
         Returns:
         {'code': 0, 'message': 'success','data':{...}}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._post(url='/provider/delete', json=params)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/service.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/service.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/site.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/site.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from ..utils.base_utils import BaseFlowAPI
 from ..utils.params_utils import filter_invalid_params
 
 
 class Site(BaseFlowAPI):
     def info(self):
         """
+        get site party_id
 
         Returns:
         {'code': 0, 'message': 'success','data':{"party_id": xxxxx}}
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
         return self._get(url='/site/info/query', params=params)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/task.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 class Task(BaseFlowAPI):
     def query(self, job_id: str = None, role: str = None, party_id: str = None, task_name: str = None,
               status: str = None, task_id: str = None, task_version: int = None):
         """
         task query info
 
         Args:
-            job_id: job id
-            role: role, such as: "guest", "host"
-            party_id: party id, such as: "9999", "10000"
-            task_name: task name
-            status: task status
-            task_id: task id
-            task_version: task version
+            job_id: job id.
+            role: role, such as: "guest", "host".
+            party_id: party id, such as: "9999", "10000".
+            task_name: task name.
+            status: task status.
+            task_id: task id.
+            task_version: task version.
 
         Returns:
         {'code': 0, 'message': 'success','data':[{...},{...}]}
         :return:
         """
         kwargs = locals()
         params = filter_invalid_params(**kwargs)
```

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/api/test.py` & `fate-client-2.1.0/fate_client/flow_sdk/api/test.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/utils/base_utils.py` & `fate-client-2.1.0/fate_client/flow_sdk/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/utils/io_utils.py` & `fate-client-2.1.0/fate_client/flow_sdk/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/flow_sdk/utils/params_utils.py` & `fate-client-2.1.0/fate_client/flow_sdk/utils/params_utils.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/component_define/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/coordinated_linr.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/coordinated_linr.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 component:
   name: coordinated_linr
   description: ''
   provider: fate
-  version: 2.0.0-beta
-  labels: [ ]
+  version: 2.1.0
+  labels: []
   roles:
     - guest
     - host
     - arbiter
   parameters:
     learning_rate_scheduler:
       type: LRSchedulerParam
@@ -369,12 +369,13 @@
         description: ''
         is_multi: false
     metric:
       metric:
         types:
           - json_metric
         optional: false
-        stages: [ ]
-        roles: [ ]
+        stages: []
+        roles: []
         description: metric, invisible for user
         is_multi: false
 schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/coordinated_lr.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/coordinated_lr.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 component:
   name: coordinated_lr
   description: ''
   provider: fate
-  version: 2.0.0-beta
-  labels: [ ]
+  version: 2.1.0
+  labels: []
   roles:
     - guest
     - host
     - arbiter
   parameters:
     learning_rate_scheduler:
       type: LRSchedulerParam
@@ -379,12 +379,13 @@
         description: ''
         is_multi: false
     metric:
       metric:
         types:
           - json_metric
         optional: false
-        stages: [ ]
-        roles: [ ]
+        stages: []
+        roles: []
         description: metric, invisible for user
         is_multi: false
 schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/data_split.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/data_split.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 component:
   name: data_split
   description: ''
   provider: fate
-  version: 2.0.0-beta
-  labels: [ ]
+  version: 2.1.0
+  labels: []
   roles:
     - guest
     - host
   parameters:
     train_size:
       type: typing.Union[fate.components.core.params._fields.ConstrainedFloatValue,
         fate.components.core.params._fields.ConstrainedIntValue]
@@ -107,15 +107,15 @@
         stages:
           - default
         roles:
           - guest
           - host
         description: ''
         is_multi: false
-    model: { }
+    model: {}
   output_artifacts:
     data:
       train_output_data:
         types:
           - dataframe
         optional: true
         stages:
@@ -143,21 +143,22 @@
         stages:
           - default
         roles:
           - guest
           - host
         description: ''
         is_multi: false
-    model: { }
+    model: {}
     metric:
       metric:
         types:
           - json_metric
         optional: false
         stages:
           - default
         roles:
           - guest
           - host
         description: metric, invisible for user
         is_multi: false
 schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/dataframe_io_test.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/dataframe_transformer.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,86 @@
 component:
-  name: dataframe_io_test
+  name: dataframe_transformer
   description: ''
   provider: fate
-  version: 2.0.0-beta
+  version: 2.1.0
   labels: []
   roles:
     - local
-  parameters: {}
+    - guest
+    - host
+  parameters:
+    namespace:
+      type: str
+      default:
+      optional: true
+      description: ''
+      type_meta:
+        title: str
+        type: string
+        default:
+        description: ''
+    name:
+      type: str
+      default:
+      optional: true
+      description: ''
+      type_meta:
+        title: str
+        type: string
+        default:
+        description: ''
+    site_name:
+      type: str
+      default:
+      optional: true
+      description: ''
+      type_meta:
+        title: str
+        type: string
+        default:
+        description: ''
   input_artifacts:
     data:
-      dataframe_input:
+      table:
         types:
-          - dataframe
+          - table
         optional: false
         stages:
           - default
         roles:
           - local
+          - guest
+          - host
         description: ''
         is_multi: false
-      dataframe_inputs:
-        types:
-          - dataframe
-        optional: false
-        stages:
-          - default
-        roles:
-          - local
-        description: ''
-        is_multi: true
     model: {}
   output_artifacts:
     data:
       dataframe_output:
         types:
           - dataframe
         optional: false
         stages:
           - default
         roles:
           - local
+          - guest
+          - host
         description: ''
         is_multi: false
-      dataframe_outputs:
-        types:
-          - dataframe
-        optional: false
-        stages:
-          - default
-        roles:
-          - local
-        description: ''
-        is_multi: true
-    model:
-      json_model_output:
-        types:
-          - json_model
-        optional: false
-        stages:
-          - default
-        roles:
-          - local
-        description: ''
-        is_multi: false
-      json_model_outputs:
-        types:
-          - json_model
-        optional: false
-        stages:
-          - default
-        roles:
-          - local
-        description: ''
-        is_multi: true
-      model_directory_output:
+    model: {}
+    metric:
+      metric:
         types:
-          - model_directory
+          - json_metric
         optional: false
         stages:
           - default
         roles:
           - local
-        description: ''
+          - guest
+          - host
+        description: metric, invisible for user
         is_multi: false
-      model_directory_outputs:
-        types:
-          - model_directory
-        optional: false
-        stages:
-          - default
-        roles:
-          - local
-        description: ''
-        is_multi: true
-    metric: {}
-schema_version: v1
+schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/evaluation.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/evaluation.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 component:
   name: evaluation
   description: ''
   provider: fate
-  version: 2.0.0-beta
+  version: 2.1.0
   labels: []
   roles:
     - guest
     - host
   parameters:
     default_eval_setting:
       type: type
@@ -28,16 +28,16 @@
         default:
         description: ''
     predict_column_name:
       type: str
       default:
       optional: true
       description: predict data column name, if None(default), will use                                         'predict_score'
-        when use binary and regression default setting,                                         and
-        use 'predict_result' on multi classification default setting
+        in the input dataframe when the default setting are binary and regression,                                         and
+        use 'predict_result' if default setting is multi
       type_meta:
         title: str
         type: string
         default:
         description: label data column namem if None(default),                                      will
           use 'label' in the input dataframe
     label_column_name:
@@ -50,15 +50,15 @@
         title: str
         type: string
         default:
         description: label data column namem if None(default),                                      will
           use 'label' in the input dataframe
   input_artifacts:
     data:
-      input_data:
+      input_datas:
         types:
           - dataframe
         optional: false
         stages:
           - default
         roles:
           - guest
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/feature_scale.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/feature_scale.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 component:
   name: feature_scale
   description: ''
   provider: fate
-  version: 2.0.0-beta
+  version: 2.1.0
   labels: []
   roles:
     - guest
     - host
   parameters:
     method:
       type: type
@@ -25,15 +25,15 @@
       description: 'Result feature value range for `min_max` method, take either dict
         in format: {col_name: [min, max]} for specific columns or [min, max] for all
         columns. Columns unspecified will be scaled to default range [0,1]'
       type_meta:
         title: typing.Union[list, dict]
         anyOf:
           - type: array
-            items: { }
+            items: {}
           - type: object
         default:
           - 0
           - 1
         description: 'Result feature value range for `min_max` method, take either
           dict in format: {col_name: [min, max]} for specific columns or [min, max]
           for all columns. Columns unspecified will be scaled to default range [0,1]'
@@ -160,12 +160,13 @@
         description: ''
         is_multi: false
     metric:
       metric:
         types:
           - json_metric
         optional: false
-        stages: [ ]
-        roles: [ ]
+        stages: []
+        roles: []
         description: metric, invisible for user
         is_multi: false
 schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/hetero_feature_binning.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/hetero_feature_binning.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 component:
   name: hetero_feature_binning
   description: ''
   provider: fate
-  version: 2.0.0-beta
-  labels: [ ]
+  version: 2.1.0
+  labels: []
   roles:
     - guest
     - host
   parameters:
     method:
       type: type
       default: quantile
@@ -262,12 +262,13 @@
         description: ''
         is_multi: false
     metric:
       metric:
         types:
           - json_metric
         optional: false
-        stages: [ ]
-        roles: [ ]
+        stages: []
+        roles: []
         description: metric, invisible for user
         is_multi: false
 schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/hetero_feature_selection.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/hetero_feature_selection.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 component:
   name: hetero_feature_selection
   description: ''
   provider: fate
-  version: 2.0.0-beta
-  labels: [ ]
+  version: 2.1.0
+  labels: []
   roles:
     - guest
     - host
   parameters:
     method:
       type: typing.List[fate.components.core.params._fields.StringChoice]
       default:
@@ -174,31 +174,31 @@
               - true
             type: array
             items:
               type: boolean
     manual_param:
       type: ModelMetaclass
       default:
-        keep_col: [ ]
-        filter_out_col: [ ]
+        keep_col: []
+        filter_out_col: []
       optional: true
       description: manual filter param
       type_meta:
         title: ManualFilterParam
         type: object
         properties:
           keep_col:
             title: Keep Col
-            default: [ ]
+            default: []
             type: array
             items:
               type: string
           filter_out_col:
             title: Filter Out Col
-            default: [ ]
+            default: []
             type: array
             items:
               type: string
     keep_one:
       type: bool
       default: true
       optional: true
@@ -305,12 +305,13 @@
         description: ''
         is_multi: false
     metric:
       metric:
         types:
           - json_metric
         optional: false
-        stages: [ ]
-        roles: [ ]
+        stages: []
+        roles: []
         description: metric, invisible for user
         is_multi: false
 schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/hetero_sbt.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/sshe_lr.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,176 +1,187 @@
 component:
-  name: hetero_sbt
+  name: sshe_lr
   description: ''
   provider: fate
-  version: 2.0.0-beta
+  version: 2.1.0
   labels: []
   roles:
     - guest
     - host
   parameters:
-    num_trees:
+    epochs:
       type: ConstrainedNumberMeta
-      default: 3
+      default: 20
       optional: true
-      description: max tree num
+      description: max iteration num
       type_meta:
         title: ConstrainedNumberMeta
         exclusiveMinimum: 0
         type: integer
-    learning_rate:
-      type: ConstrainedNumberMeta
-      default: 0.3
-      optional: true
-      description: decay factor of each tree
-      type_meta:
-        title: ConstrainedNumberMeta
-        exclusiveMinimum: 0
-        type: number
-    max_depth:
+    batch_size:
       type: ConstrainedNumberMeta
-      default: 3
+      default:
       optional: true
-      description: max depth of a tree
+      description: batch size, None means full batch, otherwise should be no less
+        than 10, default None
       type_meta:
         title: ConstrainedNumberMeta
-        exclusiveMinimum: 0
+        minimum: 10
         type: integer
-    max_bin:
+    tol:
       type: ConstrainedNumberMeta
-      default: 32
+      default: 0.0001
       optional: true
-      description: max bin number of feature binning
+      description: ''
       type_meta:
         title: ConstrainedNumberMeta
-        exclusiveMinimum: 0
-        type: integer
-    objective:
+        minimum: 0
+        type: number
+    early_stop:
       type: type
-      default: binary:bce
+      default: diff
       optional: true
-      description: "objective function, available: ['binary:bce', 'multi:ce', 'regression:l2']"
+      description: early stopping criterion, choose from {weight_diff, diff, abs},
+        if use weight_diff,weight will be revealed every epoch
       type_meta:
         title: type
         type: string
-    num_class:
-      type: ConstrainedNumberMeta
-      default: 2
-      optional: true
-      description: class number of multi classification, active when objective is
-        multi:ce
-      type_meta:
-        title: ConstrainedNumberMeta
-        exclusiveMinimum: 0
-        type: integer
-    l2:
+    learning_rate:
       type: ConstrainedNumberMeta
-      default: 0.1
+      default: 0.05
       optional: true
-      description: L2 regularization
+      description: learning rate
       type_meta:
         title: ConstrainedNumberMeta
-        exclusiveMinimum: 0
+        minimum: 0
         type: number
-    min_impurity_split:
-      type: ConstrainedNumberMeta
-      default: 0.01
+    reveal_every_epoch:
+      type: bool
+      default: false
       optional: true
-      description: min impurity when splitting a tree node
+      description: whether reveal encrypted result every epoch, only accept False
+        for now
       type_meta:
-        title: ConstrainedNumberMeta
-        exclusiveMinimum: 0
-        type: number
-    min_sample_split:
-      type: ConstrainedNumberMeta
-      default: 2
+        title: bool
+        type: boolean
+        default: true
+        description: whether output prediction result per cv fold
+    init_param:
+      type: InitParam
+      default:
+        method: random_uniform
+        fill_val: 0.0
+        fit_intercept: true
+        random_state:
       optional: true
-      description: min sample to split a tree node
+      description: Model param init setting.
       type_meta:
-        title: ConstrainedNumberMeta
-        exclusiveMinimum: 0
-        type: integer
-    min_leaf_node:
+        title: InitParam
+        $ref: '#/definitions/abc__InitParam'
+        definitions:
+          abc__InitParam:
+            title: InitParam
+            type: object
+            properties:
+              method:
+                title: Method
+                default: zeros
+                type: string
+              fill_val:
+                title: Fill Val
+                default: 0.0
+                anyOf:
+                  - type: integer
+                  - type: number
+              fit_intercept:
+                title: Fit Intercept
+                default: true
+                type: boolean
+              random_state:
+                title: Random State
+                type: integer
+        default:
+          method: random_uniform
+          fill_val: 0.0
+          fit_intercept: true
+          random_state:
+        description: Model param init setting.
+    threshold:
       type: ConstrainedNumberMeta
-      default: 1
+      default: 0.5
       optional: true
-      description: mininum sample contained in a leaf node
+      description: predict threshold for binary data
       type_meta:
         title: ConstrainedNumberMeta
-        exclusiveMinimum: 0
-        type: integer
-    min_child_weight:
+        minimum: 0.0
+        maximum: 1.0
+        type: number
+    reveal_loss_freq:
       type: ConstrainedNumberMeta
       default: 1
       optional: true
-      description: minumum hessian contained in a leaf node
+      description: rounds to reveal training loss, only effective if `early_stop`
+        is 'loss'
       type_meta:
         title: ConstrainedNumberMeta
-        exclusiveMinimum: 0
-        type: number
-    gh_pack:
-      type: bool
-      default: true
+        minimum: 1
+        type: integer
+    cv_param:
+      type: CVParam
+      default:
+        n_splits: 5
+        shuffle: false
+        random_state:
       optional: true
-      description: whether to pack gradient and hessian together
+      description: cross validation param
       type_meta:
-        title: bool
-        type: boolean
-        default: true
-        description: whether to use histogram subtraction
-    split_info_pack:
-      type: bool
-      default: true
+        title: CVParam
+        $ref: '#/definitions/abc__CVParam'
+        definitions:
+          abc__CVParam:
+            title: CVParam
+            type: object
+            properties:
+              n_splits:
+                title: N Splits
+                exclusiveMinimum: 1
+                type: integer
+              shuffle:
+                title: Shuffle
+                default: false
+                type: boolean
+              random_state:
+                title: Random State
+                type: integer
+            required:
+              - n_splits
+        default:
+          n_splits: 5
+          shuffle: false
+          random_state:
+        description: cross validation param
+    metrics:
+      type: type
+      default:
+        - auc
       optional: true
-      description: for host side, whether to pack split info together
+      description: ''
       type_meta:
-        title: bool
-        type: boolean
-        default: true
-        description: whether to use histogram subtraction
-    hist_sub:
+        title: type
+        type: string
+    output_cv_data:
       type: bool
       default: true
       optional: true
-      description: whether to use histogram subtraction
+      description: whether output prediction result per cv fold
       type_meta:
         title: bool
         type: boolean
         default: true
-        description: whether to use histogram subtraction
-    he_param:
-      type: HEParam
-      default:
-        kind: paillier
-        key_length: 1024
-      optional: true
-      description: homomorphic encryption param, support paillier, ou and mock in
-        current version
-      type_meta:
-        title: HEParam
-        $ref: '#/definitions/abc__HEParam'
-        definitions:
-          abc__HEParam:
-            title: HEParam
-            type: object
-            properties:
-              kind:
-                title: Kind
-                type: string
-              key_length:
-                title: Key Length
-                default: 1024
-                type: integer
-            required:
-              - kind
-        default:
-          kind: paillier
-          key_length: 1024
-        description: homomorphic encryption param, support paillier, ou and mock in
-          current version
+        description: whether output prediction result per cv fold
   input_artifacts:
     data:
       train_data:
         types:
           - dataframe
         optional: false
         stages:
@@ -198,66 +209,86 @@
         stages:
           - predict
         roles:
           - guest
           - host
         description: ''
         is_multi: false
+      cv_data:
+        types:
+          - dataframe
+        optional: false
+        stages:
+          - cross_validation
+        roles:
+          - guest
+          - host
+        description: ''
+        is_multi: false
     model:
-      train_model_input:
+      warm_start_model:
         types:
           - json_model
         optional: true
         stages:
           - train
         roles:
           - guest
           - host
         description: ''
         is_multi: false
-      predict_model_input:
+      input_model:
         types:
           - json_model
         optional: false
         stages:
           - predict
         roles:
           - guest
           - host
         description: ''
         is_multi: false
   output_artifacts:
     data:
-      train_data_output:
+      train_output_data:
         types:
           - dataframe
-        optional: true
+        optional: false
         stages:
           - train
         roles:
           - guest
-          - host
         description: ''
         is_multi: false
       test_output_data:
         types:
           - dataframe
         optional: false
         stages:
           - predict
         roles:
           - guest
-          - host
         description: ''
         is_multi: false
+      cv_output_datas:
+        types:
+          - dataframe
+        optional: true
+        stages:
+          - cross_validation
+        roles:
+          - guest
+          - host
+        description: ''
+        is_multi: true
     model:
-      train_model_output:
+      output_model:
         types:
           - json_model
-        optional: true
+        optional: false
         stages:
           - train
         roles:
           - guest
           - host
         description: ''
         is_multi: false
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/homo_lr.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/homo_lr.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 component:
   name: homo_lr
   description: ''
   provider: fate
-  version: 2.0.0-beta
+  version: 2.1.0
   labels: []
   roles:
     - guest
     - host
     - arbiter
   parameters:
     learning_rate_scheduler:
       type: LRSchedulerParam
       default:
-        method: linear
+        method: constant
         scheduler_params:
-          start_factor: 1.0
+          factor: 1.0
       optional: true
       description: learning rate scheduler, select method from {'step', 'linear',
         'constant'}for list of configurable arguments, refer to torch.optim.lr_scheduler
       type_meta:
         title: LRSchedulerParam
         $ref: '#/definitions/abc__LRSchedulerParam'
         definitions:
@@ -30,17 +30,17 @@
                 title: Method
                 default: constant
                 type: string
               scheduler_params:
                 title: Scheduler Params
                 type: object
         default:
-          method: linear
+          method: constant
           scheduler_params:
-            start_factor: 1.0
+            factor: 1.0
         description: learning rate scheduler, select method from {'step', 'linear',
           'constant'}for list of configurable arguments, refer to torch.optim.lr_scheduler
     epochs:
       type: ConstrainedNumberMeta
       default: 20
       optional: true
       description: max iteration num
@@ -48,18 +48,18 @@
         title: ConstrainedNumberMeta
         exclusiveMinimum: 0
         type: integer
     batch_size:
       type: ConstrainedNumberMeta
       default: 100
       optional: true
-      description: batch size, value less or equals to 0 means full batch
+      description: batch size, int > 0, if None means full batchnon
       type_meta:
         title: ConstrainedNumberMeta
-        minimum: -1
+        minimum: 0
         type: integer
     optimizer:
       type: OptimizerParam
       default:
         method: sgd
         penalty: l2
         alpha: 1.0
@@ -100,17 +100,18 @@
           optimizer_params:
             lr: 0.01
             weight_decay: 0
         description: ''
     init_param:
       type: InitParam
       default:
-        method: zeros
+        method: random
         fill_val: 0.0
         fit_intercept: true
+        random_state:
       optional: true
       description: Model param init setting.
       type_meta:
         title: InitParam
         $ref: '#/definitions/abc__InitParam'
         definitions:
           abc__InitParam:
@@ -127,18 +128,22 @@
                 anyOf:
                   - type: integer
                   - type: number
               fit_intercept:
                 title: Fit Intercept
                 default: true
                 type: boolean
+              random_state:
+                title: Random State
+                type: integer
         default:
-          method: zeros
+          method: random
           fill_val: 0.0
           fit_intercept: true
+          random_state:
         description: Model param init setting.
     threshold:
       type: ConstrainedNumberMeta
       default: 0.5
       optional: true
       description: predict threshold for binary data
       type_meta:
@@ -146,20 +151,20 @@
         minimum: 0.0
         maximum: 1.0
         type: number
     ovr:
       type: bool
       default: false
       optional: true
-      description: predict threshold for binary data
+      description: enable ovr for multi-classifcation
       type_meta:
         title: bool
         type: boolean
         default: false
-        description: predict threshold for binary data
+        description: enable ovr for multi-classifcation
     label_num:
       type: ConstrainedNumberMeta
       default:
       optional: true
       description: ''
       type_meta:
         title: ConstrainedNumberMeta
@@ -197,26 +202,26 @@
           - predict
         roles:
           - guest
           - host
         description: ''
         is_multi: false
     model:
-      train_input_model:
+      warm_start_model:
         types:
           - json_model
         optional: true
         stages:
           - train
         roles:
           - guest
           - host
         description: ''
         is_multi: false
-      predict_input_model:
+      input_model:
         types:
           - json_model
         optional: false
         stages:
           - predict
         roles:
           - guest
@@ -244,15 +249,15 @@
           - predict
         roles:
           - guest
           - host
         description: ''
         is_multi: false
     model:
-      train_output_model:
+      output_model:
         types:
           - json_model
         optional: false
         stages:
           - train
         roles:
           - guest
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/homo_nn.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/homo_nn.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 component:
   name: homo_nn
   description: ''
   provider: fate
-  version: 2.0.0-beta
+  version: 2.1.0
   labels: []
   roles:
     - guest
     - host
     - arbiter
   parameters:
     runner_module:
       type: str
-      default: default_runner
+      default: homo_default_runner
       optional: true
       description: name of your runner script
       type_meta:
         title: str
         type: string
         default:
         description: path to your runner script folder
@@ -50,93 +50,96 @@
         default:
         description: path to your runner script folder
   input_artifacts:
     data:
       train_data:
         types:
           - dataframe
+          - data_directory
         optional: false
         stages:
           - train
         roles:
           - guest
           - host
         description: ''
         is_multi: false
       validate_data:
         types:
           - dataframe
+          - data_directory
         optional: true
         stages:
           - train
         roles:
           - guest
           - host
         description: ''
         is_multi: false
       test_data:
         types:
           - dataframe
+          - data_directory
         optional: false
         stages:
           - predict
         roles:
           - guest
           - host
         description: ''
         is_multi: false
     model:
-      train_model_input:
+      warm_start_model:
         types:
           - model_directory
         optional: true
         stages:
           - train
         roles:
           - guest
           - host
         description: ''
         is_multi: false
-      predict_model_input:
+      input_model:
         types:
           - model_directory
         optional: false
         stages:
           - predict
         roles:
           - guest
           - host
         description: ''
         is_multi: false
   output_artifacts:
     data:
-      train_data_output:
+      train_output_data:
         types:
           - dataframe
         optional: true
         stages:
           - train
         roles:
           - guest
           - host
         description: ''
         is_multi: false
-      predict_data_output:
+      test_output_data:
         types:
           - dataframe
         optional: true
         stages:
           - predict
         roles:
           - guest
           - host
         description: ''
         is_multi: false
     model:
-      train_model_output:
+      output_model:
         types:
           - model_directory
         optional: true
         stages:
           - train
         roles:
           - guest
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/psi.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/psi.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 component:
   name: psi
   description: ''
   provider: fate
-  version: 2.0.0-beta
+  version: 2.1.0
   labels: []
   roles:
     - guest
     - host
   parameters:
     protocol:
       type: str
@@ -64,8 +64,9 @@
         stages:
           - default
         roles:
           - guest
           - host
         description: metric, invisible for user
         is_multi: false
-schema_version: v1
+schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/sample.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/sample.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 component:
   name: sample
   description: ''
   provider: fate
-  version: 2.0.0-beta
-  labels: [ ]
+  version: 2.1.0
+  labels: []
   roles:
     - guest
     - host
   parameters:
     replace:
       type: bool
       default: false
@@ -85,35 +85,36 @@
         stages:
           - default
         roles:
           - guest
           - host
         description: ''
         is_multi: false
-    model: { }
+    model: {}
   output_artifacts:
     data:
       output_data:
         types:
           - dataframe
         optional: false
         stages:
           - default
         roles:
           - guest
           - host
         description: ''
         is_multi: false
-    model: { }
+    model: {}
     metric:
       metric:
         types:
           - json_metric
         optional: false
         stages:
           - default
         roles:
           - guest
           - host
         description: metric, invisible for user
         is_multi: false
 schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/statistics.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/statistics.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 component:
   name: statistics
   description: ''
   provider: fate
-  version: 2.0.0-beta
-  labels: [ ]
+  version: 2.1.0
+  labels: []
   roles:
     - guest
     - host
   parameters:
     metrics:
       type: typing.Union[typing.List[typing.Union[fate.components.core.params._metrics.StatisticMetrics,
         fate.components.core.params._metrics.LegalPercentile]], fate.components.core.params._metrics.StatisticMetrics,
@@ -102,17 +102,17 @@
         stages:
           - default
         roles:
           - guest
           - host
         description: ''
         is_multi: false
-    model: { }
+    model: {}
   output_artifacts:
-    data: { }
+    data: {}
     model:
       output_model:
         types:
           - json_model
         optional: false
         stages:
           - default
@@ -130,7 +130,8 @@
           - default
         roles:
           - guest
           - host
         description: metric, invisible for user
         is_multi: false
 schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/component_define/fate/union.yaml` & `fate-client-2.1.0/fate_client/pipeline/component_define/fate/reader.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,64 @@
 component:
-  name: union
+  name: reader
   description: ''
   provider: fate
-  version: 2.0.0-beta
-  labels: [ ]
+  version: 2.1.0
+  labels: []
   roles:
     - guest
     - host
-  parameters: { }
-  input_artifacts:
-    data:
-      input_data_list:
-        types:
-          - dataframe
-        optional: false
-        stages:
-          - default
-        roles:
-          - guest
-          - host
+    - arbiter
+  parameters:
+    name:
+      type: str
+      default:
+      optional: false
+      description: ''
+      type_meta:
+        title: str
+        type: string
+        default:
         description: ''
-        is_multi: true
-    model: { }
+    namespace:
+      type: str
+      default:
+      optional: false
+      description: ''
+      type_meta:
+        title: str
+        type: string
+        default:
+        description: ''
+  input_artifacts:
+    data: {}
+    model: {}
   output_artifacts:
     data:
       output_data:
         types:
-          - dataframe
+          - data_unresolved
         optional: false
         stages:
           - default
         roles:
           - guest
           - host
+          - arbiter
         description: ''
         is_multi: false
-    model: { }
+    model: {}
     metric:
       metric:
         types:
           - json_metric
         optional: false
         stages:
           - default
         roles:
           - guest
           - host
+          - arbiter
         description: metric, invisible for user
         is_multi: false
 schema_version: v1
+
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/components/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/component_base.py` & `fate-client-2.1.0/fate_client/pipeline/components/component_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,43 +11,50 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import copy
 import uuid
 
+from types import SimpleNamespace
+from typing import List
+
 from ..conf.types import SupportRole, PlaceHolder, ArtifactSourceType, InputArtifactType, OutputArtifactType
 from ..conf.job_configuration import TaskConf
 from ..entity.component_structures import load_component_spec
 from ..interface import TaskOutputArtifactChannel, DataWarehouseChannel, ModelWarehouseChannel
-from ..entity.dag_structures import DataWarehouseChannelSpec, ModelWarehouseChannelSpec
+from ..entity.dag_structures import OutputArtifactSpec, PartySpec
+from ..entity.runtime_entity import Parties
 
 
 class Component(object):
     __instance = {}
 
     yaml_define_path = None
 
     def __init__(self, *args, **kwargs):
         self._name = None
-        self.runtime_roles = None
+        self.runtime_parties = Parties()
         self.__party_instance = {}
         self._module = None
         self._role = None
         self._index = None
         self._callable = True
         self._outputs = None
-        self._component_setting = dict()
+        self._task_parameters = dict()
         self._task_conf = TaskConf()
+        self._stage = None
 
         if self.yaml_define_path is None:
             raise ValueError("Component should have yaml define file, set yaml_define_path first please!")
 
         self._component_spec = load_component_spec(self.yaml_define_path)
-        self._init_component_setting()
+        self._provider = None
+        self._version = None
+        self._init_task_setting()
 
     def __new__(cls, *args, **kwargs):
         if cls.__name__.lower() not in cls.__instance:
             cls.__instance[cls.__name__.lower()] = 0
 
         new_cls = object.__new__(cls)
         new_cls.set_name(cls.__instance[cls.__name__.lower()])
@@ -106,14 +113,22 @@
         return inst
 
     @property
     def arbiter(self) -> "Component":
         inst = self.get_party_instance(role=SupportRole.ARBITER)[0]
         return inst
 
+    @property
+    def stage(self):
+        return self._stage
+
+    @stage.setter
+    def stage(self, stage):
+        self._stage = stage
+
     def get_party_instance(self, role="guest") -> 'Component':
         if role not in self.support_roles:
             raise ValueError("Role should be one of guest/host/arbiter")
 
         if role not in self.__party_instance:
             self.__party_instance[role] = dict()
 
@@ -152,99 +167,50 @@
 
     @property
     def conf(self):
         return self._task_conf
 
     @property
     def support_roles(self):
-        if not self.runtime_roles:
+        self._convert_party_dict_to_party_inst()
+        if not len(self.runtime_parties):
             return self._component_spec.roles
         else:
-            if not isinstance(self.runtime_roles, list):
-                self.runtime_roles = [self.runtime_roles]
-            return list(set(self._component_spec.roles) & set(self.runtime_roles))
+            return list(set(self._component_spec.roles) & set(self.runtime_parties.get_runtime_roles()))
 
-    def component_setting(self, **kwargs):
+    @property
+    def support_parties(self) -> Parties:
+        self._convert_party_dict_to_party_inst()
+        return self.runtime_parties
+
+    def task_parameters(self, **kwargs):
         for attr, val in kwargs.items():
-            self._component_setting[attr] = val
+            self._task_parameters[attr] = val
 
-    def get_component_setting(self):
-        return self._component_setting
+    def get_task_parameters(self):
+        return self._task_parameters
 
-    def get_role_setting(self, role, index):
-        component_setting = dict()
+    def get_role_parameters(self, role, index):
+        task_parameters = dict()
         if role not in self.__party_instance:
-            return component_setting
+            return task_parameters
 
         index = str(index)
 
         role_inst_dict = self.__party_instance[role]
 
         for _, inst in role_inst_dict.items():
             for party_index, party_inst in inst.party_instance.items():
                 party_index = party_index.split("|")
                 if index not in party_index:
                     continue
 
-                component_setting.update(party_inst.get_component_setting())
-
-        if not component_setting:
-            return component_setting
-
-        parameters = {}
-        input_channels = {}
-        input_artifacts = {}
-        for attr, value in component_setting.items():
-            if attr in self._component_spec.parameters:
-                parameters[attr] = value
-            else:
-                """
-                artifact
-                """
-                if not isinstance(value, (DataWarehouseChannel, ModelWarehouseChannel)) or \
-                        (isinstance(value, list) and
-                         not isinstance(value[0], (DataWarehouseChannelSpec, ModelWarehouseChannelSpec))):
-                    raise ValueError(f"attr={attr} should be data_warehouse or model_warehouse artifact")
-
-                if not isinstance(value, list):
-                    type_key = InputArtifactType.DATA if isinstance(value, DataWarehouseChannel) \
-                        else InputArtifactType.MODEL
-                else:
-                    type_key = InputArtifactType.DATA if isinstance(value[0], DataWarehouseChannel) \
-                        else InputArtifactType.MODEL
-
-                if type_key not in input_channels:
-                    input_channels[type_key] = dict()
-                    input_artifacts[type_key] = dict()
-
-                artifact_spec = getattr(self._component_spec.input_artifacts, type_key).get(attr, None)
-                if not artifact_spec:
-                    raise ValueError(f"attr={attr} does not exist in component spec")
-
-                if isinstance(value, list) and not artifact_spec.is_multi:
-                    raise ValueError(f"Artifact={attr}'s input is list, it should be a single input")
-                if not isinstance(value, list) and artifact_spec.is_multi:
-                    value = [value]
-
-                if isinstance(value, list):
-                    artifact_list = [v.get_spec(roles=[role]) for v in value]
-                    input_channels[type_key][attr] = {value[0].source: artifact_list}
-                else:
-                    input_channels[type_key][attr] = {value.source: value.get_spec(roles=[role])}
-
-                input_artifacts[type_key][attr] = artifact_spec
+                task_parameters.update(party_inst.get_task_parameters())
 
-        component_setting = dict()
-        if parameters:
-            component_setting["parameters"] = parameters
-        if input_channels:
-            component_setting["input_artifacts"] = input_artifacts
-            component_setting["input_channels"] = input_channels
-
-        return component_setting
+        return task_parameters
 
     def get_role_conf(self, role, index):
         conf = dict()
         if role not in self.__party_instance:
             return conf
 
         index = str(index)
@@ -256,26 +222,14 @@
                 if index not in party_index:
                     continue
 
                 conf.update(party_inst.conf.dict())
 
         return conf
 
-    def reset_source_inputs(self):
-        for _, role_instances in self.__party_instance.items():
-            for __, inst in role_instances.items():
-                for ___, party_inst in inst.party_instance.items():
-                    component_setting = party_inst.get_component_setting()
-                    input_artifacts = self._component_spec.input_artifacts
-
-                    for artifact_type in InputArtifactType.types():
-                        for artifact_key in getattr(input_artifacts, artifact_type):
-                            if artifact_key in component_setting:
-                                component_setting.pop(artifact_key)
-
     def validate_runtime_env(self, roles):
         runtime_roles = roles.get_runtime_roles()
         for role, role_inst in self.__party_instance.items():
             if role not in runtime_roles:
                 raise ValueError(f"role {role} does not set in pipeline")
             runtime_role_parties = roles.get_party_list_by_role(role)
 
@@ -289,37 +243,83 @@
                 raise ValueError(f"role {role}, index {mx_idx} out of bound")
 
     @property
     def component_spec(self):
         return self._component_spec
 
     @property
+    def provider(self):
+        return self._provider
+
+    @property
+    def version(self):
+        return self._version
+
+    def _get_output_by_parties(self, parties: Parties):
+        _outputs = dict()
+        for output_artifact_type in OutputArtifactType.types():
+            artifacts = getattr(self._component_spec.output_artifacts, output_artifact_type)
+            if not artifacts:
+                continue
+
+            for artifact_name, artifact in artifacts.items():
+                channel = TaskOutputArtifactChannel(
+                    name=artifact_name,
+                    channel_type=artifact.types[0],
+                    task_name=self._name,
+                    parties=parties.get_parties_spec()
+                )
+
+                _outputs[artifact_name] = channel
+
+        return _outputs
+
+    @property
     def outputs(self):
         if self._component_spec.output_artifacts is None:
             raise ValueError("Output Definitions is None")
 
         if self._outputs:
             return self._outputs
 
         self._outputs = dict()
+
+        self._convert_party_dict_to_party_inst()
+        self._outputs = self._get_output_by_parties(self.runtime_parties)
+
+        return self._outputs
+
+    def party_outputs(self, parties: dict):
+        if not parties:
+            raise ValueError("To get party_outputs, pleas pass parties setting")
+
+        party_inst = Parties()
+        for role, party_id in parties.items():
+            party_inst.set_party(role=role, party_id=party_id)
+
+        return self._get_output_by_parties(parties=party_inst)
+
+    def get_output_artifacts(self):
+        outputs = dict()
+
         for output_artifact_type in OutputArtifactType.types():
             artifacts = getattr(self._component_spec.output_artifacts, output_artifact_type)
             if not artifacts:
                 continue
 
+            if output_artifact_type not in outputs:
+                outputs[output_artifact_type] = dict()
+
             for artifact_name, artifact in artifacts.items():
-                channel = TaskOutputArtifactChannel(
-                    name=artifact_name,
-                    channel_type=artifact.types[0],
-                    task_name=self._name
+                outputs[output_artifact_type][artifact_name] = OutputArtifactSpec(
+                    output_artifact_key_alias=artifact_name,
+                    output_artifact_type_alias=output_artifact_type
                 )
 
-                self._outputs[artifact_name] = channel
-
-        return self._outputs
+        return outputs
 
     def _process_init_inputs(self, inputs):
         self._init_inputs = {}
         for key, value in inputs.items():
             if key == "self" or (key.startswith("_") and key != "_name"):
                 continue
 
@@ -349,57 +349,97 @@
                                          f"should be ArtifactChannel, {channel} find")
 
                     if channel.source == ArtifactSourceType.TASK_OUTPUT_ARTIFACT:
                         dependencies.add(channel.task_name)
 
         return list(dependencies)
 
-    def get_runtime_input_artifacts(self, runtime_roles):
+    def get_runtime_input_artifacts(self, dag_runtime_parties: Parties):
         input_artifacts_dict = dict()
         for input_artifact_type in InputArtifactType.types():
             input_artifacts_dict[input_artifact_type] = getattr(self._component_spec.input_artifacts,
                                                                 input_artifact_type)
 
         runtime_input_channels = dict()
         input_artifacts = dict()
 
+        def _channel_parties_to_party_inst(channel_parties):
+            channel_party_inst = Parties()
+            if isinstance(channel_parties, dict):
+                for role, party_id in channel_parties.items():
+                    channel_party_inst.set_party(role=role, party_id=party_id)
+            else:
+                for party_spec in channel_parties:
+                    channel_party_inst.set_party(role=party_spec.role, party_id=party_spec.party_id)
+
+            return channel_party_inst
+
+        self._convert_party_dict_to_party_inst()
         for input_artifact_type, artifacts in input_artifacts_dict.items():
             if not artifacts:
                 continue
 
             input_artifacts[input_artifact_type] = dict()
             runtime_input_channels[input_artifact_type] = dict()
             for artifact_key, artifact_spec in artifacts.items():
                 if not hasattr(self, artifact_key) or isinstance(getattr(self, artifact_key), PlaceHolder):
                     continue
 
                 channels = getattr(self, artifact_key)
 
-                roles = list(set(runtime_roles) & set(artifact_spec.roles)) \
-                    if set(runtime_roles) != set(artifact_spec.roles) else None
+                cpn_runtime_parties = self.runtime_parties if len(self.runtime_parties) else dag_runtime_parties
+                cpn_runtime_parties = cpn_runtime_parties.intersect(dag_runtime_parties)
+                cpn_runtime_parties = cpn_runtime_parties.get_party_inst_by_role(artifact_spec.roles)
 
-                if isinstance(channels, list) and not artifact_spec.is_multi:
-                    raise ValueError(f"Artifact={artifact_key}'s input is list, it should be a single input")
                 if not isinstance(channels, list) and artifact_spec.is_multi:
                     channels = [channels]
 
                 if isinstance(channels, list):
                     artifact_list = []
                     for channel in channels:
-                        artifact = channel.get_spec(roles=roles)
+                        if not channel.parties:
+                            artifact = channel.get_spec(parties=cpn_runtime_parties.get_parties_spec())
+                        else:
+                            artifact = channel.get_spec(
+                                parties=cpn_runtime_parties.intersect(
+                                    _channel_parties_to_party_inst(channel.parties)
+                                ).get_parties_spec()
+                            )
+
                         artifact_list.append(artifact)
 
                     runtime_input_channels[input_artifact_type][artifact_key] = {channels[0].source: artifact_list}
                     input_artifacts[input_artifact_type][artifact_key] = artifact_spec
                 else:
-                    artifact = channels.get_spec(roles=roles)
+                    if not channels.parties:
+                        artifact = channels.get_spec(parties=cpn_runtime_parties.get_parties_spec())
+                    else:
+                        artifact = channels.get_spec(
+                            parties=cpn_runtime_parties.intersect(
+                                _channel_parties_to_party_inst(channels.parties)
+                            ).get_parties_spec()
+                        )
+
                     runtime_input_channels[input_artifact_type][artifact_key] = {channels.source: artifact}
                     input_artifacts[input_artifact_type][artifact_key] = artifact_spec
 
         return runtime_input_channels, input_artifacts
 
-    def _init_component_setting(self):
+    def _init_task_setting(self):
         parameters = self._component_spec.parameters
         for param in parameters:
             if isinstance(self._init_inputs.get(param, PlaceHolder()), PlaceHolder):
                 continue
-            self._component_setting[param] = self._init_inputs[param]
+            self._task_parameters[param] = self._init_inputs[param]
+
+        self._provider = self._component_spec.provider
+        self._version = self._component_spec.version
+
+    def _convert_party_dict_to_party_inst(self):
+        if not self.runtime_parties:
+            self.runtime_parties = Parties()
+        elif isinstance(self.runtime_parties, dict):
+            runtime_parties = Parties()
+            for role, party_id in self.runtime_parties.items():
+                if role in self.component_spec.roles:
+                    runtime_parties.set_party(role=role, party_id=party_id)
+            self.runtime_parties = runtime_parties
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from .coordinated_linr import CoordinatedLinR
 from .coordinated_lr import CoordinatedLR
 from .data_split import DataSplit
-
 # from .multi_input import MultiInput
-from .dataframe_io_test import DataFrameIOTest
+# from .dataframe_io_test import DataFrameIOTest
 from .dataframe_transformer import DataFrameTransformer
 from .evaluation import Evaluation
+from .feature_correlation import FeatureCorrelation
 from .feature_scale import FeatureScale
 from .hetero_feature_binning import HeteroFeatureBinning
 from .hetero_feature_selection import HeteroFeatureSelection
 from .psi import PSI
 from .reader import Reader
 from .sample import Sample
+from .sshe_linr import SSHELinR
+from .sshe_lr import SSHELR
 from .statistics import Statistics
 from .union import Union
 from .homo_lr import HomoLR
-from .hetero_sbt import HeteroSBT as HeteroSecureBoost
+from .hetero_secureboost import HeteroSecureBoost
 from .homo_nn import HomoNN
+from .hetero_nn import HeteroNN
 from .evaluation import Evaluation
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/coordinated_linr.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/coordinated_linr.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class CoordinatedLinR(Component):
     yaml_define_path = "./component_define/fate/coordinated_linr.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
+        runtime_parties: dict = None,
         epochs: int = 20,
         early_stop: str = "diff",
         tol: float = 1e-4,
         batch_size: int = None,
         optimizer: dict = PlaceHolder(),
         learning_rate_scheduler: dict = PlaceHolder(),
         init_param: dict = PlaceHolder(),
@@ -44,15 +44,15 @@
         input_model: ArtifactType = PlaceHolder(),
         warm_start_model: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
         super(CoordinatedLinR, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
+        self.runtime_parties = runtime_parties
         self.epochs = epochs
         self.early_stop = early_stop
         self.tol = tol
         self.batch_size = batch_size
         self.optimizer = optimizer
         self.learning_rate_scheduler = learning_rate_scheduler
         self.init_param = init_param
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/coordinated_lr.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/coordinated_lr.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class CoordinatedLR(Component):
     yaml_define_path = "./component_define/fate/coordinated_lr.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
+        runtime_parties: dict = None,
         epochs: int = 20,
         early_stop: str = "diff",
         tol: float = 1e-4,
         batch_size: int = None,
         optimizer: dict = PlaceHolder(),
         learning_rate_scheduler: dict = PlaceHolder(),
         init_param: dict = PlaceHolder(),
@@ -45,15 +45,15 @@
         input_model: ArtifactType = PlaceHolder(),
         warm_start_model: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
         super(CoordinatedLR, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
+        self.runtime_parties = runtime_parties
         self.epochs = epochs
         self.early_stop = early_stop
         self.tol = tol
         self.batch_size = batch_size
         self.optimizer = optimizer
         self.learning_rate_scheduler = learning_rate_scheduler
         self.init_param = init_param
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/data_split.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/data_split.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 
 class DataSplit(Component):
     yaml_define_path = "./component_define/fate/data_split.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
+        runtime_parties: dict = None,
         input_data: ArtifactType = PlaceHolder(),
         train_size: Union[int, float] = None,
         validate_size: Union[int, float] = None,
         test_size: Union[int, float] = None,
         stratified: bool = False,
         random_state: int = None,
         hetero_sync: bool = True,
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
         super(DataSplit, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
+        self.runtime_parties = runtime_parties
         self.input_data = input_data
         self.train_size = train_size
         self.validate_size = validate_size
         self.test_size = test_size
         self.stratified = stratified
         self.random_state = random_state
         self.hetero_sync = hetero_sync
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/dataframe_io_test.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/psi.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import List, Union
 from ...conf.types import PlaceHolder
 from ..component_base import Component
 from ...interface import ArtifactType
 
 
-class DataFrameIOTest(Component):
-    yaml_define_path = "./component_define/fate/dataframe_io_test.yaml"
+class PSI(Component):
+    yaml_define_path = "./component_define/fate/psi.yaml"
 
     def __init__(
         self,
         _name: str,
-        dataframe_input: ArtifactType = PlaceHolder(),
-        dataframe_inputs: ArtifactType = PlaceHolder(),
+        runtime_parties: dict = None,
+        input_data: ArtifactType = PlaceHolder(),
+        protocol: str = PlaceHolder(),
+        curve_type: str = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
-        super(DataFrameIOTest, self).__init__()
+        super(PSI, self).__init__()
         self._name = _name
-        self.dataframe_input = dataframe_input
-        self.dataframe_inputs = dataframe_inputs
+        self.runtime_parties = runtime_parties
+        self.input_data = input_data
+        self.protocol = protocol
+        self.curve_type = curve_type
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/dataframe_transformer.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/evaluation.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import List, Union
+from typing import List, Literal
 from ...conf.types import PlaceHolder
 from ..component_base import Component
 from ...interface import ArtifactType
 
 
-class DataFrameTransformer(Component):
-    yaml_define_path = "./component_define/fate/dataframe_transformer.yaml"
+class Evaluation(Component):
+    yaml_define_path = "./component_define/fate/evaluation.yaml"
 
     def __init__(
         self,
         _name: str,
-        table: ArtifactType = PlaceHolder(),
-        name: str = PlaceHolder(),
-        namespace: str = PlaceHolder(),
-        anonymous_role: str = PlaceHolder(),
-        anonymous_party_id: str = PlaceHolder(),
+        runtime_parties: dict = None,
+        default_eval_setting: Literal["binary", "multi", "regression"] = PlaceHolder(),
+        metrics: List[str] = None,
+        predict_column_name: str = None,
+        label_column_name: str = None,
+        input_datas: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
-        super(DataFrameTransformer, self).__init__()
+        super(Evaluation, self).__init__()
         self._name = _name
-        self.table = table
-        self.name = name
-        self.namespace = namespace
-        self.anonymous_role = anonymous_role
-        self.anonymous_party_id = anonymous_party_id
+        self.runtime_parties = runtime_parties
+        self.input_datas = input_datas
+        self.default_eval_setting = default_eval_setting
+        self.metrics = metrics
+        self.predict_column_name = predict_column_name
+        self.label_column_name = label_column_name
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/evaluation.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/statistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #
-#  Copyright 2019 The FATE Authors. All Rights Reserved.
+#  Copyright 2023 The FATE Authors. All Rights Reserved.
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
-from typing import List, Literal
-from ...conf.types import PlaceHolder
+from typing import List, Union
+
 from ..component_base import Component
+from ...conf.types import PlaceHolder
 from ...interface import ArtifactType
 
 
-class Evaluation(Component):
-    yaml_define_path = "./component_define/fate/evaluation.yaml"
+class Statistics(Component):
+    yaml_define_path = "./component_define/fate/statistics.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
-        default_eval_setting: Literal["binary", "multi", "regression"] = PlaceHolder(),
-        metrics: List[str] = None,
-        predict_column_name: str = None,
-        label_column_name: str = None,
+        runtime_parties: dict = None,
+        metrics: Union[List[str], str] = None,
+        bias: bool = True,
+        skip_col: List[str] = PlaceHolder(),
+        use_anonymous: bool = False,
+        relative_error: float = 1e-3,
         input_data: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
-        super(Evaluation, self).__init__()
+        super(Statistics, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
-        self.input_data = input_data
-        self.default_eval_setting = default_eval_setting
+        self.runtime_parties = runtime_parties
         self.metrics = metrics
-        self.predict_column_name = predict_column_name
-        self.label_column_name = label_column_name
+        self.bias = bias
+        self.skip_col = skip_col
+        self.use_anonymous = use_anonymous
+        self.relative_error = relative_error
+        self.input_data = input_data
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/feature_scale.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/feature_scale.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 
 class FeatureScale(Component):
     yaml_define_path = "./component_define/fate/feature_scale.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
+        runtime_parties: dict = None,
         method: str = PlaceHolder(),
         feature_range: Union[list, dict] = None,
         scale_col: List[str] = None,
         scale_idx: List[int] = None,
         strict_range: bool = True,
         use_anonymous: bool = False,
         train_data: ArtifactType = PlaceHolder(),
         test_data: ArtifactType = PlaceHolder(),
         input_model: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
         super(FeatureScale, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
+        self.runtime_parties = runtime_parties
         self.method = method
         self.feature_range = feature_range
         self.scale_col = scale_col
         self.scale_idx = scale_idx
         self.strict_range = strict_range
         self.use_anonymous = use_anonymous
         self.train_data = train_data
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/hetero_feature_binning.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/hetero_feature_binning.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class HeteroFeatureBinning(Component):
     yaml_define_path = "./component_define/fate/hetero_feature_binning.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
+        runtime_parties: dict = None,
         method: str = PlaceHolder(),
         n_bins: int = None,
         split_pt_dict: dict = None,
         bin_col: List[str] = None,
         bin_idx: List[int] = None,
         category_col: List[str] = None,
         category_idx: List[int] = None,
@@ -45,15 +45,15 @@
         test_data: ArtifactType = PlaceHolder(),
         input_model: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
         super(HeteroFeatureBinning, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
+        self.runtime_parties = runtime_parties
         self.method = method
         self.n_bins = n_bins
         self.split_pt_dict = split_pt_dict
         self.bin_col = bin_col
         self.bin_idx = bin_idx
         self.category_col = category_col
         self.category_idx = category_idx
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/hetero_feature_selection.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/hetero_feature_selection.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class HeteroFeatureSelection(Component):
     yaml_define_path = "./component_define/fate/hetero_feature_selection.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
+        runtime_parties: dict = None,
         method: List[str] = PlaceHolder(),
         select_col: List[str] = None,
         iv_param: dict = None,
         statistic_param: dict = None,
         manual_param: dict = None,
         keep_one: bool = True,
         use_anonymous: bool = False,
@@ -39,15 +39,15 @@
         input_model: ArtifactType = PlaceHolder(),
         input_models: List[ArtifactType] = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
         super(HeteroFeatureSelection, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
+        self.runtime_parties = runtime_parties
         self.method = method
         self.select_col = select_col
         self.iv_param = iv_param
         self.statistic_param = statistic_param
         self.manual_param = manual_param
         self.keep_one = keep_one
         self.use_anonymous = use_anonymous
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/hetero_sbt.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/homo_lr.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,64 +15,50 @@
 from typing import List
 
 from ..component_base import Component
 from ...conf.types import PlaceHolder
 from ...interface import ArtifactType
 
 
-class HeteroSBT(Component):
-    yaml_define_path = "./component_define/fate/hetero_sbt.yaml"
+class HomoLR(Component):
+    yaml_define_path = "./component_define/fate/homo_lr.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
+        runtime_parties: dict = None,
+        epochs: int = 20,
+        early_stop: str = "diff",
+        tol: float = 1e-4,
+        batch_size: int = -1,
+        optimizer: dict = PlaceHolder(),
+        learning_rate_scheduler: dict = PlaceHolder(),
+        init_param: dict = PlaceHolder(),
+        threshold: float = 0.5,
+        ovr: bool = False,
+        label_num: int = None,
         train_data: ArtifactType = PlaceHolder(),
         validate_data: ArtifactType = PlaceHolder(),
-        num_trees: int = 20,
-        learning_rate: float = 0.3,
-        max_depth: int = 3,
-        max_bin: int = 32,
-        objective: str = "binary:bce",
-        num_class: int = 2,
-        l2: float = 0.1,
-        min_impurity_split: float = 1e-2,
-        min_sample_split: int = 2,
-        min_leaf_node: int = 1,
-        min_child_weight: float = 1,
-        gh_pack: bool = True,
-        split_info_pack: bool = True,
-        hist_sub: bool = True,
-        he_param: dict = PlaceHolder(),
-        train_data_output: ArtifactType = PlaceHolder(),
-        train_model_output: ArtifactType = PlaceHolder(),
-        train_model_input: ArtifactType = PlaceHolder(),
         test_data: ArtifactType = PlaceHolder(),
-        predict_model_input: ArtifactType = PlaceHolder(),
+        warm_start_model: ArtifactType = PlaceHolder(),
+        input_model: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
-        super(HeteroSBT, self).__init__()
+        super(HomoLR, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
+        self.runtime_parties = runtime_parties
+        self.epochs = epochs
+        self.early_stop = early_stop
+        self.tol = tol
+        self.batch_size = batch_size
+        self.optimizer = optimizer
+        self.learning_rate_scheduler = learning_rate_scheduler
+        self.init_param = init_param
+        self.threshold = threshold
         self.train_data = train_data
         self.validate_data = validate_data
-        self.train_model_input = train_model_input
-        self.num_trees = num_trees
-        self.learning_rate = learning_rate
-        self.max_depth = max_depth
-        self.max_bin = max_bin
-        self.objective = objective
-        self.num_class = num_class
-        self.l2 = l2
-        self.min_impurity_split = min_impurity_split
-        self.min_sample_split = min_sample_split
-        self.min_leaf_node = min_leaf_node
-        self.min_child_weight = min_child_weight
-        self.gh_pack = gh_pack
-        self.split_info_pack = split_info_pack
-        self.hist_sub = hist_sub
-        self.he_param = he_param
-        self.train_data_output = train_data_output
-        self.train_model_output = train_model_output
         self.test_data = test_data
-        self.predict_model_input = predict_model_input
+        self.warm_start_model = warm_start_model
+        self.input_model = input_model
+        self.ovr = ovr
+        self.label_num = label_num
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/homo_lr.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/sample.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,46 @@
 #
-#  Copyright 2019 The FATE Authors. All Rights Reserved.
+#  Copyright 2023 The FATE Authors. All Rights Reserved.
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
-from typing import List
+from typing import List, Union
 
 from ..component_base import Component
 from ...conf.types import PlaceHolder
 from ...interface import ArtifactType
 
 
-class HomoLR(Component):
-    yaml_define_path = "./component_define/fate/homo_lr.yaml"
+class Sample(Component):
+    yaml_define_path = "./component_define/fate/sample.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
-        epochs: int = 20,
-        early_stop: str = "diff",
-        tol: float = 1e-4,
-        batch_size: int = -1,
-        optimizer: dict = PlaceHolder(),
-        learning_rate_scheduler: dict = PlaceHolder(),
-        init_param: dict = PlaceHolder(),
-        threshold: float = 0.5,
-        ovr: bool = False,
-        label_num: int = None,
-        train_data: ArtifactType = PlaceHolder(),
-        validate_data: ArtifactType = PlaceHolder(),
-        test_data: ArtifactType = PlaceHolder(),
-        train_input_model: ArtifactType = PlaceHolder(),
-        predict_input_model: ArtifactType = PlaceHolder(),
+        runtime_parties: dict = None,
+        replace: bool = False,
+        frac: Union[float, dict] = None,
+        n: int = None,
+        random_state: int = None,
+        hetero_sync: bool = True,
+        input_data: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
-        super(HomoLR, self).__init__()
+        super(Sample, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
-        self.epochs = epochs
-        self.early_stop = early_stop
-        self.tol = tol
-        self.batch_size = batch_size
-        self.optimizer = optimizer
-        self.learning_rate_scheduler = learning_rate_scheduler
-        self.init_param = init_param
-        self.threshold = threshold
-        self.train_data = train_data
-        self.validate_data = validate_data
-        self.test_data = test_data
-        self.train_input_model = train_input_model
-        self.predict_input_model = predict_input_model
-        self.ovr = ovr
-        self.label_num = label_num
+        self.runtime_parties = runtime_parties
+        self.replace = replace
+        self.frac = frac
+        self.n = n
+        self.random_state = random_state
+        self.hetero_sync = hetero_sync
+        self.input_data = input_data
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/homo_nn.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/homo_nn.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from typing import List
-from fate_client.pipeline.conf.types import PlaceHolder
 from fate_client.pipeline.components.fate.nn.loader import (
     Loader,
     ModelLoader,
     CustFuncLoader,
     DatasetLoader,
 )
 from fate_client.pipeline.components.fate.nn.torch.base import (
@@ -26,14 +25,16 @@
     Sequential,
 )
 from typing import Union
 from fate_client.pipeline.components.fate.nn.algo_params import (
     TrainingArguments,
     FedArguments,
 )
+from fate_client.pipeline.components.fate.nn.common_utils import (get_config_of_default_runner
+                                                                  as _get_config_of_default_runner)
 from typing import Literal
 from ...conf.types import PlaceHolder
 from ..component_base import Component
 from ...interface import ArtifactType
 
 
 def get_config_of_default_runner(
@@ -42,105 +43,122 @@
     optimizer: Union[TorchOptimizer, Loader] = None,
     loss: Union[TorchModule, CustFuncLoader] = None,
     training_args: TrainingArguments = None,
     fed_args: FedArguments = None,
     dataset: DatasetLoader = None,
     data_collator: CustFuncLoader = None,
     tokenizer: CustFuncLoader = None,
-    task_type: Literal["binary", "multi", "regression", "others"] = "binary",
+    task_type: Literal["binary", "multi", "regression", "causal_lm", "others"] = "binary",
 ):
+
     if model is not None and not isinstance(
         model, (TorchModule, Sequential, ModelLoader)
     ):
         raise ValueError(
             f"The model is of type {type(model)}, not TorchModule, Sequential, or ModelLoader. Remember to use patched_torch_hook for passing NN Modules or Optimizers."
         )
 
-    if optimizer is not None and not isinstance(optimizer, (TorchOptimizer, Loader)):
-        raise ValueError(
-            f"The optimizer is of type {type(optimizer)}, not TorchOptimizer or Loader. Remember to use patched_torch_hook for passing NN Modules or Optimizers."
-        )
-
-    if loss is not None and not isinstance(loss, (TorchModule, CustFuncLoader)):
-        raise ValueError(
-            f"The loss function is of type {type(loss)}, not TorchModule or CustFuncLoader."
-        )
-
-    if training_args is not None and not isinstance(training_args, TrainingArguments):
-        raise ValueError(
-            f"Training arguments are of type {type(training_args)}, not TrainingArguments."
-        )
-
     if fed_args is not None and not isinstance(fed_args, FedArguments):
         raise ValueError(
             f"Federation arguments are of type {type(fed_args)}, not FedArguments."
         )
 
-    if dataset is not None and not isinstance(dataset, DatasetLoader):
-        raise ValueError(f"The dataset is of type {type(dataset)}, not DatasetLoader.")
+    runner_conf = _get_config_of_default_runner(
+        optimizer, loss, training_args, dataset, data_collator, tokenizer, task_type
+    )
+    runner_conf['algo'] = algo
+    runner_conf['model_conf'] = model.to_dict() if model is not None else None
+    runner_conf['fed_args_conf'] = fed_args.to_dict() if fed_args is not None else None
 
-    if data_collator is not None and not isinstance(data_collator, CustFuncLoader):
-        raise ValueError(
-            f"The data collator is of type {type(data_collator)}, not CustFuncLoader."
-        )
+    return runner_conf
 
-    if tokenizer is not None and not isinstance(tokenizer, CustFuncLoader):
-        raise ValueError(
-            f"The tokenizer is of type {type(tokenizer)}, not CustFuncLoader."
-        )
 
-    if task_type not in ["binary", "multi", "regression", "others"]:
-        raise ValueError(
-            f"The task type is {task_type}, not 'binary', 'multi', 'regression', 'others'."
-        )
+def get_config_of_seq2seq_runner(
+    algo: str = "fedavg",
+    model: Union[TorchModule, Sequential, ModelLoader] = None,
+    optimizer: Union[TorchOptimizer, Loader] = None,
+    training_args: TrainingArguments = None,
+    fed_args: FedArguments = None,
+    dataset: DatasetLoader = None,
+    data_collator: CustFuncLoader = None,
+    tokenizer: CustFuncLoader = None,
+    task_type: Literal["causal_lm", "others"] = "causal_lm",
+    save_trainable_weights_only: bool = False,
+):
+    runner_conf = get_config_of_default_runner(
+        algo=algo,
+        model=model,
+        optimizer=optimizer,
+        training_args=training_args,
+        fed_args=fed_args,
+        dataset=dataset,
+        data_collator=data_collator,
+        tokenizer=tokenizer,
+        task_type=task_type
+    )
+    runner_conf.pop("loss_conf")
+    runner_conf["save_trainable_weights_only"] = save_trainable_weights_only
+
+    return runner_conf
 
-    runner_conf = {
-        "algo": algo,
-        "model_conf": model.to_dict() if model is not None else None,
-        "optimizer_conf": optimizer.to_dict() if optimizer is not None else None,
-        "loss_conf": loss.to_dict() if loss is not None else None,
-        "training_args_conf": training_args.to_dict()
-        if training_args is not None
-        else None,
-        "fed_args_conf": fed_args.to_dict() if fed_args is not None else None,
-        "dataset_conf": dataset.to_dict() if dataset is not None else None,
-        "data_collator_conf": data_collator.to_dict()
-        if data_collator is not None
-        else None,
-        "tokenizer_conf": tokenizer.to_dict() if tokenizer is not None else None,
-        "task_type": task_type,
-    }
+
+def get_conf_of_ot_runner(
+    model: Union[TorchModule, Sequential, ModelLoader] = None,
+    optimizer: Union[TorchOptimizer, Loader] = None,
+    training_args: TrainingArguments = None,
+    fed_args: FedArguments = None,
+    dataset: DatasetLoader = None,
+    data_collator: CustFuncLoader = None,
+    tokenizer: CustFuncLoader = None,
+    task_type: Literal["causal_lm", "others"] = "causal_lm",
+    save_trainable_weights_only: bool = False,  
+    aggregate_model: bool = False
+):
+    runner_conf = get_config_of_default_runner(
+        algo='ot',  # offsite-tuning
+        model=model,
+        optimizer=optimizer,
+        training_args=training_args,
+        fed_args=fed_args,
+        dataset=dataset,
+        data_collator=data_collator,
+        tokenizer=tokenizer,
+        task_type=task_type
+    )
+    runner_conf.pop("loss_conf")
+    runner_conf["save_trainable_weights_only"] = save_trainable_weights_only
+    runner_conf["aggregate_model"] = aggregate_model
 
     return runner_conf
 
 
 class HomoNN(Component):
     yaml_define_path = "./component_define/fate/homo_nn.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
+        runtime_parties: dict = None,
         runner_module: str = PlaceHolder(),
         runner_class: str = PlaceHolder(),
         runner_conf: dict = PlaceHolder(),
         source: str = PlaceHolder(),
         train_data: ArtifactType = PlaceHolder(),
         validate_data: ArtifactType = PlaceHolder(),
         test_data: ArtifactType = PlaceHolder(),
-        train_model_input: ArtifactType = PlaceHolder(),
-        predict_model_input: ArtifactType = PlaceHolder(),
+        warm_start_model: ArtifactType = PlaceHolder(),
+        input_model: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
         super(HomoNN, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
+        self.runtime_parties = runtime_parties
         self.runner_module = runner_module
         self.runner_class = runner_class
         self.runner_conf = runner_conf
         self.source = source
         self.train_data = train_data
         self.validate_data = validate_data
         self.test_data = test_data
-        self.train_model_input = train_model_input
-        self.predict_model_input = predict_model_input
+        self.warm_start_model = warm_start_model
+        self.input_model = input_model
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/torch/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/nn/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/torch/base.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/nn/torch/base.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/torch/nn.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/nn/torch/nn.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/nn/torch/optim.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/nn/torch/optim.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/psi.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/union.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,31 +9,28 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from typing import List
-from ...conf.types import PlaceHolder
+
 from ..component_base import Component
+from ...conf.types import PlaceHolder
 from ...interface import ArtifactType
 
 
-class PSI(Component):
-    yaml_define_path = "./component_define/fate/psi.yaml"
+class Union(Component):
+    yaml_define_path = "./component_define/fate/union.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
-        input_data: ArtifactType = PlaceHolder(),
-        protocol: str = PlaceHolder(),
-        curve_type: str = PlaceHolder(),
+        runtime_parties: dict = None,
+            input_datas: List[ArtifactType] = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
-        super(PSI, self).__init__()
+        super(Union, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
-        self.input_data = input_data
-        self.protocol = protocol
-        self.curve_type = curve_type
+        self.runtime_parties = runtime_parties
+        self.input_datas = input_datas
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/reader.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/dataframe_transformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,41 +8,33 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import List
 from ...conf.types import PlaceHolder
 from ..component_base import Component
+from ...interface import ArtifactType
 
 
-class Reader(Component):
-    yaml_define_path = "./component_define/fate/reader.yaml"
+class DataFrameTransformer(Component):
+    yaml_define_path = "./component_define/fate/dataframe_transformer.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
-        path: str = PlaceHolder(),
-        format: str = PlaceHolder(),
-        sample_id_name: str = PlaceHolder(),
-        match_id_name: str = PlaceHolder(),
-        delimiter: str = PlaceHolder(),
-        label_name: str = PlaceHolder(),
-        label_type: str = PlaceHolder(),
-        dtype: str = PlaceHolder(),
+        runtime_parties: dict = None,
+        table: ArtifactType = PlaceHolder(),
+        name: str = PlaceHolder(),
+        namespace: str = PlaceHolder(),
+        site_name: str = PlaceHolder()
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
-        super(Reader, self).__init__()
+        super(DataFrameTransformer, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
-        self.path = path
-        self.format = format
-        self.sample_id_name = sample_id_name
-        self.match_id_name = match_id_name
-        self.delimiter = delimiter
-        self.label_name = label_name
-        self.label_type = label_type
-        self.dtype = dtype
+        self.runtime_parties = runtime_parties
+        self.table = table
+        self.name = name
+        self.namespace = namespace
+        self.site_name = site_name
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/sample.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,37 @@
 #
-#  Copyright 2023 The FATE Authors. All Rights Reserved.
+#  Copyright 2019 The FATE Authors. All Rights Reserved.
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
-from typing import List, Union
+from typing import List
 
 from ..component_base import Component
 from ...conf.types import PlaceHolder
-from ...interface import ArtifactType
 
 
-class Sample(Component):
-    yaml_define_path = "./component_define/fate/sample.yaml"
+class Reader(Component):
+    yaml_define_path = "./component_define/fate/reader.yaml"
 
     def __init__(
         self,
         _name: str,
-        runtime_roles: List[str] = None,
-        replace: bool = False,
-        frac: Union[float, dict] = None,
-        n: int = None,
-        random_state: int = None,
-        hetero_sync: bool = True,
-        input_data: ArtifactType = PlaceHolder(),
+        runtime_parties: dict = None,
+        namespace: str = PlaceHolder(),
+        name: str = PlaceHolder()
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
-        super(Sample, self).__init__()
+        super(Reader, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
-        self.replace = replace
-        self.frac = frac
-        self.n = n
-        self.random_state = random_state
-        self.hetero_sync = hetero_sync
-        self.input_data = input_data
+        self.runtime_parties = runtime_parties
+        self.name = name
+        self.namespace = namespace
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/statistics.py` & `fate-client-2.1.0/fate_client/pipeline/components/fate/feature_correlation.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,39 +8,37 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import List, Union
+from typing import List
 
 from ..component_base import Component
 from ...conf.types import PlaceHolder
 from ...interface import ArtifactType
 
 
-class Statistics(Component):
-    yaml_define_path = "./component_define/fate/statistics.yaml"
+class FeatureCorrelation(Component):
+    yaml_define_path = "./component_define/fate/feature_correlation.yaml"
 
     def __init__(
-        self,
-        _name: str,
-        runtime_roles: List[str] = None,
-        metrics: Union[List[str], str] = None,
-        bias: bool = True,
-        skip_col: List[str] = PlaceHolder(),
-        use_anonymous: bool = False,
-        relative_error: float = 1e-3,
-        input_data: ArtifactType = PlaceHolder(),
+            self,
+            _name: str,
+            runtime_parties: dict = None,
+            calc_local_vif: bool = True,
+            local_only: bool = False,
+            skip_col: List[str] = PlaceHolder(),
+            use_anonymous: bool = False,
+            input_data: ArtifactType = PlaceHolder(),
     ):
         inputs = locals()
         self._process_init_inputs(inputs)
-        super(Statistics, self).__init__()
+        super(FeatureCorrelation, self).__init__()
         self._name = _name
-        self.runtime_roles = runtime_roles
-        self.metrics = metrics
-        self.bias = bias
+        self.runtime_parties = runtime_parties
+        self.local_only = local_only
+        self.calc_local_vif = calc_local_vif
         self.skip_col = skip_col
         self.use_anonymous = use_anonymous
-        self.relative_error = relative_error
         self.input_data = input_data
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/components/fate/union.py` & `fate-client-2.1.0/fate_client/pipeline/adapters/bfia/translator/component_spec.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import List
+from pydantic import BaseModel
+from typing import Optional, Dict, List, Literal
 
-from ..component_base import Component
-from ...conf.types import PlaceHolder
-from ...interface import ArtifactType
 
+class DataSpec(BaseModel):
+    name: str
+    description: str
+    category: str
+    dataFormat: List[str]
 
-class Union(Component):
-    yaml_define_path = "./component_define/fate/union.yaml"
 
-    def __init__(
-        self,
-        _name: str,
-        runtime_roles: List[str] = None,
-        input_data_list: List[ArtifactType] = PlaceHolder(),
-    ):
-        inputs = locals()
-        self._process_init_inputs(inputs)
-        super(Union, self).__init__()
-        self._name = _name
-        self.runtime_roles = runtime_roles
-        self.input_data_list = input_data_list
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

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/conf/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/conf/env_config.py` & `fate-client-2.1.0/fate_client/pipeline/conf/env_config.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/conf/job_configuration.py` & `fate-client-2.1.0/fate_client/pipeline/conf/job_configuration.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/conf/types.py` & `fate-client-2.1.0/fate_client/pipeline/conf/types.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/entity/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/entity/component_structures.py` & `fate-client-2.1.0/fate_client/pipeline/entity/component_structures.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/entity/dag_structures.py` & `fate-client-2.1.0/fate_client/pipeline/entity/dag_structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,95 +20,97 @@
     role: Union[Literal["guest", "host", "arbiter", "local"]]
     party_id: List[str]
 
 
 class RuntimeTaskOutputChannelSpec(BaseModel):
     producer_task: str
     output_artifact_key: str
-    roles: Optional[List[Literal["guest", "host", "arbiter", "local"]]]
+    output_artifact_type_alias: Optional[str]
+    parties: Optional[List[PartySpec]]
 
     class Config:
         extra = "forbid"
 
 
-# newly add: data source
 class DataWarehouseChannelSpec(BaseModel):
-    job_id: Optional[str]
-    producer_task: Optional[str]
-    output_artifact_key: Optional[str]
-    roles: Optional[List[Literal["guest", "host", "arbiter", "local"]]]
     namespace: Optional[str]
     name: Optional[str]
+    dataset_id: Optional[str]
+    parties: Optional[List[PartySpec]]
 
     class Config:
         extra = "forbid"
 
 
 class ModelWarehouseChannelSpec(BaseModel):
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
 class RuntimeInputArtifacts(BaseModel):
-    data: Optional[Dict[str, Dict[str, Union[InputArtifactSpec, List[InputArtifactSpec]]]]]
-    model: Optional[Dict[str, Dict[str, Union[InputArtifactSpec, List[InputArtifactSpec]]]]]
-
-
-class SourceInputArtifacts(BaseModel):
-    data: Optional[Dict[str, Dict[str, Union[SourceInputArtifactSpec, List[SourceInputArtifactSpec]]]]]
-    model: Optional[Dict[str, Dict[str, Union[SourceInputArtifactSpec, List[SourceInputArtifactSpec]]]]]
+    data: Optional[Dict[str, Dict[str, Union[List[InputArtifactSpec], InputArtifactSpec]]]]
+    model: Optional[Dict[str, Dict[str, Union[List[InputArtifactSpec], InputArtifactSpec]]]]
 
 
 class ModelWarehouseConfSpec(BaseModel):
     model_id: Optional[str]
     model_version: Optional[str]
 
 
+class OutputArtifactSpec(BaseModel):
+    output_artifact_key_alias: str
+    output_artifact_type_alias: str
+    parties: Optional[List[PartySpec]]
+
+
+class OutputArtifacts(BaseModel):
+    data: Optional[Dict[str, Union[OutputArtifactSpec, List[OutputArtifactSpec]]]]
+    model: Optional[Dict[str, Union[OutputArtifactSpec, List[OutputArtifactSpec]]]]
+    metric: Optional[Dict[str, Union[OutputArtifactSpec, List[OutputArtifactSpec]]]]
+
+
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
     conf: Optional[Dict] = {}
 
 
 class PartyTaskSpec(BaseModel):
     parties: Optional[List[PartySpec]]
     tasks: Optional[Dict[str, PartyTaskRefSpec]]
     conf: Optional[dict] = {}
 
 
 class TaskConfSpec(BaseModel):
-    run: Optional[Dict]
+    engine_run: Optional[Dict]
     provider: Optional[str]
+    timeout: Optional[int]
+    launcher_name: Optional[str] = "default"
 
 
 class EngineRunSpec(BaseModel):
     name: str
     conf: Optional[Dict]
 
 
@@ -129,19 +131,22 @@
     auto_retries: Optional[int]
     model_warehouse: Optional[ModelWarehouseConfSpec]
     model_id: Optional[str]
     model_version: Optional[str]
     task: Optional[TaskConfSpec]
     engine: Optional[EngineRunSpec]
 
+    extra: Optional[Dict[Any, Any]]
+
 
 class DAGSpec(BaseModel):
     parties: List[PartySpec]
     conf: Optional[JobConfSpec]
     stage: Optional[Union[Literal["train", "predict", "default", "cross_validation"]]]
     tasks: Dict[str, TaskSpec]
     party_tasks: Optional[Dict[str, PartyTaskSpec]]
 
 
 class DAGSchema(BaseModel):
     dag: DAGSpec
     schema_version: str
+    kind: str = "fate"
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/entity/model_info.py` & `fate-client-2.1.0/fate_client/pipeline/entity/model_info.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/entity/model_structure.py` & `fate-client-2.1.0/fate_client/pipeline/entity/model_structure.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/entity/task_info.py` & `fate-client-2.1.0/fate_client/pipeline/entity/task_info.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/entity/task_structure.py` & `fate-client-2.1.0/fate_client/pipeline/entity/task_structure.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/executor/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/executor/task_executor.py` & `fate-client-2.1.0/fate_client/pipeline/executor/task_executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,48 +13,81 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from pathlib import Path
 from typing import Dict
 from ..entity.dag_structures import DAGSchema
 from ..entity.component_structures import ComponentSpec
 from ..utils.fateflow.fate_flow_job_invoker import FATEFlowJobInvoker
+from ..utils.callbacks import CallbackHandler
 from ..entity.model_info import FateFlowModelInfo
 
 
 class FateFlowExecutor(object):
     def __init__(self):
         ...
 
     def fit(self, dag_schema: DAGSchema, component_specs: Dict[str, ComponentSpec],
-            local_role: str, local_party_id: str) -> FateFlowModelInfo:
+            local_role: str, local_party_id: str, callback_handler: CallbackHandler) -> FateFlowModelInfo:
         flow_job_invoker = FATEFlowJobInvoker()
         local_party_id = self.get_site_party_id(flow_job_invoker, dag_schema, local_role, local_party_id)
 
-        return self._run(dag_schema, local_role, local_party_id, flow_job_invoker)
+        return self._run(
+            dag_schema,
+            local_role,
+            local_party_id,
+            flow_job_invoker,
+            callback_handler,
+            event="fit"
+        )
 
     def predict(self,
                 dag_schema: DAGSchema,
                 component_specs: Dict[str, ComponentSpec],
-                fit_model_info: FateFlowModelInfo) -> FateFlowModelInfo:
+                fit_model_info: FateFlowModelInfo, callback_handler: CallbackHandler) -> FateFlowModelInfo:
         flow_job_invoker = FATEFlowJobInvoker()
         schedule_role = fit_model_info.local_role
         schedule_party_id = fit_model_info.local_party_id
 
-        return self._run(dag_schema, schedule_role, schedule_party_id, flow_job_invoker)
+        return self._run(
+            dag_schema,
+            schedule_role,
+            schedule_party_id,
+            flow_job_invoker,
+            callback_handler,
+            event="predict"
+        )
 
     def _run(self,
              dag_schema: DAGSchema,
              local_role,
              local_party_id,
-             flow_job_invoker: FATEFlowJobInvoker) -> FateFlowModelInfo:
+             flow_job_invoker: FATEFlowJobInvoker,
+             callback_handler: CallbackHandler,
+             event="fit") -> FateFlowModelInfo:
 
         job_id, model_id, model_version = flow_job_invoker.submit_job(dag_schema.dict(exclude_defaults=True))
 
+        getattr(callback_handler, f"on_{event}_begin")(
+            job_info=dict(
+                job_id=job_id,
+                model_id=model_id,
+                model_version=model_version
+            )
+        )
+
         flow_job_invoker.monitor_status(job_id, local_role, local_party_id)
 
+        getattr(callback_handler, f"on_{event}_end")(
+            job_info=dict(
+                job_id=job_id,
+                model_id=model_id,
+                model_version=model_version
+            )
+        )
+
         return FateFlowModelInfo(
             job_id=job_id,
             local_role=local_role,
             local_party_id=local_party_id,
             model_id=model_id,
             model_version=model_version
         )
@@ -78,37 +111,31 @@
 
     @staticmethod
     def upload(file: str,
                head: bool,
                meta: dict,
                role,
                party_id,
+               namespace,
+               name,
                extend_sid=True,
                partitions=4,
                **kwargs):
         flow_job_invoker = FATEFlowJobInvoker()
 
-        return flow_job_invoker.upload_data(file=file,
-                                            head=head,
-                                            meta=meta,
-                                            extend_sid=extend_sid,
-                                            partitions=partitions,
-                                            role=role,
-                                            party_id=party_id,
-                                            **kwargs)
+        return flow_job_invoker.upload_file_and_convert_to_dataframe(
+            file=file,
+            head=head,
+            meta=meta,
+            extend_sid=extend_sid,
+            partitions=partitions,
+            role=role,
+            party_id=party_id,
+            namespace=namespace,
+            name=name,
+            **kwargs)
 
     @staticmethod
-    def transform_to_dataframe(namespace: str,
-                               name: str,
-                               data_warehouse: dict,
-                               site_name: str,
-                               role: str,
-                               party_id: str):
+    def bind_local_path(path: str, namespace: str, name: str):
         flow_job_invoker = FATEFlowJobInvoker()
+        return flow_job_invoker.bind_local_path(path=path, namespace=namespace, name=name)
 
-        flow_job_invoker.transform_to_dataframe(namespace=namespace,
-                                                name=name,
-                                                data_warehouse=data_warehouse,
-                                                site_name=site_name,
-                                                role=role,
-                                                party_id=party_id
-                                                )
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/interface/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/pipeline_cli.py` & `fate-client-2.1.0/fate_client/pipeline/pipeline_cli.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/scheduler/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/scheduler/component_stage.py` & `fate-client-2.1.0/fate_client/pipeline/scheduler/component_stage.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/scheduler/dag_parser.py` & `fate-client-2.1.0/fate_client/pipeline/scheduler/dag_parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,249 +19,334 @@
 from typing import Dict, List, Union
 
 from ..conf.types import (
     Stage,
     InputDataKeyType,
     ArtifactSourceType,
     InputArtifactType,
+    OutputArtifactType,
 )
 
 from ..entity.dag_structures import (
     DAGSchema,
     DAGSpec,
     RuntimeTaskOutputChannelSpec,
     ModelWarehouseChannelSpec,
     DataWarehouseChannelSpec,
+    PartySpec
 )
 from ..entity.component_structures import ArtifactSpec, ComponentSpec, InputArtifactsSpec, OutputArtifactsSpec
 
 
 class DagParser(object):
     def __init__(self):
-        self._dag = nx.DiGraph()
+        self._dag = dict()
+        self._global_dag = nx.DiGraph()
         self._links = dict()
-        self._task_parameters = dict()
-        self._task_parties = dict()
         self._tasks = dict()
+        self._task_runtime_parties = dict()
         self._conf = dict()
 
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
-
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
-                                model_warehouse_channel = ModelWarehouseChannelSpec(**channel.dict(exclude_defaults=True))
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
 
-    def _add_edge(self, src, dst, attrs=None):
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
+                continue
+
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
+
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
+                        for party_id in party.party_id:
+                            self._tasks[party.role][party_id][task_name].runtime_parameters.update(parameters)
 
-        self._tasks[task_name].runtime_parameters = task_parameters
-        self._tasks[task_name].runtime_parties = task_runtime_parties
-        self._tasks[task_name].conf = task_conf
+    def get_runtime_roles_on_party(self, task_name, party_id):
+        task_runtime_parties = self._task_runtime_parties[task_name]
 
-    def get_runtime_parties(self, task_name):
-        return self._task_parties[task_name]
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
 
-    def get_task_node(self, task_name):
-        return self._tasks[task_name]
+        return self._tasks[role][party_id][task_name]
 
-    def get_need_revisit_tasks(self, visited_tasks, failed_tasks):
+    def get_need_revisit_tasks(self, visited_tasks, failed_tasks, role, party_id):
         """
         visited_tasks: already visited tasks
         failed_tasks: failed tasks
 
         this function finds tasks need to rerun, a task need to rerun if is upstreams is failed
         """
-        invalid_tasks = set(self.topological_sort()) - set(visited_tasks)
+        invalid_tasks = set(self.party_topological_sort(role, party_id)) - set(visited_tasks)
         invalid_tasks |= set(failed_tasks)
 
         revisit_tasks = []
         for task_to_check in visited_tasks:
             if task_to_check in invalid_tasks:
                 revisit_tasks.append(task_to_check)
                 continue
 
             task_valid = True
             task_stack = {task_to_check}
             stack = [task_to_check]
 
             while len(stack) > 0 and task_valid:
                 task = stack.pop()
-                pre_tasks = self.predecessors(task)
+                pre_tasks = self.party_predecessors(role, party_id, task)
 
                 for pre_task in pre_tasks:
                     if pre_task in task_stack:
                         continue
                     if pre_task in invalid_tasks:
                         task_valid = False
                         break
@@ -270,112 +355,131 @@
                     stack.append(pre_task)
 
             if not task_valid:
                 revisit_tasks.append(task_to_check)
 
         return revisit_tasks
 
-    def topological_sort(self):
-        return nx.topological_sort(self._dag)
+    def global_topological_sort(self):
+        return nx.topological_sort(self._global_dag)
+
+    def get_component_ref(self, task_name):
+        return self._global_dag.nodes[task_name]["component_ref"]
+
+    def party_topological_sort(self, role, party_id):
+        assert role in self._dag or party_id in self._dag[role], f"role={role}, party_id={party_id} does not exist"
+        return nx.topological_sort(self._dag[role][party_id])
 
-    def predecessors(self, task):
-        return set(self._dag.predecessors(task))
+    def party_predecessors(self, role, party_id, task):
+        return set(self._dag[role][party_id].predecessors(task))
 
-    def successors(self, task):
-        return self._dag.successors(task)
+    def party_successors(self, role, party_id, task):
+        return self._dag[role][party_id].successors(task)
 
-    def get_edge_attr(self, src, dst):
-        return self._dag.edges[src, dst]
+    def get_edge_attr(self, role, party_id, src, dst):
+        return self._dag[role][party_id].edges[src, dst]
 
     @staticmethod
-    def check_and_add_runtime_roles(upstream_inputs, runtime_roles):
-        correct_inputs = copy.deepcopy(upstream_inputs)
-        for input_type in InputArtifactType.types():
-            if input_type not in upstream_inputs:
+    def check_and_add_runtime_party(artifacts, role, party_id, artifact_type):
+        correct_artifacts = copy.deepcopy(artifacts)
+        if artifact_type == "input":
+            types = InputArtifactType.types()
+        else:
+            types = OutputArtifactType.types()
+
+        for t in types:
+            if t not in artifacts:
                 continue
-            for input_key, channel_list in upstream_inputs[input_type].items():
+            for _key, channel_list in artifacts[t].items():
                 if isinstance(channel_list, list):
                     for idx, channel in enumerate(channel_list):
-                        if channel.roles is None:
-                            correct_inputs[input_type][input_key][idx].roles = runtime_roles
+                        correct_artifacts[t][_key][idx].parties = [PartySpec(role=role, party_id=[party_id])]
                 else:
-                    if channel_list.roles is None:
-                        correct_inputs[input_type][input_key].roles = runtime_roles
+                    correct_artifacts[t][_key].parties = [PartySpec(role=role, party_id=[party_id])]
 
-        return correct_inputs
+        return correct_artifacts
 
     @property
     def conf(self):
         return self._conf
 
+    @property
+    def task_runtime_parties(self):
+        return self._task_runtime_parties
+
+    def get_task_runtime_parties(self, task_name):
+        return self._task_runtime_parties[task_name]
+
     @classmethod
     def deploy(cls, task_name_list: list, dag_schema: DAGSchema, component_specs: Dict[str, ComponentSpec]):
         dag_parser = DagParser()
         dag_parser.parse_dag(dag_schema, component_specs)
 
         data_tracer = dict()
         task_name_set = set(task_name_list)
-        for task_name in dag_parser.topological_sort():
-            trace_task_name = cls.trace_back_deploy_task(
-                task_name,
-                task_name_set,
-                dag_schema.dag,
-                component_specs,
-                data_tracer
-            )
-            data_tracer[task_name] = trace_task_name
+        for task_name in dag_parser.global_topological_sort():
+            parties = dag_parser.get_task_runtime_parties(task_name)
+            task_tracer = dict()
+            for party_spec in parties:
+                if party_spec.role not in task_tracer:
+                    task_tracer[party_spec.role] = dict()
+                for party_id in party_spec.party_id:
+                    task_tracer[party_spec.role][party_id] = cls.trace_back_deploy_task(
+                        task_name,
+                        task_name_set,
+                        dag_schema.dag,
+                        component_specs,
+                        data_tracer,
+                        dag_parser.task_runtime_parties,
+                        party_spec.role,
+                        party_id
+                    )
+            data_tracer[task_name] = task_tracer
 
-        dag_spec = cls.deduce_dag(dag_parser, task_name_list, dag_schema.dag, component_specs, data_tracer)
+        dag_spec = cls.deduce_dag(dag_parser, task_name_list, dag_schema.dag,
+                                  component_specs, data_tracer, dag_parser.task_runtime_parties)
         dag_spec = cls.erase_redundant_tasks(
             task_name_set,
             dag_spec
         )
-        dag_spec = cls.erase_party_task_inputs(
-            dag_spec
-        )
 
         return dag_spec
 
     @classmethod
     def deduce_dag(cls, dag_parser: 'DagParser', task_name_list: list, dag_spec: DAGSpec,
-                   component_specs: Dict[str, ComponentSpec], data_tracer: dict):
-        stage = dag_spec.stage
+                   component_specs: Dict[str, ComponentSpec], data_tracer: dict,
+                   task_runtime_parties: Dict[str, List[PartySpec]]):
         deduced_dag = copy.deepcopy(dag_spec)
         deduced_dag.stage = Stage.PREDICT
 
         """
         linkage messages only occur in tasks field
         """
         task_name_set = set(task_name_list)
-        topological_task_list = list(dag_parser.topological_sort())
+        topological_task_list = list(dag_parser.global_topological_sort())
         for task_name in topological_task_list:
             if task_name not in task_name_set:
                 continue
 
             task = dag_spec.tasks[task_name]
             """
             job stage should be "train", so task.stage is default/predict/None, if stage is predict, erase it
             """
             if task.stage == Stage.PREDICT:
                 deduced_dag.tasks[task_name].stage = None
 
-            task_stage = task.stage if task.stage else stage
             """
             default stage should not distinguish fit & transform or fit & transform. 
             """
             component_spec = component_specs[task_name]
             if task.inputs and (data_input_artifacts := task.inputs.data):
                 for artifact_name, artifact_channel in data_input_artifacts.items():
-                    if isinstance(artifact_channel, DataWarehouseChannelSpec):
-                        continue
-
                     artifact_definition = component_spec.input_artifacts.data[artifact_name]
-
                     deduced_dag.tasks[task_name].inputs.data.pop(artifact_name)
-                    if artifact_name == InputDataKeyType.VALIDATE_DATA:
+                    if isinstance(artifact_channel, DataWarehouseChannelSpec) or artifact_name == InputDataKeyType.VALIDATE_DATA:
                         continue
                     elif artifact_name == InputDataKeyType.TRAIN_DATA:
                         """
                         change train_data to test_data, try to infer a test data key in input definition
                         """
                         test_input_key = cls.infer_test_input_data_key(artifact_name,
                                                                        task.inputs.data.keys(),
@@ -390,45 +494,73 @@
                             test_input_key = artifact_name
                         else:
                             test_input_key = cls.infer_test_input_data_key(artifact_name,
                                                                            task.inputs.data.keys(),
                                                                            component_spec.input_artifacts.data)
 
                     test_input_artifact_definition = component_spec.input_artifacts.data[test_input_key]
-                    artifact_source_type = list(artifact_channel.items())[0][0]
-                    runtime_output_channel = list(artifact_channel.items())[0][1]
-                    test_input_data = cls.infer_test_input_data(
-                        task_name_set,
-                        artifact_definition,
-                        test_input_artifact_definition,
-                        runtime_output_channel,
-                        dag_spec,
-                        component_specs,
-                        data_tracer
-                    )
-                    if test_input_data:
-                        if test_input_key not in deduced_dag.tasks[task_name].inputs.data:
-                            deduced_dag.tasks[task_name].inputs.data[test_input_key] = dict()
-                        deduced_dag.tasks[task_name].inputs.data[test_input_key][artifact_source_type] = \
-                            test_input_data
+                    for _, channel_list in artifact_channel.items():
+                        if not isinstance(channel_list, list):
+                            channel_list = [channel_list]
+                        for channel in channel_list:
+                            if isinstance(channel, DataWarehouseChannelSpec):
+                                continue
+                            assert isinstance(channel, RuntimeTaskOutputChannelSpec)
+                            parties = channel.parties if channel.parties else task_runtime_parties[channel.producer_task]
+
+                            for party_spec in parties:
+                                for party_id in party_spec.party_id:
+                                    test_input_data = cls.infer_test_input_data(
+                                        artifact_definition,
+                                        test_input_artifact_definition,
+                                        channel,
+                                        dag_spec,
+                                        component_specs,
+                                        data_tracer,
+                                        task_runtime_parties[task_name],
+                                        party_spec.role,
+                                        party_id
+                                    )
+                                    if test_input_data:
+                                        if test_input_key not in deduced_dag.tasks[task_name].inputs.data:
+                                            deduced_dag.tasks[task_name].inputs.data[test_input_key] = dict()
+                                        if _ not in deduced_dag.tasks[task_name].inputs.data[test_input_key]:
+                                            deduced_dag.tasks[task_name].inputs.data[test_input_key][_] = []
+                                        deduced_dag.tasks[task_name].inputs.data[test_input_key][_].extend(test_input_data)
+
+                        if channels := deduced_dag.tasks[task_name].inputs.data.get(test_input_key, {}).get(_):
+                            deduced_dag.tasks[task_name].inputs.data[test_input_key][_] = \
+                                cls.merge_artifact_channel_by_party(
+                                    channels,
+                                )
+
             if task.inputs and (model_input_artifacts := task.inputs.model):
                 for artifact_name in model_input_artifacts:
                     deduced_dag.tasks[task_name].inputs.model.pop(artifact_name)
 
             model_input_artifact_key, model_output_artifact_key = cls.infer_model_artifact(
                 component_spec.input_artifacts, component_spec.output_artifacts)
             if model_input_artifact_key and model_output_artifact_key:
-                deduced_dag.tasks[task_name].inputs.model = {
-                    model_input_artifact_key: {
-                        ArtifactSourceType.MODEL_WAREHOUSE: ModelWarehouseChannelSpec(
-                            producer_task=task_name,
-                            output_artifact_key=model_output_artifact_key
-                        )
+                parties = task_runtime_parties[task_name]
+                parties = list(filter(
+                    lambda party: \
+                        party.role in component_specs[task_name].output_artifacts.model[model_output_artifact_key].roles,
+                    parties)
+                )
+
+                if parties:
+                    deduced_dag.tasks[task_name].inputs.model = {
+                        model_input_artifact_key: {
+                            ArtifactSourceType.MODEL_WAREHOUSE: ModelWarehouseChannelSpec(
+                                producer_task=task_name,
+                                output_artifact_key=model_output_artifact_key,
+                                parties=parties
+                            )
+                        }
                     }
-                }
 
             if deduced_dag.tasks[task_name].inputs:
                 deduced_dag.tasks[task_name].dependent_tasks = cls.infer_dependent_tasks(
                     deduced_dag.tasks[task_name].inputs
                 )
 
         return deduced_dag
@@ -448,30 +580,14 @@
                 for task_name, task_spec in party_tasks_spec.tasks.items():
                     if task_name not in task_name_set:
                         ret_dag.party_tasks[site_name].tasks.pop(task_name)
 
         return ret_dag
 
     @classmethod
-    def erase_party_task_inputs(cls, dag_spec: DAGSpec):
-        ret_dag = copy.deepcopy(dag_spec)
-        if not dag_spec.party_tasks:
-            return ret_dag
-
-        for site_name, party_task_spec in dag_spec.party_tasks.items():
-            if not party_task_spec.tasks:
-                continue
-
-            for task_name, task_spec in party_task_spec.tasks.items():
-                if task_spec.inputs:
-                    ret_dag.party_tasks[site_name].tasks[task_name].inputs = None
-
-        return ret_dag
-
-    @classmethod
     def infer_dependent_tasks(cls, input_artifacts):
         if not input_artifacts:
             return []
 
         dependent_task_list = list()
         for input_type in InputArtifactType.types():
             artifacts = getattr(input_artifacts, input_type)
@@ -568,122 +684,182 @@
 
         if candidate_count != 1:
             raise ValueError(f"Can not infer output artifact data name from {output_artifacts}")
         return candidate_artifact_name
 
     @classmethod
     def infer_test_input_data(cls,
-                              task_name_set,
                               train_artifact_definition,
                               test_artifact_definition,
-                              output_channel: Union[RuntimeTaskOutputChannelSpec, List[RuntimeTaskOutputChannelSpec]],
+                              channel: RuntimeTaskOutputChannelSpec,
                               dag_spec,
                               component_specs,
-                              data_tracer: dict):
+                              data_tracer: dict,
+                              down_task_runtime_parties,
+                              role,
+                              party_id):
         if not (set(train_artifact_definition.types) & set(test_artifact_definition.types)):
             raise ValueError(f"train_artifact_definition's types are {train_artifact_definition.types[0]}, "
                              f"can not be changed to {test_artifact_definition.types[0]}")
-        if not isinstance(output_channel, list):
-            output_channel = [output_channel]
 
-        ret_output_channel = []
-        for channel in output_channel:
-            if isinstance(channel, DataWarehouseChannelSpec):
-                continue
+        can_link_down = False
+        for party_spec in down_task_runtime_parties:
+            if party_spec.role == role and party_id in party_spec.party_id:
+                can_link_down = True
+                break
 
-            upstream_task = data_tracer[channel.producer_task]
-            if upstream_task is None:
-                continue
+        if not can_link_down:
+            return None
 
-            test_artifact_data_key = cls.infer_test_output_data_key(
-                component_specs[upstream_task].output_artifacts.data
-            )
-            ret_output_channel.append(
-                RuntimeTaskOutputChannelSpec(
-                    producer_task=upstream_task,
-                    output_artifact_key=test_artifact_data_key
-                )
-            )
+        if role not in data_tracer[channel.producer_task] or party_id not in data_tracer[channel.producer_task][role]:
+            return None
 
-        if not ret_output_channel:
+        if role not in test_artifact_definition.roles or role not in train_artifact_definition.roles:
             return None
-        elif train_artifact_definition.is_multi:
-            return ret_output_channel
-        else:
-            return ret_output_channel[0]
+
+        parties = dag_spec.tasks[channel.producer_task].parties if dag_spec.tasks[channel.producer_task].parties else dag_spec.parties
+        can_link_up = False
+        for party_spec in parties:
+            if role == party_spec.role and party_id in party_spec.party_id:
+                can_link_up = True
+
+        if not can_link_up:
+            return None
+
+        upstream_task = data_tracer[channel.producer_task][role][party_id]
+        if not upstream_task:
+            return None
+
+        test_artifact_data_key = cls.infer_test_output_data_key(
+            component_specs[upstream_task].output_artifacts.data
+        )
+
+        return [
+            RuntimeTaskOutputChannelSpec(
+                producer_task=upstream_task,
+                output_artifact_key=test_artifact_data_key,
+                parties=[PartySpec(role=role, party_id=[party_id])]
+            )
+        ]
+
+    @classmethod
+    def merge_artifact_channel_by_party(cls, channels: List[RuntimeTaskOutputChannelSpec]):
+        channels.sort(key=lambda channel: (channel.producer_task, channel.output_artifact_key, channel.parties[0].role))
+        merge_channels = []
+        i = 0
+        while i < len(channels):
+            j = i + 1
+            merge_channels.append(channels[i])
+            while j < len(channels) and (channels[j].producer_task, channels[j].output_artifact_key) == \
+                    (channels[i].producer_task, channels[i].output_artifact_key):
+                if channels[j].parties[0].role == merge_channels[-1].parties[-1].role:
+                    merge_channels[-1].parties[-1].party_id.append(channels[j].parties[-1].party_id[0])
+                else:
+                    merge_channels[-1].parties.append(channels[j].parties[0])
+
+                j += 1
+
+            i = j
+
+        return merge_channels
 
     @classmethod
-    def trace_back_deploy_task(cls, task_name, task_name_set, dag_spec: DAGSpec, component_specs, data_tracer: dict):
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
+    @classmethod
+    def trace_back_deploy_task(
+            cls, task_name, task_name_set, dag_spec: DAGSpec,
+            component_specs: Dict[str, ComponentSpec], data_tracer: dict,
+            task_runtime_parties: Dict[str, List[PartySpec]], role, party_id):
+
         if task_name in task_name_set:
-            return task_name
+            if cls.task_can_run(role, party_id, component_specs[task_name], task_runtime_parties[task_name]):
+                return task_name
+            return None
 
         if task_name in data_tracer:
-            return data_tracer[task_name]
+            if party_id in data_tracer[task_name].get(role, {}):
+                return task_name
+            return None
 
         task_spec = dag_spec.tasks[task_name]
-        component_spec = component_specs[task_name]
 
         if task_spec.inputs is None or task_spec.inputs.data is None:
             return None
 
-        upstream_task = set()
         for artifact_name, artifact_channel in task_spec.inputs.data.items():
-            artifact_definition = component_spec.input_artifacts.data[artifact_name]
-
             if not task_spec.stage:
                 """
                 task stage is train, inherit from job is train
                 """
                 if artifact_name == InputDataKeyType.VALIDATE_DATA:
                     continue
 
-            if artifact_definition.is_multi:
-                channels = list(artifact_channel.items())[0][1]
-                for channel in channels:
+            for _, channel_list in artifact_channel.items():
+                if not isinstance(channel_list, list):
+                    channel_list = [channel_list]
+
+                for channel in channel_list:
                     if isinstance(channel, DataWarehouseChannelSpec):
                         continue
+                    assert isinstance(channel, RuntimeTaskOutputChannelSpec), f"channel={channel} not support to deploy"
 
-                    upstream_task.add(
-                        cls.trace_back_deploy_task(
-                            channel.producer_task,
-                            task_name_set,
-                            dag_spec,
-                            component_specs,
-                            data_tracer)
-                    )
-            else:
-                channel = list(artifact_channel.items())[0][1]
-                if isinstance(channel, DataWarehouseChannelSpec):
-                    continue
+                    producer_task = channel.producer_task
+                    up_component_spec = component_specs[producer_task]
+                    if not cls.task_can_run(role,
+                                            party_id,
+                                            up_component_spec,
+                                            task_runtime_parties[task_name]):
+                        continue
 
-                upstream_task.add(
-                    cls.trace_back_deploy_task(
-                        channel.producer_task,
-                        task_name_set,
-                        dag_spec,
-                        component_specs,
-                        data_tracer)
-                )
+                    if not up_component_spec.output_artifacts or not up_component_spec.output_artifacts.data:
+                        continue
 
-        if not upstream_task:
-            return None
-        elif len(upstream_task) == 1:
-            return list(upstream_task)[0]
-        else:
-            return list(upstream_task)
+                    test_output_data_key = cls.infer_test_output_data_key(up_component_spec.output_artifacts.data)
+                    if role not in up_component_spec.output_artifacts.data[test_output_data_key].roles:
+                        continue
+
+                    if (up_input_name := cls.trace_back_deploy_task(
+                                                producer_task,
+                                                task_name_set,
+                                                dag_spec,
+                                                component_specs,
+                                                data_tracer,
+                                                task_runtime_parties,
+                                                role,
+                                                party_id)
+                        ):
+                        return up_input_name
+
+        return None
+
+    @classmethod
+    def translate_dag(cls, src, dst, *args, **kwargs):
+        from ..adapters import adapter_map
+        translate_func = adapter_map[src][dst]
+
+        return translate_func(*args, **kwargs)
 
 
 class TaskNodeInfo(object):
     def __init__(self):
         self._runtime_parameters = None
-        self._runtime_parties = None
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
 
@@ -696,38 +872,30 @@
         return self._runtime_parameters
 
     @runtime_parameters.setter
     def runtime_parameters(self, runtime_parameters):
         self._runtime_parameters = runtime_parameters
 
     @property
-    def runtime_parties(self):
-        return self._runtime_parties
-
-    @runtime_parties.setter
-    def runtime_parties(self, runtime_parties):
-        self._runtime_parties = runtime_parties
-
-    @property
-    def runtime_roles(self) -> list:
-        roles = set()
-        for party_spec in self._runtime_parties:
-            roles.add(party_spec.role)
-
-        return list(roles)
-
-    @property
     def upstream_inputs(self):
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
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/utils/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/utils/fateflow/__init__.py` & `fate-client-2.1.0/fate_client/pipeline/utils/fateflow/__init__.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/utils/fateflow/fate_flow_job_invoker.py` & `fate-client-2.1.0/fate_client/pipeline/utils/fateflow/fate_flow_job_invoker.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,53 +113,45 @@
                 return None
 
             party_id = response["data"]["party_id"]
             return party_id
         except ValueError:
             return None
 
-    def upload_data(self, file, meta, head, extend_sid, role=None, party_id=None, **kwargs):
-        response = self._client.data.upload(file=file,
-                                            head=head,
-                                            meta=meta,
-                                            extend_sid=extend_sid,
-                                            **kwargs)
+    def bind_local_path(self, path, namespace, name):
+        response = self._client.table.bind_path(path=path, namespace=namespace, name=name)
         try:
             code = response["code"]
             if code != 0:
-                raise ValueError(f"Return code {code}!=0")
-
-            namespace = response["data"]["namespace"]
-            name = response["data"]["name"]
-            job_id = response["job_id"]
+                raise ValueError(f"Return code {code} != 0")
+            print(f"bind path success")
         except BaseException:
-            raise ValueError(f"Upload data fails, response={response}")
-
-        self.monitor_status(job_id, role=role, party_id=party_id)
-        return dict(namespace=namespace, name=name)
-
-    def transform_to_dataframe(self, name, namespace, data_warehouse, site_name, role, party_id):
-        response = self._client.data.dataframe_transformer(namespace=namespace,
-                                                           name=name,
-                                                           site_name=site_name,
-                                                           data_warehouse=data_warehouse)
+            raise ValueError(f"bind path fails, response={response}")
 
+    def upload_file_and_convert_to_dataframe(
+            self, file, meta, head, extend_sid,
+            namespace, name, role=None, party_id=None, **kwargs):
+        response = self._client.data.upload_file(file=file,
+                                                 head=head,
+                                                 meta=meta,
+                                                 extend_sid=extend_sid,
+                                                 namespace=namespace,
+                                                 name=name,
+                                                 **kwargs)
         try:
             code = response["code"]
             if code != 0:
                 raise ValueError(f"Return code {code}!=0")
 
             job_id = response["job_id"]
         except BaseException:
             raise ValueError(f"Upload data fails, response={response}")
 
         self.monitor_status(job_id, role=role, party_id=party_id)
 
-        return code
-
     def get_output_data(self, job_id, role, party_id, task_name):
         with tempfile.TemporaryDirectory() as data_dir:
             response = self._client.output.download_data(job_id=job_id, role=role, party_id=party_id,
                                                          task_name=task_name, path=data_dir)
             try:
                 code = response["code"]
                 if code != 0:
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/utils/fateflow/flow_client.py` & `fate-client-2.1.0/fate_client/pipeline/utils/fateflow/flow_client.py`

 * *Files identical despite different names*

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/utils/file_utils.py` & `fate-client-2.1.0/fate_client/pipeline/utils/callbacks/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from ruamel import yaml
+#
 
+from ._callback import (
+    CallbackHandler,
+    PipelineCallBack,
+    JobInfoCallBack
+)
 
-def load_yaml_file(path: str):
-    with open(path, "r") as fin:
-        buf = fin.read()
-        return yaml.safe_load(buf)
+__all__ = [
+    "CallbackHandler",
+    "PipelineCallBack",
+    "JobInfoCallBack"
+]
```

### Comparing `fate-client-2.0.0b0/fate_client/pipeline/utils/test_utils.py` & `fate-client-2.1.0/fate_client/pipeline/utils/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,20 +60,19 @@
         self.guest = parties.get("guest", None)
         self.arbiter = parties.get("arbiter", None)
 
 
 class JobConfig(object):
     def __init__(self, config):
         self.parties = Parties(config.get("parties", {}))
-        # self.backend = config.get("backend", 0)
-        # self.work_mode = config.get("work_mode", 0)
         self.data_base_dir = config.get("data_base_dir", "")
         self.system_setting = config.get("system_setting", {})
         self.task_cores = config.get("task_cores", None)
         self.timeout = config.get("timeout", None)
+        self.engine_run = config.get("engine_run", None)
 
     @staticmethod
     def load(path: typing.Union[str, Path]):
         conf = JobConfig.load_from_file(path)
         return JobConfig(conf)
 
     @staticmethod
```

### Comparing `fate-client-2.0.0b0/fate_client.egg-info/PKG-INFO` & `fate-client-2.1.0/fate_client.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fate-client
-Version: 2.0.0b0
+Version: 2.1.0
 Summary: Clients for FATE, supply pipeline this version
 Home-page: https://fate.fedai.org/
 Author: FederatedAI
 Author-email: contact@FedAI.org
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click
@@ -13,12 +13,12 @@
 Requires-Dist: requests
 Requires-Dist: requests_toolbelt
 Requires-Dist: ruamel.yaml
 Requires-Dist: setuptools
 Requires-Dist: networkx
 Requires-Dist: pydantic
 Provides-Extra: fate
-Requires-Dist: pyfate==2.0.0b0; extra == "fate"
+Requires-Dist: pyfate==2.1.0; extra == "fate"
 Provides-Extra: fate-flow
-Requires-Dist: fate_flow==2.0.0b0; extra == "fate-flow"
+Requires-Dist: fate_flow==2.1.0; extra == "fate-flow"
 
 Clients for FATE, supply pipeline this version
```

### Comparing `fate-client-2.0.0b0/fate_client.egg-info/SOURCES.txt` & `fate-client-2.1.0/fate_client.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -47,56 +47,73 @@
 fate_client/flow_sdk/utils/__init__.py
 fate_client/flow_sdk/utils/base_utils.py
 fate_client/flow_sdk/utils/io_utils.py
 fate_client/flow_sdk/utils/params_utils.py
 fate_client/pipeline/__init__.py
 fate_client/pipeline/pipeline.py
 fate_client/pipeline/pipeline_cli.py
+fate_client/pipeline/adapters/__init__.py
+fate_client/pipeline/adapters/bfia/__init__.py
+fate_client/pipeline/adapters/bfia/translator/__init__.py
+fate_client/pipeline/adapters/bfia/translator/component_spec.py
+fate_client/pipeline/adapters/bfia/translator/component_translator.py
+fate_client/pipeline/adapters/bfia/translator/dag_spec.py
+fate_client/pipeline/adapters/bfia/translator/dsl_translator.py
+fate_client/pipeline/adapters/bfia/translator/utils/__init__.py
+fate_client/pipeline/adapters/bfia/translator/utils/types.py
 fate_client/pipeline/component_define/__init__.py
 fate_client/pipeline/component_define/fate/__init__.py
 fate_client/pipeline/component_define/fate/coordinated_linr.yaml
 fate_client/pipeline/component_define/fate/coordinated_lr.yaml
 fate_client/pipeline/component_define/fate/data_split.yaml
-fate_client/pipeline/component_define/fate/dataframe_io_test.yaml
 fate_client/pipeline/component_define/fate/dataframe_transformer.yaml
 fate_client/pipeline/component_define/fate/evaluation.yaml
+fate_client/pipeline/component_define/fate/feature_correlation.yaml
 fate_client/pipeline/component_define/fate/feature_scale.yaml
 fate_client/pipeline/component_define/fate/hetero_feature_binning.yaml
 fate_client/pipeline/component_define/fate/hetero_feature_selection.yaml
-fate_client/pipeline/component_define/fate/hetero_sbt.yaml
+fate_client/pipeline/component_define/fate/hetero_nn.yaml
+fate_client/pipeline/component_define/fate/hetero_secureboost.yaml
 fate_client/pipeline/component_define/fate/homo_lr.yaml
 fate_client/pipeline/component_define/fate/homo_nn.yaml
 fate_client/pipeline/component_define/fate/psi.yaml
 fate_client/pipeline/component_define/fate/reader.yaml
 fate_client/pipeline/component_define/fate/sample.yaml
+fate_client/pipeline/component_define/fate/sshe_linr.yaml
+fate_client/pipeline/component_define/fate/sshe_lr.yaml
 fate_client/pipeline/component_define/fate/statistics.yaml
 fate_client/pipeline/component_define/fate/union.yaml
 fate_client/pipeline/components/__init__.py
 fate_client/pipeline/components/component_base.py
 fate_client/pipeline/components/fate/__init__.py
 fate_client/pipeline/components/fate/coordinated_linr.py
 fate_client/pipeline/components/fate/coordinated_lr.py
 fate_client/pipeline/components/fate/data_split.py
-fate_client/pipeline/components/fate/dataframe_io_test.py
 fate_client/pipeline/components/fate/dataframe_transformer.py
 fate_client/pipeline/components/fate/evaluation.py
+fate_client/pipeline/components/fate/feature_correlation.py
 fate_client/pipeline/components/fate/feature_scale.py
 fate_client/pipeline/components/fate/hetero_feature_binning.py
 fate_client/pipeline/components/fate/hetero_feature_selection.py
-fate_client/pipeline/components/fate/hetero_sbt.py
+fate_client/pipeline/components/fate/hetero_nn.py
+fate_client/pipeline/components/fate/hetero_secureboost.py
 fate_client/pipeline/components/fate/homo_lr.py
 fate_client/pipeline/components/fate/homo_nn.py
 fate_client/pipeline/components/fate/psi.py
 fate_client/pipeline/components/fate/reader.py
 fate_client/pipeline/components/fate/sample.py
+fate_client/pipeline/components/fate/sshe_linr.py
+fate_client/pipeline/components/fate/sshe_lr.py
 fate_client/pipeline/components/fate/statistics.py
 fate_client/pipeline/components/fate/union.py
 fate_client/pipeline/components/fate/nn/__init__.py
 fate_client/pipeline/components/fate/nn/algo_params.py
+fate_client/pipeline/components/fate/nn/common_utils.py
 fate_client/pipeline/components/fate/nn/loader.py
+fate_client/pipeline/components/fate/nn/source.yaml
 fate_client/pipeline/components/fate/nn/torch/__init__.py
 fate_client/pipeline/components/fate/nn/torch/base.py
 fate_client/pipeline/components/fate/nn/torch/nn.py
 fate_client/pipeline/components/fate/nn/torch/optim.py
 fate_client/pipeline/conf/__init__.py
 fate_client/pipeline/conf/env_config.py
 fate_client/pipeline/conf/job_configuration.py
@@ -116,10 +133,12 @@
 fate_client/pipeline/interface/channel.py
 fate_client/pipeline/scheduler/__init__.py
 fate_client/pipeline/scheduler/component_stage.py
 fate_client/pipeline/scheduler/dag_parser.py
 fate_client/pipeline/utils/__init__.py
 fate_client/pipeline/utils/file_utils.py
 fate_client/pipeline/utils/test_utils.py
+fate_client/pipeline/utils/callbacks/__init__.py
+fate_client/pipeline/utils/callbacks/_callback.py
 fate_client/pipeline/utils/fateflow/__init__.py
 fate_client/pipeline/utils/fateflow/fate_flow_job_invoker.py
 fate_client/pipeline/utils/fateflow/flow_client.py
```

### Comparing `fate-client-2.0.0b0/setup.py` & `fate-client-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     "ruamel.yaml",
     "setuptools",
     "networkx",
     "pydantic",
 ]
 
 extras_require = {
-    "fate": ["pyfate==2.0.0b0"],
-    "fate_flow": ["fate_flow==2.0.0b0"]
+    "fate": ["pyfate==2.1.0"],
+    "fate_flow": ["fate_flow==2.1.0"]
 }
 entry_points = {"console_scripts": ["flow = fate_client.flow_cli.flow:flow_cli",
                                     "pipeline = fate_client.pipeline.pipeline_cli:pipeline_group"]}
 
 setup_kwargs = {
     "name": "fate-client",
     "version": fate_client.__version__,
```

