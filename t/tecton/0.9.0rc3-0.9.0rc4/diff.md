# Comparing `tmp/tecton-0.9.0rc3.tar.gz` & `tmp/tecton-0.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecton-0.9.0rc3.tar", last modified: Tue Apr  2 00:49:24 2024, max compression
+gzip compressed data, was "tecton-0.9.0rc4.tar", last modified: Wed Apr  3 21:27:01 2024, max compression
```

## Comparing `tecton-0.9.0rc3.tar` & `tecton-0.9.0rc4.tar`

### file list

```diff
@@ -1,670 +1,670 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.274081 tecton-0.9.0rc3/
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      206 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/MANIFEST.in
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3955 2024-04-02 00:49:24.274081 tecton-0.9.0rc3/PKG-INFO
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/README.md
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.206077 tecton-0.9.0rc3/protoc_gen_openapiv2/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.206077 tecton-0.9.0rc3/protoc_gen_openapiv2/options/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18717 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2024-04-02 00:49:24.274081 tecton-0.9.0rc3/setup.cfg
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2503 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/setup.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.210077 tecton-0.9.0rc3/tecton/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6026 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_gen_version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.214077 tecton-0.9.0rc3/tecton/_internals/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10733 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/analytics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2279 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/athena_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1168 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/data_frame_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6558 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/delete_keys_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8122 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/display.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      930 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/env_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27420 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/find_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3193 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/ingest_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2359 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/ingestion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12345 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/materialization_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/metadata_service.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.214077 tecton-0.9.0rc3/tecton/_internals/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      492 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/metadata_service_impl/auth_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1870 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/metadata_service_impl/request_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      615 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/metadata_service_impl/service_modules.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/mock_source_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1357 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/offline_store_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1037 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/pandas_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16160 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/query_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21072 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/querytree_api.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.214077 tecton-0.9.0rc3/tecton/_internals/repo/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/repo/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11416 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/repo/function_serialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12059 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15912 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/run_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13055 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/sdk_decorators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2059 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/secret_resolver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7119 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/snowflake_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7034 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/spark_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5615 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/tecton_pydantic.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7071 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3769 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14505 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4985 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_internals/validations_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      322 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/_stamp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3067 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/aggregation_functions.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.218078 tecton-0.9.0rc3/tecton/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25510 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/access_control.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1583 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/api_key.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3083 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/auth.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5469 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/cli.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8462 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/cli_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5967 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/command.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2027 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/completion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18539 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/engine.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1323 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/engine_renderer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34260 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/environment.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7938 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/environment_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7691 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/error_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3759 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      515 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/pex_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/printer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5135 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/repo.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9757 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/repo_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7739 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/repo_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4711 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5824 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/service_account.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5620 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2403 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/user.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4917 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/workspace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2711 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/cli/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/fco_listers.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.218078 tecton-0.9.0rc3/tecton/framework/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6920 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/base_tecton_object.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   119708 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/configs.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28984 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/data_frame.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    38553 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13799 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/dataset.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/entity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    42563 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/feature_service.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   225468 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/feature_view.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/filtered_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4922 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/repo_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21258 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/transformation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2071 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/validation_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22520 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/framework/workspace.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.218078 tecton-0.9.0rc3/tecton/identities/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/identities/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/identities/api_keys.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14640 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/identities/credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12333 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/identities/okta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2374 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/pytest_tecton.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/run_api_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      709 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/snowflake_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2747 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/tecton_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6326 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/types.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.218078 tecton-0.9.0rc3/tecton/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.218078 tecton-0.9.0rc3/tecton/vendor/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.222078 tecton-0.9.0rc3/tecton/vendor/dill/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/__diff.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/_objects.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/detect.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/info.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/objtypes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/pointers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/settings.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/dill/dill/temp.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.222078 tecton-0.9.0rc3/tecton/vendor/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.222078 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/clientserver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/finalizer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/java_collections.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/protocol.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/signals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.226078 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/_globals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/accumulators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/broadcast.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.226078 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/daemon.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/files.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/find_spark_home.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/install.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/join.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.226078 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/base.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/fpm.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/image.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.226078 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.226078 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/param/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/param/shared.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/regression.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/stat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/tuning.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/wrapper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.230079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/fpm.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.230079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/random.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/regression.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.230079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/profiler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.230079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/python/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/python/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.230079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/python/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/rdd.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/rddsampler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.230079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resource/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resource/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resource/information.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resource/profile.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resource/requests.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resultiterable.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/shuffle.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.234079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.234079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/catalog.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/column.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/dataframe.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/group.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.234079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/readwriter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/streaming.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/udf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/window.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/statcounter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/storagelevel.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.238079 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/dstream.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/listener.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/taskcontext.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/traceback_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/worker.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/vendor_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/vendor/vendor_pyspark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1154 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.210077 tecton-0.9.0rc3/tecton.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3955 2024-04-02 00:49:22.000000 tecton-0.9.0rc3/tecton.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22872 2024-04-02 00:49:23.000000 tecton-0.9.0rc3/tecton.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2024-04-02 00:49:22.000000 tecton-0.9.0rc3/tecton.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2024-04-02 00:49:22.000000 tecton-0.9.0rc3/tecton.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1044 2024-04-02 00:49:22.000000 tecton-0.9.0rc3/tecton.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      120 2024-04-02 00:49:23.000000 tecton-0.9.0rc3/tecton.egg-info/top_level.txt
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.238079 tecton-0.9.0rc3/tecton_athena/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14977 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/athena_session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8797 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/data_catalog_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5764 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/odfv_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.238079 tecton-0.9.0rc3/tecton_athena/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2381 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17721 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.238079 tecton-0.9.0rc3/tecton_athena/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates/create_table.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3975 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_athena/templates_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.242079 tecton-0.9.0rc3/tecton_core/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/_gen_version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13149 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/aggregation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1598 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/arrow.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/aws_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3464 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/compute_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    24781 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7234 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/data_types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3520 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/duckdb_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.242079 tecton-0.9.0rc3/tecton_core/embeddings/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/embeddings/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/embeddings/config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7404 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5113 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/fco_container.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27252 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/feature_definition_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9838 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/feature_set_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      749 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/feature_view_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/filter_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2507 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/function_deserialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      739 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/http.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      616 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/id_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      546 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/iterators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7440 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/materialization_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.242079 tecton-0.9.0rc3/tecton_core/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/metadata_service_impl/base_stub.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2665 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/metadata_service_impl/error_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3488 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/metadata_service_impl/http_client.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      901 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/metadata_service_impl/providers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/metadata_service_impl/response.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/metadata_service_impl/service_calls.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      206 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/metadata_service_impl/trace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20281 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1427 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/online_serving_index.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7383 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/pipeline_common.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.246080 tecton-0.9.0rc3/tecton_core/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22026 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    56201 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5286 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/compaction_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      179 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/dialect.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.246080 tecton-0.9.0rc3/tecton_core/query/duckdb/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/duckdb/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10669 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/duckdb/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7820 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/duckdb/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      714 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/duckdb/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1526 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      746 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/executor_params.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/executor_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10749 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/node_interface.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7303 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/node_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126328 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.246080 tecton-0.9.0rc3/tecton_core/query/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3556 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/pandas/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4033 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/pandas/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22035 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/pandas/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6169 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/pandas/pipeline_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5054 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/pandas/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      192 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/pandas/sql.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1948 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/pandas/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5944 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/pipeline_sql_builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      786 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/prefixed_uri_resolver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4204 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/query_tree_compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21774 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/query_tree_executor.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      227 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/rewrite.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.246080 tecton-0.9.0rc3/tecton_core/query/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12630 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/snowflake/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20202 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query/sql_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3294 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/query_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/repo_file_handler.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/request_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3149 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/schema.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11857 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5597 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/schema_validation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1063 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2126 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/snowflake_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.246080 tecton-0.9.0rc3/tecton_core/specs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      777 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/specs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44686 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/specs/data_source_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1457 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/specs/entity_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5460 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/specs/feature_service_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    43502 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/specs/feature_view_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/specs/tecton_object_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9179 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/specs/time_window_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/specs/transformation_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4952 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/specs/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9725 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/time_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.250080 tecton-0.9.0rc3/tecton_core/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/vendor/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9361 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/vendor/queue.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.250080 tecton-0.9.0rc3/tecton_core/vendor/treelib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/vendor/treelib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/vendor/treelib/exceptions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/vendor/treelib/misc.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/vendor/treelib/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/vendor/treelib/plugins.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/vendor/treelib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_core/vendor/vendor_treelib.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.250080 tecton-0.9.0rc3/tecton_materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      718 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23171 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/batch_materialization.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.250080 tecton-0.9.0rc3/tecton_materialization/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2835 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/common/job_metadata.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5803 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/common/job_metadata_aws.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2222 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/common/job_metadata_gcp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/common/task_params.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/consumption.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1070 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/delta_maintenance.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3731 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/entity_deletion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5200 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/feature_export.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5090 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ingest_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7159 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/job_metadata.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9316 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7780 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/materialization_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.250080 tecton-0.9.0rc3/tecton_materialization/ray/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ray/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5242 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ray/batch_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23853 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ray/delta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5973 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ray/feature_export.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5009 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ray/ingest_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6869 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ray/job_status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10181 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ray/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4190 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ray/materialization_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3172 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/ray/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.250080 tecton-0.9.0rc3/tecton_materialization/remote_host/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/remote_host/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20100 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/remote_host/pyspark_remote_host.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1996 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6666 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_materialization/stream_materialization.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.250080 tecton-0.9.0rc3/tecton_proto/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.254080 tecton-0.9.0rc3/tecton_proto/amplitude/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/amplitude/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4642 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/amplitude/amplitude_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/amplitude/client_logging_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.254080 tecton-0.9.0rc3/tecton_proto/api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/api/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.254080 tecton-0.9.0rc3/tecton_proto/api/featureservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/api/featureservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    81835 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/api/featureservice/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9573 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/api/featureservice/feature_service_request_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.254080 tecton-0.9.0rc3/tecton_proto/args/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/basic_info_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/data_source_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21470 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3996 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/diff_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/diff_test_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3059 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/fco_args_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5172 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    41821 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6092 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/pipeline_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/repo_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4704 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/user_defined_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/version_constraints_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8163 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/args/virtual_data_source_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.254080 tecton-0.9.0rc3/tecton_proto/auditlog/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/auditlog/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/auditlog/metadata_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.254080 tecton-0.9.0rc3/tecton_proto/auth/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/auth/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1422 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/auth/acl_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29023 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/auth/authorization_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3224 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/auth/principal_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6551 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/auth/resource_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/auth/resource_role_assignments_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/auth/service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.254080 tecton-0.9.0rc3/tecton_proto/canary/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/canary/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/canary/type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/canary/update_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.254080 tecton-0.9.0rc3/tecton_proto/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/cli/repo_diff_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.258080 tecton-0.9.0rc3/tecton_proto/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/aggregation_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/analytics_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1823 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/aws_credentials_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/column_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1336 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/compute_mode_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1934 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/container_image_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/data_source_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/data_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/fco_locator_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/framework_version_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/id_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/pair_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/schema_container_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2819 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1518 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/secret_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/spark_schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2183 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/common/time_window_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.258080 tecton-0.9.0rc3/tecton_proto/consumption/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/consumption/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5600 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/consumption/consumption_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.262081 tecton-0.9.0rc3/tecton_proto/data/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7900 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/batch_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2313 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/fco_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2916 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/fco_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5025 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/feature_store_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20254 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/freshness_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4810 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/fv_materialization_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/hive_metastore_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1975 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/internal_spark_cluster_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1683 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/materialization_roles_allowlists_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5831 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/materialization_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/odfv_compute_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/onboarding_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/principal_group_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6827 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/remote_compute_environment_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15757 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/remote_spark_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/saved_feature_data_frame_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4545 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/serving_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10895 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/state_update_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4799 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/stream_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/summary_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2349 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/tecton_api_key_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2795 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10456 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/user_deployment_settings_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/user_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3433 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/virtual_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/data/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.262081 tecton-0.9.0rc3/tecton_proto/databricks_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/dbfs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/execution_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/instance_profiles_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/jobs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/libraries_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2911 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/permissions_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/scim_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/secrets_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2613 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/databricks_api/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.262081 tecton-0.9.0rc3/tecton_proto/dataobs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/dataobs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/dataobs/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/dataobs/expectation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/dataobs/metric_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/dataobs/validation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3723 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/dataobs/validation_task_params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/dataobs/validation_task_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.262081 tecton-0.9.0rc3/tecton_proto/feature_server/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/feature_server/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.262081 tecton-0.9.0rc3/tecton_proto/feature_server/configuration/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/feature_server/configuration/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19997 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.262081 tecton-0.9.0rc3/tecton_proto/materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9821 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/materialization/job_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2610 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/materialization/materialization_states_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14634 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/materialization/materialization_task_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8173 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/materialization/params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2752 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/materialization/spark_cluster_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/materializationjobservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/materializationjobservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16111 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/metadataservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/metadataservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/metadataservice/http_over_grpc_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   121489 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/metadataservice/metadata_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/offlinestore/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/offlinestore/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/offlinestore/delta/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/offlinestore/delta/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1570 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/offlinestore/delta/metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6554 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/offlinestore/delta/transaction_writer_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/online_store/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/online_store/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/online_store/feature_value_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/online_store/status_entry_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/online_store_writer/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/online_store_writer/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/online_store_writer/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5522 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/online_store_writer/copier_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/remoteenvironmentservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/remoteenvironmentservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13213 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/secrets/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/secrets/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10485 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/secrets/secrets_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/snowflake/location_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1392 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/snowflake/snowflake_credentials_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/spark_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/spark_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/spark_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7388 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/spark_api/jobs_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/spark_common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/spark_common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7786 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/spark_common/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/spark_common/libraries_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/testhelperservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/testhelperservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3516 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/testhelperservice/test_helper_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_proto/validation/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/validation/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_proto/validation/validator_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.266081 tecton-0.9.0rc3/tecton_snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30085 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.270081 tecton-0.9.0rc3/tecton_snowflake/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10160 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/query/dataframe_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13559 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/query/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6314 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/query/queries.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      741 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/query/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3704 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8392 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2246 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/snowflake_type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33728 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.270081 tecton-0.9.0rc3/tecton_snowflake/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1025 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/copier_macro.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/create_temp_table_for_bfv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/delete_orphaned_schemas.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/delete_staged_files.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/historical_features_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/materialized_feature_view.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/offline_materialization_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/online_store_copier.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/templates_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_snowflake/utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.274081 tecton-0.9.0rc3/tecton_spark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      808 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30278 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/data_observability.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/data_source_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    35476 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/data_source_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/errors_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6470 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/feature_view_spark_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.274081 tecton-0.9.0rc3/tecton_spark/jars/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/jars/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2633 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/jars/class_loader.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)  1794322 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/jars/tecton-udfs-spark-3.jar
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7188 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/materialization_plan.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27440 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15383 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/partial_aggregations.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33278 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:24.274081 tecton-0.9.0rc3/tecton_spark/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3356 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/query/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10751 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/query/filter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37167 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/query/join.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1515 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/query/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7533 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/query/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14752 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/query/projection.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17887 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5434 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/schema_spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/spark_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1697 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/spark_schema_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4858 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/udf_jar.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2024-04-02 00:49:20.000000 tecton-0.9.0rc3/tecton_spark/udfs.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.425795 tecton-0.9.0rc4/
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      206 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/MANIFEST.in
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3955 2024-04-03 21:27:01.425795 tecton-0.9.0rc4/PKG-INFO
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/README.md
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.289783 tecton-0.9.0rc4/protoc_gen_openapiv2/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.289783 tecton-0.9.0rc4/protoc_gen_openapiv2/options/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18717 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2024-04-03 21:27:01.425795 tecton-0.9.0rc4/setup.cfg
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2503 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.293783 tecton-0.9.0rc4/tecton/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6026 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/_gen_version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.301784 tecton-0.9.0rc4/tecton/_internals/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10733 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/analytics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2279 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/athena_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1168 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/data_frame_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6558 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/delete_keys_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8122 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/display.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      930 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/env_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28683 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/find_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3193 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/ingest_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2359 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/ingestion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12345 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/materialization_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.301784 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      492 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/auth_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1870 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/request_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      615 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/service_modules.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/mock_source_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1357 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/offline_store_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1037 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/pandas_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16160 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/query_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21292 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/querytree_api.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.301784 tecton-0.9.0rc4/tecton/_internals/repo/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/_internals/repo/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11416 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/repo/function_serialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12059 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16172 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/run_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13055 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/sdk_decorators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2059 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/secret_resolver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7119 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/snowflake_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7034 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/spark_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5615 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/tecton_pydantic.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7071 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3769 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14505 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4985 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/validations_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      322 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_stamp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3067 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/aggregation_functions.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.305784 tecton-0.9.0rc4/tecton/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26054 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/access_control.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1583 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/api_key.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3083 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/auth.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5469 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/cli.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8462 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/cli_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5967 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/command.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2027 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/completion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18539 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/engine.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1323 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/engine_renderer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34388 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/environment.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7938 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/environment_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7691 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/error_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3759 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      515 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/pex_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/printer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5135 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/repo.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9759 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/repo_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7739 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/repo_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5010 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5824 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/service_account.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5620 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2403 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/user.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4917 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/workspace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2711 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/fco_listers.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.309785 tecton-0.9.0rc4/tecton/framework/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6920 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/base_tecton_object.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   119708 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/configs.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28984 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/data_frame.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    38553 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13976 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/dataset.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/entity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    42636 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/feature_service.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   225796 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/feature_view.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/filtered_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4922 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/repo_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21258 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/transformation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2071 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/validation_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22520 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/workspace.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.309785 tecton-0.9.0rc4/tecton/identities/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/identities/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/identities/api_keys.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14640 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/identities/credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12333 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/identities/okta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2374 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/pytest_tecton.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/run_api_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      709 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/snowflake_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2747 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/tecton_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6326 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/types.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.309785 tecton-0.9.0rc4/tecton/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.309785 tecton-0.9.0rc4/tecton/vendor/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/dill/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.313785 tecton-0.9.0rc4/tecton/vendor/dill/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/__diff.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/_objects.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/detect.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/info.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/objtypes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/pointers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/settings.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/temp.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.313785 tecton-0.9.0rc4/tecton/vendor/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.313785 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/clientserver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/finalizer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/java_collections.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/protocol.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/signals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.321786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/_globals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/accumulators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/broadcast.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.321786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/daemon.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/files.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/find_spark_home.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/install.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/join.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.325786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/base.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/fpm.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/image.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.325786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.325786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/shared.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/regression.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/stat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/tuning.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/wrapper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.329786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/fpm.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.329786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/random.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/regression.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.329786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/profiler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.333787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.333787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/rdd.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/rddsampler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.333787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/information.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/profile.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/requests.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resultiterable.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/shuffle.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.337787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.337787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/catalog.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/column.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/dataframe.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/group.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.341787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/readwriter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/streaming.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/udf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/window.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/statcounter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/storagelevel.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.341787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/dstream.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/listener.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/taskcontext.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/traceback_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/worker.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/vendor_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/vendor_pyspark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1154 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.293783 tecton-0.9.0rc4/tecton.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3955 2024-04-03 21:26:58.000000 tecton-0.9.0rc4/tecton.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22872 2024-04-03 21:26:59.000000 tecton-0.9.0rc4/tecton.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2024-04-03 21:26:58.000000 tecton-0.9.0rc4/tecton.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2024-04-03 21:26:59.000000 tecton-0.9.0rc4/tecton.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1044 2024-04-03 21:26:59.000000 tecton-0.9.0rc4/tecton.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      120 2024-04-03 21:26:59.000000 tecton-0.9.0rc4/tecton.egg-info/top_level.txt
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.341787 tecton-0.9.0rc4/tecton_athena/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14977 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/athena_session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8797 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/data_catalog_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5764 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/odfv_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.341787 tecton-0.9.0rc4/tecton_athena/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2381 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17721 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.345788 tecton-0.9.0rc4/tecton_athena/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/create_table.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3975 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.349788 tecton-0.9.0rc4/tecton_core/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/_gen_version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/aggregation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1598 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/arrow.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/aws_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3464 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/compute_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    24781 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7234 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/data_types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3520 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/duckdb_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.349788 tecton-0.9.0rc4/tecton_core/embeddings/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/embeddings/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/embeddings/config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7404 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5113 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/fco_container.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27252 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/feature_definition_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9838 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/feature_set_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      749 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/feature_view_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/filter_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2507 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/function_deserialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      739 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/http.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      616 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/id_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      546 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/iterators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7440 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/materialization_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.353788 tecton-0.9.0rc4/tecton_core/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/base_stub.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2665 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/error_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3488 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/http_client.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      901 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/providers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/response.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/service_calls.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      206 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/trace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20281 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1427 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/online_serving_index.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7383 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/pipeline_common.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.357789 tecton-0.9.0rc4/tecton_core/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22026 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    56201 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5286 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/compaction_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      179 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/dialect.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.357789 tecton-0.9.0rc4/tecton_core/query/duckdb/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/query/duckdb/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10669 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/duckdb/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7820 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/duckdb/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      714 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/duckdb/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1526 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      746 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/executor_params.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/executor_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10749 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/node_interface.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7303 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/node_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126328 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.361789 tecton-0.9.0rc4/tecton_core/query/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/query/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3556 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4033 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22035 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6169 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/pipeline_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5054 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      192 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/sql.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1948 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5944 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pipeline_sql_builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      786 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/prefixed_uri_resolver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4204 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/query_tree_compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21774 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/query_tree_executor.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      227 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/rewrite.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.361789 tecton-0.9.0rc4/tecton_core/query/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/query/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12630 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/snowflake/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20202 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/sql_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3294 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/repo_file_handler.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/request_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/schema.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11989 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5597 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/schema_validation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1063 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2126 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/snowflake_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.361789 tecton-0.9.0rc4/tecton_core/specs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      777 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44686 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/data_source_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1457 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/entity_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5460 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/feature_service_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    43502 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/feature_view_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/tecton_object_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9179 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/time_window_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/transformation_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4952 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9725 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/time_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.361789 tecton-0.9.0rc4/tecton_core/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/vendor/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9361 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/queue.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.365790 tecton-0.9.0rc4/tecton_core/vendor/treelib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/exceptions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/misc.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/plugins.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/vendor_treelib.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.369790 tecton-0.9.0rc4/tecton_materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      718 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23171 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/batch_materialization.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.369790 tecton-0.9.0rc4/tecton_materialization/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_materialization/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2835 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/common/job_metadata.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5803 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/common/job_metadata_aws.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2222 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/common/job_metadata_gcp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/common/task_params.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/consumption.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1070 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/delta_maintenance.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3731 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/entity_deletion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5200 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/feature_export.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5090 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ingest_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7159 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/job_metadata.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9316 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7780 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/materialization_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_materialization/ray/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_materialization/ray/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5242 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/batch_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23853 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/delta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5973 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/feature_export.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5009 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/ingest_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6869 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/job_status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10181 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4190 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/materialization_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3172 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_materialization/remote_host/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/remote_host/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20100 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/remote_host/pyspark_remote_host.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1996 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6666 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/stream_materialization.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_proto/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_proto/amplitude/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/amplitude/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4642 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/amplitude/amplitude_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/amplitude/client_logging_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_proto/api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/api/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_proto/api/featureservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/api/featureservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    81835 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/api/featureservice/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9573 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/api/featureservice/feature_service_request_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.377791 tecton-0.9.0rc4/tecton_proto/args/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/args/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/basic_info_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/data_source_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21470 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3996 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/diff_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/diff_test_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3059 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/fco_args_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5172 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    41821 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6092 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/pipeline_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/repo_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4704 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/user_defined_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/version_constraints_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8163 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/virtual_data_source_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.381791 tecton-0.9.0rc4/tecton_proto/auditlog/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/auditlog/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auditlog/metadata_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.381791 tecton-0.9.0rc4/tecton_proto/auth/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/auth/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1422 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/acl_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29023 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/authorization_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3224 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/principal_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6551 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/resource_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/resource_role_assignments_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.381791 tecton-0.9.0rc4/tecton_proto/canary/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/canary/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/canary/type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/canary/update_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.381791 tecton-0.9.0rc4/tecton_proto/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/cli/repo_diff_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.385792 tecton-0.9.0rc4/tecton_proto/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/aggregation_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/analytics_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1823 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/aws_credentials_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/column_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1336 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/compute_mode_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1934 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/container_image_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/data_source_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/data_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/fco_locator_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/framework_version_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/id_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/pair_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/schema_container_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2819 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1518 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/secret_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/spark_schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2183 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/time_window_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.385792 tecton-0.9.0rc4/tecton_proto/consumption/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/consumption/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5600 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/consumption/consumption_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.393792 tecton-0.9.0rc4/tecton_proto/data/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/data/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7900 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/batch_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2313 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/fco_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2916 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/fco_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5025 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/feature_store_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20254 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/freshness_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4810 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/fv_materialization_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/hive_metastore_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1975 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/internal_spark_cluster_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1683 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/materialization_roles_allowlists_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5831 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/materialization_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/odfv_compute_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/onboarding_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/principal_group_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6827 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/remote_compute_environment_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15757 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/remote_spark_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/saved_feature_data_frame_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4545 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/serving_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10895 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/state_update_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4799 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/stream_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/summary_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2349 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/tecton_api_key_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2795 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10456 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/user_deployment_settings_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/user_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3433 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/virtual_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.397793 tecton-0.9.0rc4/tecton_proto/databricks_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/dbfs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/execution_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/instance_profiles_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/jobs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/libraries_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2911 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/permissions_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/scim_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/secrets_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2613 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.397793 tecton-0.9.0rc4/tecton_proto/dataobs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/dataobs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/expectation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/metric_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/validation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3723 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/validation_task_params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/validation_task_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.397793 tecton-0.9.0rc4/tecton_proto/feature_server/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/feature_server/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.397793 tecton-0.9.0rc4/tecton_proto/feature_server/configuration/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/feature_server/configuration/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19997 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9821 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/job_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2610 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/materialization_states_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14634 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/materialization_task_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8173 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2752 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/spark_cluster_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/materializationjobservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/materializationjobservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16111 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/metadataservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/metadataservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/metadataservice/http_over_grpc_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   121489 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/metadataservice/metadata_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/offlinestore/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/offlinestore/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/offlinestore/delta/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/offlinestore/delta/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1570 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/offlinestore/delta/metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6554 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/offlinestore/delta/transaction_writer_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/online_store/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/online_store/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/online_store/feature_value_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/online_store/status_entry_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/online_store_writer/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/online_store_writer/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/online_store_writer/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5522 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/online_store_writer/copier_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/remoteenvironmentservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/remoteenvironmentservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13213 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/secrets/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/secrets/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10485 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/secrets/secrets_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/snowflake/location_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1392 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/snowflake/snowflake_credentials_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/spark_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/spark_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/spark_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7388 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/spark_api/jobs_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/spark_common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/spark_common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7786 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/spark_common/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/spark_common/libraries_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.409794 tecton-0.9.0rc4/tecton_proto/testhelperservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/testhelperservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3516 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/testhelperservice/test_helper_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.409794 tecton-0.9.0rc4/tecton_proto/validation/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/validation/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/validation/validator_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.409794 tecton-0.9.0rc4/tecton_snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30085 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.413794 tecton-0.9.0rc4/tecton_snowflake/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10160 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/dataframe_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13673 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6314 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/queries.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      741 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3704 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8392 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2246 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/snowflake_type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33728 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.417795 tecton-0.9.0rc4/tecton_snowflake/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1025 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/copier_macro.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/create_temp_table_for_bfv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/delete_orphaned_schemas.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/delete_staged_files.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/historical_features_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/materialized_feature_view.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/offline_materialization_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/online_store_copier.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.421795 tecton-0.9.0rc4/tecton_spark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      808 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30278 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/data_observability.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/data_source_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    35476 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/data_source_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/errors_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6470 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/feature_view_spark_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.421795 tecton-0.9.0rc4/tecton_spark/jars/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/jars/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2633 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/jars/class_loader.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)  1794322 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/jars/tecton-udfs-spark-3.jar
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7188 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/materialization_plan.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27440 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15491 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/partial_aggregations.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33278 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.425795 tecton-0.9.0rc4/tecton_spark/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3356 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10751 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/filter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37167 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/join.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1515 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7583 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14752 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/projection.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17887 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5434 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/schema_spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/spark_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1697 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/spark_schema_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4858 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/udf_jar.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/udfs.py
```

### Comparing `tecton-0.9.0rc3/PKG-INFO` & `tecton-0.9.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.9.0rc3
+Version: 0.9.0rc4
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.9.0rc3/README.md` & `tecton-0.9.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/protoc_gen_openapiv2/options/annotations_pb2.py` & `tecton-0.9.0rc4/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `tecton-0.9.0rc4/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/setup.py` & `tecton-0.9.0rc4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     author_email='support@tecton.ai',
     url='https://tecton.ai',
     license='Tecton Proprietary',
     include_package_data=True,
     description='Tecton Python SDK',
     entry_points={'console_scripts': ['tecton=tecton.cli.cli:main'], 'pytest11': ['pytest_tecton=tecton.pytest_tecton']},
     name='tecton',
-    version='0.9.0rc3',
+    version='0.9.0rc4',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos~=1.52', 'jinja2~=3.0', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf>=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas>=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version', 'pyarrow<15,>=8', 'pydantic<3,>=1.10.13', 'pyyaml', 'setuptools', 'pip', 'pex~=2.1'],
     extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'rift': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0'], 'rift-materialization': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0', 'pydantic<2', 'urllib3<1.27'], 'snowflake': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=3.0'], 'materialization': ['statsd==3.3.0', 'urllib3<2.0.0']},
     packages=packages,
 )
```

### Comparing `tecton-0.9.0rc3/tecton/__init__.py` & `tecton-0.9.0rc4/tecton/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/analytics.py` & `tecton-0.9.0rc4/tecton/_internals/analytics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/athena_api.py` & `tecton-0.9.0rc4/tecton/_internals/athena_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/data_frame_helper.py` & `tecton-0.9.0rc4/tecton/_internals/data_frame_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/delete_keys_api.py` & `tecton-0.9.0rc4/tecton/_internals/delete_keys_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/display.py` & `tecton-0.9.0rc4/tecton/_internals/display.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/env_utils.py` & `tecton-0.9.0rc4/tecton/_internals/env_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/errors.py` & `tecton-0.9.0rc4/tecton/_internals/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -316,15 +316,15 @@
             f"Allowed arguments for Transformation '{transformation_name}' are: "
             f"tecton.const, tecton.materialization_context, transformations, and DataSource inputs. Got: '{got}'"
         )
 
 
 # Dataset
 DATASET_SPINE_COLUMNS_NOT_SET = TectonValidationError(
-    "Cannot retrieve spine DF when Dataset was created without a spine."
+    "Cannot retrieve the events dataframe when Dataset was created without one."
 )
 
 UNSUPPORTED_FETCH_AS_PANDAS_AVRO = TectonValidationError(
     "Logged datasets require spark. Please use `to_spark()` to fetch."
 )
 
 
@@ -476,14 +476,18 @@
     "Only DeltaLake is supported for entity deletion in offline feature stores."
 )
 
 FV_UNSUPPORTED_AGGREGATION = TectonValidationError(
     "Argument 'aggregation_level' is not supported for Feature Views with `aggregations` not specified."
 )
 
+RUN_API_PARTIAL_LEVEL_UNSUPPORTED_FOR_COMPACTION = TectonValidationError(
+    "aggregation_level='partial' is only supported for Aggregate Feature Views with Compaction Disabled. Use aggregation_level='full' or aggregation_level='disabled' instead."
+)
+
 
 def INVALID_JOIN_KEY_TYPE(t):
     return TectonValidationError(
         f"Invalid type of join keys '{t}'. Keys must be an instance of [pyspark.sql.dataframe.DataFrame, pandas.DataFrame]."
     )
 
 
@@ -585,14 +589,35 @@
 )
 
 GET_PARTIAL_AGGREGATES_UNSUPPORTED_COMPACTED = TectonValidationError(
     "get_partial_aggregates() is only supported for Aggregate Feature Views with Compaction Disabled."
 )
 
 
+def READ_API_DEPRECATION_TEMPLATE(old_method, new_method):
+    return f"{old_method}() has been deprecated in Tecton 0.9 and will be fully removed in the next major SDK release. Please use {new_method}() instead. See https://docs.tecton.ai/docs/reading-feature-data/reading-feature-data-for-training/offline-retrieval-methods for more information."
+
+
+GET_HISTORICAL_FEATURES_DEPRECATED_SPINE = READ_API_DEPRECATION_TEMPLATE(
+    "get_historical_features", "get_features_for_events"
+)
+
+GET_HISTORICAL_FEATURES_DEPRECATED_TIME_RANGE = READ_API_DEPRECATION_TEMPLATE(
+    "get_historical_features", "get_features_in_range"
+)
+
+RUN_DEPRECATED_TRANSFORMATION = READ_API_DEPRECATION_TEMPLATE("run", "run_transformation")
+
+RUN_DEPRECATED_PARTIAL_AGGS = READ_API_DEPRECATION_TEMPLATE("run", "get_partial_aggregates")
+
+RUN_DEPRECATED_FULL_AGG = READ_API_DEPRECATION_TEMPLATE("run", "get_features_in_range")
+
+GET_SPINE_DF_DEPRECATED = READ_API_DEPRECATION_TEMPLATE("get_spine_dataframe", "get_events_dataframe")
+
+
 class SchemaRequired(TectonValidationError):
     def __init__(self, feature_view_name: str):
         super().__init__(f"The 'schema' parameter for {feature_view_name} must be set.")
 
 
 BUILD_ARGS_INTERNAL_ERROR = TectonInternalError(
     "_build_args() is for internal use only and can only be called on local objects"
```

### Comparing `tecton-0.9.0rc3/tecton/_internals/find_spark.py` & `tecton-0.9.0rc4/tecton/_internals/find_spark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/ingest_utils.py` & `tecton-0.9.0rc4/tecton/_internals/ingest_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/ingestion.py` & `tecton-0.9.0rc4/tecton/_internals/ingestion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/materialization_api.py` & `tecton-0.9.0rc4/tecton/_internals/materialization_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/metadata_service.py` & `tecton-0.9.0rc4/tecton/_internals/metadata_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/metadata_service_impl/request_lib.py` & `tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/request_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/metadata_service_impl/service_modules.py` & `tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/service_modules.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/mock_source_utils.py` & `tecton-0.9.0rc4/tecton/_internals/mock_source_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/offline_store_credentials.py` & `tecton-0.9.0rc4/tecton/_internals/offline_store_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/pandas_compat.py` & `tecton-0.9.0rc4/tecton/_internals/pandas_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/query_helper.py` & `tecton-0.9.0rc4/tecton/_internals/query_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/querytree_api.py` & `tecton-0.9.0rc4/tecton/_internals/querytree_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     feature_set_config: feature_set_config.FeatureSetConfig,
     spine: Union[pyspark_sql.DataFrame, pd.DataFrame, TectonDataFrame, str],
     timestamp_key: Optional[str],
     from_source: Optional[bool],
     save: bool,
     save_as: Optional[str],
 ) -> TectonDataFrame:
+    logger.warning(errors.GET_HISTORICAL_FEATURES_DEPRECATED_SPINE)
+
     timestamp_required = spine is not None and any(
         _should_infer_timestamp_of_spine(fd, timestamp_key) for fd in feature_set_config.feature_definitions
     )
 
     _validate_sql_string_support(dialect, spine)
 
     if timestamp_required:
@@ -272,26 +274,30 @@
     save_as: Optional[str],
     mock_data_sources: Dict[str, pyspark_sql.DataFrame],
 ) -> TectonDataFrame:
     if not feature_definition.is_on_demand:
         check_spark_version(feature_definition.fv_spec.batch_cluster_config)
 
     if spine is not None:
+        logger.warning(errors.GET_HISTORICAL_FEATURES_DEPRECATED_SPINE)
+
         _validate_sql_string_support(dialect, spine)
 
         if _should_infer_timestamp_of_spine(feature_definition, timestamp_key):
             timestamp_key = utils.infer_timestamp(spine)
 
         tecton_spine_df = _create_tecton_df_spine(
             spine_schema=feature_definition.spine_schema, spine=spine, timestamp_key=timestamp_key
         )
         qt = _point_in_time_get_historical_features_for_feature_definition(
             dialect, compute_mode, feature_definition, tecton_spine_df, timestamp_key, from_source
         )
     else:
+        logger.warning(errors.GET_HISTORICAL_FEATURES_DEPRECATED_TIME_RANGE)
+
         if entities is not None:
             if not isinstance(entities, TectonDataFrame):
                 entities = TectonDataFrame._create(entities)
             assert set(entities._dataframe.columns).issubset(
                 set(feature_definition.join_keys)
             ), f"Entities should only contain columns that can be used as Join Keys: {feature_definition.join_keys}"
```

### Comparing `tecton-0.9.0rc3/tecton/_internals/repo/function_serialization.py` & `tecton-0.9.0rc4/tecton/_internals/repo/function_serialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/rewrite.py` & `tecton-0.9.0rc4/tecton/_internals/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/run_api.py` & `tecton-0.9.0rc4/tecton/_internals/run_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,16 +190,14 @@
     compute_mode: ComputeMode,
     fd: FeatureDefinitionWrapper,
     feature_start_time: datetime,
     feature_end_time: datetime,
     mock_data_sources: Dict[str, NodeRef],
     aggregation_level: Optional[str],
 ) -> "tecton.framework.data_frame.DataFrame":
-    aggregation_level = validate_and_get_aggregation_level(fd, aggregation_level)
-
     feature_time_limits_aligned = pendulum.period(feature_start_time, feature_end_time)
 
     qt = _build_run_batch_querytree(
         dialect, compute_mode, fd, feature_end_time, feature_time_limits_aligned, aggregation_level
     )
 
     MockDataRewrite(mock_data_sources).rewrite(qt)
@@ -257,14 +255,21 @@
         else:
             aggregation_level = AGGREGATION_LEVEL_DISABLED
 
     if aggregation_level not in SUPPORTED_AGGREGATION_LEVEL_VALUES:
         msg = "aggregation_level"
         raise errors.FV_INVALID_ARG_VALUE(msg, str(aggregation_level), str(SUPPORTED_AGGREGATION_LEVEL_VALUES))
 
+    if aggregation_level == AGGREGATION_LEVEL_FULL:
+        logger.warning(errors.RUN_DEPRECATED_FULL_AGG)
+    elif aggregation_level == AGGREGATION_LEVEL_DISABLED:
+        logger.warning(errors.RUN_DEPRECATED_TRANSFORMATION)
+    elif aggregation_level == AGGREGATION_LEVEL_PARTIAL:
+        logger.warning(errors.RUN_DEPRECATED_PARTIAL_AGGS)
+
     return aggregation_level
 
 
 # Validate that mock_inputs keys are exact match with expected inputs.
 def validate_ondemand_mock_inputs(
     mock_inputs: Dict[str, Union[Dict[str, Any], pandas.DataFrame]],
     pipeline: pipeline_pb2.Pipeline,
```

### Comparing `tecton-0.9.0rc3/tecton/_internals/sdk_decorators.py` & `tecton-0.9.0rc4/tecton/_internals/sdk_decorators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/secret_resolver.py` & `tecton-0.9.0rc4/tecton/_internals/secret_resolver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/snowflake_api.py` & `tecton-0.9.0rc4/tecton/_internals/snowflake_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/spark_api.py` & `tecton-0.9.0rc4/tecton/_internals/spark_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/spark_utils.py` & `tecton-0.9.0rc4/tecton/_internals/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/tecton_pydantic.py` & `tecton-0.9.0rc4/tecton/_internals/tecton_pydantic.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/time_utils.py` & `tecton-0.9.0rc4/tecton/_internals/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/type_utils.py` & `tecton-0.9.0rc4/tecton/_internals/type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/utils.py` & `tecton-0.9.0rc4/tecton/_internals/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/_internals/validations_api.py` & `tecton-0.9.0rc4/tecton/_internals/validations_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/aggregation_functions.py` & `tecton-0.9.0rc4/tecton/aggregation_functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/access_control.py` & `tecton-0.9.0rc4/tecton/cli/access_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,15 +185,17 @@
         ResourceType.RESOURCE_TYPE_SECRET_SCOPE in r.assignable_on_resource_types for r in role_defs
     ):
         msg = (
             "Tecton Secrets is not enabled on your cluster. "
             + "Currently, Secrets is only available on the Rift platform. Please contact Tecton Support for more assistance."
         )
         raise click.ClickException(msg)
-    role_def = next((r for r in role_defs if r.id == role), None)
+    role_def = next(
+        (r for r in role_defs if r.id == role and _is_role_assignable(r, principal_type, resource_type)), None
+    )
     if role_def is None:
         msg = f"Invalid role. Possible values are: {', '.join(r.id for r in role_defs if _is_role_assignable(r, principal_type, resource_type))}"
         raise click.ClickException(msg)
 
     assignment.resource_type = resource_type
     assignment.principal_type = principal_type
     assignment.principal_id = principal_id
@@ -270,27 +272,28 @@
     group_assignments_by_role: Mapping[str, List[str]]
 
 
 @access_control.command("get-roles")
 @click.option("-u", "--user", default=None, help="User Email")
 @click.option("-s", "--service-account", default=None, help="Service Account ID")
 @click.option("-g", "--principal-group", default=None, help="Principal Group ID")
+@click.option("-w", "--workspace", default=None, help="Workspace Principal Name")
 @click.option(
     "-r",
     "--resource_type",
     default=None,
     type=click.Choice(RESOURCE_TYPES.keys()),
     help="Optional Resource Type to which the Principal has roles assigned.",
 )
 @click.option("--json-out", default=False, is_flag=True, help="Format Output as JSON")
-def get_assigned_roles(user, service_account, principal_group, resource_type, json_out):
+def get_assigned_roles(user, service_account, principal_group, workspace, resource_type, json_out):
     """Get the roles assigned to a principal."""
     if resource_type is not None:
         resource_type = RESOURCE_TYPES[resource_type]
-    principal_type, principal_id = get_principal_details(user, service_account, principal_group, None)
+    principal_type, principal_id = get_principal_details(user, service_account, principal_group, workspace)
 
     role_defs = _get_role_definitions()
 
     ws_roles_response = None
     org_roles_response = None
     try:
         if resource_type is None or resource_type == ResourceType.RESOURCE_TYPE_WORKSPACE:
@@ -374,21 +377,23 @@
         )
         printer.safe_print(json.dumps(json_output, indent=4))
     else:
         _pretty_print_get_roles_output(
             ws_roles=ws_roles,
             org_roles=org_roles,
             scope_roles=scope_roles,
+            show_principal_group_col=workspace is None,
         )
 
 
 @access_control.command("get-principals")
 @click.option("-w", "--workspace", required=False, help="Workspace name")
 @click.option("-c", "--secret-scope", required=False, help="Secret scope name")
 def get_assigned_principals(workspace, secret_scope):
+    """Get principals with access to a resource."""
     if workspace and secret_scope:
         msg = "At most one of --workspace and --secret-scope can be used at the same time."
 
     request = ListAssignedPrincipalsRequest()
     if workspace:
         request.resource_type = ResourceType.RESOURCE_TYPE_WORKSPACE
         request.resource_id = workspace
@@ -488,27 +493,32 @@
     json_output += _convert_assigned_roles_json_generic_resource("SECRET_SCOPE", "name", scope_roles)
     return json_output
 
 
 def _pretty_print_assigned_roles_generic_resource(
     resource_type_for_display: str,
     roles: List[ResourceWithRoleAssignments],
+    show_principal_groups_col: bool,
 ):
     """For generic resources of which there can be many (e.g. workspace, secret scope)"""
-    headings = [resource_type_for_display, "Role", "Assigned Directly", "Assigned via Groups"]
+    headings = [resource_type_for_display, "Role", "Assigned Directly"]
+    if show_principal_groups_col:
+        headings += ["Assigned via Groups"]
     display_rows = []
     for assignment_for_resource in roles:
         resource_name = assignment_for_resource.resource_id
         already_displayed_resource_name = False
         for role in assignment_for_resource.roles_sorted:
             resource_name_to_display = "" if already_displayed_resource_name else resource_name
             already_displayed_resource_name = True
             assigned_directly = "direct" if role in assignment_for_resource.directly_assigned_roles else ""
-            group_names = ", ".join(assignment_for_resource.group_assignments_by_role[role])
-            resource_role_row = (resource_name_to_display, role, assigned_directly, group_names)
+            resource_role_row = (resource_name_to_display, role, assigned_directly)
+            if show_principal_groups_col:
+                group_names = ", ".join(assignment_for_resource.group_assignments_by_role[role])
+                resource_role_row += (group_names,)
 
             display_rows.append(resource_role_row)
     display_table(headings, display_rows)
 
 
 def _pretty_print_assigned_roles_org_resource(
     org_roles: ResourceWithRoleAssignments,
@@ -525,23 +535,24 @@
     display_table(headings, display_rows)
 
 
 def _pretty_print_get_roles_output(
     ws_roles: List[ResourceWithRoleAssignments],
     org_roles: ResourceWithRoleAssignments,
     scope_roles: List[ResourceWithRoleAssignments],
+    show_principal_group_col: bool,
 ):
     if len(ws_roles) > 0:
-        _pretty_print_assigned_roles_generic_resource("Workspace", ws_roles)
+        _pretty_print_assigned_roles_generic_resource("Workspace", ws_roles, True)
         printer.safe_print()
     if len(org_roles.roles_sorted) > 0:
         _pretty_print_assigned_roles_org_resource(org_roles)
         printer.safe_print()
     if len(scope_roles) > 0:
-        _pretty_print_assigned_roles_generic_resource("Secret Scope", scope_roles)
+        _pretty_print_assigned_roles_generic_resource("Secret Scope", scope_roles, show_principal_group_col)
 
 
 def _maybe_convert_legacy_role_id(role_defs, id):
     role_def = next((r for r in role_defs if r.id == id or r.legacy_id == id), None)
     role_id = id if role_def is None else role_def.id
     return role_id
 
@@ -567,9 +578,9 @@
     elif service_account:
         return PrincipalType.PRINCIPAL_TYPE_SERVICE_ACCOUNT, service_account
     elif principal_group:
         return PrincipalType.PRINCIPAL_TYPE_GROUP, principal_group
     elif workspace_principal:
         return PrincipalType.PRINCIPAL_TYPE_WORKSPACE, workspace_principal
     else:
-        msg = "Please mention a Principal Type using --user, --service-account, or --principal-group (or --workspace if using --secret-scope)."
+        msg = "Please mention a Principal Type using --user, --service-account, or --principal-group (or --workspace for workspace authorization on secret scopes)."
         raise click.ClickException(msg)
```

### Comparing `tecton-0.9.0rc3/tecton/cli/api_key.py` & `tecton-0.9.0rc4/tecton/cli/api_key.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/auth.py` & `tecton-0.9.0rc4/tecton/cli/auth.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/cli.py` & `tecton-0.9.0rc4/tecton/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/cli_utils.py` & `tecton-0.9.0rc4/tecton/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/command.py` & `tecton-0.9.0rc4/tecton/cli/command.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/completion.py` & `tecton-0.9.0rc4/tecton/cli/completion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/engine.py` & `tecton-0.9.0rc4/tecton/cli/engine.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/engine_renderer.py` & `tecton-0.9.0rc4/tecton/cli/engine_renderer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/environment.py` & `tecton-0.9.0rc4/tecton/cli/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,16 +166,16 @@
     _python_version = python_version or DEFAULT_PYTHON_VERSION
     on_demand_transform_runtime_version = _on_demand_transform_runtime_version(requirements)
     rift_runtime_version = _rift_materialization_runtime_version(requirements)
     if not on_demand_transform_runtime_version and not rift_runtime_version:
         printer.safe_print(
             f"{ERROR_MESSAGE_PREFIX} Please include these Tecton supporting libraries:\n"
             f"💡  `tecton-runtime` package (https://pypi.org/project/tecton-runtime) to support On Demand Feature Views.\n"
-            f"💡  `tecton[rift]` package (https://pypi.org/project/tecton) to support Rift Batch Feature Views.\n",
-            "💡  `tecton[rift]` and `tecton-runtime` package to support OnDemand Feature Views, Rift Batch Feature Views and Rift Stream Feature Views.\n",
+            f"💡  `tecton[rift-materialization]` package (https://pypi.org/project/tecton) to support Rift Batch Feature Views.\n",
+            "💡  `tecton[rift-materialization]` and `tecton-runtime` package to support OnDemand Feature Views, Rift Batch Feature Views and Rift Stream Feature Views.\n",
             file=sys.stderr,
         )
         sys.exit(1)
 
     with tempfile.TemporaryDirectory() as tmpdir:
         try:
             resolved_requirements_path, _ = _run_dependency_resolution(
@@ -247,15 +247,15 @@
     on_demand_transform_runtime_version = _on_demand_transform_runtime_version(requirements)
     rift_runtime_version = _rift_materialization_runtime_version(requirements)
     if not on_demand_transform_runtime_version and not rift_runtime_version:
         # TODO (vitaly): update the doc link for more information on custom Rift materialization envs
         printer.safe_print(
             f"{ERROR_MESSAGE_PREFIX} Please include at least one of the supporting Tecton libraries:\n"
             f"💡  `tecton-runtime` package (https://pypi.org/project/tecton-runtime) to support On Demand environments\n"
-            f"💡  `tecton[rift]` package (https://pypi.org/project/tecton) to support Rift materialization environments",
+            f"💡  `tecton[rift-materialization]` package (https://pypi.org/project/tecton) to support Rift materialization environments",
             "\nFor more information, please see: https://docs.tecton.ai/docs/defining-features/feature-views/on-demand-feature-view/on-demand-feature-view-environments/custom-on-demand-feature-view-environments",
             file=sys.stderr,
         )
         sys.exit(1)
     else:
         printer.safe_print(
             f"\n💡 Creating environment '{name}' for job types:\n"
@@ -593,23 +593,23 @@
     requirements_path = Path(requirements_path_str)
     try:
         req = get_requirement(
             requirements_path=requirements_path, package_name=TECTON_RIFT_MATERIALIZATION_RUNTIME_PACKAGE
         )
         if req is None:
             return
-        if "rift" not in req.extras:
+        if "rift-materialization" not in req.extras:
             printer.safe_print(
-                f"{ERROR_MESSAGE_PREFIX} `rift` extra must be included to support Rift materialization (tecton[rift]==x.x.x)",
+                f"{ERROR_MESSAGE_PREFIX} `rift-materialization` extra must be included to support Rift materialization (tecton[rift-materialization]==x.x.x)",
                 file=sys.stderr,
             )
             sys.exit(1)
         if not req.specs or req.specs[0][0] != "==":
             printer.safe_print(
-                f"{ERROR_MESSAGE_PREFIX} `tecton[rift]` must be pinned to a version (tecton[rift]==x.x.x)",
+                f"{ERROR_MESSAGE_PREFIX} `tecton[rift-materialization]` must be pinned to a version (tecton[rift-materialization]==x.x.x)",
                 file=sys.stderr,
             )
             sys.exit(1)
         return re.sub(r"\s*--hash=[^ ]+", "", req.specs[0][1])
     except InvalidRequirement:
         printer.safe_print(
             f"{ERROR_MESSAGE_PREFIX} Invalid `requirements` file. Please pass a valid Requirements file formatted according to https://pip.pypa.io/en/stable/reference/requirements-file-format/",
```

### Comparing `tecton-0.9.0rc3/tecton/cli/environment_utils.py` & `tecton-0.9.0rc4/tecton/cli/environment_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/error_utils.py` & `tecton-0.9.0rc4/tecton/cli/error_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/materialization.py` & `tecton-0.9.0rc4/tecton/cli/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/pex_wrapper.py` & `tecton-0.9.0rc4/tecton/cli/pex_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/printer.py` & `tecton-0.9.0rc4/tecton/cli/printer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/repo.py` & `tecton-0.9.0rc4/tecton/cli/repo.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/repo_config.py` & `tecton-0.9.0rc4/tecton/cli/repo_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 
 def create_starter_repo_config(config_path: Path):
     """Create a starter repo config to config_path."""
     sdk_version = version.get_version()
 
     # TODO (TEC-19058): hard-coded pending a process that publishes the environments at the same time as the SDK
-    environment = "tecton-rift-core:0.9" if sdk_version != "99.99.99" else ""
+    environment = "tecton-rift-core-0.9.0" if sdk_version != "99.99.99" else ""
     formatted_start_repo_config = _STARTER_REPO_CONFIG.format(current_version=sdk_version, environment=environment)
 
     with open(config_path, "w") as file:
         file.write(formatted_start_repo_config)
 
 
 def get_default_repo_config_path() -> Path:
```

### Comparing `tecton-0.9.0rc3/tecton/cli/repo_utils.py` & `tecton-0.9.0rc4/tecton/cli/repo_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/secrets.py` & `tecton-0.9.0rc4/tecton/cli/secrets.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,24 +30,25 @@
 @secrets.command("create-scope", requires_auth=True, cls=TectonCommand)
 @click.option("-s", "--scope", default=None, required=True, help="Secret scope name")
 @click_exception_wrapper
 def create_scope(scope):
     """Create a new secret scope."""
     request = CreateSecretScopeRequest(scope=scope)
     response = metadata_service.instance().CreateSecretScope(request)
+    printer.safe_print('Created secret scope "{scope}"')
 
 
 @secrets.command("list-scopes", requires_auth=True, cls=TectonCommand)
 @click_exception_wrapper
 def list_scopes():
     """List secret scopes."""
     request = ListSecretScopesRequest()
     response = metadata_service.instance().ListSecretScopes(request)
 
-    if response.scopes == []:
+    if len(response.scopes) == 0:
         printer.safe_print("No secret scopes found", file=sys.stderr)
     else:
         for scope in response.scopes:
             printer.safe_print(scope.name)
 
 
 @secrets.command("delete-scope", requires_auth=True, cls=TectonCommand)
@@ -69,15 +70,15 @@
 
     try:
         response = metadata_service.instance().ListSecrets(request)
     except TectonNotFoundError as e:
         printer.safe_print("Error: Secret scope not found", file=sys.stderr)
         return
 
-    if response.keys == []:
+    if len(response.keys) == 0:
         printer.safe_print("No secrets found")
     else:
         for key in response.keys:
             printer.safe_print(key.name)
 
 
 @secrets.command("get", requires_auth=True, cls=TectonCommand)
@@ -95,16 +96,23 @@
 @secrets.command("put", requires_auth=True, cls=TectonCommand)
 @click.option("-s", "--scope", default=None, required=True, help="Secret scope name")
 @click.option("-k", "--key", default=None, required=True, help="Secret key")
 @click.option("-f", "--file", default=None, required=False, help="File containing secret value, stdin if not included")
 @click_exception_wrapper
 def put_secret_value(scope, key, file):
     """Put secret value in a scope. Updates if secret already exists."""
-    with open(file, "rt") if file is not None else sys.stdin as f:
-        value = f.readline().strip()
+    if file:
+        with open(file, "rt") as f:
+            value = f.read().rstrip("\n")
+    else:
+        printer.safe_print("File omitted, reading from stdin. Ctrl+D or Ctrl+Z on a new line then Enter to stop.")
+        lines = []
+        for line in sys.stdin:
+            lines.append(line.strip())
+        value = "\n".join(lines)
 
     request = PutSecretValueRequest(scope=scope, key=key, value=value)
     metadata_service.instance().PutSecretValue(request)
 
 
 @secrets.command("delete", requires_auth=True, cls=TectonCommand)
 @click.option("-s", "--scope", default=None, required=True, help="Secret scope name")
```

### Comparing `tecton-0.9.0rc3/tecton/cli/service_account.py` & `tecton-0.9.0rc4/tecton/cli/service_account.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/test.py` & `tecton-0.9.0rc4/tecton/cli/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/user.py` & `tecton-0.9.0rc4/tecton/cli/user.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/workspace.py` & `tecton-0.9.0rc4/tecton/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/cli/workspace_utils.py` & `tecton-0.9.0rc4/tecton/cli/workspace_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/fco_listers.py` & `tecton-0.9.0rc4/tecton/fco_listers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/base_tecton_object.py` & `tecton-0.9.0rc4/tecton/framework/base_tecton_object.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/configs.py` & `tecton-0.9.0rc4/tecton/framework/configs.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/data_frame.py` & `tecton-0.9.0rc4/tecton/framework/data_frame.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/data_source.py` & `tecton-0.9.0rc4/tecton/framework/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/dataset.py` & `tecton-0.9.0rc4/tecton/framework/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,19 @@
         request = ArchiveSavedFeatureDataFrameRequest()
         request.saved_feature_dataframe_id.CopyFrom(IdHelper.from_string(self._id))
         metadata_service.instance().ArchiveSavedFeatureDataFrame(request)
         logger.info(f"Dataset {self.name} deleted")
 
     @sdk_public_method
     def get_spine_dataframe(self) -> TectonDataFrame:
+        logger.warning(errors.GET_SPINE_DF_DEPRECATED)
+        return self.get_events_dataframe()
+
+    @sdk_public_method
+    def get_events_dataframe(self) -> TectonDataFrame:
         """
         Get a :py:class:`tecton.TectonDataFrame` containing the spine.
         """
         if not (self._proto.join_key_column_names and self._proto.timestamp_column_name):
             raise errors.DATASET_SPINE_COLUMNS_NOT_SET
 
         if self._pandas_df is not None:
```

### Comparing `tecton-0.9.0rc3/tecton/framework/entity.py` & `tecton-0.9.0rc4/tecton/framework/entity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/feature_service.py` & `tecton-0.9.0rc4/tecton/framework/feature_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,14 +585,16 @@
                 include_feature_view_timestamp_columns=include_feature_view_timestamp_columns,
                 from_source=from_source,
                 save=save,
                 save_as=save_as,
                 feature_set_config=self._feature_set_config,
             )
 
+        logger.warning(errors.GET_HISTORICAL_FEATURES_DEPRECATED_SPINE)
+
         return querytree_api.get_historical_features_for_feature_service(
             dialect=compute_mode.default_dialect(),
             compute_mode=compute_mode,
             feature_service_spec=self._spec,
             feature_set_config=self._feature_set_config,
             spine=spine,
             timestamp_key=timestamp_key,
```

### Comparing `tecton-0.9.0rc3/tecton/framework/feature_view.py` & `tecton-0.9.0rc4/tecton/framework/feature_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import pandas
 import pendulum
 from google.protobuf import duration_pb2
 from pyspark.sql import dataframe as pyspark_dataframe
 from pyspark.sql import streaming
 from typeguard import typechecked
 
+from tecton import run_api_consts
 from tecton import tecton_context
 from tecton import types
 from tecton._internals import athena_api
 from tecton._internals import delete_keys_api
 from tecton._internals import display
 from tecton._internals import errors
 from tecton._internals import materialization_api
@@ -1375,14 +1376,20 @@
             feature_definition = self._create_unvalidated_feature_definition(resolved_mock_inputs)
         else:
             feature_definition = self._feature_definition
 
         if feature_definition.is_temporal and aggregation_level is not None:
             raise errors.FV_UNSUPPORTED_AGGREGATION
 
+        if (
+            feature_definition.batch_compaction_enabled
+            and aggregation_level == run_api_consts.AGGREGATION_LEVEL_PARTIAL
+        ):
+            raise errors.RUN_API_PARTIAL_LEVEL_UNSUPPORTED_FOR_COMPACTION
+
         aggregation_level = run_api.validate_and_get_aggregation_level(feature_definition, aggregation_level)
 
         run_api.maybe_warn_incorrect_time_range_size(feature_definition, start_time, end_time, aggregation_level)
 
         compute_mode = offline_retrieval_compute_mode(compute_mode)
 
         if compute_mode == ComputeMode.SNOWFLAKE and (
@@ -3516,14 +3523,15 @@
 
             print(result)
             # {'higher_than_average': False}
 
         :return: A `Dict` object for the "python" mode and a tecton DataFrame of the results for the "pandas" mode.
         """
         # Snowflake compute uses the same code for run_ondemand as Spark.
+        logger.warning(errors.RUN_DEPRECATED_TRANSFORMATION)
         return run_api.run_ondemand(self._feature_definition, self.info.name, mock_inputs)
 
     @sdk_decorators.sdk_public_method
     @sdk_decorators.assert_local_object(error_message=errors.CANNOT_USE_LOCAL_RUN_ON_REMOTE_OBJECT)
     def test_run(
         self, **mock_inputs: Union[Dict[str, Any], pandas.DataFrame]
     ) -> Union[Dict[str, Any], pandas.DataFrame]:
```

### Comparing `tecton-0.9.0rc3/tecton/framework/filtered_source.py` & `tecton-0.9.0rc4/tecton/framework/filtered_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/repo_config.py` & `tecton-0.9.0rc4/tecton/framework/repo_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/transformation.py` & `tecton-0.9.0rc4/tecton/framework/transformation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/utils.py` & `tecton-0.9.0rc4/tecton/framework/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/validation_mode.py` & `tecton-0.9.0rc4/tecton/framework/validation_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/framework/workspace.py` & `tecton-0.9.0rc4/tecton/framework/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/identities/api_keys.py` & `tecton-0.9.0rc4/tecton/identities/api_keys.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/identities/credentials.py` & `tecton-0.9.0rc4/tecton/identities/credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/identities/okta.py` & `tecton-0.9.0rc4/tecton/identities/okta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/pytest_tecton.py` & `tecton-0.9.0rc4/tecton/pytest_tecton.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/snowflake_context.py` & `tecton-0.9.0rc4/tecton/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/tecton_context.py` & `tecton-0.9.0rc4/tecton/tecton_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/types.py` & `tecton-0.9.0rc4/tecton/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/__diff.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/__diff.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/_dill.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/_objects.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/_objects.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/detect.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/detect.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/info.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/info.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/objtypes.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/objtypes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/pointers.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/pointers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/settings.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/settings.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/source.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/dill/dill/temp.py` & `tecton-0.9.0rc4/tecton/vendor/dill/dill/temp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/clientserver.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/clientserver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/compat.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/finalizer.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/finalizer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/java_collections.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/java_collections.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/java_gateway.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/protocol.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/protocol.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/py4j/signals.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/signals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/_globals.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/_globals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/accumulators.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/accumulators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/broadcast.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/broadcast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/conf.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/context.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/daemon.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/daemon.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/files.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/files.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/find_spark_home.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/find_spark_home.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/install.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/install.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/java_gateway.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/join.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/base.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/base.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/classification.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/clustering.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/common.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/evaluation.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/feature.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/fpm.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/functions.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/image.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/image.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/param/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/param/shared.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/shared.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/pipeline.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/recommendation.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/regression.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/stat.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/stat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/tree.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/tuning.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/tuning.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/util.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/ml/wrapper.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/classification.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/clustering.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/common.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/evaluation.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/feature.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/fpm.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/random.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/random.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/recommendation.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/regression.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/stat/test.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/tree.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/mllib/util.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/profiler.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/profiler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/rdd.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/rdd.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/rddsampler.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/rddsampler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resource/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resource/information.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/information.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resource/profile.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/profile.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resource/requests.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/requests.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/resultiterable.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resultiterable.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/serializers.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/shell.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/shuffle.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/shuffle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/avro/functions.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/catalog.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/column.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/column.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/conf.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/context.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/dataframe.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/functions.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/group.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/group.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/types.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/readwriter.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/readwriter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/session.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/streaming.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/streaming.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/types.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/udf.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/udf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/utils.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/sql/window.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/window.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/statcounter.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/statcounter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/status.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/storagelevel.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/storagelevel.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/__init__.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/context.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/dstream.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/dstream.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/kinesis.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/kinesis.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/listener.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/listener.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/streaming/util.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/taskcontext.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/taskcontext.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/traceback_utils.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/util.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/pyspark/pyspark/worker.py` & `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/worker.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/vendor_dill.py` & `tecton-0.9.0rc4/tecton/vendor/vendor_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/vendor/vendor_pyspark.py` & `tecton-0.9.0rc4/tecton/vendor/vendor_pyspark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton/version.py` & `tecton-0.9.0rc4/tecton/version.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton.egg-info/PKG-INFO` & `tecton-0.9.0rc4/tecton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.9.0rc3
+Version: 0.9.0rc4
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.9.0rc3/tecton.egg-info/SOURCES.txt` & `tecton-0.9.0rc4/tecton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton.egg-info/requires.txt` & `tecton-0.9.0rc4/tecton.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/athena_session.py` & `tecton-0.9.0rc4/tecton_athena/athena_session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/data_catalog_helper.py` & `tecton-0.9.0rc4/tecton_athena/data_catalog_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/odfv_helper.py` & `tecton-0.9.0rc4/tecton_athena/odfv_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/query/translate.py` & `tecton-0.9.0rc4/tecton_athena/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/sql_helper.py` & `tecton-0.9.0rc4/tecton_athena/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/templates/create_table.sql` & `tecton-0.9.0rc4/tecton_athena/templates/create_table.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/templates/historical_features.sql` & `tecton-0.9.0rc4/tecton_athena/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/templates/materialization_tile.sql` & `tecton-0.9.0rc4/tecton_athena/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/templates/run_full_aggregation.sql` & `tecton-0.9.0rc4/tecton_athena/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/templates/time_limit.sql` & `tecton-0.9.0rc4/tecton_athena/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_athena/templates_utils.py` & `tecton-0.9.0rc4/tecton_athena/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/aggregation_utils.py` & `tecton-0.9.0rc4/tecton_core/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/arrow.py` & `tecton-0.9.0rc4/tecton_core/arrow.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/aws_credentials.py` & `tecton-0.9.0rc4/tecton_core/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/compute_mode.py` & `tecton-0.9.0rc4/tecton_core/compute_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/conf.py` & `tecton-0.9.0rc4/tecton_core/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/data_types.py` & `tecton-0.9.0rc4/tecton_core/data_types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/duckdb_context.py` & `tecton-0.9.0rc4/tecton_core/duckdb_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/errors.py` & `tecton-0.9.0rc4/tecton_core/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/fco_container.py` & `tecton-0.9.0rc4/tecton_core/fco_container.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/feature_definition_wrapper.py` & `tecton-0.9.0rc4/tecton_core/feature_definition_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/feature_set_config.py` & `tecton-0.9.0rc4/tecton_core/feature_set_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/feature_view_utils.py` & `tecton-0.9.0rc4/tecton_core/feature_view_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/function_deserialization.py` & `tecton-0.9.0rc4/tecton_core/function_deserialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/http.py` & `tecton-0.9.0rc4/tecton_core/http.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/id_helper.py` & `tecton-0.9.0rc4/tecton_core/id_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/iterators.py` & `tecton-0.9.0rc4/tecton_core/iterators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/materialization_context.py` & `tecton-0.9.0rc4/tecton_core/materialization_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/metadata_service_impl/error_lib.py` & `tecton-0.9.0rc4/tecton_core/metadata_service_impl/error_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/metadata_service_impl/http_client.py` & `tecton-0.9.0rc4/tecton_core/metadata_service_impl/http_client.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/metadata_service_impl/providers.py` & `tecton-0.9.0rc4/tecton_core/metadata_service_impl/providers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/metadata_service_impl/response.py` & `tecton-0.9.0rc4/tecton_core/metadata_service_impl/response.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/metadata_service_impl/service_calls.py` & `tecton-0.9.0rc4/tecton_core/metadata_service_impl/service_calls.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/offline_store.py` & `tecton-0.9.0rc4/tecton_core/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/online_serving_index.py` & `tecton-0.9.0rc4/tecton_core/online_serving_index.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/pipeline_common.py` & `tecton-0.9.0rc4/tecton_core/pipeline_common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/aggregation_plans.py` & `tecton-0.9.0rc4/tecton_core/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/builder.py` & `tecton-0.9.0rc4/tecton_core/query/builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/compaction_utils.py` & `tecton-0.9.0rc4/tecton_core/query/compaction_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/duckdb/compute.py` & `tecton-0.9.0rc4/tecton_core/query/duckdb/compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/duckdb/nodes.py` & `tecton-0.9.0rc4/tecton_core/query/duckdb/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/duckdb/rewrite.py` & `tecton-0.9.0rc4/tecton_core/query/duckdb/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/errors.py` & `tecton-0.9.0rc4/tecton_core/query/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/executor_params.py` & `tecton-0.9.0rc4/tecton_core/query/executor_params.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/executor_utils.py` & `tecton-0.9.0rc4/tecton_core/query/executor_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/node_interface.py` & `tecton-0.9.0rc4/tecton_core/query/node_interface.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/node_utils.py` & `tecton-0.9.0rc4/tecton_core/query/node_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/nodes.py` & `tecton-0.9.0rc4/tecton_core/query/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/pandas/compute.py` & `tecton-0.9.0rc4/tecton_core/query/pandas/compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/pandas/node.py` & `tecton-0.9.0rc4/tecton_core/query/pandas/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/pandas/nodes.py` & `tecton-0.9.0rc4/tecton_core/query/pandas/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/pandas/pipeline_helper.py` & `tecton-0.9.0rc4/tecton_core/query/pandas/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/pandas/rewrite.py` & `tecton-0.9.0rc4/tecton_core/query/pandas/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/pandas/translate.py` & `tecton-0.9.0rc4/tecton_core/query/pandas/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/pipeline_sql_builder.py` & `tecton-0.9.0rc4/tecton_core/query/pipeline_sql_builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/prefixed_uri_resolver.py` & `tecton-0.9.0rc4/tecton_core/query/prefixed_uri_resolver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/query_tree_compute.py` & `tecton-0.9.0rc4/tecton_core/query/query_tree_compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/query_tree_executor.py` & `tecton-0.9.0rc4/tecton_core/query/query_tree_executor.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/snowflake/compute.py` & `tecton-0.9.0rc4/tecton_core/query/snowflake/compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query/sql_compat.py` & `tecton-0.9.0rc4/tecton_core/query/sql_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/query_consts.py` & `tecton-0.9.0rc4/tecton_core/query_consts.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/repo_file_handler.py` & `tecton-0.9.0rc4/tecton_core/repo_file_handler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/request_context.py` & `tecton-0.9.0rc4/tecton_core/request_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/schema.py` & `tecton-0.9.0rc4/tecton_core/schema.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/schema_derivation_utils.py` & `tecton-0.9.0rc4/tecton_core/schema_derivation_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,19 @@
 
 def compute_batch_table_format(
     feature_view_args: feature_view_pb2.FeatureViewArgs,
     view_schema: schema_pb2.Schema,
 ) -> schema_pb2.OnlineBatchTableFormat:
     aggregations = feature_view_args.materialized_feature_view_args.aggregations
     if aggregations:
-        return _compute_batch_table_schema_for_aggregate_feature_view(view_schema, aggregations)
+        is_continuous = (
+            feature_view_args.materialized_feature_view_args.stream_processing_mode
+            == feature_view_pb2.StreamProcessingMode.STREAM_PROCESSING_MODE_CONTINUOUS
+        )
+        return _compute_batch_table_schema_for_aggregate_feature_view(view_schema, aggregations, is_continuous)
 
     join_keys = specs.get_join_keys_from_feature_view_args(feature_view_args)
     ttl = utils.get_duration_field_or_none(feature_view_args.materialized_feature_view_args, "serving_ttl")
     timestamp_field = specs.resolve_timestamp_field(feature_view_args, view_schema)
     return _compute_batch_table_schema_for_temporal_feature_view(view_schema, join_keys, timestamp_field, ttl)
 
 
@@ -208,14 +212,15 @@
     )
     return schema_pb2.OnlineBatchTableFormat(online_batch_table_parts=[part])
 
 
 def _compute_batch_table_schema_for_aggregate_feature_view(
     view_schema: schema_pb2.Schema,
     aggregations: List[feature_view__args_pb2.FeatureAggregation],
+    is_continuous: bool,
 ) -> schema_pb2.OnlineBatchTableFormat:
     view_schema_column_map = {column.name: column for column in view_schema.columns}
 
     grouped_aggs = defaultdict(list)
 
     # Group by
     for aggregation in aggregations:
@@ -234,17 +239,17 @@
 
     parts = []
 
     for index, (window, sub_aggs) in enumerate(sorted_grouped_aggs):
         added = set()
         columns = []
         for aggregation in sub_aggs:
-            # NOTE: we are intentionally avoiding the special code paths for is_continuous
-            # since they are not a desired pattern long term.
-            aggregation_columns = _get_aggregation_columns(view_schema_column_map, aggregation, is_continuous=False)
+            aggregation_columns = _get_aggregation_columns(
+                view_schema_column_map, aggregation, is_continuous=is_continuous
+            )
             for col in aggregation_columns:
                 if col.name not in added:
                     columns.append(col)
                     added.add(col.name)
 
         output_schema = schema_pb2.Schema(columns=sorted(columns, key=lambda col: col.name))
         part = schema_pb2.OnlineBatchTablePart(
```

### Comparing `tecton-0.9.0rc3/tecton_core/schema_validation.py` & `tecton-0.9.0rc4/tecton_core/schema_validation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/secrets.py` & `tecton-0.9.0rc4/tecton_core/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/snowflake_context.py` & `tecton-0.9.0rc4/tecton_core/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/specs/__init__.py` & `tecton-0.9.0rc4/tecton_core/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/specs/data_source_spec.py` & `tecton-0.9.0rc4/tecton_core/specs/data_source_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/specs/entity_spec.py` & `tecton-0.9.0rc4/tecton_core/specs/entity_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/specs/feature_service_spec.py` & `tecton-0.9.0rc4/tecton_core/specs/feature_service_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/specs/feature_view_spec.py` & `tecton-0.9.0rc4/tecton_core/specs/feature_view_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/specs/tecton_object_spec.py` & `tecton-0.9.0rc4/tecton_core/specs/tecton_object_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/specs/time_window_spec.py` & `tecton-0.9.0rc4/tecton_core/specs/time_window_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/specs/transformation_spec.py` & `tecton-0.9.0rc4/tecton_core/specs/transformation_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/specs/utils.py` & `tecton-0.9.0rc4/tecton_core/specs/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/time_utils.py` & `tecton-0.9.0rc4/tecton_core/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/vendor/queue.py` & `tecton-0.9.0rc4/tecton_core/vendor/queue.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/vendor/treelib/__init__.py` & `tecton-0.9.0rc4/tecton_core/vendor/treelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/vendor/treelib/exceptions.py` & `tecton-0.9.0rc4/tecton_core/vendor/treelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/vendor/treelib/misc.py` & `tecton-0.9.0rc4/tecton_core/vendor/treelib/misc.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/vendor/treelib/node.py` & `tecton-0.9.0rc4/tecton_core/vendor/treelib/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/vendor/treelib/plugins.py` & `tecton-0.9.0rc4/tecton_core/vendor/treelib/plugins.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/vendor/treelib/tree.py` & `tecton-0.9.0rc4/tecton_core/vendor/treelib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_core/vendor/vendor_treelib.py` & `tecton-0.9.0rc4/tecton_core/vendor/vendor_treelib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/__init__.py` & `tecton-0.9.0rc4/tecton_materialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/batch_materialization.py` & `tecton-0.9.0rc4/tecton_materialization/batch_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/common/job_metadata.py` & `tecton-0.9.0rc4/tecton_materialization/common/job_metadata.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/common/job_metadata_aws.py` & `tecton-0.9.0rc4/tecton_materialization/common/job_metadata_aws.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/common/job_metadata_gcp.py` & `tecton-0.9.0rc4/tecton_materialization/common/job_metadata_gcp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/common/task_params.py` & `tecton-0.9.0rc4/tecton_materialization/common/task_params.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/consumption.py` & `tecton-0.9.0rc4/tecton_materialization/consumption.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/delta_maintenance.py` & `tecton-0.9.0rc4/tecton_materialization/delta_maintenance.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/entity_deletion.py` & `tecton-0.9.0rc4/tecton_materialization/entity_deletion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/feature_export.py` & `tecton-0.9.0rc4/tecton_materialization/feature_export.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/ingest_materialization.py` & `tecton-0.9.0rc4/tecton_materialization/ingest_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/job_metadata.py` & `tecton-0.9.0rc4/tecton_materialization/job_metadata.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/materialization.py` & `tecton-0.9.0rc4/tecton_materialization/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/materialization_utils.py` & `tecton-0.9.0rc4/tecton_materialization/materialization_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/ray/batch_materialization.py` & `tecton-0.9.0rc4/tecton_materialization/ray/batch_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/ray/delta.py` & `tecton-0.9.0rc4/tecton_materialization/ray/delta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/ray/feature_export.py` & `tecton-0.9.0rc4/tecton_materialization/ray/feature_export.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/ray/ingest_materialization.py` & `tecton-0.9.0rc4/tecton_materialization/ray/ingest_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/ray/job_status.py` & `tecton-0.9.0rc4/tecton_materialization/ray/job_status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/ray/materialization.py` & `tecton-0.9.0rc4/tecton_materialization/ray/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/ray/materialization_utils.py` & `tecton-0.9.0rc4/tecton_materialization/ray/materialization_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/ray/nodes.py` & `tecton-0.9.0rc4/tecton_materialization/ray/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/remote_host/pyspark_remote_host.py` & `tecton-0.9.0rc4/tecton_materialization/remote_host/pyspark_remote_host.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/secrets.py` & `tecton-0.9.0rc4/tecton_materialization/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_materialization/stream_materialization.py` & `tecton-0.9.0rc4/tecton_materialization/stream_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/amplitude/amplitude_pb2.py` & `tecton-0.9.0rc4/tecton_proto/amplitude/amplitude_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/amplitude/client_logging_pb2.py` & `tecton-0.9.0rc4/tecton_proto/amplitude/client_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/api/featureservice/feature_service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/api/featureservice/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/api/featureservice/feature_service_request_pb2.py` & `tecton-0.9.0rc4/tecton_proto/api/featureservice/feature_service_request_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/basic_info_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/basic_info_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/data_source_config_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/data_source_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/data_source_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/diff_options_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/diff_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/diff_test_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/diff_test_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/entity_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/fco_args_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/fco_args_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/feature_service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/feature_view_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/pipeline_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/repo_metadata_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/repo_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/transformation_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/user_defined_function_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/user_defined_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/version_constraints_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/version_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/args/virtual_data_source_pb2.py` & `tecton-0.9.0rc4/tecton_proto/args/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/auditlog/metadata_pb2.py` & `tecton-0.9.0rc4/tecton_proto/auditlog/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/auth/acl_pb2.py` & `tecton-0.9.0rc4/tecton_proto/auth/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/auth/authorization_service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/auth/authorization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/auth/principal_pb2.py` & `tecton-0.9.0rc4/tecton_proto/auth/principal_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/auth/resource_pb2.py` & `tecton-0.9.0rc4/tecton_proto/auth/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/auth/resource_role_assignments_pb2.py` & `tecton-0.9.0rc4/tecton_proto/auth/resource_role_assignments_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/auth/service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/auth/service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/canary/type_pb2.py` & `tecton-0.9.0rc4/tecton_proto/canary/type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/canary/update_pb2.py` & `tecton-0.9.0rc4/tecton_proto/canary/update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/cli/repo_diff_pb2.py` & `tecton-0.9.0rc4/tecton_proto/cli/repo_diff_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/aggregation_function_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/aggregation_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/analytics_options_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/analytics_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/aws_credentials_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/aws_credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/column_type_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/column_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/compute_mode_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/compute_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/container_image_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/container_image_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/data_source_type_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/data_source_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/data_type_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/fco_locator_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/fco_locator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/framework_version_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/framework_version_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/id_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/id_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/pair_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/schema_container_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/schema_container_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/schema_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/secret_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/spark_schema_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/spark_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/common/time_window_pb2.py` & `tecton-0.9.0rc4/tecton_proto/common/time_window_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/consumption/consumption_pb2.py` & `tecton-0.9.0rc4/tecton_proto/consumption/consumption_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/batch_data_source_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/batch_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/entity_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/fco_metadata_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/fco_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/fco_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/fco_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/feature_service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/feature_store_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/feature_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/feature_view_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/freshness_status_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/freshness_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/fv_materialization_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/fv_materialization_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/hive_metastore_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/hive_metastore_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/internal_spark_cluster_status_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/internal_spark_cluster_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/materialization_roles_allowlists_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/materialization_roles_allowlists_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/materialization_status_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/materialization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/odfv_compute_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/odfv_compute_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/onboarding_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/onboarding_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/principal_group_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/principal_group_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/remote_compute_environment_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/remote_compute_environment_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/remote_spark_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/remote_spark_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/saved_feature_data_frame_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/saved_feature_data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/serving_status_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/serving_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/state_update_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/stream_data_source_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/stream_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/summary_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/tecton_api_key_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/tecton_api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/transformation_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/user_deployment_settings_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/user_deployment_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/user_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/user_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/virtual_data_source_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/data/workspace_pb2.py` & `tecton-0.9.0rc4/tecton_proto/data/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/clusters_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/dbfs_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/dbfs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/error_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/execution_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/instance_profiles_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/instance_profiles_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/jobs_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/libraries_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/permissions_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/permissions_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/scim_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/scim_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/secrets_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/databricks_api/workspace_pb2.py` & `tecton-0.9.0rc4/tecton_proto/databricks_api/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/dataobs/config_pb2.py` & `tecton-0.9.0rc4/tecton_proto/dataobs/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/dataobs/expectation_pb2.py` & `tecton-0.9.0rc4/tecton_proto/dataobs/expectation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/dataobs/metric_pb2.py` & `tecton-0.9.0rc4/tecton_proto/dataobs/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/dataobs/validation_pb2.py` & `tecton-0.9.0rc4/tecton_proto/dataobs/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/dataobs/validation_task_params_pb2.py` & `tecton-0.9.0rc4/tecton_proto/dataobs/validation_task_params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/dataobs/validation_task_pb2.py` & `tecton-0.9.0rc4/tecton_proto/dataobs/validation_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py` & `tecton-0.9.0rc4/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/materialization/job_metadata_pb2.py` & `tecton-0.9.0rc4/tecton_proto/materialization/job_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/materialization/materialization_states_pb2.py` & `tecton-0.9.0rc4/tecton_proto/materialization/materialization_states_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/materialization/materialization_task_pb2.py` & `tecton-0.9.0rc4/tecton_proto/materialization/materialization_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/materialization/params_pb2.py` & `tecton-0.9.0rc4/tecton_proto/materialization/params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/materialization/spark_cluster_pb2.py` & `tecton-0.9.0rc4/tecton_proto/materialization/spark_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/materializationjobservice/materialization_job_service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/materializationjobservice/materialization_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/metadataservice/http_over_grpc_pb2.py` & `tecton-0.9.0rc4/tecton_proto/metadataservice/http_over_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/metadataservice/metadata_service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/metadataservice/metadata_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/offlinestore/delta/metadata_pb2.py` & `tecton-0.9.0rc4/tecton_proto/offlinestore/delta/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/offlinestore/delta/transaction_writer_pb2.py` & `tecton-0.9.0rc4/tecton_proto/offlinestore/delta/transaction_writer_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/online_store/feature_value_pb2.py` & `tecton-0.9.0rc4/tecton_proto/online_store/feature_value_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/online_store/status_entry_pb2.py` & `tecton-0.9.0rc4/tecton_proto/online_store/status_entry_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/online_store_writer/config_pb2.py` & `tecton-0.9.0rc4/tecton_proto/online_store_writer/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/online_store_writer/copier_pb2.py` & `tecton-0.9.0rc4/tecton_proto/online_store_writer/copier_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/secrets/secrets_service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/secrets/secrets_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/snowflake/location_pb2.py` & `tecton-0.9.0rc4/tecton_proto/snowflake/location_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/snowflake/snowflake_credentials_pb2.py` & `tecton-0.9.0rc4/tecton_proto/snowflake/snowflake_credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/spark_api/error_pb2.py` & `tecton-0.9.0rc4/tecton_proto/spark_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/spark_api/jobs_pb2.py` & `tecton-0.9.0rc4/tecton_proto/spark_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/spark_common/clusters_pb2.py` & `tecton-0.9.0rc4/tecton_proto/spark_common/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/spark_common/libraries_pb2.py` & `tecton-0.9.0rc4/tecton_proto/spark_common/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/testhelperservice/test_helper_service_pb2.py` & `tecton-0.9.0rc4/tecton_proto/testhelperservice/test_helper_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_proto/validation/validator_pb2.py` & `tecton-0.9.0rc4/tecton_proto/validation/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/pipeline_helper.py` & `tecton-0.9.0rc4/tecton_snowflake/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/query/aggregation_plans.py` & `tecton-0.9.0rc4/tecton_snowflake/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/query/dataframe_helper.py` & `tecton-0.9.0rc4/tecton_snowflake/query/dataframe_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/query/nodes.py` & `tecton-0.9.0rc4/tecton_snowflake/query/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,19 @@
         :param aggregate_feature: AggregateFeature data proto
         :return: Query
         """
         left_df = self.spine.node._to_query()
         right_df = self.partial_agg_node.node._to_query()
         join_keys = self.fdw.join_keys
         # When calling ghf() with time range, spine only has _ANCHOR_TIME but not time_key
-        timestamp_join_cols = [self.fdw.time_key] if self.fdw.time_key in join_keys else [query_consts.anchor_time()]
+        timestamp_join_cols = (
+            [self.fdw.time_key, query_consts.anchor_time()]
+            if self.fdw.time_key in self.spine.node.columns
+            else [query_consts.anchor_time()]
+        )
         common_cols = join_keys + timestamp_join_cols
 
         output_columns = list(self.spine.node.columns)
 
         left_name = self.spine.name
 
         agg_name = self.partial_agg_node.name
@@ -181,14 +185,15 @@
             afpb.AggregationFunction.AGGREGATION_FUNCTION_LAST_NON_DISTINCT_N,
             afpb.AggregationFunction.AGGREGATION_FUNCTION_FIRST_NON_DISTINCT_N,
         }:
             agg_from = agg_from.lateral(pypika.Field(f"FLATTEN(input=>{names[0]})"))
         # Add the condition that spine time is between partial agg time and partial agg time + window, and run the aggregation function
         agg = (
             agg_from.select(*agg_columns)
+            .distinct()
             .where(pypika.AliasedQuery(left_name)._ANCHOR_TIME >= pypika.AliasedQuery(agg_name)._ANCHOR_TIME)
             .where(pypika.AliasedQuery(left_name)._ANCHOR_TIME < pypika.AliasedQuery(agg_name)._ANCHOR_TIME + window)
             .groupby(*(pypika.AliasedQuery(left_name).field(column) for column in common_cols))
         )
 
         output_feature_name = query_consts.default_case(aggregate_feature.output_feature_name)
         spine_name = left_name + "_" + output_feature_name
```

### Comparing `tecton-0.9.0rc3/tecton_snowflake/query/queries.py` & `tecton-0.9.0rc4/tecton_snowflake/query/queries.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/query/rewrite.py` & `tecton-0.9.0rc4/tecton_snowflake/query/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/query/translate.py` & `tecton-0.9.0rc4/tecton_snowflake/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/schema_derivation_utils.py` & `tecton-0.9.0rc4/tecton_snowflake/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/snowflake_type_utils.py` & `tecton-0.9.0rc4/tecton_snowflake/snowflake_type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/sql_helper.py` & `tecton-0.9.0rc4/tecton_snowflake/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/copier_macro.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/copier_macro.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/delete_orphaned_schemas.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/delete_orphaned_schemas.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/delete_staged_files.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/delete_staged_files.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/historical_features.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/historical_features_macros.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/historical_features_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/materialization_tile.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/materialized_feature_view.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/materialized_feature_view.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/offline_materialization_macros.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/offline_materialization_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/run_full_aggregation.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/run_partial_aggregation.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/run_partial_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates/time_limit.sql` & `tecton-0.9.0rc4/tecton_snowflake/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_snowflake/templates_utils.py` & `tecton-0.9.0rc4/tecton_snowflake/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/__init__.py` & `tecton-0.9.0rc4/tecton_spark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/aggregation_plans.py` & `tecton-0.9.0rc4/tecton_spark/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/data_observability.py` & `tecton-0.9.0rc4/tecton_spark/data_observability.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/data_source_credentials.py` & `tecton-0.9.0rc4/tecton_spark/data_source_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/data_source_helper.py` & `tecton-0.9.0rc4/tecton_spark/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/feature_view_spark_utils.py` & `tecton-0.9.0rc4/tecton_spark/feature_view_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/jars/class_loader.py` & `tecton-0.9.0rc4/tecton_spark/jars/class_loader.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/jars/tecton-udfs-spark-3.jar` & `tecton-0.9.0rc4/tecton_spark/jars/tecton-udfs-spark-3.jar`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/materialization_plan.py` & `tecton-0.9.0rc4/tecton_spark/materialization_plan.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/offline_store.py` & `tecton-0.9.0rc4/tecton_spark/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/partial_aggregations.py` & `tecton-0.9.0rc4/tecton_spark/partial_aggregations.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 aggregation_plan.intermediate_column_names(feature.input_feature_name)
                 if aggregation_plan.intermediate_column_prefixes is not None
                 else [feature.input_feature_name]
             )
             continuous_columns = aggregation_plan.continuous_partial_aggregation_transform(input_columns)
 
             continuous_column_prefixes = get_materialization_aggregation_column_prefixes(
-                feature.function, is_continuous=True
+                feature.function, function_params=feature.function_params, is_continuous=time_aggregation.is_continuous
             )
             continuous_column_names = [
                 f"{column_prefix}_{feature.input_feature_name}" for column_prefix in continuous_column_prefixes
             ]
 
             for column_name, column in zip(continuous_column_names, continuous_columns):
                 if column_name in output_columns:
@@ -257,14 +257,15 @@
 
 def construct_online_partial_agg_v2_df(
     df: pyspark.sql.DataFrame,
     group_by_columns: List[str],
     aggregation_groups: Tuple[compaction_utils.AggregationGroup, ...],
     time_key: str,
     view_schema: Schema,
+    is_continuous: bool = False,
 ) -> pyspark.sql.DataFrame:
     """Constructs a dataframe that performs partial aggregations for online materialization on the input dataframe.
 
     This is built to follow the pattern used for the batch-compacted online store format. It does the aggregations
     specified by the `aggregation_groups`, grouped by the `group_by_columns`. Rows in the input dataframe are already mapped
     to the appropriate aggregation_group via the `AGGREGATION_GROUP_ID` column.
     """
@@ -278,15 +279,15 @@
     for agg_group in aggregation_groups:
         sub_aggs = []
         sub_outputs = set()
 
         for feature in agg_group.aggregate_features:
             col_datatype = view_schema.to_dict()[feature.input_feature_name]
             aggregation_plan = get_aggregation_plan(
-                feature.function, feature.function_params, False, time_key, col_datatype
+                feature.function, feature.function_params, is_continuous, time_key, col_datatype
             )
 
             # partial_aggregation_preprocessor is used by approximate count distinct
             if aggregation_plan.partial_aggregation_preprocessor is not None:
                 intermediate_columns = aggregation_plan.partial_aggregation_preprocessor(feature.input_feature_name)
                 intermediate_column_names = aggregation_plan.intermediate_column_names(feature.input_feature_name)
                 for column, column_name in zip(intermediate_columns, intermediate_column_names):
```

### Comparing `tecton-0.9.0rc3/tecton_spark/pipeline_helper.py` & `tecton-0.9.0rc4/tecton_spark/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/query/data_source.py` & `tecton-0.9.0rc4/tecton_spark/query/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/query/filter.py` & `tecton-0.9.0rc4/tecton_spark/query/filter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/query/join.py` & `tecton-0.9.0rc4/tecton_spark/query/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/query/node.py` & `tecton-0.9.0rc4/tecton_spark/query/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/query/pipeline.py` & `tecton-0.9.0rc4/tecton_spark/query/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     def _to_dataframe(self, spark: pyspark.sql.SparkSession) -> pyspark.sql.DataFrame:
         df = partial_aggregations.construct_online_partial_agg_v2_df(
             self.input_node.to_dataframe(spark),
             [*self.fdw.partial_aggregate_group_by_columns, query_consts.aggregation_group_id()],
             self.aggregation_groups,
             time_key=self.fdw.trailing_time_window_aggregation.time_key,
             view_schema=self.fdw.view_schema,
+            is_continuous=self.fdw.is_continuous,
         )
         return df
 
 
 @attrs.frozen
 class MetricsCollectorSparkNode(SparkExecNode):
     input_node: SparkExecNode
```

### Comparing `tecton-0.9.0rc3/tecton_spark/query/projection.py` & `tecton-0.9.0rc4/tecton_spark/query/projection.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/query/translate.py` & `tecton-0.9.0rc4/tecton_spark/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/schema_derivation_utils.py` & `tecton-0.9.0rc4/tecton_spark/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/schema_spark_utils.py` & `tecton-0.9.0rc4/tecton_spark/schema_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/spark_helper.py` & `tecton-0.9.0rc4/tecton_spark/spark_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/spark_schema_wrapper.py` & `tecton-0.9.0rc4/tecton_spark/spark_schema_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/time_utils.py` & `tecton-0.9.0rc4/tecton_spark/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc3/tecton_spark/udfs.py` & `tecton-0.9.0rc4/tecton_spark/udfs.py`

 * *Files identical despite different names*

