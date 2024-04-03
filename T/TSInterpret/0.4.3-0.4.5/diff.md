# Comparing `tmp/TSInterpret-0.4.3.tar.gz` & `tmp/TSInterpret-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.4.3.tar", last modified: Mon Feb 26 05:26:37 2024, max compression
+gzip compressed data, was "TSInterpret-0.4.5.tar", last modified: Wed Apr  3 10:05:47 2024, max compression
```

## Comparing `TSInterpret-0.4.3.tar` & `TSInterpret-0.4.5.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.157702 TSInterpret-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.129702 TSInterpret-0.4.3/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15297 2024-02-26 05:26:37.157702 TSInterpret-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.129702 TSInterpret-0.4.3/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.133702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.133702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.133702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (127)    17487 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.133702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/CF.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.133702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Problem.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTECF.py
--rw-r--r--   0 runner    (1001) docker     (127)    13001 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.137702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETS/
--rw-r--r--   0 runner    (1001) docker     (127)    40792 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETS/ContractedST.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETS/sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9391 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETS/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETSCF.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.137702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.137702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.137702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.137702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.137702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.137702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.141702 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.141702 TSInterpret-0.4.3/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 05:26:37.141702 TSInterpret-0.4.3/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15297 2024-02-26 05:26:37.000000 TSInterpret-0.4.3/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-02-26 05:26:37.000000 TSInterpret-0.4.3/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 05:26:37.000000 TSInterpret-0.4.3/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-02-26 05:26:37.000000 TSInterpret-0.4.3/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-26 05:26:37.000000 TSInterpret-0.4.3/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 05:26:37.157702 TSInterpret-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-02-26 05:26:24.000000 TSInterpret-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.207413 TSInterpret-0.4.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.179413 TSInterpret-0.4.5/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-03 10:05:42.000000 TSInterpret-0.4.5/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-03 10:05:42.000000 TSInterpret-0.4.5/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-03 10:05:42.000000 TSInterpret-0.4.5/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-03 10:05:42.000000 TSInterpret-0.4.5/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-03 10:05:42.000000 TSInterpret-0.4.5/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-03 10:05:42.000000 TSInterpret-0.4.5/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:42.000000 TSInterpret-0.4.5/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-04-03 10:05:47.207413 TSInterpret-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.179413 TSInterpret-0.4.5/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.183413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.183413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.183413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.183413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.183413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTE/
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTECF.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.183413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETS/
+-rw-r--r--   0 runner    (1001) docker     (127)    40792 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETS/ContractedST.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETS/sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9391 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETS/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETSCF.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.187413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.187413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.187413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.187413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.187413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.187413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.191413 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.191413 TSInterpret-0.4.5/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:05:47.191413 TSInterpret-0.4.5/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-04-03 10:05:47.000000 TSInterpret-0.4.5/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-03 10:05:47.000000 TSInterpret-0.4.5/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:05:47.000000 TSInterpret-0.4.5/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-03 10:05:47.000000 TSInterpret-0.4.5/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 10:05:47.000000 TSInterpret-0.4.5/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:05:47.207413 TSInterpret-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-03 10:05:43.000000 TSInterpret-0.4.5/setup.py
```

### Comparing `TSInterpret-0.4.3/ClassificationModels/CNN.py` & `TSInterpret-0.4.5/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/ClassificationModels/CNN_T.py` & `TSInterpret-0.4.5/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/ClassificationModels/DecisionTree.py` & `TSInterpret-0.4.5/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/ClassificationModels/LSTM.py` & `TSInterpret-0.4.5/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/ClassificationModels/LSTM_T.py` & `TSInterpret-0.4.5/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/ClassificationModels/ResNet.py` & `TSInterpret-0.4.5/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/ClassificationModels/utils.py` & `TSInterpret-0.4.5/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/LICENSE` & `TSInterpret-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/PKG-INFO` & `TSInterpret-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.4.3
+Version: 0.4.5
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 Requires-Dist: h5py
 Requires-Dist: joblib<2.0,>=1.0.1
 Requires-Dist: Markdown<4.0,==3.3.4
 Requires-Dist: matplotlib<4.0,>=3.3.4
 Requires-Dist: partd==1.2.0
 Requires-Dist: pytz>=2021.3
 Requires-Dist: shap<1.0,>=0.39.0
-Requires-Dist: tensorflow<3.0,>=2.9.1
+Requires-Dist: tensorflow<=2.14.1,>=2.9.1
 Requires-Dist: keras<3.0,>=2.9.0
 Requires-Dist: tsfresh<1.0,>=0.18.0
 Requires-Dist: tslearn<1.0,>=0.5.2
 Requires-Dist: seaborn<1.0,>=0.11.2
 Requires-Dist: scikit_optimize<1.0,>=0.9.0
 Requires-Dist: torchcam<1.0,>=0.3.1
 Requires-Dist: tf_explain<1.0,>=0.3.1
@@ -55,15 +55,15 @@
 Requires-Dist: h5py; extra == "dev"
 Requires-Dist: joblib<2.0,>=1.0.1; extra == "dev"
 Requires-Dist: Markdown<4.0,==3.3.4; extra == "dev"
 Requires-Dist: matplotlib<4.0,>=3.3.4; extra == "dev"
 Requires-Dist: partd==1.2.0; extra == "dev"
 Requires-Dist: pytz>=2021.3; extra == "dev"
 Requires-Dist: shap<1.0,>=0.39.0; extra == "dev"
-Requires-Dist: tensorflow<3.0,>=2.9.1; extra == "dev"
+Requires-Dist: tensorflow<=2.14.1,>=2.9.1; extra == "dev"
 Requires-Dist: keras<3.0,>=2.9.0; extra == "dev"
 Requires-Dist: tsfresh<1.0,>=0.18.0; extra == "dev"
 Requires-Dist: tslearn<1.0,>=0.5.2; extra == "dev"
 Requires-Dist: seaborn<1.0,>=0.11.2; extra == "dev"
 Requires-Dist: scikit_optimize<1.0,>=0.9.0; extra == "dev"
 Requires-Dist: torchcam<1.0,>=0.3.1; extra == "dev"
 Requires-Dist: tf_explain<1.0,>=0.3.1; extra == "dev"
@@ -91,15 +91,15 @@
 Requires-Dist: h5py; extra == "test"
 Requires-Dist: joblib<2.0,>=1.0.1; extra == "test"
 Requires-Dist: Markdown<4.0,==3.3.4; extra == "test"
 Requires-Dist: matplotlib<4.0,>=3.3.4; extra == "test"
 Requires-Dist: partd==1.2.0; extra == "test"
 Requires-Dist: pytz>=2021.3; extra == "test"
 Requires-Dist: shap<1.0,>=0.39.0; extra == "test"
-Requires-Dist: tensorflow<3.0,>=2.9.1; extra == "test"
+Requires-Dist: tensorflow<=2.14.1,>=2.9.1; extra == "test"
 Requires-Dist: keras<3.0,>=2.9.0; extra == "test"
 Requires-Dist: tsfresh<1.0,>=0.18.0; extra == "test"
 Requires-Dist: tslearn<1.0,>=0.5.2; extra == "test"
 Requires-Dist: seaborn<1.0,>=0.11.2; extra == "test"
 Requires-Dist: scikit_optimize<1.0,>=0.9.0; extra == "test"
 Requires-Dist: torchcam<1.0,>=0.3.1; extra == "test"
 Requires-Dist: tf_explain<1.0,>=0.3.1; extra == "test"
@@ -145,15 +145,15 @@
 Requires-Dist: h5py; extra == "all"
 Requires-Dist: joblib<2.0,>=1.0.1; extra == "all"
 Requires-Dist: Markdown<4.0,==3.3.4; extra == "all"
 Requires-Dist: matplotlib<4.0,>=3.3.4; extra == "all"
 Requires-Dist: partd==1.2.0; extra == "all"
 Requires-Dist: pytz>=2021.3; extra == "all"
 Requires-Dist: shap<1.0,>=0.39.0; extra == "all"
-Requires-Dist: tensorflow<3.0,>=2.9.1; extra == "all"
+Requires-Dist: tensorflow<=2.14.1,>=2.9.1; extra == "all"
 Requires-Dist: keras<3.0,>=2.9.0; extra == "all"
 Requires-Dist: tsfresh<1.0,>=0.18.0; extra == "all"
 Requires-Dist: tslearn<1.0,>=0.5.2; extra == "all"
 Requires-Dist: seaborn<1.0,>=0.11.2; extra == "all"
 Requires-Dist: scikit_optimize<1.0,>=0.9.0; extra == "all"
 Requires-Dist: torchcam<1.0,>=0.3.1; extra == "all"
 Requires-Dist: tf_explain<1.0,>=0.3.1; extra == "all"
```

### Comparing `TSInterpret-0.4.3/README.md` & `TSInterpret-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,27 +45,29 @@
         self,
         model,
         NumTimeSteps: int,
         NumFeatures: int,
         method: str = "GRAD",
         mode: str = "time",
         tsr: bool = True,
+        normalize:bool=True,
         device: str = "cpu",
     ) -> None:
         """Initialization
         Arguments:
             model [torch.nn.Module]: model to be explained
             NumTimeSteps int : Number of Time Step
             NumFeatures int : Number Features
             method str: Saliency Methode to be used
             mode str: Second dimension 'time'->`(1,time,feat)`  or 'feat'->`(1,feat,time)`
         """
-        super().__init__(model, NumTimeSteps, NumFeatures, method, mode)
+        super().__init__(model, NumTimeSteps, NumFeatures, method, mode,normalize)
         self.method = method
         self.tsr = tsr
+        #self.normalize=normalize
         if method == "GRAD":
             self.Grad = Saliency(model)
         elif method == "IG":
             self.Grad = IntegratedGradients(model)
         elif method == "GS":
             self.Grad = GradientShap(model)
         elif method == "DL":
@@ -101,16 +103,19 @@
         mask = np.zeros((self.NumTimeSteps, self.NumFeatures), dtype=int)
         for i in range(self.NumTimeSteps):
             mask[i, :] = i
         rescaledGrad = np.zeros(item.shape)
         idx = 0
         item = np.array(item.tolist())  # , dtype=np.float64)
         input = torch.from_numpy(item)
-
-        input = input.reshape(-1, self.NumTimeSteps, self.NumFeatures).to(self.device)
+        if self.mode=='feat':
+            input = np.swapaxes(input, -1, -2)
+        #if self.mode =='time':
+        #    input = input.reshape(-1, self.NumTimeSteps, self.NumFeatures).to(self.device)
+        
         input = Variable(input, volatile=False, requires_grad=True)
 
         batch_size = input.shape[0]
 
         if "inputMask" in kwargs.keys():
             inputMask = kwargs = ["inputMask"]
         else:
@@ -119,15 +124,15 @@
         inputMask = torch.from_numpy(inputMask).to(self.device)
         mask_single = torch.from_numpy(mask).to(self.device)
         mask_single = mask_single.reshape(1, self.NumTimeSteps, self.NumFeatures).to(
             self.device
         )
         # input = samples.reshape(-1, args.NumTimeSteps, args.NumFeatures).to(device)
         if self.mode == "feat":
-            input = input.reshape(-1, self.NumFeatures, self.NumTimeSteps)
+            input = np.swapaxes(input, -1, -2)
         if "baseline_single" in kwargs.keys():
             baseline_single = kwargs["baseline_single"]
         else:
             baseline_single = (
                 torch.from_numpy(np.random.random(input.shape)).float().to(self.device)
             )  # random.random
         if "baseline_multiple" in kwargs.keys():
@@ -213,21 +218,22 @@
             # print('TSR Attribution', TSR_attributions.shape)
             TSR_saliency = self._givenAttGetRescaledSaliency(
                 TSR_attributions, isTensor=False
             )
             # print('TSR Saliency', TSR_saliency.shape)
             return TSR_saliency
         else:
-            # print('TSR', TSR)
-            # TODO attributions does not exist for SVS and Fo
-            rescaledGrad[
-                idx : idx + batch_size, :, :
-            ] = self._givenAttGetRescaledSaliency(attributions)
-            # print('Rescaled', rescaledGrad.shape)
-            return rescaledGrad[0]
+            if self.normalize:
+            
+                rescaledGrad[
+                    idx : idx + batch_size, :, :
+                ] = self._givenAttGetRescaledSaliency(attributions)
+                return rescaledGrad[0]
+            else:
+                return attributions.detach().numpy()[0]
 
     def _getTwoStepRescaling(
         self,
         input,
         TestingLabel,
         hasBaseline=None,
         hasFeatureMask=None,
@@ -237,22 +243,18 @@
         sequence_length = self.NumTimeSteps
         input_size = self.NumFeatures
         if assignment is None:
             assignment = input[0, 0, 0]
         timeGrad = np.zeros((1, sequence_length))
         inputGrad = np.zeros((input_size, 1))
         newGrad = np.zeros((input_size, sequence_length))
-        # print("has Sliding Window", hasSliding_window_shapes)
-        if self.mode == "time":
-            newGrad = np.swapaxes(newGrad, -1, -2)
-            #    print(input.shape)
-        #    print('mode timw')
-        #    print('inüut1',input)
-        #    input = np.swapaxes(input,-1,-2)#.reshape(-1, sequence_length, input_size)
-        #    print('inüut1',input)
+
+        #if self.mode == "time":
+        #    newGrad = np.swapaxes(newGrad, -1, -2)
+
 
         if hasBaseline is None:
             ActualGrad = (
                 self.Grad.attribute(input, target=TestingLabel).data.cpu().numpy()
             )
         else:
             if hasFeatureMask is not None:
@@ -282,32 +284,29 @@
                 ActualGrad = (
                     self.Grad.attribute(
                         input, baselines=hasBaseline, target=TestingLabel
                     )
                     .data.cpu()
                     .numpy()
                 )
-        # if self.mode == "time":
-        #    ActualGrad = ActualGrad.reshape(-1, input_size, sequence_length)
+  
         if self.mode == "time":
             input = np.swapaxes(
                 input, -1, -2
-            )  # input.reshape(-1, input_size, sequence_length)
+            )  
         for t in range(sequence_length):
             newInput = input.clone()
-            # if newInput.shape[-1] == self.NumTimeSteps:
-            #    print('A')
+
             newInput[:, :, t] = assignment
             # else:
-            #    print('B')
-            #    newInput[:, t,:] = assignment
+
             if self.mode == "time":
                 newInput = np.swapaxes(
                     newInput, -1, -2
-                )  # .reshape(-1, sequence_length, input_size)
+                )  
             if hasBaseline is None:
                 timeGrad_perTime = (
                     self.Grad.attribute(newInput, target=TestingLabel)
                     .data.cpu()
                     .numpy()
                 )
             else:
@@ -319,15 +318,15 @@
                             target=TestingLabel,
                             feature_mask=hasFeatureMask,
                         )
                         .data.cpu()
                         .numpy()
                     )
                 elif hasSliding_window_shapes is not None:
-                    # print("HAS SLIDING WINDOW")
+  
                     timeGrad_perTime = (
                         self.Grad.attribute(
                             newInput,
                             sliding_window_shapes=hasSliding_window_shapes,
                             baselines=hasBaseline,
                             target=TestingLabel,
                         )
@@ -338,97 +337,95 @@
                     timeGrad_perTime = (
                         self.Grad.attribute(
                             newInput, baselines=hasBaseline, target=TestingLabel
                         )
                         .data.cpu()
                         .numpy()
                     )
-            # import sys
-            # sys.exit(1)
 
             timeGrad_perTime = np.absolute(ActualGrad - timeGrad_perTime)
             if self.mode == "time":
-                timeGrad_perTime = np.swapaxes(timeGrad_perTime, -1, -2)  # .reshape(
-                #    -1, input_size, sequence_length
-                # )
+                timeGrad_perTime = np.swapaxes(timeGrad_perTime, -1, -2)  
             timeGrad[:, t] = np.sum(timeGrad_perTime)
 
         timeContribution = preprocessing.minmax_scale(timeGrad, axis=1)
-        # print(timeContribution.shape)
+
         meanTime = np.quantile(timeContribution, 0.55)
 
-        for t in range(sequence_length):
-            if timeContribution[0, t] > meanTime:
-                for c in range(input_size):
-                    newInput = input.clone()
-                    newInput[:, c, t] = assignment
-                    if self.mode == "time":
-                        newInput = np.swapaxes(
-                            newInput, -1, -2
-                        )  # .reshape(-1, sequence_length, input_size)
-
-                    if hasBaseline is None:
-                        inputGrad_perInput = (
-                            self.Grad.attribute(newInput, target=TestingLabel)
-                            .data.cpu()
-                            .numpy()
-                        )
-                    else:
-                        if hasFeatureMask is not None:
-                            inputGrad_perInput = (
-                                self.Grad.attribute(
-                                    newInput,
-                                    baselines=hasBaseline,
-                                    target=TestingLabel,
-                                    feature_mask=hasFeatureMask,
-                                )
-                                .data.cpu()
-                                .numpy()
-                            )
-                        elif hasSliding_window_shapes is not None:
+        if input_size>1:
+            for t in range(sequence_length):
+                print('TIME CONR',timeContribution[0, t])
+                if timeContribution[0, t] > meanTime:
+                    for c in range(input_size):
+                        newInput = input.clone()
+                        newInput[:, c, t] = assignment
+                        if self.mode == "time":
+                            newInput = np.swapaxes(
+                                newInput, -1, -2
+                            )  # .reshape(-1, sequence_length, input_size)
+
+                        if hasBaseline is None:
                             inputGrad_perInput = (
-                                self.Grad.attribute(
-                                    newInput,
-                                    sliding_window_shapes=hasSliding_window_shapes,
-                                    baselines=hasBaseline,
-                                    target=TestingLabel,
-                                )
+                                self.Grad.attribute(newInput, target=TestingLabel)
                                 .data.cpu()
                                 .numpy()
                             )
                         else:
-                            inputGrad_perInput = (
-                                self.Grad.attribute(
-                                    newInput, baselines=hasBaseline, target=TestingLabel
+                            if hasFeatureMask is not None:
+                                inputGrad_perInput = (
+                                    self.Grad.attribute(
+                                        newInput,
+                                        baselines=hasBaseline,
+                                        target=TestingLabel,
+                                        feature_mask=hasFeatureMask,
+                                    )
+                                    .data.cpu()
+                                    .numpy()
+                                )
+                            elif hasSliding_window_shapes is not None:
+                                inputGrad_perInput = (
+                                    self.Grad.attribute(
+                                        newInput,
+                                        sliding_window_shapes=hasSliding_window_shapes,
+                                        baselines=hasBaseline,
+                                        target=TestingLabel,
+                                    )
+                                    .data.cpu()
+                                    .numpy()
+                                )
+                            else:
+                                inputGrad_perInput = (
+                                    self.Grad.attribute(
+                                        newInput, baselines=hasBaseline, target=TestingLabel
+                                    )
+                                    .data.cpu()
+                                    .numpy()
                                 )
-                                .data.cpu()
-                                .numpy()
-                            )
 
-                    inputGrad_perInput = np.absolute(ActualGrad - inputGrad_perInput)
-                    inputGrad_perInput = np.swapaxes(
-                        inputGrad_perInput, -1, -2
-                    )  # .reshape(
-                    # -1, input_size, sequence_length
-                    # )
-                    inputGrad[c, :] = np.sum(inputGrad_perInput)
-                featureContribution = preprocessing.minmax_scale(inputGrad, axis=0)
+                        inputGrad_perInput = np.absolute(ActualGrad - inputGrad_perInput)
+                        inputGrad_perInput = np.swapaxes(
+                            inputGrad_perInput, -1, -2
+                        )  # .reshape(
+                        # -1, input_size, sequence_length
+                        # )
+                        inputGrad[c, :] = np.sum(inputGrad_perInput)
+                    featureContribution = preprocessing.minmax_scale(inputGrad, axis=0)
 
-            else:
-                featureContribution = np.ones((input_size, 1)) * 0.1
-            # print('FC',featureContribution)
-            # newGrad = newGrad#.reshape(input_size, sequence_length)
-            if self.mode == "time":
-                # newGrad = newGrad.reshape(sequence_length, input_size)
-                newGrad = np.swapaxes(newGrad, -1, -2)
-            for c in range(input_size):
-                newGrad[c, t] = timeContribution[0, t] * featureContribution[c, 0]
-            if self.mode == "time":
-                # newGrad = newGrad.reshape(sequence_length, input_size)
-                newGrad = np.swapaxes(newGrad, -1, -2)
+                else:
+                    featureContribution = np.ones((input_size, 1)) * 0.1
+                
+
+                for c in range(input_size):
+                    newGrad[c, t] = timeContribution[0, t] * featureContribution[c, 0]
+
+        else: 
+            newGrad=timeContribution
+            
+        if self.mode == "time":
+            newGrad = np.swapaxes(newGrad, -1, -2)
         return newGrad
 
     def _givenAttGetRescaledSaliency(self, attributions, isTensor=True):
         if isTensor:
             saliency = np.absolute(attributions.data.cpu().numpy())
         else:
             saliency = np.absolute(attributions)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,27 +23,30 @@
     def __init__(
         self,
         model,
         NumTimeSteps: int,
         NumFeatures: int,
         method: str = "GRAD",
         mode: str = "time",
+        normalize:bool=True,
     ) -> None:
         """
         Arguments:
             model [torch.nn.Module,tf.keras.models]: model to be explained.
             NumTimeSteps int: number of timesteps.
             NumFeatures int: number of features.
             method str: Saliency Method to be used.
             mode str: Second dimension 'time'->`(1,time,feat)`  or 'feat'->`(1,feat,time)`.
+            normalize bool: Wheather or not to normalize the results
         """
         super().__init__(model, mode)
         self.NumTimeSteps = NumTimeSteps
         self.NumFeatures = NumFeatures
         self.method = method
+        self.normalize=normalize
 
     def explain(self):
         raise NotImplementedError("Don't use the base CF class directly")
 
     def plot(self, item, exp, figsize=(6.4, 4.8), heatmap=False, save=None):
         """
         Plots explanation on the explained Sample.
@@ -52,14 +55,15 @@
             item np.array: instance to be explained,if `mode = time`->`(1,time,feat)`  or `mode = feat`->`(1,feat,time)`.
             exp np.array: explanation, ,if `mode = time`->`(time,feat)`  or `mode = feat`->`(feat,time)`.
             figsize (int,int): desired size of plot.
             heatmap bool: 'True' if only heatmap, otherwise 'False'.
             save str: Path to save figure.
         """
         plt.style.use("classic")
+        print(self.normalize)
         i = 0
         if self.mode == "time":
             print("time mode")
             item = np.swapaxes(
                 item, -1, -2
             )  # item.reshape(1, item.shape[2], item.shape[1])
             exp = np.swapaxes(exp, -1, -2)  # exp.reshape(exp.shape[-1], -1)
@@ -71,33 +75,42 @@
             sns.heatmap(
                 exp,
                 fmt="g",
                 cmap="viridis",
                 cbar=True,
                 ax=ax011,
                 yticklabels=False,
-                vmin=0,
-                vmax=1,
+                #vmin=0,
+                #vmax=1,
             )
         elif len(item[0]) == 1:
             # if only onedimensional input
             fig, axn = plt.subplots(
                 len(item[0]), 1, sharex=True, sharey=True, figsize=figsize
             )
             # cbar_ax = fig.add_axes([.91, .3, .03, .4])
             axn012 = axn.twinx()
-            sns.heatmap(
-                exp.reshape(1, -1),
-                fmt="g",
-                cmap="viridis",
-                ax=axn,
-                yticklabels=False,
-                vmin=0,
-                vmax=1,
-            )
+            if self.normalize:
+                sns.heatmap(
+                    exp.reshape(1, -1),
+                    fmt="g",
+                    cmap="viridis",
+                    ax=axn,
+                    yticklabels=False,
+                    vmin=0,
+                    vmax=1,
+                )
+            else: 
+                sns.heatmap(
+                    exp.reshape(1, -1),
+                    fmt="g",
+                    cmap="viridis",
+                    ax=axn,
+                    yticklabels=False,
+                )
             sns.lineplot(
                 x=range(0, len(item[0][0].reshape(-1))),
                 y=item[0][0].flatten(),
                 ax=axn012,
                 color="white",
             )
         else:
@@ -110,26 +123,38 @@
 
             for channel in item[0]:
                 # print(item.shape)
                 # ax011.append(plt.subplot(len(item[0]),1,i+1))
                 # ax012.append(ax011[i].twinx())
                 # ax011[i].set_facecolor("#440154FF")
                 axn012 = axn[i].twinx()
+                if self.normalize: 
+
+                    sns.heatmap(
+                        exp[i].reshape(1, -1),
+                        fmt="g",
+                        cmap="viridis",
+                        cbar=i == 0,
+                        cbar_ax=None if i else cbar_ax,
+                        ax=axn[i],
+                        yticklabels=False,
+                        vmin=0,
+                        vmax=1,
+                    )
+                else: 
+                    sns.heatmap(
+                        exp[i].reshape(1, -1),
+                        fmt="g",
+                        cmap="viridis",
+                        cbar=i == 0,
+                        cbar_ax=None if i else cbar_ax,
+                        ax=axn[i],
+                        yticklabels=False,
+                    )
 
-                sns.heatmap(
-                    exp[i].reshape(1, -1),
-                    fmt="g",
-                    cmap="viridis",
-                    cbar=i == 0,
-                    cbar_ax=None if i else cbar_ax,
-                    ax=axn[i],
-                    yticklabels=False,
-                    vmin=0,
-                    vmax=1,
-                )
                 sns.lineplot(
                     x=range(0, len(channel.reshape(-1))),
                     y=channel.flatten(),
                     ax=axn012,
                     color="white",
                 )
                 plt.xlabel("Time", fontweight="bold", fontsize="large")
```

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class TSR:
     """
     Wrapper Class for Saliency Calculation.
     Automatically calls the corresponding PYT or TF implementation.
     """
 
     def __new__(
-        self, model, NumTimeSteps, NumFeatures, method="GRAD", mode="time", device="cpu"
+        self, model, NumTimeSteps, NumFeatures, method="GRAD", mode="time", device="cpu", normalize=True, tsr=True
     ):
         """Initialization
         Arguments:
             model [torch.nn.Module, tf.keras.Model]: model to be explained
             NumTimeSteps int : Number of Time Step
             NumFeatures int : Number Features
             method str: Saliency Methode to be used
@@ -26,19 +26,21 @@
             return Saliency_PTY(
                 model,
                 NumTimeSteps,
                 NumFeatures,
                 method=method,
                 mode=mode,
                 device=device,
+                normalize=normalize,
+                tsr=tsr
             )
 
         elif isinstance(model, tensorflow.keras.Model):
             return Saliency_TF(
-                model, NumTimeSteps, NumFeatures, method=method, mode=mode
+                model, NumTimeSteps, NumFeatures, method=method, mode=mode, tsr=tsr
             )
         else:
             raise NotImplementedError(
                 "Please use a TF or PYT Classification model! \
                 If the current model is a TF or PYT Model, \
                 try calling the wrappers directly \
                 (TF -> Saliency_TF, PYT -> Saliency_PYT)"
```

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization_helpers.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization_helpers.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Problem.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Problem.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/COMTECF.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/COMTECF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,28 +160,31 @@
             return None, None
 
         return nun, np.argmax(out)
 
     def _findSubarray(
         self, a, k
     ):  # used to find the maximum contigious subarray of length k in the explanation weight vector
+        
         if len(a.shape) == 2:
             a = a.reshape(-1)
         n = len(a)
         a = a.tolist()
 
         vec = []
 
         # Iterate to find all the sub-arrays
         for i in range(n - k + 1):
             temp = []
 
             # Store the sub-array elements in the array
             for j in range(i, i + k):
                 temp.append(a[j])
+            
+            
 
             # Push the vector in the container
             vec.append(temp)
         sum_arr = []
         for v in vec:
             sum_arr.append(np.sum(v))
 
@@ -213,14 +216,16 @@
         individual = np.array(instance.tolist())  # , dtype=np.float64)
         out = self.predict(individual)
 
         most_influencial_array = self._findSubarray((training_weights), subarray_length)
 
         if np.any(np.isnan(most_influencial_array)):
             return np.full(individual.shape, None), None
+        if len(training_weights)==1:
+            training_weights=training_weights[0]
 
         starting_point = np.where(training_weights == most_influencial_array[0])[0][0]
 
         X_example = instance.copy().reshape(1, -1)
 
         nun = nun.reshape(1, -1)
         X_example[0, starting_point : subarray_length + starting_point] = nun[
@@ -236,14 +241,16 @@
         ]  # torch.nn.functional.softmax(model(torch.from_numpy(test_x))).detach().numpy()[0][y_pred[instance]]
         counter = 0
         while prob_target > 0.5 and counter < max_iter:
             subarray_length += 1
             most_influencial_array = self._findSubarray(
                 (training_weights), subarray_length
             )
+            if len(training_weights)==1:
+                training_weights=training_weights[0]
             starting_point = np.where(training_weights == most_influencial_array[0])[0][
                 0
             ]
             X_example = instance.copy().reshape(1, -1)
             X_example[:, starting_point : subarray_length + starting_point] = nun[
                 :, starting_point : subarray_length + starting_point
             ]
```

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETS/ContractedST.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETS/ContractedST.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETS/sets.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETS/sets.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETS/utils.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETS/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/SETSCF.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/SETSCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.4.5/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.4.5/TSInterpret/Models/PyTorchModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.4.5/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.4.5/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret/Models/base_model.py` & `TSInterpret-0.4.5/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.4.5/TSInterpret.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.4.3
+Version: 0.4.5
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 Requires-Dist: h5py
 Requires-Dist: joblib<2.0,>=1.0.1
 Requires-Dist: Markdown<4.0,==3.3.4
 Requires-Dist: matplotlib<4.0,>=3.3.4
 Requires-Dist: partd==1.2.0
 Requires-Dist: pytz>=2021.3
 Requires-Dist: shap<1.0,>=0.39.0
-Requires-Dist: tensorflow<3.0,>=2.9.1
+Requires-Dist: tensorflow<=2.14.1,>=2.9.1
 Requires-Dist: keras<3.0,>=2.9.0
 Requires-Dist: tsfresh<1.0,>=0.18.0
 Requires-Dist: tslearn<1.0,>=0.5.2
 Requires-Dist: seaborn<1.0,>=0.11.2
 Requires-Dist: scikit_optimize<1.0,>=0.9.0
 Requires-Dist: torchcam<1.0,>=0.3.1
 Requires-Dist: tf_explain<1.0,>=0.3.1
@@ -55,15 +55,15 @@
 Requires-Dist: h5py; extra == "dev"
 Requires-Dist: joblib<2.0,>=1.0.1; extra == "dev"
 Requires-Dist: Markdown<4.0,==3.3.4; extra == "dev"
 Requires-Dist: matplotlib<4.0,>=3.3.4; extra == "dev"
 Requires-Dist: partd==1.2.0; extra == "dev"
 Requires-Dist: pytz>=2021.3; extra == "dev"
 Requires-Dist: shap<1.0,>=0.39.0; extra == "dev"
-Requires-Dist: tensorflow<3.0,>=2.9.1; extra == "dev"
+Requires-Dist: tensorflow<=2.14.1,>=2.9.1; extra == "dev"
 Requires-Dist: keras<3.0,>=2.9.0; extra == "dev"
 Requires-Dist: tsfresh<1.0,>=0.18.0; extra == "dev"
 Requires-Dist: tslearn<1.0,>=0.5.2; extra == "dev"
 Requires-Dist: seaborn<1.0,>=0.11.2; extra == "dev"
 Requires-Dist: scikit_optimize<1.0,>=0.9.0; extra == "dev"
 Requires-Dist: torchcam<1.0,>=0.3.1; extra == "dev"
 Requires-Dist: tf_explain<1.0,>=0.3.1; extra == "dev"
@@ -91,15 +91,15 @@
 Requires-Dist: h5py; extra == "test"
 Requires-Dist: joblib<2.0,>=1.0.1; extra == "test"
 Requires-Dist: Markdown<4.0,==3.3.4; extra == "test"
 Requires-Dist: matplotlib<4.0,>=3.3.4; extra == "test"
 Requires-Dist: partd==1.2.0; extra == "test"
 Requires-Dist: pytz>=2021.3; extra == "test"
 Requires-Dist: shap<1.0,>=0.39.0; extra == "test"
-Requires-Dist: tensorflow<3.0,>=2.9.1; extra == "test"
+Requires-Dist: tensorflow<=2.14.1,>=2.9.1; extra == "test"
 Requires-Dist: keras<3.0,>=2.9.0; extra == "test"
 Requires-Dist: tsfresh<1.0,>=0.18.0; extra == "test"
 Requires-Dist: tslearn<1.0,>=0.5.2; extra == "test"
 Requires-Dist: seaborn<1.0,>=0.11.2; extra == "test"
 Requires-Dist: scikit_optimize<1.0,>=0.9.0; extra == "test"
 Requires-Dist: torchcam<1.0,>=0.3.1; extra == "test"
 Requires-Dist: tf_explain<1.0,>=0.3.1; extra == "test"
@@ -145,15 +145,15 @@
 Requires-Dist: h5py; extra == "all"
 Requires-Dist: joblib<2.0,>=1.0.1; extra == "all"
 Requires-Dist: Markdown<4.0,==3.3.4; extra == "all"
 Requires-Dist: matplotlib<4.0,>=3.3.4; extra == "all"
 Requires-Dist: partd==1.2.0; extra == "all"
 Requires-Dist: pytz>=2021.3; extra == "all"
 Requires-Dist: shap<1.0,>=0.39.0; extra == "all"
-Requires-Dist: tensorflow<3.0,>=2.9.1; extra == "all"
+Requires-Dist: tensorflow<=2.14.1,>=2.9.1; extra == "all"
 Requires-Dist: keras<3.0,>=2.9.0; extra == "all"
 Requires-Dist: tsfresh<1.0,>=0.18.0; extra == "all"
 Requires-Dist: tslearn<1.0,>=0.5.2; extra == "all"
 Requires-Dist: seaborn<1.0,>=0.11.2; extra == "all"
 Requires-Dist: scikit_optimize<1.0,>=0.9.0; extra == "all"
 Requires-Dist: torchcam<1.0,>=0.3.1; extra == "all"
 Requires-Dist: tf_explain<1.0,>=0.3.1; extra == "all"
```

### Comparing `TSInterpret-0.4.3/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.4.5/TSInterpret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.4.3/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.4.5/TSInterpret.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 h5py
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
 pytz>=2021.3
 shap<1.0,>=0.39.0
-tensorflow<3.0,>=2.9.1
+tensorflow<=2.14.1,>=2.9.1
 keras<3.0,>=2.9.0
 tsfresh<1.0,>=0.18.0
 tslearn<1.0,>=0.5.2
 seaborn<1.0,>=0.11.2
 scikit_optimize<1.0,>=0.9.0
 torchcam<1.0,>=0.3.1
 tf_explain<1.0,>=0.3.1
@@ -39,15 +39,15 @@
 h5py
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
 pytz>=2021.3
 shap<1.0,>=0.39.0
-tensorflow<3.0,>=2.9.1
+tensorflow<=2.14.1,>=2.9.1
 keras<3.0,>=2.9.0
 tsfresh<1.0,>=0.18.0
 tslearn<1.0,>=0.5.2
 seaborn<1.0,>=0.11.2
 scikit_optimize<1.0,>=0.9.0
 torchcam<1.0,>=0.3.1
 tf_explain<1.0,>=0.3.1
@@ -93,15 +93,15 @@
 h5py
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
 pytz>=2021.3
 shap<1.0,>=0.39.0
-tensorflow<3.0,>=2.9.1
+tensorflow<=2.14.1,>=2.9.1
 keras<3.0,>=2.9.0
 tsfresh<1.0,>=0.18.0
 tslearn<1.0,>=0.5.2
 seaborn<1.0,>=0.11.2
 scikit_optimize<1.0,>=0.9.0
 torchcam<1.0,>=0.3.1
 tf_explain<1.0,>=0.3.1
@@ -149,15 +149,15 @@
 h5py
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
 pytz>=2021.3
 shap<1.0,>=0.39.0
-tensorflow<3.0,>=2.9.1
+tensorflow<=2.14.1,>=2.9.1
 keras<3.0,>=2.9.0
 tsfresh<1.0,>=0.18.0
 tslearn<1.0,>=0.5.2
 seaborn<1.0,>=0.11.2
 scikit_optimize<1.0,>=0.9.0
 torchcam<1.0,>=0.3.1
 tf_explain<1.0,>=0.3.1
```

### Comparing `TSInterpret-0.4.3/setup.py` & `TSInterpret-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "joblib>=1.0.1,< 2.0",
     # "lime==0.2.0.1",
     "Markdown==3.3.4,< 4.0",
     "matplotlib>=3.3.4,< 4.0",
     "partd==1.2.0",
     "pytz>=2021.3",
     "shap>=0.39.0,< 1.0",
-    "tensorflow>=2.9.1,< 3.0",
+    "tensorflow>=2.9.1,<= 2.14.1",
     "keras>=2.9.0,< 3.0",
     "tsfresh>=0.18.0,< 1.0",
     "tslearn>= 0.5.2,< 1.0",
     "seaborn>=0.11.2,< 1.0",
     "scikit_optimize>=0.9.0,< 1.0",
     "torchcam>=0.3.1,< 1.0",
     "tf_explain>=0.3.1,< 1.0",
@@ -132,8 +132,8 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     ext_modules=[],
-)
+)
```

