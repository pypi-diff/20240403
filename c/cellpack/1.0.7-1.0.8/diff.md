# Comparing `tmp/cellpack-1.0.7.tar.gz` & `tmp/cellpack-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpack-1.0.7.tar", last modified: Tue Mar  5 23:49:40 2024, max compression
+gzip compressed data, was "cellpack-1.0.8.tar", last modified: Tue Apr  2 22:31:53 2024, max compression
```

## Comparing `cellpack-1.0.7.tar` & `cellpack-1.0.8.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.974048 cellpack-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-05 23:49:35.000000 cellpack-1.0.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-05 23:49:35.000000 cellpack-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-05 23:49:35.000000 cellpack-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-03-05 23:49:40.974048 cellpack-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-03-05 23:49:35.000000 cellpack-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.958047 cellpack-1.0.7/cellpack/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.966048 cellpack-1.0.7/cellpack/autopack/
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/AWSHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)   100376 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/Analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    32496 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/BaseGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)   127183 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/Compartment.py
--rw-r--r--   0 runner    (1001) docker     (127)    29928 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/DBRecipeHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)   114166 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/Environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/FirebaseHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/GeometryTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/Gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)   110301 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/Graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/Grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    59480 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/IOutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14049 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/MeshStore.py
--rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/OutputSimularium.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10077 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/Recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/Serializable.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20250 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/binvox_rw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.966048 cellpack-1.0.7/cellpack/autopack/ingredient/
--rw-r--r--   0 runner    (1001) docker     (127)    88481 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/Ingredient.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    69689 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/grow.py
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/multi_cylinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/multi_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/single_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/single_cylinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/single_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ingredient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.966048 cellpack-1.0.7/cellpack/autopack/interface_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/interface_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/interface_objects/database_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/interface_objects/default_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/interface_objects/gradient_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/interface_objects/ingredient_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/interface_objects/meta_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/interface_objects/packed_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/interface_objects/partners.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/interface_objects/representations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ldSequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.970048 cellpack-1.0.7/cellpack/autopack/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/loaders/analysis_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/loaders/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/loaders/migrate_v1_to_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/loaders/migrate_v2_to_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/loaders/recipe_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/loaders/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/loaders/v1_v2_attribute_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/octree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/plotly_result.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7137 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/randomRot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18980 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    16910 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)    70147 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.970048 cellpack-1.0.7/cellpack/autopack/upy/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/upy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12668 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/upy/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)   164444 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/upy/hostHelper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.970048 cellpack-1.0.7/cellpack/autopack/upy/simularium/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/upy/simularium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48568 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/upy/simularium/simularium_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.970048 cellpack-1.0.7/cellpack/autopack/writers/
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/writers/ImageWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18116 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/autopack/writers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.970048 cellpack-1.0.7/cellpack/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/bin/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/bin/get-pdb-offset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/bin/pack.py
--rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/bin/simularium_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-05 23:49:35.000000 cellpack-1.0.7/cellpack/bin/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.962048 cellpack-1.0.7/cellpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-03-05 23:49:40.000000 cellpack-1.0.7/cellpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-05 23:49:40.000000 cellpack-1.0.7/cellpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 23:49:40.000000 cellpack-1.0.7/cellpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-05 23:49:40.000000 cellpack-1.0.7/cellpack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 23:49:40.000000 cellpack-1.0.7/cellpack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-05 23:49:40.000000 cellpack-1.0.7/cellpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-05 23:49:40.000000 cellpack-1.0.7/cellpack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 23:49:40.974048 cellpack-1.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-05 23:49:35.000000 cellpack-1.0.7/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     5300 2024-03-05 23:49:35.000000 cellpack-1.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-05 23:49:35.000000 cellpack-1.0.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-05 23:49:35.000000 cellpack-1.0.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-05 23:49:35.000000 cellpack-1.0.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-05 23:49:35.000000 cellpack-1.0.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-05 23:49:35.000000 cellpack-1.0.7/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-05 23:49:35.000000 cellpack-1.0.7/docs/recipe-schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-05 23:49:40.974048 cellpack-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-05 23:49:35.000000 cellpack-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.547665 cellpack-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-02 22:31:48.000000 cellpack-1.0.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-02 22:31:48.000000 cellpack-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-02 22:31:48.000000 cellpack-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-02 22:31:53.547665 cellpack-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-02 22:31:48.000000 cellpack-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.531665 cellpack-1.0.8/cellpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.539666 cellpack-1.0.8/cellpack/autopack/
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/AWSHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100376 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32496 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/BaseGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127182 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/Compartment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32180 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/DBRecipeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114166 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/Environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/FirebaseHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/GeometryTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/Gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110301 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/Graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/Grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59480 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/IOutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14049 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/MeshStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/OutputSimularium.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10077 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/Recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/Serializable.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20295 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/binvox_rw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.539666 cellpack-1.0.8/cellpack/autopack/ingredient/
+-rw-r--r--   0 runner    (1001) docker     (127)    88481 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/Ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69689 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/grow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/multi_cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/multi_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/single_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/single_cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/single_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ingredient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.543666 cellpack-1.0.8/cellpack/autopack/interface_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/interface_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/interface_objects/database_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/interface_objects/default_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/interface_objects/gradient_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/interface_objects/ingredient_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/interface_objects/meta_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/interface_objects/packed_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/interface_objects/partners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/interface_objects/representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ldSequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.543666 cellpack-1.0.8/cellpack/autopack/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/loaders/analysis_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/loaders/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/loaders/migrate_v1_to_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/loaders/migrate_v2_to_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15598 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/loaders/recipe_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/loaders/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/loaders/v1_v2_attribute_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/octree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/plotly_result.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7137 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/randomRot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18980 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16910 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70147 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.543666 cellpack-1.0.8/cellpack/autopack/upy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/upy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12668 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/upy/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164444 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/upy/hostHelper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.543666 cellpack-1.0.8/cellpack/autopack/upy/simularium/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/upy/simularium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48750 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/upy/simularium/simularium_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.543666 cellpack-1.0.8/cellpack/autopack/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/writers/ImageWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18116 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/autopack/writers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.547665 cellpack-1.0.8/cellpack/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/bin/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/bin/cleanup_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/bin/get-pdb-offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/bin/pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/bin/simularium_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-02 22:31:48.000000 cellpack-1.0.8/cellpack/bin/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.535665 cellpack-1.0.8/cellpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-02 22:31:53.000000 cellpack-1.0.8/cellpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-02 22:31:53.000000 cellpack-1.0.8/cellpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:31:53.000000 cellpack-1.0.8/cellpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 22:31:53.000000 cellpack-1.0.8/cellpack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:31:53.000000 cellpack-1.0.8/cellpack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-02 22:31:53.000000 cellpack-1.0.8/cellpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 22:31:53.000000 cellpack-1.0.8/cellpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:31:53.547665 cellpack-1.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 22:31:48.000000 cellpack-1.0.8/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5300 2024-04-02 22:31:48.000000 cellpack-1.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 22:31:48.000000 cellpack-1.0.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-02 22:31:48.000000 cellpack-1.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-02 22:31:48.000000 cellpack-1.0.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 22:31:48.000000 cellpack-1.0.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 22:31:48.000000 cellpack-1.0.8/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 22:31:48.000000 cellpack-1.0.8/docs/recipe-schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-02 22:31:53.547665 cellpack-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-02 22:31:48.000000 cellpack-1.0.8/setup.py
```

### Comparing `cellpack-1.0.7/CONTRIBUTING.md` & `cellpack-1.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/LICENSE` & `cellpack-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/PKG-INFO` & `cellpack-1.0.8/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpack
-Version: 1.0.7
+Version: 1.0.8
 Summary: algorithm to pack molecular recipes
 Home-page: https://github.com/mesoscope/cellpack
 Author: Megan Riel-Mehan
 Author-email: meganr@alleninstitute.org
 License: MIT license
 Keywords: cellpack
 Platform: UNKNOWN
```

### Comparing `cellpack-1.0.7/README.md` & `cellpack-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/Analysis.py` & `cellpack-1.0.8/cellpack/autopack/Analysis.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/BaseGrid.py` & `cellpack-1.0.8/cellpack/autopack/BaseGrid.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/Compartment.py` & `cellpack-1.0.8/cellpack/autopack/Compartment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1214,15 +1214,15 @@
         (
             surface_points_in_bounding_box,
             surfPtsBBNorms,
         ) = self.filter_surface_pts_to_fill_box(off_grid_surface_points, env)
 
         off_grid_surface_points = surface_points_in_bounding_box
 
-        ex = False  # True if nbGridPoints == len(idarray) else False
+        ex = True  # True if nbGridPoints == len(idarray) else False
 
         surfacePoints, surfacePointsNormals = self.extendGridArrays(
             nbGridPoints,
             off_grid_surface_points,
             surfPtsBBNorms,
             env,
             surfacePointsNormals=self.surfacePointsNormals,
```

### Comparing `cellpack-1.0.7/cellpack/autopack/DBRecipeHandler.py` & `cellpack-1.0.8/cellpack/autopack/DBRecipeHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import copy
+from datetime import datetime, timezone
 from enum import Enum
 
 from deepdiff import DeepDiff
+import requests
 
 from cellpack.autopack.utils import deep_merge
 
 
 class DataDoc(object):
     def __init__(
         self,
@@ -372,14 +374,44 @@
                 db_data = db.doc_to_dict(doc)
                 difference = DeepDiff(db_data, local_data, ignore_order=True)
                 if not difference:
                     return doc, db.doc_id(doc)
         return None, None
 
 
+class ResultDoc:
+    def __init__(self, db):
+        self.db = db
+
+    def handle_expired_results(self):
+        """
+        Check if the results in the database are expired and delete them if the linked object expired.
+        """
+        current_utc = datetime.now(timezone.utc)
+        results = self.db.get_all_docs("results")
+        if results:
+            for result in results:
+                result_data = self.db.doc_to_dict(result)
+                result_age = current_utc - result_data["timestamp"]
+                if result_age.days > 180 and not self.validate_existence(
+                    result_data["url"]
+                ):
+                    self.db.delete_doc("results", self.db.doc_id(result))
+            print("Results cleanup complete.")
+        else:
+            print("No results found in the database.")
+
+    def validate_existence(self, url):
+        """
+        Validate the existence of an S3 object by checking if the URL is accessible.
+        Returns True if the URL is accessible.
+        """
+        return requests.head(url).status_code == requests.codes.ok
+
+
 class DBUploader(object):
     """
     Handles the uploading of data to the database.
     """
 
     def __init__(self, db_handler):
         self.db = db_handler
@@ -572,27 +604,28 @@
         recipe_id = self._get_recipe_id(recipe_data)
         # if the recipe is already exists in db, just return
         recipe, _ = self.db.get_doc_by_id("recipes", recipe_id)
         if recipe:
             print(f"{recipe_id} is already in firestore")
             return
         recipe_to_save = self.upload_collections(recipe_meta_data, recipe_data)
+        recipe_to_save["recipe_path"] = self.db.create_path("recipes", recipe_id)
         self.upload_data("recipes", recipe_to_save, recipe_id)
 
     def upload_result_metadata(self, file_name, url):
         """
         Upload the metadata of the result file to the database.
         """
         if self.db:
             username = self.db.get_username()
             timestamp = self.db.create_timestamp()
             self.db.update_or_create(
                 "results",
                 file_name,
-                {"user": username, "timestamp": timestamp, "url": url.split("?")[0]},
+                {"user": username, "timestamp": timestamp, "url": url},
             )
 
 
 class DBRecipeLoader(object):
     """
     Handles the logic for downloading and parsing the recipe data from the database.
     """
@@ -630,14 +663,26 @@
                 else:
                     prep_data[key] = value
         return prep_data
 
     def collect_docs_by_id(self, collection, id):
         return self.db.get_doc_by_id(collection, id)
 
+    def validate_input_recipe_path(self, path):
+        """
+        Validates if the input path corresponds to a recipe path in the database.
+        Format of a recipe path: firebase:recipes/[RECIPE-ID]
+        """
+        collection, id = self.db.get_collection_id_from_path(path)
+        recipe_path = self.db.get_value(collection, id, "recipe_path")
+        if not recipe_path:
+            raise ValueError(
+                f"No recipe found at the input path: '{path}'. Please ensure the recipe exists in the database and is spelled correctly. Expected path format: 'firebase:recipes/[RECIPE-ID]'"
+            )
+
     @staticmethod
     def _get_grad_and_obj(obj_data, obj_dict, grad_dict):
         """
         Collect gradient and inherited object data from the downloaded object data
         return object data dict and gradient data dict with name as key
         """
         obj_name = obj_data["name"]
@@ -706,7 +751,23 @@
             },
             "objects": obj_dict,
             "composition": comp_dict,
         }
         if grad_dict:
             recipe_data["gradients"] = [{**v} for v in grad_dict.values()]
         return recipe_data
+
+
+class DBMaintenance(object):
+    """
+    Handles the maintenance of the database.
+    """
+
+    def __init__(self, db_handler):
+        self.db = db_handler
+        self.result_doc = ResultDoc(self.db)
+
+    def cleanup_results(self):
+        """
+        Check if the results in the database are expired and delete them if the linked object expired.
+        """
+        self.result_doc.handle_expired_results()
```

### Comparing `cellpack-1.0.7/cellpack/autopack/Environment.py` & `cellpack-1.0.8/cellpack/autopack/Environment.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/FirebaseHandler.py` & `cellpack-1.0.8/cellpack/autopack/FirebaseHandler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 import ast
+import logging
 import os
 import firebase_admin
 from firebase_admin import credentials, firestore
 from dotenv import load_dotenv
 from google.cloud.exceptions import NotFound
 from cellpack.autopack.loaders.utils import read_json_file, write_json_file
+from cellpack.autopack.interface_objects.default_values import (
+    default_firebase_collection_names,
+)
 
 
 class FirebaseHandler(object):
     """
     Retrieve data and perform common tasks when working with firebase.
     """
 
     # use class attributes to maintain a consistent state across all instances
     _initialized = False
     _db = None
 
-    def __init__(self):
+    def __init__(self, default_db=None):
         # check if firebase is already initialized
         if not FirebaseHandler._initialized:
-            db_choice = FirebaseHandler.which_db()
+            db_choice = FirebaseHandler.which_db(default_db=default_db)
             if db_choice == "staging":
                 cred = FirebaseHandler.get_staging_creds()
             else:
                 cred = FirebaseHandler.get_dev_creds()
             login = credentials.Certificate(cred)
             firebase_admin.initialize_app(login)
             FirebaseHandler._initialized = True
             FirebaseHandler._db = firestore.client()
 
         self.db = FirebaseHandler._db
         self.name = "firebase"
 
     # common utility methods
     @staticmethod
-    def which_db():
+    def which_db(default_db=None):
         options = {"1": "dev", "2": "staging"}
-        print("Choose database:")
+        if default_db in options.values():
+            print(f"Using {default_db} database -------------")
+            return default_db
         for key, value in options.items():
             print(f"[{key}] {value}")
         choice = input("Enter number: ").strip()
         print(f"Using {options.get(choice, 'dev')} database -------------")
-        return options.get(choice, "dev")  # default to dev db
+        return options.get(choice, "dev")  # default to dev db for recipe uploads
 
     @staticmethod
     def doc_to_dict(doc):
         return doc.to_dict()
 
     @staticmethod
     def doc_id(doc):
@@ -61,30 +67,38 @@
 
     @staticmethod
     def get_path_from_ref(doc):
         return doc.path
 
     @staticmethod
     def get_collection_id_from_path(path):
-        # path example = firebase:composition/uid_1
-        components = path.split(":")[1].split("/")
-        collection = components[0]
-        id = components[1]
+        try:
+            components = path.split(":")[1].split("/")
+            collection = components[0]
+            id = components[1]
+            if collection not in default_firebase_collection_names:
+                raise ValueError(
+                    f"Invalid collection name: '{collection}'. Choose from: {default_firebase_collection_names}"
+                )
+        except IndexError:
+            raise ValueError(
+                "Invalid path provided. Expected format: firebase:collection/id"
+            )
         return collection, id
 
     # Create methods
     def set_doc(self, collection, id, data):
         doc, doc_ref = self.get_doc_by_id(collection, id)
         if not doc:
             doc_ref = self.db.collection(collection).document(id)
             doc_ref.set(data)
-            print(f"successfully uploaded to path: {doc_ref.path}")
+            logging.info(f"successfully uploaded to path: {doc_ref.path}")
             return doc_ref
         else:
-            print(
+            logging.error(
                 f"ERROR: {doc_ref.path} already exists. If uploading new data, provide a unique recipe name."
             )
             return
 
     def upload_doc(self, collection, data):
         return self.db.collection(collection).add(data)
 
@@ -97,20 +111,21 @@
         return creds["firebase"]
 
     @staticmethod
     def get_staging_creds():
         # set override=True to refresh the .env file if softwares or tokens updated
         load_dotenv(dotenv_path="./.env", override=False)
         FIREBASE_TOKEN = os.getenv("FIREBASE_TOKEN")
+        firebase_key = FIREBASE_TOKEN.replace("\\n", "\n")
         FIREBASE_EMAIL = os.getenv("FIREBASE_EMAIL")
         return {
             "type": "service_account",
             "project_id": "cell-pack-database",
             "client_email": FIREBASE_EMAIL,
-            "private_key": FIREBASE_TOKEN,
+            "private_key": firebase_key,
             "token_uri": "https://oauth2.googleapis.com/token",
         }
 
     @staticmethod
     def get_username():
         creds = read_json_file("./.creds")
         try:
@@ -137,19 +152,36 @@
         else:
             return None, None
 
     def get_doc_by_ref(self, path):
         collection, id = FirebaseHandler.get_collection_id_from_path(path)
         return self.get_doc_by_id(collection, id)
 
+    def get_all_docs(self, collection):
+        try:
+            docs_stream = self.db.collection(collection).stream()
+            docs = list(docs_stream)
+            return docs
+        except Exception as e:
+            logging.error(
+                f"An error occurred while retrieving docs from collection '{collection}': {e}"
+            )
+            return None
+
+    def get_value(self, collection, id, field):
+        doc, _ = self.get_doc_by_id(collection, id)
+        if doc is None:
+            return None
+        return doc[field]
+
     # Update methods
     def update_doc(self, collection, id, data):
         doc_ref = self.db.collection(collection).document(id)
         doc_ref.update(data)
-        print(f"successfully updated to path: {doc_ref.path}")
+        logging.info(f"successfully updated to path: {doc_ref.path}")
         return doc_ref
 
     @staticmethod
     def update_reference_on_doc(doc_ref, index, new_item_ref):
         doc_ref.update({index: new_item_ref})
 
     @staticmethod
@@ -162,14 +194,21 @@
         If the input id exists, update the doc. If not, create a new file.
         """
         try:
             self.update_doc(collection, id, data)
         except NotFound:
             self.set_doc(collection, id, data)
 
+    # Delete methods
+    def delete_doc(self, collection, id):
+        doc_ref = self.db.collection(collection).document(id)
+        doc_ref.delete()
+        logging.info(f"successfully deleted path: {doc_ref.path}")
+        return doc_ref.id
+
     # other utils
     @staticmethod
     def write_creds_path():
         path = ast.literal_eval(input("provide path to firebase credentials: "))
         data = read_json_file(path)
         if data is None:
             raise ValueError("The path to your credentials doesn't exist")
```

### Comparing `cellpack-1.0.7/cellpack/autopack/GeometryTools.py` & `cellpack-1.0.8/cellpack/autopack/GeometryTools.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/Gradient.py` & `cellpack-1.0.8/cellpack/autopack/Gradient.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/Graphics.py` & `cellpack-1.0.8/cellpack/autopack/Graphics.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/Grid.py` & `cellpack-1.0.8/cellpack/autopack/Grid.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/IOutils.py` & `cellpack-1.0.8/cellpack/autopack/IOutils.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/MeshStore.py` & `cellpack-1.0.8/cellpack/autopack/MeshStore.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/OutputSimularium.py` & `cellpack-1.0.8/cellpack/autopack/OutputSimularium.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/Recipe.py` & `cellpack-1.0.8/cellpack/autopack/Recipe.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/Serializable.py` & `cellpack-1.0.8/cellpack/autopack/Serializable.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/__init__.py` & `cellpack-1.0.8/cellpack/autopack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,15 +382,16 @@
 
 def load_file(filename, destination="", cache="geometries", force=None):
     if is_remote_path(filename):
         database_name, file_path = convert_db_shortname_to_url(filename)
         # command example: `pack -r firebase:recipes/[FIREBASE-RECIPE-ID] -c [CONFIG-FILE-PATH]`
         if database_name == "firebase":
             db = DATABASE_IDS.handlers().get(database_name)
-            db_handler = DBRecipeLoader(db)
+            initialize_db = db()
+            db_handler = DBRecipeLoader(initialize_db)
             recipe_id = file_path.split("/")[-1]
             db_doc, _ = db_handler.collect_docs_by_id(
                 collection="recipes", id=recipe_id
             )
             downloaded_recipe_data = db_handler.prep_db_doc_for_download(db_doc)
             return downloaded_recipe_data, database_name
         else:
```

### Comparing `cellpack-1.0.7/cellpack/autopack/binvox_rw.py` & `cellpack-1.0.8/cellpack/autopack/binvox_rw.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/Ingredient.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/Ingredient.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/__init__.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/agent.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/agent.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/grow.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/grow.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/multi_cylinder.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/multi_cylinder.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/multi_sphere.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/multi_sphere.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/single_cube.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/single_cube.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/single_cylinder.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/single_cylinder.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/single_sphere.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/single_sphere.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ingredient/utils.py` & `cellpack-1.0.8/cellpack/autopack/ingredient/utils.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/interface_objects/database_ids.py` & `cellpack-1.0.8/cellpack/autopack/interface_objects/database_ids.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,12 +17,15 @@
         def create_aws_handler(bucket_name, sub_folder_name, region_name):
             return AWSHandler(
                 bucket_name=bucket_name,
                 sub_folder_name=sub_folder_name,
                 region_name=region_name,
             )
 
+        def create_firebase_handler(default_db=None):
+            return FirebaseHandler(default_db=default_db)
+
         handlers_dict = {
-            cls.FIREBASE: FirebaseHandler(),
+            cls.FIREBASE: create_firebase_handler,
             cls.AWS: create_aws_handler,
         }
         return handlers_dict
```

### Comparing `cellpack-1.0.7/cellpack/autopack/interface_objects/gradient_data.py` & `cellpack-1.0.8/cellpack/autopack/interface_objects/gradient_data.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/interface_objects/packed_objects.py` & `cellpack-1.0.8/cellpack/autopack/interface_objects/packed_objects.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/interface_objects/partners.py` & `cellpack-1.0.8/cellpack/autopack/interface_objects/partners.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/interface_objects/representations.py` & `cellpack-1.0.8/cellpack/autopack/interface_objects/representations.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ldSequence.py` & `cellpack-1.0.8/cellpack/autopack/ldSequence.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/loaders/analysis_config_loader.py` & `cellpack-1.0.8/cellpack/autopack/loaders/analysis_config_loader.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/loaders/config_loader.py` & `cellpack-1.0.8/cellpack/autopack/loaders/config_loader.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/loaders/migrate_v1_to_v2.py` & `cellpack-1.0.8/cellpack/autopack/loaders/migrate_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/loaders/migrate_v2_to_v2_1.py` & `cellpack-1.0.8/cellpack/autopack/loaders/migrate_v2_to_v2_1.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/loaders/recipe_loader.py` & `cellpack-1.0.8/cellpack/autopack/loaders/recipe_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             for _, obj in recipe_data["objects"].items():
                 reps = obj["representations"] if "representations" in obj else {}
                 obj["representations"] = Representations(
                     mesh=reps.get("mesh", None),
                     atomic=reps.get("atomic", None),
                     packing=reps.get("packing", None),
                 )
-                # the key "all_partners" exists in obj["partners"] if the recipe is downloaded from a remote db
+                # the key "all_partners" already exists in obj["partners"] if the recipe is downloaded from firebase
                 partner_settings = (
                     []
                     if (
                         "partners" in obj
                         and "all_partners" in obj["partners"]
                         and not obj["partners"]["all_partners"]
                     )
```

### Comparing `cellpack-1.0.7/cellpack/autopack/loaders/utils.py` & `cellpack-1.0.8/cellpack/autopack/loaders/utils.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/loaders/v1_v2_attribute_changes.py` & `cellpack-1.0.8/cellpack/autopack/loaders/v1_v2_attribute_changes.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/octree.py` & `cellpack-1.0.8/cellpack/autopack/octree.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/plotly_result.py` & `cellpack-1.0.8/cellpack/autopack/plotly_result.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/randomRot.py` & `cellpack-1.0.8/cellpack/autopack/randomRot.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/ray.py` & `cellpack-1.0.8/cellpack/autopack/ray.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/trajectory.py` & `cellpack-1.0.8/cellpack/autopack/trajectory.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/transformation.py` & `cellpack-1.0.8/cellpack/autopack/transformation.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/upy/__init__.py` & `cellpack-1.0.8/cellpack/autopack/upy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/upy/colors.py` & `cellpack-1.0.8/cellpack/autopack/upy/colors.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/upy/hostHelper.py` & `cellpack-1.0.8/cellpack/autopack/upy/hostHelper.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/upy/simularium/__init__.py` & `cellpack-1.0.8/cellpack/autopack/upy/simularium/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/upy/simularium/simularium_helper.py` & `cellpack-1.0.8/cellpack/autopack/upy/simularium/simularium_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1409,25 +1409,29 @@
 
     @staticmethod
     def store_result_file(file_path, storage=None):
         if storage == "aws":
             handler = DATABASE_IDS.handlers().get(storage)
             initialized_handler = handler(
                 bucket_name="cellpack-results",
-                sub_folder_name="simularium/",
+                sub_folder_name="simularium",
                 region_name="us-west-2",
             )
-        file_name, url = initialized_handler.save_file(file_path)
+        file_name, url = initialized_handler.save_file_and_get_url(file_path)
         simulariumHelper.store_metadata(file_name, url, db="firebase")
         return file_name, url
 
     @staticmethod
     def store_metadata(file_name, url, db=None):
         if db == "firebase":
-            db_handler = DBUploader(DATABASE_IDS.handlers().get(db))
-            db_handler.upload_result_metadata(file_name, url)
+            handler = DATABASE_IDS.handlers().get(db)
+            initialized_db = handler(
+                default_db="staging"
+            )  # default to staging for metadata uploads
+            db_uploader = DBUploader(initialized_db)
+            db_uploader.upload_result_metadata(file_name, url)
 
     @staticmethod
     def open_in_simularium(aws_url):
         webbrowser.open_new_tab(
             f"https://simularium.allencell.org/viewer?trajUrl={aws_url}"
         )
```

### Comparing `cellpack-1.0.7/cellpack/autopack/utils.py` & `cellpack-1.0.8/cellpack/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/writers/ImageWriter.py` & `cellpack-1.0.8/cellpack/autopack/writers/ImageWriter.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/autopack/writers/__init__.py` & `cellpack-1.0.8/cellpack/autopack/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/bin/analyze.py` & `cellpack-1.0.8/cellpack/bin/analyze.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/bin/get-pdb-offset.py` & `cellpack-1.0.8/cellpack/bin/get-pdb-offset.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/bin/pack.py` & `cellpack-1.0.8/cellpack/bin/pack.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/bin/simularium_converter.py` & `cellpack-1.0.8/cellpack/bin/simularium_converter.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack/bin/upload.py` & `cellpack-1.0.8/cellpack/bin/upload.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/cellpack.egg-info/PKG-INFO` & `cellpack-1.0.8/cellpack.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpack
-Version: 1.0.7
+Version: 1.0.8
 Summary: algorithm to pack molecular recipes
 Home-page: https://github.com/mesoscope/cellpack
 Author: Megan Riel-Mehan
 Author-email: meganr@alleninstitute.org
 License: MIT license
 Keywords: cellpack
 Platform: UNKNOWN
```

### Comparing `cellpack-1.0.7/cellpack.egg-info/SOURCES.txt` & `cellpack-1.0.8/cellpack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 cellpack/autopack/upy/hostHelper.py
 cellpack/autopack/upy/simularium/__init__.py
 cellpack/autopack/upy/simularium/simularium_helper.py
 cellpack/autopack/writers/ImageWriter.py
 cellpack/autopack/writers/__init__.py
 cellpack/bin/__init__.py
 cellpack/bin/analyze.py
+cellpack/bin/cleanup_tasks.py
 cellpack/bin/get-pdb-offset.py
 cellpack/bin/pack.py
 cellpack/bin/simularium_converter.py
 cellpack/bin/upload.py
 docs/Makefile
 docs/conf.py
 docs/contributing.rst
```

### Comparing `cellpack-1.0.7/cellpack.egg-info/requires.txt` & `cellpack-1.0.8/cellpack.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 tqdm>=4.64.1
+mdutils>=1.4.0
 scikit-learn>=1.1.3
 seaborn>=0.12.1
 aicsimageio>=4.10.0
 pandas>=1.2.4
+mdutils>=1.4.0
 boto3>=1.28.3
 fire>=0.4.0
 firebase_admin>=6.0.1
 matplotlib>=3.3.4
 numpy>=1.19.2
 pmw==2.0.1
 scipy>=1.6.2
@@ -14,21 +16,24 @@
 plotly>=5.3.1
 pycollada==0.7.2
 pyembree>=0.1.8
 pymunk>=6.2.0
 trimesh>=3.9.34
 deepdiff>=5.5.0
 python-dotenv>=1.0.0
+moto>=5.0.2
 
 [all]
 tqdm>=4.64.1
+mdutils>=1.4.0
 scikit-learn>=1.1.3
 seaborn>=0.12.1
 aicsimageio>=4.10.0
 pandas>=1.2.4
+mdutils>=1.4.0
 boto3>=1.28.3
 fire>=0.4.0
 firebase_admin>=6.0.1
 matplotlib>=3.3.4
 numpy>=1.19.2
 pmw==2.0.1
 scipy>=1.6.2
@@ -36,27 +41,29 @@
 plotly>=5.3.1
 pycollada==0.7.2
 pyembree>=0.1.8
 pymunk>=6.2.0
 trimesh>=3.9.34
 deepdiff>=5.5.0
 python-dotenv>=1.0.0
+moto>=5.0.2
 pytest-runner>=5.2
 black<=23.0,>=19.10b0
 flake8<=6.0.0,>=3.8.3
 flake8-debugger>=3.2.1
-mdutils>=1.4.0
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 tqdm>=4.64.1
+mdutils>=1.4.0
 scikit-learn>=1.1.3
 seaborn>=0.12.1
 aicsimageio>=4.10.0
 pandas>=1.2.4
+mdutils>=1.4.0
 bump2version>=1.0.1
 coverage>=5.1
 ipython>=7.15.0
 m2r2>=0.2.7
 pytest-runner>=5.2
 Sphinx>=3.4.3
 sphinx_rtd_theme>=0.5.1
@@ -65,23 +72,24 @@
 wheel>=0.34.2
 
 [dev]
 pytest-runner>=5.2
 black<=23.0,>=19.10b0
 flake8<=6.0.0,>=3.8.3
 flake8-debugger>=3.2.1
-mdutils>=1.4.0
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 tqdm>=4.64.1
+mdutils>=1.4.0
 scikit-learn>=1.1.3
 seaborn>=0.12.1
 aicsimageio>=4.10.0
 pandas>=1.2.4
+mdutils>=1.4.0
 bump2version>=1.0.1
 coverage>=5.1
 ipython>=7.15.0
 m2r2>=0.2.7
 pytest-runner>=5.2
 Sphinx>=3.4.3
 sphinx_rtd_theme>=0.5.1
@@ -92,11 +100,10 @@
 [setup]
 pytest-runner>=5.2
 
 [test]
 black<=23.0,>=19.10b0
 flake8<=6.0.0,>=3.8.3
 flake8-debugger>=3.2.1
-mdutils>=1.4.0
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
```

### Comparing `cellpack-1.0.7/docs/Makefile` & `cellpack-1.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/docs/conf.py` & `cellpack-1.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/docs/installation.rst` & `cellpack-1.0.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/docs/make.bat` & `cellpack-1.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellpack-1.0.7/setup.py` & `cellpack-1.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,27 @@
     "pytest-runner>=5.2",
 ]
 
 test_requirements = [
     "black>=19.10b0, <=23.0",
     "flake8>=3.8.3, <=6.0.0",
     "flake8-debugger>=3.2.1",
-    "mdutils>=1.4.0",
     "pytest>=5.4.3",
     "pytest-cov>=2.9.0",
     "pytest-raises>=0.11",
 ]
 
 analysis_requirements = [
     "tqdm>=4.64.1",
+    "mdutils>=1.4.0",
     "scikit-learn>=1.1.3",
     "seaborn>=0.12.1",
     "aicsimageio>=4.10.0",
     "pandas>=1.2.4",
+    "mdutils>=1.4.0",
 ]
 
 dev_requirements = [
     *setup_requirements,
     *test_requirements,
     *analysis_requirements,
     "bump2version>=1.0.1",
@@ -59,14 +60,15 @@
     "plotly>=5.3.1",
     "pycollada==0.7.2",
     "pyembree>=0.1.8",
     "pymunk>=6.2.0",
     "trimesh>=3.9.34",
     "deepdiff>=5.5.0",
     "python-dotenv>=1.0.0",
+    "moto>=5.0.2",
 ]
 
 extra_requirements = {
     "setup": setup_requirements,
     "test": test_requirements,
     "dev": dev_requirements,
     "all": [
@@ -115,10 +117,10 @@
     setup_requires=setup_requirements,
     test_suite="cellpack/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/mesoscope/cellpack",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="1.0.7",
+    version="1.0.8",
     zip_safe=False,
 )
```

