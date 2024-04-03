# Comparing `tmp/nerfstudio-1.0.2.tar.gz` & `tmp/nerfstudio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfstudio-1.0.2.tar", last modified: Thu Feb 22 20:59:27 2024, max compression
+gzip compressed data, was "nerfstudio-1.0.3.tar", last modified: Wed Apr  3 01:25:34 2024, max compression
```

## Comparing `nerfstudio-1.0.2.tar` & `nerfstudio-1.0.3.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.839305 nerfstudio-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23708 2024-02-22 20:59:27.839305 nerfstudio-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20055 2024-02-22 20:59:22.000000 nerfstudio-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.799305 nerfstudio-1.0.2/nerfstudio/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.803305 nerfstudio-1.0.2/nerfstudio/cameras/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/cameras/camera_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/cameras/camera_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    32815 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/cameras/camera_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    50983 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/cameras/cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/cameras/lie_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/cameras/rays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.803305 nerfstudio-1.0.2/nerfstudio/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/configs/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/configs/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/configs/dataparser_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/configs/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/configs/external_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    25998 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/configs/method_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.803305 nerfstudio-1.0.2/nerfstudio/data/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.807305 nerfstudio-1.0.2/nerfstudio/data/datamanagers/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datamanagers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datamanagers/base_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22118 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datamanagers/full_images_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15085 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datamanagers/parallel_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datamanagers/random_cameras_datamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.807305 nerfstudio-1.0.2/nerfstudio/data/dataparsers/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/base_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/blender_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    26907 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/colmap_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/dnerf_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/dycheck_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/minimal_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/nerfosr_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    21922 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/nuscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/phototourism_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/scannet_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/scannetpp_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.811305 nerfstudio-1.0.2/nerfstudio/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datasets/depth_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datasets/sdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/datasets/semantic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    21620 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/pixel_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/scene_box.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.811305 nerfstudio-1.0.2/nerfstudio/data/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20474 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/utils/colmap_parsing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/utils/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/utils/dataparsers_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/utils/nerfstudio_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/data/utils/pixel_sampling_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.811305 nerfstudio-1.0.2/nerfstudio/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/engine/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/engine/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/engine/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24265 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.811305 nerfstudio-1.0.2/nerfstudio/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14319 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/exporter/exporter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/exporter/marching_cubes.py
--rw-r--r--   0 runner    (1001) docker     (127)    21099 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/exporter/texture_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/exporter/tsdf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.815305 nerfstudio-1.0.2/nerfstudio/field_components/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/field_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/field_components/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/field_components/base_field_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/field_components/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    32841 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/field_components/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/field_components/field_heads.py
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/field_components/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/field_components/spatial_distortions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/field_components/temporal_distortions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.815305 nerfstudio-1.0.2/nerfstudio/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/base_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/density_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/generfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/nerfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/nerfw_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18116 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/sdf_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/semantic_nerf_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/tensorf_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/fields/vanilla_nerf_field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.815305 nerfstudio-1.0.2/nerfstudio/generative/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/generative/deepfloyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/generative/positional_text_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/generative/stable_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.815305 nerfstudio-1.0.2/nerfstudio/model_components/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/model_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22329 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/model_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/model_components/ray_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)    29334 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/model_components/ray_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/model_components/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/model_components/scene_colliders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/model_components/shaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.819305 nerfstudio-1.0.2/nerfstudio/models/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/base_surface_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/depth_nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/generfacto.py
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/instant_ngp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/mipnerf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19375 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/neus.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/neus_facto.py
--rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/semantic_nerfw.py
--rw-r--r--   0 runner    (1001) docker     (127)    40844 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/splatfacto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15818 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/tensorf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/models/vanilla_nerf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.819305 nerfstudio-1.0.2/nerfstudio/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/pipelines/base_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/pipelines/dynamic_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.819305 nerfstudio-1.0.2/nerfstudio/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/plugins/registry_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/plugins/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.823305 nerfstudio-1.0.2/nerfstudio/process_data/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27598 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/colmap_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/equirect_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/hloc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/images_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/metashape_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/odm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/polycam_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25483 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/process_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/realitycapture_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/record3d_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/process_data/video_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.823305 nerfstudio-1.0.2/nerfstudio/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.823305 nerfstudio-1.0.2/nerfstudio/scripts/blender/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/blender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17246 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/blender/nerfstudio_blender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.823305 nerfstudio-1.0.2/nerfstudio/scripts/completions/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/completions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/completions/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/completions/setup.bash
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/completions/setup.zsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.823305 nerfstudio-1.0.2/nerfstudio/scripts/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/datasets/process_nuscenes_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/datasets/process_project_aria.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.827305 nerfstudio-1.0.2/nerfstudio/scripts/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/docs/add_nb_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/docs/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.827305 nerfstudio-1.0.2/nerfstudio/scripts/downloads/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/downloads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24960 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/downloads/download_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/downloads/eyeful_tower.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/downloads/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    24456 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.827305 nerfstudio-1.0.2/nerfstudio/scripts/github/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/github/run_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21495 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/process_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    41704 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/texture.py
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.827305 nerfstudio-1.0.2/nerfstudio/scripts/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/viewer/run_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/scripts/viewer/sync_viser_message_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.831305 nerfstudio-1.0.2/nerfstudio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/comms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/install_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    18643 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16909 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/plotly_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/poses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/tensor_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)    18988 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/utils/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.831305 nerfstudio-1.0.2/nerfstudio/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/export_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    46795 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/render_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/render_state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.831305 nerfstudio-1.0.2/nerfstudio/viewer/server/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/server/viewer_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24095 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer/viewer_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.831305 nerfstudio-1.0.2/nerfstudio/viewer_legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.831305 nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.831305 nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/public/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/run_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.799305 nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.831305 nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/src/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/src/themes/leva_theme.json
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.835305 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/render_state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.835305 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/state/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/state/state_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18868 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/viewer_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    19998 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/viewer_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/viewer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.835305 nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/message_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.835305 nerfstudio-1.0.2/nerfstudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23708 2024-02-22 20:59:27.000000 nerfstudio-1.0.2/nerfstudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-02-22 20:59:27.000000 nerfstudio-1.0.2/nerfstudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 20:59:27.000000 nerfstudio-1.0.2/nerfstudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-22 20:59:27.000000 nerfstudio-1.0.2/nerfstudio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-02-22 20:59:27.000000 nerfstudio-1.0.2/nerfstudio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-22 20:59:27.000000 nerfstudio-1.0.2/nerfstudio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 20:59:27.839305 nerfstudio-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:59:27.835305 nerfstudio-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-02-22 20:59:16.000000 nerfstudio-1.0.2/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.643997 nerfstudio-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23709 2024-04-03 01:25:34.643997 nerfstudio-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20055 2024-04-03 01:25:32.000000 nerfstudio-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.599997 nerfstudio-1.0.3/nerfstudio/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.603997 nerfstudio-1.0.3/nerfstudio/cameras/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/camera_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/camera_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33058 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/camera_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50983 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/lie_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/rays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.603997 nerfstudio-1.0.3/nerfstudio/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/dataparser_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/external_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27707 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/method_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.603997 nerfstudio-1.0.3/nerfstudio/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.607997 nerfstudio-1.0.3/nerfstudio/data/datamanagers/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/base_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/full_images_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15085 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/parallel_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/random_cameras_datamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.607997 nerfstudio-1.0.3/nerfstudio/data/dataparsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/base_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/blender_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26907 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/colmap_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/dnerf_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/dycheck_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/minimal_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/nerfosr_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21922 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/nuscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/phototourism_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/scannet_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/scannetpp_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.611997 nerfstudio-1.0.3/nerfstudio/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/depth_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/sdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/semantic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23230 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/pixel_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/scene_box.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.611997 nerfstudio-1.0.3/nerfstudio/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20474 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/colmap_parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/dataparsers_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/nerfstudio_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/pixel_sampling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.611997 nerfstudio-1.0.3/nerfstudio/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24265 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.611997 nerfstudio-1.0.3/nerfstudio/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14319 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/exporter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/marching_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21099 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/texture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/tsdf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.615997 nerfstudio-1.0.3/nerfstudio/field_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/base_field_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32841 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/field_heads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/spatial_distortions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/temporal_distortions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.615997 nerfstudio-1.0.3/nerfstudio/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/base_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/density_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/generfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/nerfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/nerfw_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18116 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/sdf_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/semantic_nerf_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/tensorf_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/vanilla_nerf_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.615997 nerfstudio-1.0.3/nerfstudio/generative/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/generative/deepfloyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/generative/positional_text_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/generative/stable_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.619997 nerfstudio-1.0.3/nerfstudio/model_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22329 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/ray_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29334 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/ray_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/scene_colliders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/shaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.619997 nerfstudio-1.0.3/nerfstudio/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/base_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/depth_nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/generfacto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/instant_ngp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/mipnerf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19375 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/neus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/neus_facto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/semantic_nerfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39464 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/splatfacto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/tensorf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/vanilla_nerf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.619997 nerfstudio-1.0.3/nerfstudio/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/pipelines/base_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/pipelines/dynamic_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.623997 nerfstudio-1.0.3/nerfstudio/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/plugins/registry_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/plugins/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.623997 nerfstudio-1.0.3/nerfstudio/process_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27598 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/colmap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/equirect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/hloc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/images_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/metashape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/odm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/polycam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25630 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/process_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/realitycapture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/record3d_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/video_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.623997 nerfstudio-1.0.3/nerfstudio/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.623997 nerfstudio-1.0.3/nerfstudio/scripts/blender/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/blender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17246 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/blender/nerfstudio_blender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/completions/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/completions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/completions/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/completions/setup.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/completions/setup.zsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/datasets/process_nuscenes_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/datasets/process_project_aria.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/docs/add_nb_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/docs/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/downloads/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/downloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24960 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/downloads/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/downloads/eyeful_tower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/downloads/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26818 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/github/run_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21495 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41704 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/viewer/run_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/viewer/sync_viser_message_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.631997 nerfstudio-1.0.3/nerfstudio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/comms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/install_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18643 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16909 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/plotly_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/tensor_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18988 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.631997 nerfstudio-1.0.3/nerfstudio/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/export_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46800 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/render_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/render_state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.631997 nerfstudio-1.0.3/nerfstudio/viewer/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/server/viewer_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24095 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24037 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/viewer_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.631997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/public/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/run_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.599997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/src/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/src/themes/leva_theme.json
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/render_state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/state_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18868 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19998 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/message_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23709 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:25:34.643997 nerfstudio-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/tests/test_train.py
```

### Comparing `nerfstudio-1.0.2/LICENSE` & `nerfstudio-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/PKG-INFO` & `nerfstudio-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 1.0.2
+Version: 1.0.3
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: mediapy>=1.1.0
 Requires-Dist: msgpack>=1.0.4
 Requires-Dist: msgpack_numpy>=0.4.8
 Requires-Dist: nerfacc==0.5.2
 Requires-Dist: open3d>=0.16.0
 Requires-Dist: opencv-python==4.8.0.76
-Requires-Dist: Pillow>=9.3.0
+Requires-Dist: Pillow>=10.3.0
 Requires-Dist: plotly>=5.7.0
 Requires-Dist: protobuf!=3.20.0,<=3.20.3
 Requires-Dist: pymeshlab>=2022.2.post2; platform_machine != "arm64" and platform_machine != "aarch64"
 Requires-Dist: pyngrok>=5.1.0
 Requires-Dist: python-socketio>=5.7.1
 Requires-Dist: pyquaternion>=0.9.9
 Requires-Dist: rawpy>=0.18.1; platform_machine != "arm64"
@@ -44,21 +44,21 @@
 Requires-Dist: scikit-image>=0.19.3
 Requires-Dist: splines==0.3.0
 Requires-Dist: tensorboard>=2.13.0
 Requires-Dist: torch>=1.13.1
 Requires-Dist: torchvision>=0.14.1
 Requires-Dist: torchmetrics[image]>=1.0.1
 Requires-Dist: typing_extensions>=4.4.0
-Requires-Dist: viser==0.1.21
+Requires-Dist: viser==0.1.26
 Requires-Dist: nuscenes-devkit>=1.1.1
 Requires-Dist: wandb>=0.13.3
 Requires-Dist: xatlas
 Requires-Dist: trimesh>=3.20.2
 Requires-Dist: timm==0.6.7
-Requires-Dist: gsplat>=0.1.6
+Requires-Dist: gsplat>=0.1.9
 Requires-Dist: pytorch-msssim
 Requires-Dist: pathos
 Requires-Dist: packaging
 Provides-Extra: gen
 Requires-Dist: diffusers==0.16.1; extra == "gen"
 Requires-Dist: transformers==4.29.2; extra == "gen"
 Requires-Dist: accelerate==0.19.0; extra == "gen"
@@ -80,15 +80,15 @@
 Requires-Dist: torch<2.2,>=1.13.1; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: furo==2022.09.29; extra == "docs"
 Requires-Dist: ipython==8.6.0; extra == "docs"
 Requires-Dist: readthedocs-sphinx-search==0.1.2; extra == "docs"
 Requires-Dist: myst-nb==0.16.0; extra == "docs"
 Requires-Dist: nbconvert==7.2.5; extra == "docs"
-Requires-Dist: nbformat==5.5.0; extra == "docs"
+Requires-Dist: nbformat==5.9.2; extra == "docs"
 Requires-Dist: sphinx==5.2.1; extra == "docs"
 Requires-Dist: sphinxemoji==0.2.0; extra == "docs"
 Requires-Dist: sphinx-argparse==0.3.1; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.0; extra == "docs"
 Requires-Dist: sphinx-design==0.2.0; extra == "docs"
 Requires-Dist: sphinxext-opengraph==0.6.3; extra == "docs"
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 1.0.2 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 1.0.3 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 appdirs>=1.4 Requires-Dist: av>=9.2.0 Requires-Dist: awscli>=1.31.10 Requires-
 Dist: comet_ml>=3.33.8 Requires-Dist: cryptography>=38 Requires-Dist:
 tyro>=0.6.6 Requires-Dist: gdown>=4.6.0 Requires-Dist: ninja>=1.10 Requires-
 Dist: h5py>=2.9.0 Requires-Dist: imageio>=2.21.1 Requires-Dist: importlib-
 metadata>=6.0.0; python_version < "3.10" Requires-Dist: ipywidgets>=7.6
 Requires-Dist: jaxtyping>=0.2.15 Requires-Dist: jupyterlab>=3.3.4 Requires-
 Dist: matplotlib>=3.6.0 Requires-Dist: mediapy>=1.1.0 Requires-Dist:
 msgpack>=1.0.4 Requires-Dist: msgpack_numpy>=0.4.8 Requires-Dist:
 nerfacc==0.5.2 Requires-Dist: open3d>=0.16.0 Requires-Dist: opencv-
-python==4.8.0.76 Requires-Dist: Pillow>=9.3.0 Requires-Dist: plotly>=5.7.0
+python==4.8.0.76 Requires-Dist: Pillow>=10.3.0 Requires-Dist: plotly>=5.7.0
 Requires-Dist: protobuf!=3.20.0,<=3.20.3 Requires-Dist:
 pymeshlab>=2022.2.post2; platform_machine != "arm64" and platform_machine !=
 "aarch64" Requires-Dist: pyngrok>=5.1.0 Requires-Dist: python-socketio>=5.7.1
 Requires-Dist: pyquaternion>=0.9.9 Requires-Dist: rawpy>=0.18.1;
 platform_machine != "arm64" Requires-Dist: newrawpy>=1.0.0b0; platform_machine
 == "arm64" Requires-Dist: requests Requires-Dist: rich>=12.5.1 Requires-Dist:
 scikit-image>=0.19.3 Requires-Dist: splines==0.3.0 Requires-Dist:
 tensorboard>=2.13.0 Requires-Dist: torch>=1.13.1 Requires-Dist:
 torchvision>=0.14.1 Requires-Dist: torchmetrics[image]>=1.0.1 Requires-Dist:
-typing_extensions>=4.4.0 Requires-Dist: viser==0.1.21 Requires-Dist: nuscenes-
+typing_extensions>=4.4.0 Requires-Dist: viser==0.1.26 Requires-Dist: nuscenes-
 devkit>=1.1.1 Requires-Dist: wandb>=0.13.3 Requires-Dist: xatlas Requires-Dist:
-trimesh>=3.20.2 Requires-Dist: timm==0.6.7 Requires-Dist: gsplat>=0.1.6
+trimesh>=3.20.2 Requires-Dist: timm==0.6.7 Requires-Dist: gsplat>=0.1.9
 Requires-Dist: pytorch-msssim Requires-Dist: pathos Requires-Dist: packaging
 Provides-Extra: gen Requires-Dist: diffusers==0.16.1; extra == "gen" Requires-
 Dist: transformers==4.29.2; extra == "gen" Requires-Dist: accelerate==0.19.0;
 extra == "gen" Requires-Dist: bitsandbytes==0.39.0; extra == "gen" Requires-
 Dist: sentencepiece==0.1.99; extra == "gen" Provides-Extra: dev Requires-Dist:
 pre-commit==3.3.2; extra == "dev" Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: pytest-xdist==2.5.0; extra == "dev" Requires-Dist:
@@ -38,15 +38,15 @@
 opencv-stubs==0.0.7; extra == "dev" Requires-Dist: transformers==4.29.2; extra
 == "dev" Requires-Dist: pyright==1.1.331; extra == "dev" Requires-Dist:
 projectaria-tools>=1.3.1; sys_platform != "win32" and extra == "dev" Requires-
 Dist: torch<2.2,>=1.13.1; extra == "dev" Provides-Extra: docs Requires-Dist:
 furo==2022.09.29; extra == "docs" Requires-Dist: ipython==8.6.0; extra ==
 "docs" Requires-Dist: readthedocs-sphinx-search==0.1.2; extra == "docs"
 Requires-Dist: myst-nb==0.16.0; extra == "docs" Requires-Dist:
-nbconvert==7.2.5; extra == "docs" Requires-Dist: nbformat==5.5.0; extra ==
+nbconvert==7.2.5; extra == "docs" Requires-Dist: nbformat==5.9.2; extra ==
 "docs" Requires-Dist: sphinx==5.2.1; extra == "docs" Requires-Dist:
 sphinxemoji==0.2.0; extra == "docs" Requires-Dist: sphinx-argparse==0.3.1;
 extra == "docs" Requires-Dist: sphinx-copybutton==0.5.0; extra == "docs"
 Requires-Dist: sphinx-design==0.2.0; extra == "docs" Requires-Dist: sphinxext-
 opengraph==0.6.3; extra == "docs"
 _[_h_t_t_p_s_:_/_/_d_c_b_a_d_g_e_._v_e_r_c_e_l_._a_p_p_/_a_p_i_/_s_e_r_v_e_r_/_u_M_b_N_q_c_r_a_F_c_?_s_t_y_l_e_=_p_l_a_s_t_i_c_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n
                   _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_T_e_s_t_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]
```

### Comparing `nerfstudio-1.0.2/README.md` & `nerfstudio-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/__init__.py` & `nerfstudio-1.0.3/nerfstudio/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/cameras/__init__.py` & `nerfstudio-1.0.3/nerfstudio/cameras/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/cameras/camera_optimizers.py` & `nerfstudio-1.0.3/nerfstudio/cameras/camera_optimizers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/cameras/camera_paths.py` & `nerfstudio-1.0.3/nerfstudio/cameras/camera_paths.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/cameras/camera_utils.py` & `nerfstudio-1.0.3/nerfstudio/cameras/camera_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,40 +442,45 @@
 
         x = x + step_x
         y = y + step_y
 
     return torch.stack([x, y], dim=-1)
 
 
-def rotation_matrix(a: Float[Tensor, "3"], b: Float[Tensor, "3"]) -> Float[Tensor, "3 3"]:
+def rotation_matrix_between(a: Float[Tensor, "3"], b: Float[Tensor, "3"]) -> Float[Tensor, "3 3"]:
     """Compute the rotation matrix that rotates vector a to vector b.
 
     Args:
         a: The vector to rotate.
         b: The vector to rotate to.
     Returns:
         The rotation matrix.
     """
     a = a / torch.linalg.norm(a)
     b = b / torch.linalg.norm(b)
-    v = torch.cross(a, b)
-    c = torch.dot(a, b)
-    # If vectors are exactly opposite, we add a little noise to one of them
-    if c < -1 + 1e-8:
-        eps = (torch.rand(3) - 0.5) * 0.01
-        return rotation_matrix(a + eps, b)
-    s = torch.linalg.norm(v)
+    v = torch.linalg.cross(a, b)  # Axis of rotation.
+
+    # Handle cases where `a` and `b` are parallel.
+    eps = 1e-6
+    if torch.sum(torch.abs(v)) < eps:
+        x = torch.tensor([1.0, 0, 0]) if abs(a[0]) < eps else torch.tensor([0, 1.0, 0])
+        v = torch.linalg.cross(a, x)
+
+    v = v / torch.linalg.norm(v)
     skew_sym_mat = torch.Tensor(
         [
             [0, -v[2], v[1]],
             [v[2], 0, -v[0]],
             [-v[1], v[0], 0],
         ]
     )
-    return torch.eye(3) + skew_sym_mat + skew_sym_mat @ skew_sym_mat * ((1 - c) / (s**2 + 1e-8))
+    theta = torch.acos(torch.clip(torch.dot(a, b), -1, 1))
+
+    # Rodrigues rotation formula. https://en.wikipedia.org/wiki/Rodrigues%27_rotation_formula
+    return torch.eye(3) + torch.sin(theta) * skew_sym_mat + (1 - torch.cos(theta)) * (skew_sym_mat @ skew_sym_mat)
 
 
 def focus_of_attention(poses: Float[Tensor, "*num_poses 4 4"], initial_focus: Float[Tensor, "3"]) -> Float[Tensor, "3"]:
     """Compute the focus of attention of a set of cameras. Only cameras
     that have the focus of attention in front of them are considered.
 
      Args:
@@ -605,15 +610,15 @@
                 # the last two right singular vectors (which are orthogonal to the
                 # first). v_0 is a unit vector, no need to divide by its norm when
                 # projecting.
                 up = up - Vh[0, :] * torch.dot(up, Vh[0, :])
                 # re-normalize
                 up = up / torch.linalg.norm(up)
 
-        rotation = rotation_matrix(up, torch.Tensor([0, 0, 1]))
+        rotation = rotation_matrix_between(up, torch.Tensor([0, 0, 1]))
         transform = torch.cat([rotation, rotation @ -translation[..., None]], dim=-1)
         oriented_poses = transform @ poses
     elif method == "none":
         transform = torch.eye(4)
         transform[:3, 3] = -translation
         transform = transform[:3, :]
         oriented_poses = transform @ poses
```

### Comparing `nerfstudio-1.0.2/nerfstudio/cameras/cameras.py` & `nerfstudio-1.0.3/nerfstudio/cameras/cameras.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/cameras/lie_groups.py` & `nerfstudio-1.0.3/nerfstudio/cameras/lie_groups.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/cameras/rays.py` & `nerfstudio-1.0.3/nerfstudio/cameras/rays.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/configs/__init__.py` & `nerfstudio-1.0.3/nerfstudio/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/configs/base_config.py` & `nerfstudio-1.0.3/nerfstudio/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/configs/config_utils.py` & `nerfstudio-1.0.3/nerfstudio/configs/config_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/configs/dataparser_configs.py` & `nerfstudio-1.0.3/nerfstudio/configs/dataparser_configs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/configs/experiment_config.py` & `nerfstudio-1.0.3/nerfstudio/configs/experiment_config.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/configs/external_methods.py` & `nerfstudio-1.0.3/nerfstudio/configs/external_methods.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/configs/method_configs.py` & `nerfstudio-1.0.3/nerfstudio/configs/method_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -595,47 +595,98 @@
     method_name="splatfacto",
     steps_per_eval_image=100,
     steps_per_eval_batch=0,
     steps_per_save=2000,
     steps_per_eval_all_images=1000,
     max_num_iterations=30000,
     mixed_precision=False,
-    gradient_accumulation_steps={"camera_opt": 100},
     pipeline=VanillaPipelineConfig(
         datamanager=FullImageDatamanagerConfig(
             dataparser=NerfstudioDataParserConfig(load_3D_points=True),
             cache_images_type="uint8",
         ),
         model=SplatfactoModelConfig(),
     ),
     optimizers={
-        "xyz": {
+        "means": {
             "optimizer": AdamOptimizerConfig(lr=1.6e-4, eps=1e-15),
             "scheduler": ExponentialDecaySchedulerConfig(
                 lr_final=1.6e-6,
                 max_steps=30000,
             ),
         },
         "features_dc": {
             "optimizer": AdamOptimizerConfig(lr=0.0025, eps=1e-15),
             "scheduler": None,
         },
         "features_rest": {
             "optimizer": AdamOptimizerConfig(lr=0.0025 / 20, eps=1e-15),
             "scheduler": None,
         },
-        "opacity": {
+        "opacities": {
             "optimizer": AdamOptimizerConfig(lr=0.05, eps=1e-15),
             "scheduler": None,
         },
-        "scaling": {
+        "scales": {
             "optimizer": AdamOptimizerConfig(lr=0.005, eps=1e-15),
             "scheduler": None,
         },
-        "rotation": {"optimizer": AdamOptimizerConfig(lr=0.001, eps=1e-15), "scheduler": None},
+        "quats": {"optimizer": AdamOptimizerConfig(lr=0.001, eps=1e-15), "scheduler": None},
+        "camera_opt": {
+            "optimizer": AdamOptimizerConfig(lr=1e-3, eps=1e-15),
+            "scheduler": ExponentialDecaySchedulerConfig(lr_final=5e-5, max_steps=30000),
+        },
+    },
+    viewer=ViewerConfig(num_rays_per_chunk=1 << 15),
+    vis="viewer",
+)
+
+method_configs["splatfacto-big"] = TrainerConfig(
+    method_name="splatfacto",
+    steps_per_eval_image=100,
+    steps_per_eval_batch=0,
+    steps_per_save=2000,
+    steps_per_eval_all_images=1000,
+    max_num_iterations=30000,
+    mixed_precision=False,
+    pipeline=VanillaPipelineConfig(
+        datamanager=FullImageDatamanagerConfig(
+            dataparser=NerfstudioDataParserConfig(load_3D_points=True),
+            cache_images_type="uint8",
+        ),
+        model=SplatfactoModelConfig(
+            cull_alpha_thresh=0.005,
+            continue_cull_post_densification=False,
+        ),
+    ),
+    optimizers={
+        "means": {
+            "optimizer": AdamOptimizerConfig(lr=1.6e-4, eps=1e-15),
+            "scheduler": ExponentialDecaySchedulerConfig(
+                lr_final=1.6e-6,
+                max_steps=30000,
+            ),
+        },
+        "features_dc": {
+            "optimizer": AdamOptimizerConfig(lr=0.0025, eps=1e-15),
+            "scheduler": None,
+        },
+        "features_rest": {
+            "optimizer": AdamOptimizerConfig(lr=0.0025 / 20, eps=1e-15),
+            "scheduler": None,
+        },
+        "opacities": {
+            "optimizer": AdamOptimizerConfig(lr=0.05, eps=1e-15),
+            "scheduler": None,
+        },
+        "scales": {
+            "optimizer": AdamOptimizerConfig(lr=0.005, eps=1e-15),
+            "scheduler": None,
+        },
+        "quats": {"optimizer": AdamOptimizerConfig(lr=0.001, eps=1e-15), "scheduler": None},
         "camera_opt": {
             "optimizer": AdamOptimizerConfig(lr=1e-3, eps=1e-15),
             "scheduler": ExponentialDecaySchedulerConfig(lr_final=5e-5, max_steps=30000),
         },
     },
     viewer=ViewerConfig(num_rays_per_chunk=1 << 15),
     vis="viewer",
```

### Comparing `nerfstudio-1.0.2/nerfstudio/data/__init__.py` & `nerfstudio-1.0.3/nerfstudio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datamanagers/__init__.py` & `nerfstudio-1.0.3/nerfstudio/data/datamanagers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datamanagers/base_datamanager.py` & `nerfstudio-1.0.3/nerfstudio/data/datamanagers/base_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datamanagers/full_images_datamanager.py` & `nerfstudio-1.0.3/nerfstudio/data/datamanagers/full_images_datamanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,34 +176,38 @@
             self.eval_dataset.cameras.cx[idx] = float(K[0, 2])
             self.eval_dataset.cameras.cy[idx] = float(K[1, 2])
             self.eval_dataset.cameras.width[idx] = image.shape[1]
             self.eval_dataset.cameras.height[idx] = image.shape[0]
             return data
 
         CONSOLE.log("Caching / undistorting train images")
-        with ThreadPoolExecutor() as executor:
+        with ThreadPoolExecutor(max_workers=2) as executor:
             cached_train = list(
-                executor.map(
-                    process_train_data,
-                    track(
+                track(
+                    executor.map(
+                        process_train_data,
                         range(len(self.train_dataset)),
-                        description="Caching / undistorting train images",
-                        transient=True,
                     ),
+                    description="Caching / undistorting train images",
+                    transient=True,
+                    total=len(self.train_dataset),
                 )
             )
 
         CONSOLE.log("Caching / undistorting eval images")
-        with ThreadPoolExecutor() as executor:
+        with ThreadPoolExecutor(max_workers=2) as executor:
             cached_eval = list(
-                executor.map(
-                    process_eval_data,
-                    track(
-                        range(len(self.eval_dataset)), description="Caching / undistorting eval images", transient=True
+                track(
+                    executor.map(
+                        process_eval_data,
+                        range(len(self.eval_dataset)),
                     ),
+                    description="Caching / undistorting eval images",
+                    transient=True,
+                    total=len(self.eval_dataset),
                 )
             )
 
         if cache_images_option == "gpu":
             for cache in cached_train:
                 cache["image"] = cache["image"].to(self.device)
                 if "mask" in cache:
@@ -379,14 +383,16 @@
         if "mask" in data:
             mask = data["mask"].numpy()
             mask = mask.astype(np.uint8) * 255
             if np.any(distortion_params):
                 mask = cv2.undistort(mask, K, distortion_params, None, newK)  # type: ignore
             mask = mask[y : y + h, x : x + w]
             mask = torch.from_numpy(mask).bool()
+            if len(mask.shape) == 2:
+                mask = mask[:, :, None]
         K = newK
 
     elif camera.camera_type.item() == CameraType.FISHEYE.value:
         distortion_params = np.array(
             [distortion_params[0], distortion_params[1], distortion_params[2], distortion_params[3]]
         )
         newK = cv2.fisheye.estimateNewCameraMatrixForUndistortRectify(
@@ -398,14 +404,16 @@
         # and then remap:
         image = cv2.remap(image, map1, map2, interpolation=cv2.INTER_LINEAR)
         if "mask" in data:
             mask = data["mask"].numpy()
             mask = mask.astype(np.uint8) * 255
             mask = cv2.fisheye.undistortImage(mask, K, distortion_params, None, newK)
             mask = torch.from_numpy(mask).bool()
+            if len(mask.shape) == 2:
+                mask = mask[:, :, None]
         K = newK
     elif camera.camera_type.item() == CameraType.FISHEYE624.value:
         fisheye624_params = torch.cat(
             [camera.fx, camera.fy, camera.cx, camera.cy, torch.from_numpy(distortion_params)], dim=0
         )
         assert fisheye624_params.shape == (16,)
         assert (
@@ -490,13 +498,15 @@
                 map2,
                 interpolation=cv2.INTER_LINEAR,
                 borderMode=cv2.BORDER_CONSTANT,
                 borderValue=0,
             )
             / 255.0
         ).bool()[..., None]
+        if len(mask.shape) == 2:
+            mask = mask[:, :, None]
         assert mask.shape == (undist_h, undist_w, 1)
         K = undist_K.numpy()
     else:
         raise NotImplementedError("Only perspective and fisheye cameras are supported")
 
     return K, image, mask
```

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datamanagers/parallel_datamanager.py` & `nerfstudio-1.0.3/nerfstudio/data/datamanagers/parallel_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datamanagers/random_cameras_datamanager.py` & `nerfstudio-1.0.3/nerfstudio/data/datamanagers/random_cameras_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/__init__.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/arkitscenes_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/arkitscenes_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/base_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/base_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/blender_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/blender_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/colmap_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/colmap_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/dnerf_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/dnerf_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/dycheck_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/dycheck_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/instant_ngp_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/instant_ngp_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/minimal_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/minimal_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/nerfosr_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/nerfosr_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/nerfstudio_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/nerfstudio_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/nuscenes_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/nuscenes_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/phototourism_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/phototourism_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/scannet_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/scannet_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/scannetpp_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/scannetpp_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/sdfstudio_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/sdfstudio_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datasets/__init__.py` & `nerfstudio-1.0.3/nerfstudio/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datasets/base_dataset.py` & `nerfstudio-1.0.3/nerfstudio/data/datasets/base_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             image_idx: The image index in the dataset.
         """
         image_filename = self._dataparser_outputs.image_filenames[image_idx]
         pil_image = Image.open(image_filename)
         if self.scale_factor != 1.0:
             width, height = pil_image.size
             newsize = (int(width * self.scale_factor), int(height * self.scale_factor))
-            pil_image = pil_image.resize(newsize, resample=Image.BILINEAR)
+            pil_image = pil_image.resize(newsize, resample=Image.Resampling.BILINEAR)
         image = np.array(pil_image, dtype="uint8")  # shape is (h, w) or (h, w, 3 or 4)
         if len(image.shape) == 2:
             image = image[:, :, None].repeat(3, axis=2)
         assert len(image.shape) == 3
         assert image.dtype == np.uint8
         assert image.shape[2] in [3, 4], f"Image shape of {image.shape} is in correct."
         return image
```

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datasets/depth_dataset.py` & `nerfstudio-1.0.3/nerfstudio/data/datasets/depth_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datasets/sdf_dataset.py` & `nerfstudio-1.0.3/nerfstudio/data/datasets/sdf_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/datasets/semantic_dataset.py` & `nerfstudio-1.0.3/nerfstudio/data/datasets/semantic_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/pixel_samplers.py` & `nerfstudio-1.0.3/nerfstudio/data/pixel_samplers.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,30 +174,58 @@
         image_width: int,
         mask: Optional[Tensor] = None,
         device: Union[torch.device, str] = "cpu",
     ) -> Int[Tensor, "batch_size 3"]:
         if isinstance(mask, torch.Tensor) and not self.config.ignore_mask:
             indices = self.sample_method(batch_size, num_images, image_height, image_width, mask=mask, device=device)
         else:
-            rand_samples = torch.rand((batch_size, 3), device=device)
-            # convert random samples tto radius and theta
-            radii = self.config.fisheye_crop_radius * torch.sqrt(rand_samples[:, 1])
-            theta = 2.0 * torch.pi * rand_samples[:, 2]
-
-            # convert radius and theta to x and y between -radii and radii
-            x = radii * torch.cos(theta)
-            y = radii * torch.sin(theta)
-
-            # Multiply by the batch size and height/width to get pixel indices.
-            indices = torch.floor(
-                torch.stack([rand_samples[:, 0], y, x], dim=1)
-                * torch.tensor([num_images, image_height // 2, image_width // 2], device=device)
-                + torch.tensor([0, image_height // 2, image_width // 2], device=device)
-            ).long()
+            # Rejection sampling.
+            valid: Optional[torch.Tensor] = None
+            indices = None
+            while True:
+                samples_needed = batch_size if valid is None else int(batch_size - torch.sum(valid).item())
+
+                # Check if done!
+                if samples_needed == 0:
+                    break
+
+                rand_samples = torch.rand((samples_needed, 2), device=device)
+                # Convert random samples to radius and theta.
+                radii = self.config.fisheye_crop_radius * torch.sqrt(rand_samples[:, 0])
+                theta = 2.0 * torch.pi * rand_samples[:, 1]
+
+                # Convert radius and theta to x and y.
+                x = (radii * torch.cos(theta) + image_width // 2).long()
+                y = (radii * torch.sin(theta) + image_height // 2).long()
+                sampled_indices = torch.stack(
+                    [torch.randint(0, num_images, size=(samples_needed,), device=device), y, x], dim=-1
+                )
+
+                # Update indices.
+                if valid is None:
+                    indices = sampled_indices
+                    valid = (
+                        (sampled_indices[:, 1] >= 0)
+                        & (sampled_indices[:, 1] < image_height)
+                        & (sampled_indices[:, 2] >= 0)
+                        & (sampled_indices[:, 2] < image_width)
+                    )
+                else:
+                    assert indices is not None
+                    not_valid = ~valid
+                    indices[not_valid, :] = sampled_indices
+                    valid[not_valid] = (
+                        (sampled_indices[:, 1] >= 0)
+                        & (sampled_indices[:, 1] < image_height)
+                        & (sampled_indices[:, 2] >= 0)
+                        & (sampled_indices[:, 2] < image_width)
+                    )
+            assert indices is not None
 
+        assert indices.shape == (batch_size, 3)
         return indices
 
     def collate_image_dataset_batch(self, batch: Dict, num_rays_per_batch: int, keep_full_image: bool = False):
         """
         Operates on a batch of images and samples pixels to use for generating rays.
         Returns a collated batch which is input to the Graph.
         It will sample only within the valid 'mask' if it's specified.
@@ -268,56 +296,65 @@
 
         device = batch["image"][0].device
         num_images = len(batch["image"])
 
         # only sample within the mask, if the mask is in the batch
         all_indices = []
         all_images = []
+        all_depth_images = []
+
+        num_rays_in_batch = num_rays_per_batch // num_images
+        if num_rays_in_batch % 2 != 0:
+            num_rays_in_batch += 1
 
         if "mask" in batch:
-            num_rays_in_batch = num_rays_per_batch // num_images
             for i in range(num_images):
                 image_height, image_width, _ = batch["image"][i].shape
 
                 if i == num_images - 1:
                     num_rays_in_batch = num_rays_per_batch - (num_images - 1) * num_rays_in_batch
 
                 indices = self.sample_method(
                     num_rays_in_batch, 1, image_height, image_width, mask=batch["mask"][i].unsqueeze(0), device=device
                 )
                 indices[:, 0] = i
                 all_indices.append(indices)
                 all_images.append(batch["image"][i][indices[:, 1], indices[:, 2]])
+                if "depth_image" in batch:
+                    all_depth_images.append(batch["depth_image"][i][indices[:, 1], indices[:, 2]])
 
         else:
-            num_rays_in_batch = num_rays_per_batch // num_images
             for i in range(num_images):
                 image_height, image_width, _ = batch["image"][i].shape
                 if i == num_images - 1:
                     num_rays_in_batch = num_rays_per_batch - (num_images - 1) * num_rays_in_batch
                 if self.config.is_equirectangular:
                     indices = self.sample_method_equirectangular(
                         num_rays_in_batch, 1, image_height, image_width, device=device
                     )
                 else:
                     indices = self.sample_method(num_rays_in_batch, 1, image_height, image_width, device=device)
                 indices[:, 0] = i
                 all_indices.append(indices)
                 all_images.append(batch["image"][i][indices[:, 1], indices[:, 2]])
+                if "depth_image" in batch:
+                    all_depth_images.append(batch["depth_image"][i][indices[:, 1], indices[:, 2]])
 
         indices = torch.cat(all_indices, dim=0)
 
         c, y, x = (i.flatten() for i in torch.split(indices, 1, dim=-1))
         collated_batch = {
             key: value[c, y, x]
             for key, value in batch.items()
-            if key != "image_idx" and key != "image" and key != "mask" and value is not None
+            if key != "image_idx" and key != "image" and key != "mask" and key != "depth_image" and value is not None
         }
 
         collated_batch["image"] = torch.cat(all_images, dim=0)
+        if "depth_image" in batch:
+            collated_batch["depth_image"] = torch.cat(all_depth_images, dim=0)
 
         assert collated_batch["image"].shape[0] == num_rays_per_batch
 
         # Needed to correct the random indices to their actual camera idx locations.
         indices[:, 0] = batch["image_idx"][c]
         collated_batch["indices"] = indices  # with the abs camera indices
```

### Comparing `nerfstudio-1.0.2/nerfstudio/data/scene_box.py` & `nerfstudio-1.0.3/nerfstudio/data/scene_box.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     """Data to represent the scene box."""
 
     aabb: Float[Tensor, "2 3"]
     """aabb: axis-aligned bounding box.
     aabb[0] is the minimum (x,y,z) point.
     aabb[1] is the maximum (x,y,z) point."""
 
+    def within(self, pts: Float[Tensor, "n 3"]):
+        """Returns a boolean mask indicating whether each point is within the box."""
+        return torch.all(pts > self.aabb[0], dim=-1) & torch.all(pts < self.aabb[1], dim=-1)
+
     def get_diagonal_length(self):
         """Returns the longest diagonal length."""
         diff = self.aabb[1] - self.aabb[0]
         length = torch.sqrt((diff**2).sum() + 1e-20)
         return length
 
     def get_center(self):
```

### Comparing `nerfstudio-1.0.2/nerfstudio/data/utils/__init__.py` & `nerfstudio-1.0.3/nerfstudio/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/utils/colmap_parsing_utils.py` & `nerfstudio-1.0.3/nerfstudio/data/utils/colmap_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/utils/data_utils.py` & `nerfstudio-1.0.3/nerfstudio/data/utils/data_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """
     Utility function to read a mask image from the given path and return a boolean tensor
     """
     pil_mask = Image.open(filepath)
     if scale_factor != 1.0:
         width, height = pil_mask.size
         newsize = (int(width * scale_factor), int(height * scale_factor))
-        pil_mask = pil_mask.resize(newsize, resample=Image.NEAREST)
+        pil_mask = pil_mask.resize(newsize, resample=Image.Resampling.NEAREST)
     mask_tensor = torch.from_numpy(np.array(pil_mask)).unsqueeze(-1).bool()
     if len(mask_tensor.shape) != 3:
         raise ValueError("The mask image should have 1 channel")
     return mask_tensor
 
 
 def get_semantics_and_mask_tensors_from_path(
@@ -46,15 +46,15 @@
     """
     if isinstance(mask_indices, List):
         mask_indices = torch.tensor(mask_indices, dtype=torch.int64).view(1, 1, -1)
     pil_image = Image.open(filepath)
     if scale_factor != 1.0:
         width, height = pil_image.size
         newsize = (int(width * scale_factor), int(height * scale_factor))
-        pil_image = pil_image.resize(newsize, resample=Image.NEAREST)
+        pil_image = pil_image.resize(newsize, resample=Image.Resampling.NEAREST)
     semantics = torch.from_numpy(np.array(pil_image, dtype="int64"))[..., None]
     mask = torch.sum(semantics == mask_indices, dim=-1, keepdim=True) == 0
     return semantics, mask
 
 
 def get_depth_image_from_path(
     filepath: Path,
```

### Comparing `nerfstudio-1.0.2/nerfstudio/data/utils/dataloaders.py` & `nerfstudio-1.0.3/nerfstudio/data/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/utils/dataparsers_utils.py` & `nerfstudio-1.0.3/nerfstudio/data/utils/dataparsers_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/utils/nerfstudio_collate.py` & `nerfstudio-1.0.3/nerfstudio/data/utils/nerfstudio_collate.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/data/utils/pixel_sampling_utils.py` & `nerfstudio-1.0.3/nerfstudio/data/utils/pixel_sampling_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/engine/__init__.py` & `nerfstudio-1.0.3/nerfstudio/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/engine/callbacks.py` & `nerfstudio-1.0.3/nerfstudio/engine/callbacks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/engine/optimizers.py` & `nerfstudio-1.0.3/nerfstudio/engine/optimizers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/engine/schedulers.py` & `nerfstudio-1.0.3/nerfstudio/engine/schedulers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/engine/trainer.py` & `nerfstudio-1.0.3/nerfstudio/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/exporter/__init__.py` & `nerfstudio-1.0.3/nerfstudio/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/exporter/exporter_utils.py` & `nerfstudio-1.0.3/nerfstudio/exporter/exporter_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/exporter/marching_cubes.py` & `nerfstudio-1.0.3/nerfstudio/exporter/marching_cubes.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/exporter/texture_utils.py` & `nerfstudio-1.0.3/nerfstudio/exporter/texture_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/exporter/tsdf_utils.py` & `nerfstudio-1.0.3/nerfstudio/exporter/tsdf_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/field_components/__init__.py` & `nerfstudio-1.0.3/nerfstudio/field_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/field_components/activations.py` & `nerfstudio-1.0.3/nerfstudio/field_components/activations.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/field_components/base_field_component.py` & `nerfstudio-1.0.3/nerfstudio/field_components/base_field_component.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/field_components/embedding.py` & `nerfstudio-1.0.3/nerfstudio/field_components/embedding.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/field_components/encodings.py` & `nerfstudio-1.0.3/nerfstudio/field_components/encodings.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/field_components/field_heads.py` & `nerfstudio-1.0.3/nerfstudio/field_components/field_heads.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/field_components/mlp.py` & `nerfstudio-1.0.3/nerfstudio/field_components/mlp.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/field_components/spatial_distortions.py` & `nerfstudio-1.0.3/nerfstudio/field_components/spatial_distortions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/field_components/temporal_distortions.py` & `nerfstudio-1.0.3/nerfstudio/field_components/temporal_distortions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/__init__.py` & `nerfstudio-1.0.3/nerfstudio/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/base_field.py` & `nerfstudio-1.0.3/nerfstudio/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/density_fields.py` & `nerfstudio-1.0.3/nerfstudio/fields/density_fields.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/generfacto_field.py` & `nerfstudio-1.0.3/nerfstudio/fields/generfacto_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/nerfacto_field.py` & `nerfstudio-1.0.3/nerfstudio/fields/nerfacto_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/nerfw_field.py` & `nerfstudio-1.0.3/nerfstudio/fields/nerfw_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/sdf_field.py` & `nerfstudio-1.0.3/nerfstudio/fields/sdf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/semantic_nerf_field.py` & `nerfstudio-1.0.3/nerfstudio/fields/semantic_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/tensorf_field.py` & `nerfstudio-1.0.3/nerfstudio/fields/tensorf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/fields/vanilla_nerf_field.py` & `nerfstudio-1.0.3/nerfstudio/fields/vanilla_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/generative/__init__.py` & `nerfstudio-1.0.3/nerfstudio/generative/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/generative/deepfloyd.py` & `nerfstudio-1.0.3/nerfstudio/generative/deepfloyd.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/generative/positional_text_embeddings.py` & `nerfstudio-1.0.3/nerfstudio/generative/positional_text_embeddings.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/generative/stable_diffusion.py` & `nerfstudio-1.0.3/nerfstudio/generative/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/model_components/__init__.py` & `nerfstudio-1.0.3/nerfstudio/model_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/model_components/losses.py` & `nerfstudio-1.0.3/nerfstudio/model_components/losses.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/model_components/ray_generators.py` & `nerfstudio-1.0.3/nerfstudio/model_components/ray_generators.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/model_components/ray_samplers.py` & `nerfstudio-1.0.3/nerfstudio/model_components/ray_samplers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/model_components/renderers.py` & `nerfstudio-1.0.3/nerfstudio/model_components/renderers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/model_components/scene_colliders.py` & `nerfstudio-1.0.3/nerfstudio/model_components/scene_colliders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/model_components/shaders.py` & `nerfstudio-1.0.3/nerfstudio/model_components/shaders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/__init__.py` & `nerfstudio-1.0.3/nerfstudio/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/base_model.py` & `nerfstudio-1.0.3/nerfstudio/models/base_model.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/base_surface_model.py` & `nerfstudio-1.0.3/nerfstudio/models/base_surface_model.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/depth_nerfacto.py` & `nerfstudio-1.0.3/nerfstudio/models/depth_nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/generfacto.py` & `nerfstudio-1.0.3/nerfstudio/models/generfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/instant_ngp.py` & `nerfstudio-1.0.3/nerfstudio/models/instant_ngp.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         image = self.renderer_rgb.blend_background(image)
         metrics_dict = {}
         metrics_dict["psnr"] = self.psnr(outputs["rgb"], image)
         metrics_dict["num_samples_per_batch"] = outputs["num_samples_per_ray"].sum()
         return metrics_dict
 
     def get_loss_dict(self, outputs, batch, metrics_dict=None):
-        image = batch["image"][..., :3].to(self.device)
+        image = batch["image"].to(self.device)
         pred_rgb, image = self.renderer_rgb.blend_background_for_loss_computation(
             pred_image=outputs["rgb"],
             pred_accumulation=outputs["accumulation"],
             gt_image=image,
         )
         rgb_loss = self.rgb_loss(image, pred_rgb)
         loss_dict = {"rgb_loss": rgb_loss}
```

### Comparing `nerfstudio-1.0.2/nerfstudio/models/mipnerf.py` & `nerfstudio-1.0.3/nerfstudio/models/mipnerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/nerfacto.py` & `nerfstudio-1.0.3/nerfstudio/models/nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/neus.py` & `nerfstudio-1.0.3/nerfstudio/models/neus.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/neus_facto.py` & `nerfstudio-1.0.3/nerfstudio/models/neus_facto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/semantic_nerfw.py` & `nerfstudio-1.0.3/nerfstudio/models/semantic_nerfw.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/models/splatfacto.py` & `nerfstudio-1.0.3/nerfstudio/models/splatfacto.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,49 +75,28 @@
     """
     Converts from the 0th spherical harmonic coefficient to RGB values [0,1]
     """
     C0 = 0.28209479177387814
     return sh * C0 + 0.5
 
 
-def projection_matrix(znear, zfar, fovx, fovy, device: Union[str, torch.device] = "cpu"):
-    """
-    Constructs an OpenGL-style perspective projection matrix.
-    """
-    t = znear * math.tan(0.5 * fovy)
-    b = -t
-    r = znear * math.tan(0.5 * fovx)
-    l = -r
-    n = znear
-    f = zfar
-    return torch.tensor(
-        [
-            [2 * n / (r - l), 0.0, (r + l) / (r - l), 0.0],
-            [0.0, 2 * n / (t - b), (t + b) / (t - b), 0.0],
-            [0.0, 0.0, (f + n) / (f - n), -1.0 * f * n / (f - n)],
-            [0.0, 0.0, 1.0, 0.0],
-        ],
-        device=device,
-    )
-
-
 @dataclass
 class SplatfactoModelConfig(ModelConfig):
     """Splatfacto Model Config, nerfstudio's implementation of Gaussian Splatting"""
 
     _target: Type = field(default_factory=lambda: SplatfactoModel)
     warmup_length: int = 500
     """period of steps where refinement is turned off"""
     refine_every: int = 100
     """period of steps where gaussians are culled and densified"""
-    resolution_schedule: int = 250
+    resolution_schedule: int = 3000
     """training starts at 1/d resolution, every n steps this is doubled"""
     background_color: Literal["random", "black", "white"] = "random"
     """Whether to randomize the background color."""
-    num_downscales: int = 0
+    num_downscales: int = 2
     """at the beginning, resolution is 1/2^d, where d is this number"""
     cull_alpha_thresh: float = 0.1
     """threshold of opacity for culling gaussians. One can set it to a lower value (e.g. 0.005) for higher quality."""
     cull_scale_thresh: float = 0.5
     """threshold of scale for culling huge gaussians"""
     continue_cull_post_densification: bool = True
     """If True, continue to cull gaussians post refinement"""
@@ -185,25 +164,26 @@
         **kwargs,
     ):
         self.seed_points = seed_points
         super().__init__(*args, **kwargs)
 
     def populate_modules(self):
         if self.seed_points is not None and not self.config.random_init:
-            self.means = torch.nn.Parameter(self.seed_points[0])  # (Location, Color)
+            means = torch.nn.Parameter(self.seed_points[0])  # (Location, Color)
         else:
-            self.means = torch.nn.Parameter((torch.rand((self.config.num_random, 3)) - 0.5) * self.config.random_scale)
+            means = torch.nn.Parameter((torch.rand((self.config.num_random, 3)) - 0.5) * self.config.random_scale)
         self.xys_grad_norm = None
         self.max_2Dsize = None
-        distances, _ = self.k_nearest_sklearn(self.means.data, 3)
+        distances, _ = self.k_nearest_sklearn(means.data, 3)
         distances = torch.from_numpy(distances)
         # find the average of the three nearest neighbors for each point and use that as the scale
         avg_dist = distances.mean(dim=-1, keepdim=True)
-        self.scales = torch.nn.Parameter(torch.log(avg_dist.repeat(1, 3)))
-        self.quats = torch.nn.Parameter(random_quat_tensor(self.num_points))
+        scales = torch.nn.Parameter(torch.log(avg_dist.repeat(1, 3)))
+        num_points = means.shape[0]
+        quats = torch.nn.Parameter(random_quat_tensor(num_points))
         dim_sh = num_sh_bases(self.config.sh_degree)
 
         if (
             self.seed_points is not None
             and not self.config.random_init
             # We can have colors without points.
             and self.seed_points[1].shape[0] > 0
@@ -211,21 +191,31 @@
             shs = torch.zeros((self.seed_points[1].shape[0], dim_sh, 3)).float().cuda()
             if self.config.sh_degree > 0:
                 shs[:, 0, :3] = RGB2SH(self.seed_points[1] / 255)
                 shs[:, 1:, 3:] = 0.0
             else:
                 CONSOLE.log("use color only optimization with sigmoid activation")
                 shs[:, 0, :3] = torch.logit(self.seed_points[1] / 255, eps=1e-10)
-            self.features_dc = torch.nn.Parameter(shs[:, 0, :])
-            self.features_rest = torch.nn.Parameter(shs[:, 1:, :])
+            features_dc = torch.nn.Parameter(shs[:, 0, :])
+            features_rest = torch.nn.Parameter(shs[:, 1:, :])
         else:
-            self.features_dc = torch.nn.Parameter(torch.rand(self.num_points, 3))
-            self.features_rest = torch.nn.Parameter(torch.zeros((self.num_points, dim_sh - 1, 3)))
+            features_dc = torch.nn.Parameter(torch.rand(num_points, 3))
+            features_rest = torch.nn.Parameter(torch.zeros((num_points, dim_sh - 1, 3)))
 
-        self.opacities = torch.nn.Parameter(torch.logit(0.1 * torch.ones(self.num_points, 1)))
+        opacities = torch.nn.Parameter(torch.logit(0.1 * torch.ones(num_points, 1)))
+        self.gauss_params = torch.nn.ParameterDict(
+            {
+                "means": means,
+                "scales": scales,
+                "quats": quats,
+                "features_dc": features_dc,
+                "features_rest": features_rest,
+                "opacities": opacities,
+            }
+        )
 
         # metrics
         from torchmetrics.image import PeakSignalNoiseRatio
         from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = SSIM(data_range=1.0, size_average=True, channel=3)
@@ -251,26 +241,55 @@
     def shs_0(self):
         return self.features_dc
 
     @property
     def shs_rest(self):
         return self.features_rest
 
+    @property
+    def num_points(self):
+        return self.means.shape[0]
+
+    @property
+    def means(self):
+        return self.gauss_params["means"]
+
+    @property
+    def scales(self):
+        return self.gauss_params["scales"]
+
+    @property
+    def quats(self):
+        return self.gauss_params["quats"]
+
+    @property
+    def features_dc(self):
+        return self.gauss_params["features_dc"]
+
+    @property
+    def features_rest(self):
+        return self.gauss_params["features_rest"]
+
+    @property
+    def opacities(self):
+        return self.gauss_params["opacities"]
+
     def load_state_dict(self, dict, **kwargs):  # type: ignore
         # resize the parameters to match the new number of points
         self.step = 30000
-        newp = dict["means"].shape[0]
-        self.means = torch.nn.Parameter(torch.zeros(newp, 3, device=self.device))
-        self.scales = torch.nn.Parameter(torch.zeros(newp, 3, device=self.device))
-        self.quats = torch.nn.Parameter(torch.zeros(newp, 4, device=self.device))
-        self.opacities = torch.nn.Parameter(torch.zeros(newp, 1, device=self.device))
-        self.features_dc = torch.nn.Parameter(torch.zeros(newp, 3, device=self.device))
-        self.features_rest = torch.nn.Parameter(
-            torch.zeros(newp, num_sh_bases(self.config.sh_degree) - 1, 3, device=self.device)
-        )
+        if "means" in dict:
+            # For backwards compatibility, we remap the names of parameters from
+            # means->gauss_params.means since old checkpoints have that format
+            for p in ["means", "scales", "quats", "features_dc", "features_rest", "opacities"]:
+                dict[f"gauss_params.{p}"] = dict[p]
+        newp = dict["gauss_params.means"].shape[0]
+        for name, param in self.gauss_params.items():
+            old_shape = param.shape
+            new_shape = (newp,) + old_shape[1:]
+            self.gauss_params[name] = torch.nn.Parameter(torch.zeros(new_shape, device=self.device))
         super().load_state_dict(dict, **kwargs)
 
     def k_nearest_sklearn(self, x: torch.Tensor, k: int):
         """
             Find k-nearest neighbors using sklearn's NearestNeighbors.
         x: The data tensor of shape [num_samples, num_features]
         k: The number of neighbors to retrieve
@@ -295,16 +314,17 @@
         # assert isinstance(optimizer, torch.optim.Adam), "Only works with Adam"
 
         param = optimizer.param_groups[0]["params"][0]
         param_state = optimizer.state[param]
         del optimizer.state[param]
 
         # Modify the state directly without deleting and reassigning.
-        param_state["exp_avg"] = param_state["exp_avg"][~deleted_mask]
-        param_state["exp_avg_sq"] = param_state["exp_avg_sq"][~deleted_mask]
+        if "exp_avg" in param_state:
+            param_state["exp_avg"] = param_state["exp_avg"][~deleted_mask]
+            param_state["exp_avg_sq"] = param_state["exp_avg_sq"][~deleted_mask]
 
         # Update the parameter in the optimizer's param group.
         del optimizer.param_groups[0]["params"][0]
         del optimizer.param_groups[0]["params"]
         optimizer.param_groups[0]["params"] = new_params
         optimizer.state[new_params[0]] = param_state
 
@@ -314,29 +334,30 @@
             self.remove_from_optim(optimizers.optimizers[group], deleted_mask, param)
         torch.cuda.empty_cache()
 
     def dup_in_optim(self, optimizer, dup_mask, new_params, n=2):
         """adds the parameters to the optimizer"""
         param = optimizer.param_groups[0]["params"][0]
         param_state = optimizer.state[param]
-        repeat_dims = (n,) + tuple(1 for _ in range(param_state["exp_avg"].dim() - 1))
-        param_state["exp_avg"] = torch.cat(
-            [
-                param_state["exp_avg"],
-                torch.zeros_like(param_state["exp_avg"][dup_mask.squeeze()]).repeat(*repeat_dims),
-            ],
-            dim=0,
-        )
-        param_state["exp_avg_sq"] = torch.cat(
-            [
-                param_state["exp_avg_sq"],
-                torch.zeros_like(param_state["exp_avg_sq"][dup_mask.squeeze()]).repeat(*repeat_dims),
-            ],
-            dim=0,
-        )
+        if "exp_avg" in param_state:
+            repeat_dims = (n,) + tuple(1 for _ in range(param_state["exp_avg"].dim() - 1))
+            param_state["exp_avg"] = torch.cat(
+                [
+                    param_state["exp_avg"],
+                    torch.zeros_like(param_state["exp_avg"][dup_mask.squeeze()]).repeat(*repeat_dims),
+                ],
+                dim=0,
+            )
+            param_state["exp_avg_sq"] = torch.cat(
+                [
+                    param_state["exp_avg_sq"],
+                    torch.zeros_like(param_state["exp_avg_sq"][dup_mask.squeeze()]).repeat(*repeat_dims),
+                ],
+                dim=0,
+            )
         del optimizer.state[param]
         optimizer.state[new_params[0]] = param_state
         optimizer.param_groups[0]["params"] = new_params
         del param
 
     def dup_in_all_optim(self, optimizers, dup_mask, n):
         param_groups = self.get_gaussian_param_groups()
@@ -398,59 +419,30 @@
                 avg_grad_norm = (self.xys_grad_norm / self.vis_counts) * 0.5 * max(self.last_size[0], self.last_size[1])
                 high_grads = (avg_grad_norm > self.config.densify_grad_thresh).squeeze()
                 splits = (self.scales.exp().max(dim=-1).values > self.config.densify_size_thresh).squeeze()
                 if self.step < self.config.stop_screen_size_at:
                     splits |= (self.max_2Dsize > self.config.split_screen_size).squeeze()
                 splits &= high_grads
                 nsamps = self.config.n_split_samples
-                (
-                    split_means,
-                    split_features_dc,
-                    split_features_rest,
-                    split_opacities,
-                    split_scales,
-                    split_quats,
-                ) = self.split_gaussians(splits, nsamps)
+                split_params = self.split_gaussians(splits, nsamps)
 
                 dups = (self.scales.exp().max(dim=-1).values <= self.config.densify_size_thresh).squeeze()
                 dups &= high_grads
-                (
-                    dup_means,
-                    dup_features_dc,
-                    dup_features_rest,
-                    dup_opacities,
-                    dup_scales,
-                    dup_quats,
-                ) = self.dup_gaussians(dups)
-                self.means = Parameter(torch.cat([self.means.detach(), split_means, dup_means], dim=0))
-                self.features_dc = Parameter(
-                    torch.cat(
-                        [self.features_dc.detach(), split_features_dc, dup_features_dc],
-                        dim=0,
+                dup_params = self.dup_gaussians(dups)
+                for name, param in self.gauss_params.items():
+                    self.gauss_params[name] = torch.nn.Parameter(
+                        torch.cat([param.detach(), split_params[name], dup_params[name]], dim=0)
                     )
-                )
-                self.features_rest = Parameter(
-                    torch.cat(
-                        [
-                            self.features_rest.detach(),
-                            split_features_rest,
-                            dup_features_rest,
-                        ],
-                        dim=0,
-                    )
-                )
-                self.opacities = Parameter(torch.cat([self.opacities.detach(), split_opacities, dup_opacities], dim=0))
-                self.scales = Parameter(torch.cat([self.scales.detach(), split_scales, dup_scales], dim=0))
-                self.quats = Parameter(torch.cat([self.quats.detach(), split_quats, dup_quats], dim=0))
+
                 # append zeros to the max_2Dsize tensor
                 self.max_2Dsize = torch.cat(
                     [
                         self.max_2Dsize,
-                        torch.zeros_like(split_scales[:, 0]),
-                        torch.zeros_like(dup_scales[:, 0]),
+                        torch.zeros_like(split_params["scales"][:, 0]),
+                        torch.zeros_like(dup_params["scales"][:, 0]),
                     ],
                     dim=0,
                 )
 
                 split_idcs = torch.where(splits)[0]
                 self.dup_in_all_optim(optimizers, split_idcs, nsamps)
 
@@ -483,15 +475,15 @@
                 # Reset value is set to be twice of the cull_alpha_thresh
                 reset_value = self.config.cull_alpha_thresh * 2.0
                 self.opacities.data = torch.clamp(
                     self.opacities.data,
                     max=torch.logit(torch.tensor(reset_value, device=self.device)).item(),
                 )
                 # reset the exp of optimizer
-                optim = optimizers.optimizers["opacity"]
+                optim = optimizers.optimizers["opacities"]
                 param = optim.param_groups[0]["params"][0]
                 param_state = optim.state[param]
                 param_state["exp_avg"] = torch.zeros_like(param_state["exp_avg"])
                 param_state["exp_avg_sq"] = torch.zeros_like(param_state["exp_avg_sq"])
 
             self.xys_grad_norm = None
             self.vis_counts = None
@@ -514,33 +506,28 @@
             toobigs = (torch.exp(self.scales).max(dim=-1).values > self.config.cull_scale_thresh).squeeze()
             if self.step < self.config.stop_screen_size_at:
                 # cull big screen space
                 assert self.max_2Dsize is not None
                 toobigs = toobigs | (self.max_2Dsize > self.config.cull_screen_size).squeeze()
             culls = culls | toobigs
             toobigs_count = torch.sum(toobigs).item()
-        self.means = Parameter(self.means[~culls].detach())
-        self.scales = Parameter(self.scales[~culls].detach())
-        self.quats = Parameter(self.quats[~culls].detach())
-        self.features_dc = Parameter(self.features_dc[~culls].detach())
-        self.features_rest = Parameter(self.features_rest[~culls].detach())
-        self.opacities = Parameter(self.opacities[~culls].detach())
+        for name, param in self.gauss_params.items():
+            self.gauss_params[name] = torch.nn.Parameter(param[~culls])
 
         CONSOLE.log(
             f"Culled {n_bef - self.num_points} gaussians "
             f"({below_alpha_count} below alpha thresh, {toobigs_count} too bigs, {self.num_points} remaining)"
         )
 
         return culls
 
     def split_gaussians(self, split_mask, samps):
         """
         This function splits gaussians that are too large
         """
-
         n_splits = split_mask.sum().item()
         CONSOLE.log(f"Splitting {split_mask.sum().item()/self.num_points} gaussians: {n_splits}/{self.num_points}")
         centered_samples = torch.randn((samps * n_splits, 3), device=self.device)  # Nx3 of axis-aligned scales
         scaled_samples = (
             torch.exp(self.scales[split_mask].repeat(samps, 1)) * centered_samples
         )  # how these scales are rotated
         quats = self.quats[split_mask] / self.quats[split_mask].norm(dim=-1, keepdim=True)  # normalize them first
@@ -554,47 +541,37 @@
         new_opacities = self.opacities[split_mask].repeat(samps, 1)
         # step 4, sample new scales
         size_fac = 1.6
         new_scales = torch.log(torch.exp(self.scales[split_mask]) / size_fac).repeat(samps, 1)
         self.scales[split_mask] = torch.log(torch.exp(self.scales[split_mask]) / size_fac)
         # step 5, sample new quats
         new_quats = self.quats[split_mask].repeat(samps, 1)
-        return (
-            new_means,
-            new_features_dc,
-            new_features_rest,
-            new_opacities,
-            new_scales,
-            new_quats,
-        )
+        out = {
+            "means": new_means,
+            "features_dc": new_features_dc,
+            "features_rest": new_features_rest,
+            "opacities": new_opacities,
+            "scales": new_scales,
+            "quats": new_quats,
+        }
+        for name, param in self.gauss_params.items():
+            if name not in out:
+                out[name] = param[split_mask].repeat(samps, 1)
+        return out
 
     def dup_gaussians(self, dup_mask):
         """
         This function duplicates gaussians that are too small
         """
         n_dups = dup_mask.sum().item()
         CONSOLE.log(f"Duplicating {dup_mask.sum().item()/self.num_points} gaussians: {n_dups}/{self.num_points}")
-        dup_means = self.means[dup_mask]
-        dup_features_dc = self.features_dc[dup_mask]
-        dup_features_rest = self.features_rest[dup_mask]
-        dup_opacities = self.opacities[dup_mask]
-        dup_scales = self.scales[dup_mask]
-        dup_quats = self.quats[dup_mask]
-        return (
-            dup_means,
-            dup_features_dc,
-            dup_features_rest,
-            dup_opacities,
-            dup_scales,
-            dup_quats,
-        )
-
-    @property
-    def num_points(self):
-        return self.means.shape[0]
+        new_dups = {}
+        for name, param in self.gauss_params.items():
+            new_dups[name] = param[dup_mask]
+        return new_dups
 
     def get_training_callbacks(
         self, training_callback_attributes: TrainingCallbackAttributes
     ) -> List[TrainingCallback]:
         cbs = []
         cbs.append(TrainingCallback([TrainingCallbackLocation.BEFORE_TRAIN_ITERATION], self.step_cb))
         # The order of these matters
@@ -614,21 +591,19 @@
         )
         return cbs
 
     def step_cb(self, step):
         self.step = step
 
     def get_gaussian_param_groups(self) -> Dict[str, List[Parameter]]:
+        # Here we explicitly use the means, scales as parameters so that the user can override this function and
+        # specify more if they want to add more optimizable params to gaussians.
         return {
-            "xyz": [self.means],
-            "features_dc": [self.features_dc],
-            "features_rest": [self.features_rest],
-            "opacity": [self.opacities],
-            "scaling": [self.scales],
-            "rotation": [self.quats],
+            name: [self.gauss_params[name]]
+            for name in ["means", "scales", "quats", "features_dc", "features_rest", "opacities"]
         }
 
     def get_param_groups(self) -> Dict[str, List[Parameter]]:
         """Obtain the parameter groups for the optimizers
 
         Returns:
             Mapping of different parameter groups
@@ -709,19 +684,16 @@
         T_inv = -R_inv @ T
         viewmat = torch.eye(4, device=R.device, dtype=R.dtype)
         viewmat[:3, :3] = R_inv
         viewmat[:3, 3:4] = T_inv
         # calculate the FOV of the camera given fx and fy, width and height
         cx = camera.cx.item()
         cy = camera.cy.item()
-        fovx = 2 * math.atan(camera.width / (2 * camera.fx))
-        fovy = 2 * math.atan(camera.height / (2 * camera.fy))
         W, H = int(camera.width.item()), int(camera.height.item())
         self.last_size = (H, W)
-        projmat = projection_matrix(0.001, 1000, fovx, fovy, device=self.device)
 
         if crop_ids is not None:
             opacities_crop = self.opacities[crop_ids]
             means_crop = self.means[crop_ids]
             features_dc_crop = self.features_dc[crop_ids]
             features_rest_crop = self.features_rest[crop_ids]
             scales_crop = self.scales[crop_ids]
@@ -738,15 +710,14 @@
         BLOCK_WIDTH = 16  # this controls the tile size of rasterization, 16 is a good default
         self.xys, depths, self.radii, conics, comp, num_tiles_hit, cov3d = project_gaussians(  # type: ignore
             means_crop,
             torch.exp(scales_crop),
             1,
             quats_crop / quats_crop.norm(dim=-1, keepdim=True),
             viewmat.squeeze()[:3, :],
-            projmat.squeeze() @ viewmat.squeeze(),
             camera.fx.item(),
             camera.fy.item(),
             cx,
             cy,
             H,
             W,
             BLOCK_WIDTH,
@@ -807,15 +778,15 @@
             depth_im = rasterize_gaussians(  # type: ignore
                 self.xys,
                 depths,
                 self.radii,
                 conics,
                 num_tiles_hit,  # type: ignore
                 depths[:, None].repeat(1, 3),
-                torch.sigmoid(opacities_crop),
+                opacities,
                 H,
                 W,
                 BLOCK_WIDTH,
                 background=torch.zeros(3, device=self.device),
             )[..., 0:1]  # type: ignore
             depth_im = torch.where(alpha > 0, depth_im / alpha, depth_im.detach().max())
```

### Comparing `nerfstudio-1.0.2/nerfstudio/models/tensorf.py` & `nerfstudio-1.0.3/nerfstudio/models/tensorf.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
 
         outputs = {"rgb": rgb, "accumulation": accumulation, "depth": depth}
         return outputs
 
     def get_loss_dict(self, outputs, batch, metrics_dict=None) -> Dict[str, torch.Tensor]:
         # Scaling metrics by coefficients to create the losses.
         device = outputs["rgb"].device
-        image = batch["image"][..., :3].to(device)
+        image = batch["image"].to(device)
         pred_image, image = self.renderer_rgb.blend_background_for_loss_computation(
             pred_image=outputs["rgb"],
             pred_accumulation=outputs["accumulation"],
             gt_image=image,
         )
 
         rgb_loss = self.rgb_loss(image, pred_image)
```

### Comparing `nerfstudio-1.0.2/nerfstudio/models/vanilla_nerf.py` & `nerfstudio-1.0.3/nerfstudio/models/vanilla_nerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/pipelines/__init__.py` & `nerfstudio-1.0.3/nerfstudio/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/pipelines/base_pipeline.py` & `nerfstudio-1.0.3/nerfstudio/pipelines/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/pipelines/dynamic_batch.py` & `nerfstudio-1.0.3/nerfstudio/pipelines/dynamic_batch.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/plugins/__init__.py` & `nerfstudio-1.0.3/nerfstudio/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/plugins/registry.py` & `nerfstudio-1.0.3/nerfstudio/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/plugins/registry_dataparser.py` & `nerfstudio-1.0.3/nerfstudio/plugins/registry_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/plugins/types.py` & `nerfstudio-1.0.3/nerfstudio/plugins/types.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/__init__.py` & `nerfstudio-1.0.3/nerfstudio/process_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py` & `nerfstudio-1.0.3/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py` & `nerfstudio-1.0.3/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from nerfstudio.utils.rich_utils import CONSOLE
 
 
 @dataclass
 class ColmapConverterToNerfstudioDataset(BaseConverterToNerfstudioDataset):
     """Base class to process images or video into a nerfstudio dataset using colmap"""
 
-    camera_type: Literal["perspective", "fisheye", "equirectangular"] = "perspective"
+    camera_type: Literal["perspective", "fisheye", "equirectangular", "pinhole", "simple_pinhole"] = "perspective"
     """Camera model to use."""
     matching_method: Literal["exhaustive", "sequential", "vocab_tree"] = "vocab_tree"
     """Feature matching method to use. Vocab tree is recommended for a balance of speed
     and accuracy. Exhaustive is slower but more accurate. Sequential is faster but
     should only be used for videos."""
     sfm_tool: Literal["any", "colmap", "hloc"] = "any"
     """Structure from motion tool to use. Colmap will use sift features, hloc can use
```

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/colmap_utils.py` & `nerfstudio-1.0.3/nerfstudio/process_data/colmap_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/equirect_utils.py` & `nerfstudio-1.0.3/nerfstudio/process_data/equirect_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/hloc_utils.py` & `nerfstudio-1.0.3/nerfstudio/process_data/hloc_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/images_to_nerfstudio_dataset.py` & `nerfstudio-1.0.3/nerfstudio/process_data/images_to_nerfstudio_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,17 @@
                     verbose=self.verbose,
                     num_downscales=self.num_downscales,
                     same_dimensions=self.same_dimensions,
                     keep_image_dir=True,
                 )
                 image_rename_map_paths.update(eval_image_rename_map_paths)
 
-            image_rename_map = dict((a.name, b.name) for a, b in image_rename_map_paths.items())
+            image_rename_map = dict(
+                (a.relative_to(self.data).as_posix(), b.name) for a, b in image_rename_map_paths.items()
+            )
             num_frames = len(image_rename_map)
             summary_log.append(f"Starting with {num_frames} images")
 
             # # Create mask
             mask_path = process_data_utils.save_mask(
                 image_dir=self.image_dir,
                 num_downscales=self.num_downscales,
```

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/metashape_utils.py` & `nerfstudio-1.0.3/nerfstudio/process_data/metashape_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/odm_utils.py` & `nerfstudio-1.0.3/nerfstudio/process_data/odm_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/polycam_utils.py` & `nerfstudio-1.0.3/nerfstudio/process_data/polycam_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/process_data_utils.py` & `nerfstudio-1.0.3/nerfstudio/process_data/process_data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,24 +45,28 @@
 
 class CameraModel(Enum):
     """Enum for camera types."""
 
     OPENCV = "OPENCV"
     OPENCV_FISHEYE = "OPENCV_FISHEYE"
     EQUIRECTANGULAR = "EQUIRECTANGULAR"
+    PINHOLE = "PINHOLE"
+    SIMPLE_PINHOLE = "SIMPLE_PINHOLE"
 
 
 CAMERA_MODELS = {
     "perspective": CameraModel.OPENCV,
     "fisheye": CameraModel.OPENCV_FISHEYE,
     "equirectangular": CameraModel.EQUIRECTANGULAR,
+    "pinhole": CameraModel.PINHOLE,
+    "simple_pinhole": CameraModel.SIMPLE_PINHOLE,
 }
 
 
-def list_images(data: Path, recursive: bool = False) -> List[Path]:
+def list_images(data: Path, recursive: bool = True) -> List[Path]:
     """Lists all supported images in a directory
 
     Args:
         data: Path to the directory of images.
         recursive: Whether to search check nested folders in `data`.
     Returns:
         Paths to images contained in the directory
```

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/realitycapture_utils.py` & `nerfstudio-1.0.3/nerfstudio/process_data/realitycapture_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/record3d_utils.py` & `nerfstudio-1.0.3/nerfstudio/process_data/record3d_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/process_data/video_to_nerfstudio_dataset.py` & `nerfstudio-1.0.3/nerfstudio/process_data/video_to_nerfstudio_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/__init__.py` & `nerfstudio-1.0.3/nerfstudio/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/blender/__init__.py` & `nerfstudio-1.0.3/nerfstudio/scripts/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/blender/nerfstudio_blender.py` & `nerfstudio-1.0.3/nerfstudio/scripts/blender/nerfstudio_blender.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/completions/__init__.py` & `nerfstudio-1.0.3/nerfstudio/scripts/completions/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/completions/install.py` & `nerfstudio-1.0.3/nerfstudio/scripts/completions/install.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/completions/setup.zsh` & `nerfstudio-1.0.3/nerfstudio/scripts/completions/setup.zsh`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/datasets/process_nuscenes_masks.py` & `nerfstudio-1.0.3/nerfstudio/scripts/datasets/process_nuscenes_masks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/datasets/process_project_aria.py` & `nerfstudio-1.0.3/nerfstudio/scripts/datasets/process_project_aria.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,14 +219,19 @@
             "camera_model": ARIA_CAMERA_MODEL,
             "frames": [to_nerfstudio_frame(frame) for frame in aria_frames],
             "fisheye_crop_radius": rgb_valid_radius,
         }
 
         # save global point cloud, which is useful for Gaussian Splatting.
         points_path = self.mps_data_dir / "global_points.csv.gz"
+        if not points_path.exists():
+            # MPS point cloud output was renamed in Aria's December 4th, 2023 update.
+            # https://facebookresearch.github.io/projectaria_tools/docs/ARK/sw_release_notes#project-aria-updates-aria-mobile-app-v140-and-changes-to-mps
+            points_path = self.mps_data_dir / "semidense_points.csv.gz"
+
         if points_path.exists():
             print("Found global points, saving to PLY...")
             points_data = mps.read_global_point_cloud(str(points_path))  # type: ignore
             points_data = filter_points_from_confidence(points_data)
             pcd = o3d.geometry.PointCloud()
             pcd.points = o3d.utility.Vector3dVector(np.array([cast(Any, it).position_world for it in points_data]))
             ply_file_path = self.output_dir / "global_points.ply"
```

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/docs/__init__.py` & `nerfstudio-1.0.3/nerfstudio/scripts/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/docs/add_nb_tags.py` & `nerfstudio-1.0.3/nerfstudio/scripts/docs/add_nb_tags.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/docs/build_docs.py` & `nerfstudio-1.0.3/nerfstudio/scripts/docs/build_docs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/downloads/__init__.py` & `nerfstudio-1.0.3/nerfstudio/scripts/downloads/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/downloads/download_data.py` & `nerfstudio-1.0.3/nerfstudio/scripts/downloads/download_data.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/downloads/eyeful_tower.py` & `nerfstudio-1.0.3/nerfstudio/scripts/downloads/eyeful_tower.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/downloads/utils.py` & `nerfstudio-1.0.3/nerfstudio/scripts/downloads/utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/eval.py` & `nerfstudio-1.0.3/nerfstudio/scripts/eval.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/exporter.py` & `nerfstudio-1.0.3/nerfstudio/scripts/exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 from __future__ import annotations
 
 import json
 import os
 import sys
+from collections import OrderedDict
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import List, Optional, Tuple, Union, cast
 
 import numpy as np
 import open3d as o3d
 import torch
@@ -478,33 +479,83 @@
 
 @dataclass
 class ExportGaussianSplat(Exporter):
     """
     Export 3D Gaussian Splatting model to a .ply
     """
 
+    @staticmethod
+    def write_ply(filename: str, count: int, map_to_tensors: OrderedDict[str, np.ndarray]):
+        """
+        Writes a PLY file with given vertex properties and their float values in the order specified by the OrderedDict.
+        Note: All float values will be converted to float32 for writing.
+
+        Parameters:
+        filename (str): The name of the file to write.
+        count (int): The number of vertices to write.
+        map_to_tensors (OrderedDict[str, np.ndarray]): An ordered dictionary mapping property names to numpy arrays of float values.
+            Each array should be 1-dimensional and of equal length matching 'count'. Arrays should not be empty.
+        """
+
+        # Ensure count matches the length of all tensors
+        if not all(len(tensor) == count for tensor in map_to_tensors.values()):
+            raise ValueError("Count does not match the length of all tensors")
+
+        # Type check for numpy arrays of type float and non-empty
+        if not all(
+            isinstance(tensor, np.ndarray) and tensor.dtype.kind in ["f", "d"] and tensor.size > 0
+            for tensor in map_to_tensors.values()
+        ):
+            raise ValueError("All tensors must be numpy arrays of float type and not empty")
+
+        with open(filename, "wb") as ply_file:
+            # Write PLY header
+            ply_file.write(b"ply\n")
+            ply_file.write(b"format binary_little_endian 1.0\n")
+
+            ply_file.write(f"element vertex {count}\n".encode())
+
+            # Write properties, in order due to OrderedDict
+            for key in map_to_tensors.keys():
+                ply_file.write(f"property float {key}\n".encode())
+
+            ply_file.write(b"end_header\n")
+
+            # Write binary data
+            # Note: If this is a perfromance bottleneck consider using numpy.hstack for efficiency improvement
+            for i in range(count):
+                for tensor in map_to_tensors.values():
+                    value = tensor[i]
+                    ply_file.write(np.float32(value).tobytes())
+
     def main(self) -> None:
         if not self.output_dir.exists():
             self.output_dir.mkdir(parents=True)
 
         _, pipeline, _, _ = eval_setup(self.load_config)
 
         assert isinstance(pipeline.model, SplatfactoModel)
 
         model: SplatfactoModel = pipeline.model
 
         filename = self.output_dir / "splat.ply"
 
-        map_to_tensors = {}
+        count = 0
+        map_to_tensors = OrderedDict()
 
         with torch.no_grad():
             positions = model.means.cpu().numpy()
-            n = positions.shape[0]
-            map_to_tensors["positions"] = positions
-            map_to_tensors["normals"] = np.zeros_like(positions, dtype=np.float32)
+            count = positions.shape[0]
+            n = count
+            map_to_tensors["x"] = positions[:, 0]
+            map_to_tensors["y"] = positions[:, 1]
+            map_to_tensors["z"] = positions[:, 2]
+            map_to_tensors["nx"] = np.zeros(n, dtype=np.float32)
+            map_to_tensors["ny"] = np.zeros(n, dtype=np.float32)
+            map_to_tensors["nz"] = np.zeros(n, dtype=np.float32)
 
             if model.config.sh_degree > 0:
                 shs_0 = model.shs_0.contiguous().cpu().numpy()
                 for i in range(shs_0.shape[1]):
                     map_to_tensors[f"f_dc_{i}"] = shs_0[:, i, None]
 
                 # transpose(1, 2) was needed to match the sh order in Inria version
@@ -527,27 +578,26 @@
                 map_to_tensors[f"rot_{i}"] = quats[:, i, None]
 
         # post optimization, it is possible have NaN/Inf values in some attributes
         # to ensure the exported ply file has finite values, we enforce finite filters.
         select = np.ones(n, dtype=bool)
         for k, t in map_to_tensors.items():
             n_before = np.sum(select)
-            select = np.logical_and(select, np.isfinite(t).all(axis=1))
+            select = np.logical_and(select, np.isfinite(t).all(axis=-1))
             n_after = np.sum(select)
             if n_after < n_before:
                 CONSOLE.print(f"{n_before - n_after} NaN/Inf elements in {k}")
 
         if np.sum(select) < n:
             CONSOLE.print(f"values have NaN/Inf in map_to_tensors, only export {np.sum(select)}/{n}")
             for k, t in map_to_tensors.items():
-                map_to_tensors[k] = map_to_tensors[k][select, :]
-
-        pcd = o3d.t.geometry.PointCloud(map_to_tensors)
+                map_to_tensors[k] = map_to_tensors[k][select]
+            count = np.sum(select)
 
-        o3d.t.io.write_point_cloud(str(filename), pcd)
+        ExportGaussianSplat.write_ply(str(filename), count, map_to_tensors)
 
 
 Commands = tyro.conf.FlagConversionOff[
     Union[
         Annotated[ExportPointCloud, tyro.conf.subcommand(name="pointcloud")],
         Annotated[ExportTSDFMesh, tyro.conf.subcommand(name="tsdf")],
         Annotated[ExportPoissonMesh, tyro.conf.subcommand(name="poisson")],
```

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/github/__init__.py` & `nerfstudio-1.0.3/nerfstudio/scripts/github/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/github/run_actions.py` & `nerfstudio-1.0.3/nerfstudio/scripts/github/run_actions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/process_data.py` & `nerfstudio-1.0.3/nerfstudio/scripts/process_data.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/render.py` & `nerfstudio-1.0.3/nerfstudio/scripts/render.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/texture.py` & `nerfstudio-1.0.3/nerfstudio/scripts/texture.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/train.py` & `nerfstudio-1.0.3/nerfstudio/scripts/train.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/viewer/__init__.py` & `nerfstudio-1.0.3/nerfstudio/scripts/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/viewer/run_viewer.py` & `nerfstudio-1.0.3/nerfstudio/scripts/viewer/run_viewer.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/scripts/viewer/sync_viser_message_defs.py` & `nerfstudio-1.0.3/nerfstudio/scripts/viewer/sync_viser_message_defs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/__init__.py` & `nerfstudio-1.0.3/nerfstudio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/colormaps.py` & `nerfstudio-1.0.3/nerfstudio/utils/colormaps.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/colors.py` & `nerfstudio-1.0.3/nerfstudio/utils/colors.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/comms.py` & `nerfstudio-1.0.3/nerfstudio/utils/comms.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/decorators.py` & `nerfstudio-1.0.3/nerfstudio/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/eval_utils.py` & `nerfstudio-1.0.3/nerfstudio/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/external.py` & `nerfstudio-1.0.3/nerfstudio/utils/external.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/install_checks.py` & `nerfstudio-1.0.3/nerfstudio/utils/install_checks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/io.py` & `nerfstudio-1.0.3/nerfstudio/utils/io.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/math.py` & `nerfstudio-1.0.3/nerfstudio/utils/math.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/misc.py` & `nerfstudio-1.0.3/nerfstudio/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/plotly_utils.py` & `nerfstudio-1.0.3/nerfstudio/utils/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/poses.py` & `nerfstudio-1.0.3/nerfstudio/utils/poses.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/printing.py` & `nerfstudio-1.0.3/nerfstudio/utils/printing.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/profiler.py` & `nerfstudio-1.0.3/nerfstudio/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/rich_utils.py` & `nerfstudio-1.0.3/nerfstudio/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/scripts.py` & `nerfstudio-1.0.3/nerfstudio/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/tensor_dataclass.py` & `nerfstudio-1.0.3/nerfstudio/utils/tensor_dataclass.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/utils/writer.py` & `nerfstudio-1.0.3/nerfstudio/utils/writer.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/__init__.py` & `nerfstudio-1.0.3/nerfstudio/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/control_panel.py` & `nerfstudio-1.0.3/nerfstudio/viewer/control_panel.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/export_panel.py` & `nerfstudio-1.0.3/nerfstudio/viewer/export_panel.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/render_panel.py` & `nerfstudio-1.0.3/nerfstudio/viewer/render_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 import json
 import threading
 import time
 from pathlib import Path
 from typing import Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
-import scipy
 import splines
 import splines.quaternion
 import viser
 import viser.transforms as tf
+from scipy import interpolate
 
 from nerfstudio.viewer.control_panel import ControlPanel
 
 
 @dataclasses.dataclass
 class Keyframe:
     position: np.ndarray
@@ -262,27 +262,27 @@
         """
         transition_times_cumsum = self.compute_transition_times_cumsum()
         spline_indices = np.arange(transition_times_cumsum.shape[0])
 
         if self.loop:
             # In the case of a loop, we pad the spline to match the start/end
             # slopes.
-            interpolator = scipy.interpolate.PchipInterpolator(
+            interpolator = interpolate.PchipInterpolator(
                 x=np.concatenate(
                     [
                         [-(transition_times_cumsum[-1] - transition_times_cumsum[-2])],
                         transition_times_cumsum,
                         transition_times_cumsum[-1:] + transition_times_cumsum[1:2],
                     ],
                     axis=0,
                 ),
                 y=np.concatenate([[-1], spline_indices, [spline_indices[-1] + 1]], axis=0),
             )
         else:
-            interpolator = scipy.interpolate.PchipInterpolator(x=transition_times_cumsum, y=spline_indices)
+            interpolator = interpolate.PchipInterpolator(x=transition_times_cumsum, y=spline_indices)
 
         # Clip to account for floating point error.
         return np.clip(interpolator(time), 0, spline_indices[-1])
 
     def interpolate_pose_and_fov_rad(
         self, normalized_t: float
     ) -> Optional[Union[Tuple[tf.SE3, float], Tuple[tf.SE3, float, float]]]:
```

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/render_state_machine.py` & `nerfstudio-1.0.3/nerfstudio/viewer/render_state_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
         )
         self.client.set_background_image(
             selected_output,
             format=self.viewer.config.image_format,
             jpeg_quality=jpg_quality,
             depth=depth,
         )
-        res = f"{selected_output.shape[0]}x{selected_output.shape[1]}px"
+        res = f"{selected_output.shape[1]}x{selected_output.shape[0]}px"
         self.viewer.stats_markdown.content = self.viewer.make_stats_markdown(None, res)
 
     def _calculate_image_res(self, aspect_ratio: float) -> Tuple[int, int]:
         """Calculate the maximum image height that can be rendered in the time budget
 
         Args:
             apect_ratio: the aspect ratio of the current view
```

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/server/__init__.py` & `nerfstudio-1.0.3/nerfstudio/viewer/server/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/server/viewer_elements.py` & `nerfstudio-1.0.3/nerfstudio/viewer/server/viewer_elements.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/utils.py` & `nerfstudio-1.0.3/nerfstudio/viewer/utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/viewer.py` & `nerfstudio-1.0.3/nerfstudio/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer/viewer_elements.py` & `nerfstudio-1.0.3/nerfstudio/viewer/viewer_elements.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 
 """ Viewer GUI elements for the nerfstudio viewer """
 
 
 from __future__ import annotations
 
+import warnings
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Callable, Generic, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Generic, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import torch
 import viser.transforms as vtf
 from typing_extensions import LiteralString, TypeVar
 from viser import (
     GuiButtonGroupHandle,
@@ -32,14 +33,15 @@
     GuiDropdownHandle,
     GuiInputHandle,
     ScenePointerEvent,
     ViserServer,
 )
 
 from nerfstudio.cameras.cameras import Cameras, CameraType
+from nerfstudio.utils.rich_utils import CONSOLE
 from nerfstudio.viewer.utils import CameraState, get_camera
 
 if TYPE_CHECKING:
     from nerfstudio.viewer.viewer import Viewer
 
 TValue = TypeVar("TValue")
 TString = TypeVar("TString", default=str, bound=str)
@@ -56,25 +58,38 @@
     origin: Tuple[float, float, float]
     """The origin of the click in world coordinates (center of camera)"""
     direction: Tuple[float, float, float]
     """
     The direction of the click if projected from the camera through the clicked pixel,
     in world coordinates
     """
+    screen_pos: Tuple[float, float]
+    """The screen position of the click in OpenCV screen coordinates, normalized to [0, 1]"""
+
+
+@dataclass
+class ViewerRectSelect:
+    """
+    Class representing a rectangle selection in the viewer (screen-space).
+
+    The screen coordinates follow OpenCV image coordinates, with the origin at the top-left corner,
+    but the bounds are also normalized to [0, 1] in both dimensions.
+    """
+
+    min_bounds: Tuple[float, float]
+    """The minimum bounds of the rectangle selection in screen coordinates."""
+    max_bounds: Tuple[float, float]
+    """The maximum bounds of the rectangle selection in screen coordinates."""
 
 
 class ViewerControl:
     """
     class for exposing non-gui controls of the viewer to the user
     """
 
-    def __init__(self):
-        # this should be a user-facing constructor, since it will be used inside the model/pipeline class
-        self._click_cbs = {}
-
     def _setup(self, viewer: Viewer):
         """
         Internal use only, setup the viewer control with the viewer state object
 
         Args:
             viewer: The viewer object (viewer.py)
         """
@@ -143,50 +158,91 @@
         c2w = torch.concatenate([R, pos[:, None]], dim=1)
         camera_state = CameraState(
             fov=client.camera.fov, aspect=client.camera.aspect, c2w=c2w, camera_type=CameraType.PERSPECTIVE
         )
         return get_camera(camera_state, img_height, img_width)
 
     def register_click_cb(self, cb: Callable):
+        """Deprecated, use register_pointer_cb instead."""
+        CONSOLE.log("`register_click_cb` is deprecated, use `register_pointer_cb` instead.")
+        self.register_pointer_cb("click", cb)
+
+    def register_pointer_cb(
+        self, event_type: Literal["click", "rect-select"], cb: Callable, done_cb: Optional[Callable] = None
+    ):
         """
-        Add a callback which will be called when a click is detected in the viewer.
+        Add a callback which will be called when a scene pointer event is detected in the viewer.
+        Scene pointer events include:
+        - "click": A click event, which includes the origin and direction of the click
+        - "rect-select": A rectangle selection event, which includes the screen bounds of the box selection
+
+        The callback should take a ViewerClick object as an argument if the event type is "click",
+        and a ViewerRectSelect object as an argument if the event type is "rect-select".
 
         Args:
-            cb: The callback to call when a click is detected.
-                The callback should take a ViewerClick object as an argument
+            cb: The callback to call when a click or a rect-select is detected.
         """
         from nerfstudio.viewer.viewer import VISER_NERFSTUDIO_SCALE_RATIO
 
         def wrapped_cb(scene_pointer_msg: ScenePointerEvent):
-            # only call the callback if the event is a click
-            if scene_pointer_msg.event != "click":
-                return
-            origin = scene_pointer_msg.ray_origin
-            direction = scene_pointer_msg.ray_direction
-
-            origin = tuple([x / VISER_NERFSTUDIO_SCALE_RATIO for x in origin])
-            assert len(origin) == 3
-
-            click = ViewerClick(origin, direction)
-            cb(click)
+            # Check that the event type is the same as the one we are interested in.
+            if scene_pointer_msg.event_type != event_type:
+                raise ValueError(f"Expected event type {event_type}, got {scene_pointer_msg.event_type}")
+
+            if scene_pointer_msg.event_type == "click":
+                origin = scene_pointer_msg.ray_origin
+                direction = scene_pointer_msg.ray_direction
+                screen_pos = scene_pointer_msg.screen_pos[0]
+                assert (origin is not None) and (
+                    direction is not None
+                ), "Origin and direction should not be None for click event."
+                origin = tuple([x / VISER_NERFSTUDIO_SCALE_RATIO for x in origin])
+                assert len(origin) == 3
+                pointer_event = ViewerClick(origin, direction, screen_pos)
+            elif scene_pointer_msg.event_type == "rect-select":
+                pointer_event = ViewerRectSelect(scene_pointer_msg.screen_pos[0], scene_pointer_msg.screen_pos[1])
+            else:
+                raise ValueError(f"Unknown event type: {scene_pointer_msg.event_type}")
+
+            cb(pointer_event)
+
+        cb_overriden = False
+        with warnings.catch_warnings(record=True) as w:
+            # Register the callback with the viser server.
+            self.viser_server.on_scene_pointer(event_type=event_type)(wrapped_cb)
+            # If there exists a warning, it's because a callback was overriden.
+            cb_overriden = len(w) > 0
+
+        if cb_overriden:
+            warnings.warn(
+                "A ScenePointer callback has already been registered for this event type. "
+                "The new callback will override the existing one."
+            )
+
+        # If there exists a cleanup callback after the pointer event is done, register it.
+        if done_cb:
+            self.viser_server.on_scene_pointer_done(done_cb)
+
+    def unregister_click_cb(self, cb: Optional[Callable] = None):
+        """Deprecated, use unregister_pointer_cb instead. `cb` is ignored."""
+        warnings.warn("`unregister_click_cb` is deprecated, use `unregister_pointer_cb` instead.")
+        if cb is not None:
+            # raise warning
+            warnings.warn("cb argument is ignored in unregister_click_cb.")
 
-        self._click_cbs[cb] = wrapped_cb
-        self.viser_server.on_scene_click(wrapped_cb)
+        self.unregister_pointer_cb()
 
-    def unregister_click_cb(self, cb: Callable):
+    def unregister_pointer_cb(self):
         """
-        Remove a callback which will be called when a click is detected in the viewer.
+        Remove a callback which will be called, when a scene pointer event is detected in the viewer.
 
         Args:
             cb: The callback to remove
         """
-        if cb not in self._click_cbs:
-            raise ValueError(f"Callback {cb} not registered, cannot remove")
-        self.viser_server.remove_scene_click_callback(self._click_cbs[cb])
-        self._click_cbs.pop(cb)
+        self.viser_server.remove_scene_pointer_callback()
 
     @property
     def server(self):
         return self.viser_server
 
 
 class ViewerElement(Generic[TValue]):
```

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/__init__.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/package.json` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/package.json`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/run_deploy.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/run_deploy.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/app/src/themes/leva_theme.json` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/src/themes/leva_theme.json`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/__init__.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/control_panel.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/control_panel.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/gui_utils.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/gui_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/path.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/path.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/render_state_machine.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/render_state_machine.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/state/node.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/state/state_node.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/state_node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/utils.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/viewer_elements.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_elements.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/viewer_state.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_state.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/server/viewer_utils.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/__init__.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/gui.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/gui.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/message_api.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/message_api.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/messages.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/messages.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio/viewer_legacy/viser/server.py` & `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/server.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio.egg-info/PKG-INFO` & `nerfstudio-1.0.3/nerfstudio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 1.0.2
+Version: 1.0.3
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
 Requires-Dist: matplotlib>=3.6.0
 Requires-Dist: mediapy>=1.1.0
 Requires-Dist: msgpack>=1.0.4
 Requires-Dist: msgpack_numpy>=0.4.8
 Requires-Dist: nerfacc==0.5.2
 Requires-Dist: open3d>=0.16.0
 Requires-Dist: opencv-python==4.8.0.76
-Requires-Dist: Pillow>=9.3.0
+Requires-Dist: Pillow>=10.3.0
 Requires-Dist: plotly>=5.7.0
 Requires-Dist: protobuf!=3.20.0,<=3.20.3
 Requires-Dist: pymeshlab>=2022.2.post2; platform_machine != "arm64" and platform_machine != "aarch64"
 Requires-Dist: pyngrok>=5.1.0
 Requires-Dist: python-socketio>=5.7.1
 Requires-Dist: pyquaternion>=0.9.9
 Requires-Dist: rawpy>=0.18.1; platform_machine != "arm64"
@@ -44,21 +44,21 @@
 Requires-Dist: scikit-image>=0.19.3
 Requires-Dist: splines==0.3.0
 Requires-Dist: tensorboard>=2.13.0
 Requires-Dist: torch>=1.13.1
 Requires-Dist: torchvision>=0.14.1
 Requires-Dist: torchmetrics[image]>=1.0.1
 Requires-Dist: typing_extensions>=4.4.0
-Requires-Dist: viser==0.1.21
+Requires-Dist: viser==0.1.26
 Requires-Dist: nuscenes-devkit>=1.1.1
 Requires-Dist: wandb>=0.13.3
 Requires-Dist: xatlas
 Requires-Dist: trimesh>=3.20.2
 Requires-Dist: timm==0.6.7
-Requires-Dist: gsplat>=0.1.6
+Requires-Dist: gsplat>=0.1.9
 Requires-Dist: pytorch-msssim
 Requires-Dist: pathos
 Requires-Dist: packaging
 Provides-Extra: gen
 Requires-Dist: diffusers==0.16.1; extra == "gen"
 Requires-Dist: transformers==4.29.2; extra == "gen"
 Requires-Dist: accelerate==0.19.0; extra == "gen"
@@ -80,15 +80,15 @@
 Requires-Dist: torch<2.2,>=1.13.1; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: furo==2022.09.29; extra == "docs"
 Requires-Dist: ipython==8.6.0; extra == "docs"
 Requires-Dist: readthedocs-sphinx-search==0.1.2; extra == "docs"
 Requires-Dist: myst-nb==0.16.0; extra == "docs"
 Requires-Dist: nbconvert==7.2.5; extra == "docs"
-Requires-Dist: nbformat==5.5.0; extra == "docs"
+Requires-Dist: nbformat==5.9.2; extra == "docs"
 Requires-Dist: sphinx==5.2.1; extra == "docs"
 Requires-Dist: sphinxemoji==0.2.0; extra == "docs"
 Requires-Dist: sphinx-argparse==0.3.1; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.0; extra == "docs"
 Requires-Dist: sphinx-design==0.2.0; extra == "docs"
 Requires-Dist: sphinxext-opengraph==0.6.3; extra == "docs"
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 1.0.2 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 1.0.3 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 appdirs>=1.4 Requires-Dist: av>=9.2.0 Requires-Dist: awscli>=1.31.10 Requires-
 Dist: comet_ml>=3.33.8 Requires-Dist: cryptography>=38 Requires-Dist:
 tyro>=0.6.6 Requires-Dist: gdown>=4.6.0 Requires-Dist: ninja>=1.10 Requires-
 Dist: h5py>=2.9.0 Requires-Dist: imageio>=2.21.1 Requires-Dist: importlib-
 metadata>=6.0.0; python_version < "3.10" Requires-Dist: ipywidgets>=7.6
 Requires-Dist: jaxtyping>=0.2.15 Requires-Dist: jupyterlab>=3.3.4 Requires-
 Dist: matplotlib>=3.6.0 Requires-Dist: mediapy>=1.1.0 Requires-Dist:
 msgpack>=1.0.4 Requires-Dist: msgpack_numpy>=0.4.8 Requires-Dist:
 nerfacc==0.5.2 Requires-Dist: open3d>=0.16.0 Requires-Dist: opencv-
-python==4.8.0.76 Requires-Dist: Pillow>=9.3.0 Requires-Dist: plotly>=5.7.0
+python==4.8.0.76 Requires-Dist: Pillow>=10.3.0 Requires-Dist: plotly>=5.7.0
 Requires-Dist: protobuf!=3.20.0,<=3.20.3 Requires-Dist:
 pymeshlab>=2022.2.post2; platform_machine != "arm64" and platform_machine !=
 "aarch64" Requires-Dist: pyngrok>=5.1.0 Requires-Dist: python-socketio>=5.7.1
 Requires-Dist: pyquaternion>=0.9.9 Requires-Dist: rawpy>=0.18.1;
 platform_machine != "arm64" Requires-Dist: newrawpy>=1.0.0b0; platform_machine
 == "arm64" Requires-Dist: requests Requires-Dist: rich>=12.5.1 Requires-Dist:
 scikit-image>=0.19.3 Requires-Dist: splines==0.3.0 Requires-Dist:
 tensorboard>=2.13.0 Requires-Dist: torch>=1.13.1 Requires-Dist:
 torchvision>=0.14.1 Requires-Dist: torchmetrics[image]>=1.0.1 Requires-Dist:
-typing_extensions>=4.4.0 Requires-Dist: viser==0.1.21 Requires-Dist: nuscenes-
+typing_extensions>=4.4.0 Requires-Dist: viser==0.1.26 Requires-Dist: nuscenes-
 devkit>=1.1.1 Requires-Dist: wandb>=0.13.3 Requires-Dist: xatlas Requires-Dist:
-trimesh>=3.20.2 Requires-Dist: timm==0.6.7 Requires-Dist: gsplat>=0.1.6
+trimesh>=3.20.2 Requires-Dist: timm==0.6.7 Requires-Dist: gsplat>=0.1.9
 Requires-Dist: pytorch-msssim Requires-Dist: pathos Requires-Dist: packaging
 Provides-Extra: gen Requires-Dist: diffusers==0.16.1; extra == "gen" Requires-
 Dist: transformers==4.29.2; extra == "gen" Requires-Dist: accelerate==0.19.0;
 extra == "gen" Requires-Dist: bitsandbytes==0.39.0; extra == "gen" Requires-
 Dist: sentencepiece==0.1.99; extra == "gen" Provides-Extra: dev Requires-Dist:
 pre-commit==3.3.2; extra == "dev" Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: pytest-xdist==2.5.0; extra == "dev" Requires-Dist:
@@ -38,15 +38,15 @@
 opencv-stubs==0.0.7; extra == "dev" Requires-Dist: transformers==4.29.2; extra
 == "dev" Requires-Dist: pyright==1.1.331; extra == "dev" Requires-Dist:
 projectaria-tools>=1.3.1; sys_platform != "win32" and extra == "dev" Requires-
 Dist: torch<2.2,>=1.13.1; extra == "dev" Provides-Extra: docs Requires-Dist:
 furo==2022.09.29; extra == "docs" Requires-Dist: ipython==8.6.0; extra ==
 "docs" Requires-Dist: readthedocs-sphinx-search==0.1.2; extra == "docs"
 Requires-Dist: myst-nb==0.16.0; extra == "docs" Requires-Dist:
-nbconvert==7.2.5; extra == "docs" Requires-Dist: nbformat==5.5.0; extra ==
+nbconvert==7.2.5; extra == "docs" Requires-Dist: nbformat==5.9.2; extra ==
 "docs" Requires-Dist: sphinx==5.2.1; extra == "docs" Requires-Dist:
 sphinxemoji==0.2.0; extra == "docs" Requires-Dist: sphinx-argparse==0.3.1;
 extra == "docs" Requires-Dist: sphinx-copybutton==0.5.0; extra == "docs"
 Requires-Dist: sphinx-design==0.2.0; extra == "docs" Requires-Dist: sphinxext-
 opengraph==0.6.3; extra == "docs"
 _[_h_t_t_p_s_:_/_/_d_c_b_a_d_g_e_._v_e_r_c_e_l_._a_p_p_/_a_p_i_/_s_e_r_v_e_r_/_u_M_b_N_q_c_r_a_F_c_?_s_t_y_l_e_=_p_l_a_s_t_i_c_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n
                   _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_T_e_s_t_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]
```

### Comparing `nerfstudio-1.0.2/nerfstudio.egg-info/SOURCES.txt` & `nerfstudio-1.0.3/nerfstudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio.egg-info/entry_points.txt` & `nerfstudio-1.0.3/nerfstudio.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.2/nerfstudio.egg-info/requires.txt` & `nerfstudio-1.0.3/nerfstudio.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 matplotlib>=3.6.0
 mediapy>=1.1.0
 msgpack>=1.0.4
 msgpack_numpy>=0.4.8
 nerfacc==0.5.2
 open3d>=0.16.0
 opencv-python==4.8.0.76
-Pillow>=9.3.0
+Pillow>=10.3.0
 plotly>=5.7.0
 protobuf!=3.20.0,<=3.20.3
 pyngrok>=5.1.0
 python-socketio>=5.7.1
 pyquaternion>=0.9.9
 requests
 rich>=12.5.1
 scikit-image>=0.19.3
 splines==0.3.0
 tensorboard>=2.13.0
 torch>=1.13.1
 torchvision>=0.14.1
 torchmetrics[image]>=1.0.1
 typing_extensions>=4.4.0
-viser==0.1.21
+viser==0.1.26
 nuscenes-devkit>=1.1.1
 wandb>=0.13.3
 xatlas
 trimesh>=3.20.2
 timm==0.6.7
-gsplat>=0.1.6
+gsplat>=0.1.9
 pytorch-msssim
 pathos
 packaging
 
 [:platform_machine != "arm64"]
 rawpy>=0.18.1
 
@@ -75,15 +75,15 @@
 
 [docs]
 furo==2022.09.29
 ipython==8.6.0
 readthedocs-sphinx-search==0.1.2
 myst-nb==0.16.0
 nbconvert==7.2.5
-nbformat==5.5.0
+nbformat==5.9.2
 sphinx==5.2.1
 sphinxemoji==0.2.0
 sphinx-argparse==0.3.1
 sphinx-copybutton==0.5.0
 sphinx-design==0.2.0
 sphinxext-opengraph==0.6.3
```

### Comparing `nerfstudio-1.0.2/pyproject.toml` & `nerfstudio-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nerfstudio"
-version = "1.0.2"
+version = "1.0.3"
 description = "All-in-one repository for state-of-the-art NeRFs"
 readme = "README.md"
 license = { text="Apache 2.0"}
 requires-python = ">=3.8.0"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
@@ -31,15 +31,15 @@
     "matplotlib>=3.6.0",
     "mediapy>=1.1.0",
     "msgpack>=1.0.4",
     "msgpack_numpy>=0.4.8",
     "nerfacc==0.5.2",
     "open3d>=0.16.0",
     "opencv-python==4.8.0.76",
-    "Pillow>=9.3.0",
+    "Pillow>=10.3.0",
     "plotly>=5.7.0",
     "protobuf<=3.20.3,!=3.20.0",
     # TODO(1480) enable when pycolmap windows wheels are available
     # "pycolmap==0.3.0",
     "pymeshlab>=2022.2.post2; platform_machine != 'arm64' and platform_machine != 'aarch64'",
     "pyngrok>=5.1.0",
     "python-socketio>=5.7.1",
@@ -53,21 +53,21 @@
     "scikit-image>=0.19.3",
     "splines==0.3.0",
     "tensorboard>=2.13.0",
     "torch>=1.13.1",
     "torchvision>=0.14.1",
     "torchmetrics[image]>=1.0.1",
     "typing_extensions>=4.4.0",
-    "viser==0.1.21",
+    "viser==0.1.26",
     "nuscenes-devkit>=1.1.1",
     "wandb>=0.13.3",
     "xatlas",
     "trimesh>=3.20.2",
     "timm==0.6.7",
-    "gsplat>=0.1.6",
+    "gsplat>=0.1.9",
     "pytorch-msssim",
     "pathos",
     "packaging"
 ]
 
 [project.urls]
 "Documentation" = "https://docs.nerf.studio"
@@ -109,15 +109,15 @@
 docs = [
     "furo==2022.09.29",
     # Specifying ipython for https://github.com/ipython/ipython/issues/13845
     "ipython==8.6.0",
     "readthedocs-sphinx-search==0.1.2",
     "myst-nb==0.16.0",
     "nbconvert==7.2.5",
-    "nbformat==5.5.0",
+    "nbformat==5.9.2",
     "sphinx==5.2.1",
     "sphinxemoji==0.2.0",
     "sphinx-argparse==0.3.1",
     "sphinx-copybutton==0.5.0",
     "sphinx-design==0.2.0",
     "sphinxext-opengraph==0.6.3"
 ]
```

### Comparing `nerfstudio-1.0.2/tests/test_train.py` & `nerfstudio-1.0.3/tests/test_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "nerfacto-big",
     "phototourism",
     "depth-nerfacto",
     "neus",
     "generfacto",
     "neus-facto",
     "splatfacto",
+    "splatfacto-big",
 ]
 
 
 def set_reduced_config(config: TrainerConfig, tmp_path: Path):
     """Reducing the config settings to speedup test"""
     config.machine.device_type = "cpu"
     if hasattr(config.pipeline.model, "implementation"):
```

