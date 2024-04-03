# Comparing `tmp/truss-0.9.7rc8.tar.gz` & `tmp/truss-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.9.7rc8.tar", max compression
+gzip compressed data, was "truss-0.9.8.tar", max compression
```

## Comparing `truss-0.9.7rc8.tar` & `truss-0.9.8.tar`

### file list

```diff
@@ -1,226 +1,231 @@
--rw-r--r--   0        0        0     5483 2024-03-22 23:12:22.785233 truss-0.9.7rc8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1842 2024-03-22 23:12:22.785233 truss-0.9.7rc8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2024-03-22 23:12:22.785233 truss-0.9.7rc8/LICENSE
--rw-r--r--   0        0        0     5107 2024-03-22 23:12:22.785233 truss-0.9.7rc8/README.md
--rw-r--r--   0        0        0      933 2024-03-22 23:12:22.785233 truss-0.9.7rc8/context_builder.Dockerfile
--rw-r--r--   0        0        0     2654 2024-03-27 14:52:57.744271 truss-0.9.7rc8/pyproject.toml
--rw-r--r--   0        0        0      255 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/__init__.py
--rw-r--r--   0        0        0      252 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0     4518 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/build.py
--rw-r--r--   0        0        0       51 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/cli/__init__.py
--rw-r--r--   0        0        0    17836 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/cli/cli.py
--rw-r--r--   0        0        0      115 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/cli/console.py
--rw-r--r--   0        0        0      134 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/cli/create.py
--rw-r--r--   0        0        0     2747 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/config/trt_llm.py
--rw-r--r--   0        0        0     3254 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/constants.py
--rw-r--r--   0        0        0     7425 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/contexts/image_builder/cache_warmer.py
--rw-r--r--   0        0        0     1456 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0    18319 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     1561 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2120 2024-03-22 23:12:22.801233 truss-0.9.7rc8/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     5711 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/decorators.py
--rw-r--r--   0        0        0     3641 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/docker.py
--rw-r--r--   0        0        0      643 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/errors.py
--rw-r--r--   0        0        0      824 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     3934 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/model_inference.py
--rw-r--r--   0        0        0      510 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/notebook.py
--rw-r--r--   0        0        0    15195 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      139 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/patch/constants.py
--rw-r--r--   0        0        0      908 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2110 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/patch/hash.py
--rw-r--r--   0        0        0     2930 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/patch/local_truss_patch_applier.py
--rw-r--r--   0        0        0      570 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/patch/signature.py
--rw-r--r--   0        0        0     3410 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/patch/truss_dir_patch_applier.py
--rw-r--r--   0        0        0      960 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/patch/types.py
--rw-r--r--   0        0        0      237 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/pytest.ini
--rw-r--r--   0        0        0      705 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/readme_generator.py
--rw-r--r--   0        0        0      176 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/baseten/__init__.py
--rw-r--r--   0        0        0     7198 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/baseten/api.py
--rw-r--r--   0        0        0      752 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/baseten/auth.py
--rw-r--r--   0        0        0     6952 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/baseten/core.py
--rw-r--r--   0        0        0      541 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/baseten/error.py
--rw-r--r--   0        0        0    11775 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/baseten/remote.py
--rw-r--r--   0        0        0     2665 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/baseten/service.py
--rw-r--r--   0        0        0     1951 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/baseten/utils/tar.py
--rw-r--r--   0        0        0      985 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/baseten/utils/transfer.py
--rw-r--r--   0        0        0     1854 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/remote_cli.py
--rw-r--r--   0        0        0     4219 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/remote_factory.py
--rw-r--r--   0        0        0     7474 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/remote/truss_remote.py
--rw-r--r--   0        0        0     2482 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/templates/__init__.py
--rw-r--r--   0        0        0     2275 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     1026 2024-03-27 03:52:29.863327 truss-0.9.7rc8/truss/templates/cache.Dockerfile.jinja
--rw-r--r--   0        0        0       87 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/templates/cache_requirements.txt
--rw-r--r--   0        0        0     3819 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     5397 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      955 2024-03-22 23:12:22.805233 truss-0.9.7rc8/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     6317 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     4245 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2652 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0      998 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/helpers/truss_patch/__init__.py
--rw-r--r--   0        0        0     1842 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
--rw-r--r--   0        0        0     7419 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
--rw-r--r--   0        0        0      551 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
--rw-r--r--   0        0        0      208 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/helpers/truss_patch/system_packages.py
--rw-r--r--   0        0        0     5930 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     2354 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/control/server.py
--rw-r--r--   0        0        0      158 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       98 2024-03-27 03:52:29.863327 truss-0.9.7rc8/truss/templates/copy_cache_files.Dockerfile.jinja
--rw-r--r--   0        0        0       48 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0     1079 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2561 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     2382 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     5758 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/common/schema.py
--rw-r--r--   0        0        0     2340 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/common/termination_handler_middleware.py
--rw-r--r--   0        0        0    14186 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      727 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0    15698 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      263 2024-03-26 22:02:49.952139 truss-0.9.7rc8/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     3196 2024-03-27 03:52:29.863327 truss-0.9.7rc8/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1352 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/shared/logging.py
--rw-r--r--   0        0        0     2163 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0     3318 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/shared/serialization.py
--rw-r--r--   0        0        0     2396 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/shared/util.py
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/trtllm/README.md
--rw-r--r--   0        0        0     3157 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/trtllm/model/model.py
--rw-r--r--   0        0        0     1043 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/trtllm/packages/build_engine_utils.py
--rw-r--r--   0        0        0      387 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/trtllm/packages/constants.py
--rw-r--r--   0        0        0     7447 2024-03-26 22:02:49.952139 truss-0.9.7rc8/truss/templates/trtllm/packages/schema.py
--rw-r--r--   0        0        0     5498 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt
--rw-r--r--   0        0        0     9023 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py
--rw-r--r--   0        0        0     2034 2024-03-22 23:12:22.809233 truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt
--rw-r--r--   0        0        0    10875 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py
--rw-r--r--   0        0        0     2737 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt
--rw-r--r--   0        0        0     4457 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt
--rw-r--r--   0        0        0     4388 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/templates/trtllm/packages/triton_client.py
--rw-r--r--   0        0        0     1378 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/templates/trtllm/packages/utils.py
--rw-r--r--   0        0        0      147 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/annotated_types_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/annotated_types_truss/model/__init__.py
--rw-r--r--   0        0        0      274 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/annotated_types_truss/model/model.py
--rw-r--r--   0        0        0    30286 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0      234 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/gcs_fix/config.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/gcs_fix/model/__init__.py
--rw-r--r--   0        0        0     1079 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/gcs_fix/model/model.py
--rw-r--r--   0        0        0     1394 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0       51 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/model_load_failure_test/config.yaml
--rw-r--r--   0        0        0      552 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/model_load_failure_test/model/model.py
--rw-r--r--   0        0        0     1267 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1566 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0       57 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0       44 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_async_truss/config.yaml
--rw-r--r--   0        0        0      646 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_async_truss/model/model.py
--rw-r--r--   0        0        0      238 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_basic_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_basic_truss/model/__init__.py
--rw-r--r--   0        0        0     1079 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_basic_truss/model/model.py
--rw-r--r--   0        0        0       34 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_concurrency_truss/config.yaml
--rw-r--r--   0        0        0      547 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_concurrency_truss/model/model.py
--rw-r--r--   0        0        0      270 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_pyantic_v1/config.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_pyantic_v1/model/__init__.py
--rw-r--r--   0        0        0      850 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_pyantic_v1/model/model.py
--rw-r--r--   0        0        0       13 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_pyantic_v1/requirements.txt
--rw-r--r--   0        0        0      270 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_pyantic_v2/config.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_pyantic_v2/model/__init__.py
--rw-r--r--   0        0        0      903 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_pyantic_v2/model/model.py
--rw-r--r--   0        0        0       14 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_pyantic_v2/requirements.txt
--rw-r--r--   0        0        0      270 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_requirements_file_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.813233 truss-0.9.7rc8/truss/test_data/test_requirements_file_truss/model/__init__.py
--rw-r--r--   0        0        0     1106 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_requirements_file_truss/model/model.py
--rw-r--r--   0        0        0       13 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_requirements_file_truss/requirements.txt
--rw-r--r--   0        0        0       64 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_streaming_async_generator_truss/config.yaml
--rw-r--r--   0        0        0      521 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_streaming_async_generator_truss/model/model.py
--rw-r--r--   0        0        0      206 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_streaming_read_timeout/config.yaml
--rw-r--r--   0        0        0      636 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_streaming_read_timeout/model/model.py
--rw-r--r--   0        0        0       49 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_streaming_truss/config.yaml
--rw-r--r--   0        0        0      606 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_streaming_truss/model/model.py
--rw-r--r--   0        0        0       59 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_streaming_truss_with_error/config.yaml
--rw-r--r--   0        0        0      673 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_streaming_truss_with_error/model/model.py
--rw-r--r--   0        0        0       38 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        6 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_truss/packages/test_package/test.py
--rw-r--r--   0        0        0      352 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_truss_server_caching_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_truss_server_caching_truss/model/__init__.py
--rw-r--r--   0        0        0      448 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/test_data/test_truss_server_caching_truss/model/model.py
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/__init__.py
--rw-r--r--   0        0        0    17477 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/conftest.py
--rw-r--r--   0        0        0    10496 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      555 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/helpers.py
--rw-r--r--   0        0        0        0 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0    19223 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0     1090 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      715 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0     2604 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/patch/test_truss_dir_patch_applier.py
--rw-r--r--   0        0        0      273 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0     7658 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/remote/baseten/test_api.py
--rw-r--r--   0        0        0      580 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/remote/baseten/test_auth.py
--rw-r--r--   0        0        0     2589 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/remote/baseten/test_core.py
--rw-r--r--   0        0        0     8243 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/remote/baseten/test_remote.py
--rw-r--r--   0        0        0     4626 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/remote/test_remote_factory.py
--rw-r--r--   0        0        0     2475 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/remote/test_truss_remote.py
--rw-r--r--   0        0        0      283 2024-03-22 23:12:22.817233 truss-0.9.7rc8/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     6060 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
--rw-r--r--   0        0        0      964 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
--rw-r--r--   0        0        0     7513 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0     8326 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/control/control/test_server_integration.py
--rw-r--r--   0        0        0     1560 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/core/server/common/test_truss_server.py
--rw-r--r--   0        0        0      821 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2605 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/server/common/test_termination_handler_middleware.py
--rw-r--r--   0        0        0     3131 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     7941 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/templates/server/test_schema.py
--rw-r--r--   0        0        0     1952 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_build.py
--rw-r--r--   0        0        0     9997 2024-03-27 12:56:21.952089 truss-0.9.7rc8/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0    15051 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_control_truss_patching.py
--rw-r--r--   0        0        0      517 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_docker.py
--rw-r--r--   0        0        0    29185 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0    13995 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_model_schema.py
--rw-r--r--   0        0        0     1483 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    28421 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0     1358 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_util.py
--rw-r--r--   0        0        0     1865 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/test_validation.py
--rw-r--r--   0        0        0     7480 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/tests/util/test_path.py
--rw-r--r--   0        0        0    23137 2024-03-27 12:56:21.952089 truss-0.9.7rc8/truss/truss_config.py
--rw-r--r--   0        0        0     2843 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/truss_gatherer.py
--rw-r--r--   0        0        0    37089 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/truss_handle.py
--rw-r--r--   0        0        0     5568 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/truss_spec.py
--rw-r--r--   0        0        0     2729 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/types.py
--rw-r--r--   0        0        0     3110 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/util/.truss_ignore
--rw-r--r--   0        0        0      379 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/util/data_structures.py
--rw-r--r--   0        0        0     2566 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/util/download.py
--rw-r--r--   0        0        0      553 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/util/jinja.py
--rw-r--r--   0        0        0     6183 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/util/path.py
--rw-r--r--   0        0        0     2868 2024-03-22 23:12:22.821233 truss-0.9.7rc8/truss/validation.py
--rw-r--r--   0        0        0     6990 1970-01-01 00:00:00.000000 truss-0.9.7rc8/PKG-INFO
+-rw-r--r--   0        0        0     5483 2024-04-03 15:02:20.047835 truss-0.9.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1842 2024-04-03 15:02:20.047835 truss-0.9.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2024-04-03 15:02:20.047835 truss-0.9.8/LICENSE
+-rw-r--r--   0        0        0     5107 2024-04-03 15:02:20.047835 truss-0.9.8/README.md
+-rw-r--r--   0        0        0      933 2024-04-03 15:02:20.047835 truss-0.9.8/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2651 2024-04-03 15:02:20.055836 truss-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0      255 2024-04-03 15:02:20.055836 truss-0.9.8/truss/__init__.py
+-rw-r--r--   0        0        0      252 2024-04-03 15:02:20.059836 truss-0.9.8/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2024-04-03 15:02:20.059836 truss-0.9.8/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2024-04-03 15:02:20.059836 truss-0.9.8/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0     4518 2024-04-03 15:02:20.059836 truss-0.9.8/truss/build.py
+-rw-r--r--   0        0        0       51 2024-04-03 15:02:20.059836 truss-0.9.8/truss/cli/__init__.py
+-rw-r--r--   0        0        0    17836 2024-04-03 15:02:20.059836 truss-0.9.8/truss/cli/cli.py
+-rw-r--r--   0        0        0      115 2024-04-03 15:02:20.059836 truss-0.9.8/truss/cli/console.py
+-rw-r--r--   0        0        0      134 2024-04-03 15:02:20.059836 truss-0.9.8/truss/cli/create.py
+-rw-r--r--   0        0        0     3096 2024-04-03 15:02:20.059836 truss-0.9.8/truss/config/trt_llm.py
+-rw-r--r--   0        0        0     3259 2024-04-03 15:02:20.059836 truss-0.9.8/truss/constants.py
+-rw-r--r--   0        0        0     7425 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/image_builder/cache_warmer.py
+-rw-r--r--   0        0        0     1456 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0    18184 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     1561 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2120 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     5711 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2024-04-03 15:02:20.059836 truss-0.9.8/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2024-04-03 15:02:20.059836 truss-0.9.8/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2024-04-03 15:02:20.059836 truss-0.9.8/truss/docker.py
+-rw-r--r--   0        0        0      643 2024-04-03 15:02:20.059836 truss-0.9.8/truss/errors.py
+-rw-r--r--   0        0        0      824 2024-04-03 15:02:20.059836 truss-0.9.8/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2024-04-03 15:02:20.059836 truss-0.9.8/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     3934 2024-04-03 15:02:20.059836 truss-0.9.8/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2024-04-03 15:02:20.059836 truss-0.9.8/truss/notebook.py
+-rw-r--r--   0        0        0    15195 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      139 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/constants.py
+-rw-r--r--   0        0        0      908 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2110 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/hash.py
+-rw-r--r--   0        0        0     2930 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/local_truss_patch_applier.py
+-rw-r--r--   0        0        0      570 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/signature.py
+-rw-r--r--   0        0        0     3410 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      960 2024-04-03 15:02:20.059836 truss-0.9.8/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2024-04-03 15:02:20.059836 truss-0.9.8/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2024-04-03 15:02:20.059836 truss-0.9.8/truss/readme_generator.py
+-rw-r--r--   0        0        0      176 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/__init__.py
+-rw-r--r--   0        0        0     7198 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/api.py
+-rw-r--r--   0        0        0      752 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/auth.py
+-rw-r--r--   0        0        0     6952 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/core.py
+-rw-r--r--   0        0        0      541 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/error.py
+-rw-r--r--   0        0        0    11775 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/remote.py
+-rw-r--r--   0        0        0     2665 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/service.py
+-rw-r--r--   0        0        0     1951 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/utils/tar.py
+-rw-r--r--   0        0        0      985 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/baseten/utils/transfer.py
+-rw-r--r--   0        0        0     1854 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/remote_cli.py
+-rw-r--r--   0        0        0     4219 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/remote_factory.py
+-rw-r--r--   0        0        0     7474 2024-04-03 15:02:20.059836 truss-0.9.8/truss/remote/truss_remote.py
+-rw-r--r--   0        0        0     2482 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/__init__.py
+-rw-r--r--   0        0        0     2275 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     1026 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/cache.Dockerfile.jinja
+-rw-r--r--   0        0        0       87 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/cache_requirements.txt
+-rw-r--r--   0        0        0     3819 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     5397 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     6317 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     4245 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2652 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0      998 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/__init__.py
+-rw-r--r--   0        0        0     1842 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
+-rw-r--r--   0        0        0     7419 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
+-rw-r--r--   0        0        0      551 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
+-rw-r--r--   0        0        0      208 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/truss_patch/system_packages.py
+-rw-r--r--   0        0        0     5930 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     2354 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      158 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       98 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/copy_cache_files.Dockerfile.jinja
+-rw-r--r--   0        0        0       48 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2561 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     2382 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     5758 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/schema.py
+-rw-r--r--   0        0        0     2340 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/termination_handler_middleware.py
+-rw-r--r--   0        0        0    14186 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      727 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0    15698 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      263 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     3196 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1352 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/logging.py
+-rw-r--r--   0        0        0     2163 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0     3318 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/serialization.py
+-rw-r--r--   0        0        0     2396 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/shared/util.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/README.md
+-rw-r--r--   0        0        0     4779 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/model/model.py
+-rw-r--r--   0        0        0      860 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/build_engine_utils.py
+-rw-r--r--   0        0        0      387 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/constants.py
+-rw-r--r--   0        0        0     5775 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/schema.py
+-rw-r--r--   0        0        0     5498 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt
+-rw-r--r--   0        0        0     9023 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py
+-rw-r--r--   0        0        0     2034 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt
+-rw-r--r--   0        0        0    10875 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py
+-rw-r--r--   0        0        0     2737 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt
+-rw-r--r--   0        0        0     4457 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt
+-rw-r--r--   0        0        0     4797 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/triton_client.py
+-rw-r--r--   0        0        0     1729 2024-04-03 15:02:20.059836 truss-0.9.8/truss/templates/trtllm/packages/utils.py
+-rw-r--r--   0        0        0      147 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/annotated_types_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/annotated_types_truss/model/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/annotated_types_truss/model/model.py
+-rw-r--r--   0        0        0    30286 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0      234 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/gcs_fix/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.059836 truss-0.9.8/truss/test_data/gcs_fix/model/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/gcs_fix/model/model.py
+-rw-r--r--   0        0        0     1394 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0       51 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1566 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0       57 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0       44 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_async_truss/config.yaml
+-rw-r--r--   0        0        0      646 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_async_truss/model/model.py
+-rw-r--r--   0        0        0      238 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_basic_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_basic_truss/model/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_basic_truss/model/model.py
+-rw-r--r--   0        0        0       34 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_concurrency_truss/config.yaml
+-rw-r--r--   0        0        0      547 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_concurrency_truss/model/model.py
+-rw-r--r--   0        0        0      270 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v1/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v1/model/__init__.py
+-rw-r--r--   0        0        0      850 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v1/model/model.py
+-rw-r--r--   0        0        0       13 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v1/requirements.txt
+-rw-r--r--   0        0        0      270 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v2/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v2/model/__init__.py
+-rw-r--r--   0        0        0      903 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v2/model/model.py
+-rw-r--r--   0        0        0       14 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_pyantic_v2/requirements.txt
+-rw-r--r--   0        0        0      270 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_requirements_file_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_requirements_file_truss/model/__init__.py
+-rw-r--r--   0        0        0     1106 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_requirements_file_truss/model/model.py
+-rw-r--r--   0        0        0       13 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_requirements_file_truss/requirements.txt
+-rw-r--r--   0        0        0       64 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_async_generator_truss/config.yaml
+-rw-r--r--   0        0        0      521 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_async_generator_truss/model/model.py
+-rw-r--r--   0        0        0      206 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_read_timeout/config.yaml
+-rw-r--r--   0        0        0      636 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_read_timeout/model/model.py
+-rw-r--r--   0        0        0       49 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_truss/config.yaml
+-rw-r--r--   0        0        0      606 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_truss/model/model.py
+-rw-r--r--   0        0        0       59 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_truss_with_error/config.yaml
+-rw-r--r--   0        0        0      673 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_streaming_truss_with_error/model/model.py
+-rw-r--r--   0        0        0       38 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        6 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss/packages/test_package/test.py
+-rw-r--r--   0        0        0      352 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss_server_caching_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss_server_caching_truss/model/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/test_truss_server_caching_truss/model/model.py
+-rw-r--r--   0        0        0       67 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/workflow_text_to_num/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/workflow_text_to_num/user_package/__init__.py
+-rw-r--r--   0        0        0      469 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/workflow_text_to_num/user_package/shared_processor.py
+-rw-r--r--   0        0        0     2340 2024-04-03 15:02:20.063835 truss-0.9.8/truss/test_data/workflow_text_to_num/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/__init__.py
+-rw-r--r--   0        0        0    17477 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/conftest.py
+-rw-r--r--   0        0        0    10496 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      555 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0    19223 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0     1090 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      715 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0     2604 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      273 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0     7658 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/baseten/test_api.py
+-rw-r--r--   0        0        0      580 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/baseten/test_auth.py
+-rw-r--r--   0        0        0     2589 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/baseten/test_core.py
+-rw-r--r--   0        0        0     8243 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/baseten/test_remote.py
+-rw-r--r--   0        0        0     4626 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/test_remote_factory.py
+-rw-r--r--   0        0        0     2475 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/remote/test_truss_remote.py
+-rw-r--r--   0        0        0      283 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     6060 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
+-rw-r--r--   0        0        0      964 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
+-rw-r--r--   0        0        0     7513 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0     8326 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/control/control/test_server_integration.py
+-rw-r--r--   0        0        0     1560 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/core/server/common/test_truss_server.py
+-rw-r--r--   0        0        0      821 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2605 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/server/common/test_termination_handler_middleware.py
+-rw-r--r--   0        0        0     3131 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     7941 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/templates/server/test_schema.py
+-rw-r--r--   0        0        0     1952 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_build.py
+-rw-r--r--   0        0        0     9997 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0    15051 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_control_truss_patching.py
+-rw-r--r--   0        0        0      517 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_docker.py
+-rw-r--r--   0        0        0    29185 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0    13995 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_model_schema.py
+-rw-r--r--   0        0        0     1483 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    28421 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0     1358 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_util.py
+-rw-r--r--   0        0        0     1865 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_validation.py
+-rw-r--r--   0        0        0     1748 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/test_workflows.py
+-rw-r--r--   0        0        0     7480 2024-04-03 15:02:20.063835 truss-0.9.8/truss/tests/util/test_path.py
+-rw-r--r--   0        0        0    23145 2024-04-03 15:02:20.063835 truss-0.9.8/truss/truss_config.py
+-rw-r--r--   0        0        0     2843 2024-04-03 15:02:20.063835 truss-0.9.8/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    37089 2024-04-03 15:02:20.063835 truss-0.9.8/truss/truss_handle.py
+-rw-r--r--   0        0        0     5568 2024-04-03 15:02:20.063835 truss-0.9.8/truss/truss_spec.py
+-rw-r--r--   0        0        0     2729 2024-04-03 15:02:20.063835 truss-0.9.8/truss/types.py
+-rw-r--r--   0        0        0     3110 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/.truss_ignore
+-rw-r--r--   0        0        0      379 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/data_structures.py
+-rw-r--r--   0        0        0     2566 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/download.py
+-rw-r--r--   0        0        0      553 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/jinja.py
+-rw-r--r--   0        0        0     6183 2024-04-03 15:02:20.063835 truss-0.9.8/truss/util/path.py
+-rw-r--r--   0        0        0     2868 2024-04-03 15:02:20.063835 truss-0.9.8/truss/validation.py
+-rw-r--r--   0        0        0     6987 1970-01-01 00:00:00.000000 truss-0.9.8/PKG-INFO
```

### Comparing `truss-0.9.7rc8/CODE_OF_CONDUCT.md` & `truss-0.9.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/CONTRIBUTING.md` & `truss-0.9.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/LICENSE` & `truss-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/README.md` & `truss-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/context_builder.Dockerfile` & `truss-0.9.8/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/pyproject.toml` & `truss-0.9.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.9.7rc8"
+version = "0.9.8"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = [
```

### Comparing `truss-0.9.7rc8/truss/blob/blob_backend_registry.py` & `truss-0.9.8/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/blob/http_public_blob_backend.py` & `truss-0.9.8/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/build.py` & `truss-0.9.8/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/cli/cli.py` & `truss-0.9.8/truss/cli/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/config/trt_llm.py` & `truss-0.9.8/truss/config/trt_llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+import json
 import logging
 from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
-class TRTLLMModelArchitecture(Enum):
+class TRTLLMModelArchitecture(str, Enum):
     LLAMA: str = "llama"
     MISTRAL: str = "mistral"
     DEEPSEEK: str = "deepseek"
 
 
-class TRTLLMQuantizationType(Enum):
+class TRTLLMQuantizationType(str, Enum):
     NO_QUANT: str = "no_quant"
     WEIGHTS_ONLY_INT8: str = "weights_int8"
     WEIGHTS_KV_INT8: str = "weights_kv_int8"
     WEIGHTS_ONLY_INT4: str = "weights_int4"
     WEIGHTS_KV_INT4: str = "weights_kv_int4"
     SMOOTH_QUANT: str = "smooth_quant"
     FP8: str = "fp8"
@@ -44,14 +45,20 @@
     quantization_type: TRTLLMQuantizationType = TRTLLMQuantizationType.NO_QUANT
     tensor_parallel_count: int = 1
     pipeline_parallel_count: int = 1
     plugin_configuration: TrussTRTLLMPluginConfiguration = (
         TrussTRTLLMPluginConfiguration()
     )
 
+    class Config:
+        json_encoders = {
+            TRTLLMModelArchitecture: lambda x: x.value,
+            TRTLLMQuantizationType: lambda x: x.value,
+        }
+
 
 class TrussTRTLLMServingConfiguration(BaseModel):
     engine_repository: str
     tokenizer_repository: str
     tensor_parallel_count: int = 1
     pipeline_parallel_count: int = 1
 
@@ -81,7 +88,12 @@
         return self
 
     @property
     def requires_build(self):
         if self.build is not None:
             return True
         return False
+
+    # TODO(Abu): Replace this with model_dump(json=True)
+    # when pydantic v2 is used here
+    def to_json_dict(self):
+        return json.loads(self.json())
```

### Comparing `truss-0.9.7rc8/truss/constants.py` & `truss-0.9.8/truss/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,13 +94,13 @@
 
 INFERENCE_SERVER_PORT = 8080
 
 HTTP_PUBLIC_BLOB_BACKEND = "http_public"
 
 REGISTRY_BUILD_SECRET_PREFIX = "DOCKER_REGISTRY_"
 
-TRTLLM_BASE_IMAGE = "baseten/trtllm-build-server:r23.12_baseten_v0.7.1_20240111"
+TRTLLM_BASE_IMAGE = "baseten/trtllm-build-server:r23.12_baseten_v0.9.0_20240325_dev3"
 BASE_TRTLLM_REQUIREMENTS = [
     "tritonclient[all]==2.42.0",
     "transformers==4.33.1",
     "jinja2==3.1.3",
 ]
```

### Comparing `truss-0.9.7rc8/truss/contexts/image_builder/cache_warmer.py` & `truss-0.9.8/truss/contexts/image_builder/cache_warmer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/contexts/image_builder/image_builder.py` & `truss-0.9.8/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.9.8/truss/contexts/image_builder/serving_image_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     file_is_not_empty,
     to_dotted_python_version,
     truss_base_image_name,
     truss_base_image_tag,
 )
 from truss.contexts.truss_context import TrussContext
 from truss.patch.hash import directory_content_hash
-from truss.truss_config import BaseImage, ModelServer, TrussConfig
+from truss.truss_config import BaseImage, TrussConfig
 from truss.truss_spec import TrussSpec
 from truss.util.jinja import read_template_from_fs
 from truss.util.path import (
     build_truss_target_directory,
     copy_tree_or_file,
     copy_tree_path,
     load_trussignore_patterns,
@@ -327,28 +327,28 @@
             truss_ignore_patterns = load_trussignore_patterns(
                 truss_dir / USER_TRUSS_IGNORE_FILE
             )
 
         # Copy over truss
         copy_tree_path(truss_dir, build_dir, ignore_patterns=truss_ignore_patterns)
         # Copy over template truss for TRT-LLM (we overwrite the model and packages dir)
-        if config.build.model_server is ModelServer.TRT_LLM:
+
+        if config.trt_llm is not None:
             copy_tree_path(TRTLLM_TRUSS_DIR, build_dir, ignore_patterns=[])
 
-            # Check to see if TP and GPU count are the same
-            # TODO(Abu): Consolidate these config parameters so that we don't have to
-            # keep truss + template in sync if we change th einterface
-            if "tensor_parallel_count" in config.build.arguments:
-                if (
-                    config.build.arguments["tensor_parallel_count"]
-                    != config.resources.accelerator.count
-                ):
-                    raise ValueError(
-                        "Tensor parallelism and GPU count must be the same for TRT-LLM"
-                    )
+            tensor_parallel_count = (
+                config.trt_llm.build.tensor_parallel_count  # type: ignore[union-attr]
+                if config.trt_llm.build is not None
+                else config.trt_llm.serve.tensor_parallel_count  # type: ignore[union-attr]
+            )
+
+            if tensor_parallel_count != config.resources.accelerator.count:
+                raise ValueError(
+                    "Tensor parallelism and GPU count must be the same for TRT-LLM"
+                )
 
             config.base_image = BaseImage(
                 image=TRTLLM_BASE_IMAGE, python_executable_path="/usr/bin/python3"
             )
             config.requirements.extend(BASE_TRTLLM_REQUIREMENTS)
 
         # Override config.yml
```

### Comparing `truss-0.9.7rc8/truss/contexts/image_builder/util.py` & `truss-0.9.8/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.9.8/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/contexts/local_loader/load_model_local.py` & `truss-0.9.8/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.9.8/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/contexts/local_loader/utils.py` & `truss-0.9.8/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/docker.py` & `truss-0.9.8/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/errors.py` & `truss-0.9.8/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/local/local_config.py` & `truss-0.9.8/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/local/local_config_handler.py` & `truss-0.9.8/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/model_inference.py` & `truss-0.9.8/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/patch/calc_patch.py` & `truss-0.9.8/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/patch/dir_signature.py` & `truss-0.9.8/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/patch/hash.py` & `truss-0.9.8/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/patch/local_truss_patch_applier.py` & `truss-0.9.8/truss/patch/local_truss_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/patch/signature.py` & `truss-0.9.8/truss/patch/signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/patch/truss_dir_patch_applier.py` & `truss-0.9.8/truss/patch/truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/patch/types.py` & `truss-0.9.8/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/readme_generator.py` & `truss-0.9.8/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/baseten/api.py` & `truss-0.9.8/truss/remote/baseten/api.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/baseten/auth.py` & `truss-0.9.8/truss/remote/baseten/auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/baseten/core.py` & `truss-0.9.8/truss/remote/baseten/core.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/baseten/error.py` & `truss-0.9.8/truss/remote/baseten/error.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/baseten/remote.py` & `truss-0.9.8/truss/remote/baseten/remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/baseten/service.py` & `truss-0.9.8/truss/remote/baseten/service.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/baseten/utils/tar.py` & `truss-0.9.8/truss/remote/baseten/utils/tar.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/baseten/utils/transfer.py` & `truss-0.9.8/truss/remote/baseten/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/remote_cli.py` & `truss-0.9.8/truss/remote/remote_cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/remote_factory.py` & `truss-0.9.8/truss/remote/remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/remote/truss_remote.py` & `truss-0.9.8/truss/remote/truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/README.md.jinja` & `truss-0.9.8/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/base.Dockerfile.jinja` & `truss-0.9.8/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/cache.Dockerfile.jinja` & `truss-0.9.8/truss/templates/cache.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/application.py` & `truss-0.9.8/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/endpoints.py` & `truss-0.9.8/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/helpers/errors.py` & `truss-0.9.8/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.9.8/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.9.8/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.9.8/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/helpers/truss_patch/__init__.py` & `truss-0.9.8/truss/templates/control/control/helpers/truss_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py` & `truss-0.9.8/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py` & `truss-0.9.8/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py` & `truss-0.9.8/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/helpers/types.py` & `truss-0.9.8/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/control/control/server.py` & `truss-0.9.8/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/custom/model/model.py` & `truss-0.9.8/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server/common/errors.py` & `truss-0.9.8/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.9.8/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server/common/patches.py` & `truss-0.9.8/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server/common/retry.py` & `truss-0.9.8/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server/common/schema.py` & `truss-0.9.8/truss/templates/server/common/schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server/common/termination_handler_middleware.py` & `truss-0.9.8/truss/templates/server/common/termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server/common/truss_server.py` & `truss-0.9.8/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server/inference_server.py` & `truss-0.9.8/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server/model_wrapper.py` & `truss-0.9.8/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/server.Dockerfile.jinja` & `truss-0.9.8/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/shared/logging.py` & `truss-0.9.8/truss/templates/shared/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/shared/secrets_resolver.py` & `truss-0.9.8/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/shared/serialization.py` & `truss-0.9.8/truss/templates/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/shared/util.py` & `truss-0.9.8/truss/templates/shared/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt` & `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py` & `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt` & `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py` & `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt` & `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt` & `truss-0.9.8/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/templates/trtllm/packages/triton_client.py` & `truss-0.9.8/truss/templates/trtllm/packages/triton_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import shutil
 import subprocess
 import time
 from pathlib import Path
 from typing import AsyncGenerator, Optional
 
 import tritonclient.grpc.aio as grpcclient
 import tritonclient.http as httpclient
@@ -25,24 +26,31 @@
     def create_model_repository(
         self,
         truss_data_dir: Path,
         engine_repository_path: Optional[str] = None,
         huggingface_auth_token: Optional[str] = None,
     ) -> None:
         if engine_repository_path:
-            download_engine(
-                engine_repository=engine_repository_path,
-                fp=truss_data_dir,
-                auth_token=huggingface_auth_token,
-            )
+            if Path(engine_repository_path).is_dir():
+                if str(engine_repository_path) != str(truss_data_dir):
+                    shutil.copytree(
+                        engine_repository_path, truss_data_dir, dirs_exist_ok=True
+                    )
+            else:
+                # If engine_repository_path is not a local directory, download the engine
+                download_engine(
+                    engine_repository=engine_repository_path,
+                    fp=truss_data_dir,
+                    auth_token=huggingface_auth_token,
+                )
+
         prepare_model_repository(truss_data_dir)
         return
 
     def start(self, world_size: int = 1, env: dict = {}) -> None:
-
         mpirun_command = ["mpirun", "--allow-run-as-root"]
         mpi_commands = []
         for i in range(world_size):
             mpi_command = [
                 "-n",
                 "1",
                 "tritonserver",
```

### Comparing `truss-0.9.7rc8/truss/templates/trtllm/packages/utils.py` & `truss-0.9.8/truss/templates/trtllm/packages/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import subprocess
 from pathlib import Path
 
 from constants import TENSORRT_LLM_MODEL_REPOSITORY_PATH
 from huggingface_hub import snapshot_download
 
 
 def move_all_files(src: Path, dest: Path) -> None:
@@ -37,7 +38,20 @@
     snapshot_download(
         engine_repository,
         local_dir=fp,
         local_dir_use_symlinks=False,
         max_workers=4,
         **({"use_auth_token": auth_token} if auth_token is not None else {}),
     )
+
+
+def execute_command(command):
+    process = subprocess.Popen(
+        command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, text=True
+    )
+
+    for line in process.stdout:
+        print(line.strip())
+
+    return_code = process.wait()
+    if return_code != 0:
+        raise subprocess.CalledProcessError(return_code, command)
```

### Comparing `truss-0.9.7rc8/truss/test_data/auto-mpg.data` & `truss-0.9.8/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/gcs_fix/model/model.py` & `truss-0.9.8/truss/test_data/gcs_fix/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/happy.ipynb` & `truss-0.9.8/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/model_load_failure_test/model/model.py` & `truss-0.9.8/truss/test_data/model_load_failure_test/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/patch_ping_test_server/app.py` & `truss-0.9.8/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/pima-indians-diabetes.csv` & `truss-0.9.8/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/readme_int_example.md` & `truss-0.9.8/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/readme_no_example.md` & `truss-0.9.8/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/readme_str_example.md` & `truss-0.9.8/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/server.Dockerfile` & `truss-0.9.8/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.9.8/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_async_truss/model/model.py` & `truss-0.9.8/truss/test_data/test_async_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_basic_truss/model/model.py` & `truss-0.9.8/truss/test_data/test_basic_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_concurrency_truss/model/model.py` & `truss-0.9.8/truss/test_data/test_concurrency_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_pyantic_v1/model/model.py` & `truss-0.9.8/truss/test_data/test_pyantic_v1/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_pyantic_v2/model/model.py` & `truss-0.9.8/truss/test_data/test_pyantic_v2/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_requirements_file_truss/model/model.py` & `truss-0.9.8/truss/test_data/test_requirements_file_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_streaming_async_generator_truss/model/model.py` & `truss-0.9.8/truss/test_data/test_streaming_async_generator_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_streaming_read_timeout/model/model.py` & `truss-0.9.8/truss/test_data/test_streaming_read_timeout/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_streaming_truss/model/model.py` & `truss-0.9.8/truss/test_data/test_streaming_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_streaming_truss_with_error/model/model.py` & `truss-0.9.8/truss/test_data/test_streaming_truss_with_error/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/test_data/test_truss/model/model.py` & `truss-0.9.8/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/conftest.py` & `truss-0.9.8/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.9.8/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.9.8/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.9.8/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/helpers.py` & `truss-0.9.8/truss/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/local/test_local_config_handler.py` & `truss-0.9.8/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/patch/test_calc_patch.py` & `truss-0.9.8/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/patch/test_dir_signature.py` & `truss-0.9.8/truss/tests/patch/test_dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/patch/test_hash.py` & `truss-0.9.8/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/patch/test_signature.py` & `truss-0.9.8/truss/tests/patch/test_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/patch/test_truss_dir_patch_applier.py` & `truss-0.9.8/truss/tests/patch/test_truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/remote/baseten/test_api.py` & `truss-0.9.8/truss/tests/remote/baseten/test_api.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/remote/baseten/test_auth.py` & `truss-0.9.8/truss/tests/remote/baseten/test_auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/remote/baseten/test_core.py` & `truss-0.9.8/truss/tests/remote/baseten/test_core.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/remote/baseten/test_remote.py` & `truss-0.9.8/truss/tests/remote/baseten/test_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/remote/test_remote_factory.py` & `truss-0.9.8/truss/tests/remote/test_remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/remote/test_truss_remote.py` & `truss-0.9.8/truss/tests/remote/test_truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py` & `truss-0.9.8/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py` & `truss-0.9.8/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/control/control/test_server.py` & `truss-0.9.8/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/control/control/test_server_integration.py` & `truss-0.9.8/truss/tests/templates/control/control/test_server_integration.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/core/server/common/test_truss_server.py` & `truss-0.9.8/truss/tests/templates/core/server/common/test_truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/core/server/common/test_util.py` & `truss-0.9.8/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.9.8/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/server/common/test_retry.py` & `truss-0.9.8/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/server/common/test_termination_handler_middleware.py` & `truss-0.9.8/truss/tests/templates/server/common/test_termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.9.8/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/templates/server/test_schema.py` & `truss-0.9.8/truss/tests/templates/server/test_schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_build.py` & `truss-0.9.8/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_config.py` & `truss-0.9.8/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_context_builder_image.py` & `truss-0.9.8/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_control_truss_patching.py` & `truss-0.9.8/truss/tests/test_control_truss_patching.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_docker.py` & `truss-0.9.8/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_model_inference.py` & `truss-0.9.8/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_model_schema.py` & `truss-0.9.8/truss/tests/test_model_schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.9.8/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_truss_gatherer.py` & `truss-0.9.8/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_truss_handle.py` & `truss-0.9.8/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_util.py` & `truss-0.9.8/truss/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/test_validation.py` & `truss-0.9.8/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/tests/util/test_path.py` & `truss-0.9.8/truss/tests/util/test_path.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/truss_config.py` & `truss-0.9.8/truss/truss_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,15 @@
                 )
             elif isinstance(field_curr_value, ModelCache):
                 d["model_cache"] = transform_optional(
                     field_curr_value, lambda data: data.to_list(verbose=verbose)
                 )
             elif isinstance(field_curr_value, TRTLLMConfiguration):
                 d["trt_llm"] = transform_optional(
-                    field_curr_value, lambda data: data.dict()
+                    field_curr_value, lambda data: data.to_json_dict()
                 )
             elif isinstance(field_curr_value, BaseImage):
                 d["base_image"] = transform_optional(
                     field_curr_value, lambda data: data.to_dict()
                 )
             elif isinstance(field_curr_value, DockerAuthSettings):
                 d["docker_auth"] = transform_optional(
```

### Comparing `truss-0.9.7rc8/truss/truss_gatherer.py` & `truss-0.9.8/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/truss_handle.py` & `truss-0.9.8/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/truss_spec.py` & `truss-0.9.8/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/types.py` & `truss-0.9.8/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/util/.truss_ignore` & `truss-0.9.8/truss/util/.truss_ignore`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/util/download.py` & `truss-0.9.8/truss/util/download.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/util/gpu.py` & `truss-0.9.8/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/util/path.py` & `truss-0.9.8/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/truss/validation.py` & `truss-0.9.8/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.7rc8/PKG-INFO` & `truss-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.9.7rc8
+Version: 0.9.8
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
```

