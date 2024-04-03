# Comparing `tmp/nixtlats-0.2.0.tar.gz` & `tmp/nixtlats-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixtlats-0.2.0.tar", last modified: Fri Mar 22 04:07:11 2024, max compression
+gzip compressed data, was "nixtlats-0.3.0.tar", last modified: Wed Apr  3 02:32:11 2024, max compression
```

## Comparing `nixtlats-0.2.0.tar` & `nixtlats-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:11.515025 nixtlats-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-03-22 04:07:05.000000 nixtlats-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-03-22 04:07:11.515025 nixtlats-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-03-22 04:07:05.000000 nixtlats-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:11.507025 nixtlats-0.2.0/action_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:05.000000 nixtlats-0.2.0/action_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:11.507025 nixtlats-0.2.0/nixtlats/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)    47299 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:11.511025 nixtlats-0.2.0/nixtlats/core/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/core/api_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/core/client_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/core/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/core/jsonable_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/core/remove_none_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/date_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:11.511025 nixtlats-0.2.0/nixtlats/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/distributed/timegpt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:11.511025 nixtlats-0.2.0/nixtlats/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/errors/unprocessable_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    60403 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/timegpt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:11.515025 nixtlats-0.2.0/nixtlats/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_anomaly_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_cross_validation_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_cross_validation_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_cross_validation_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_forecast_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_forecast_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_insample_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/multi_series_insample_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/single_series_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/single_series_forecast_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/single_series_forecast_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/single_series_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/single_series_insample_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/single_series_insample_forecast_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/types/validation_error_loc_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-22 04:07:05.000000 nixtlats-0.2.0/nixtlats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 04:07:11.515025 nixtlats-0.2.0/nixtlats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-03-22 04:07:11.000000 nixtlats-0.2.0/nixtlats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-22 04:07:11.000000 nixtlats-0.2.0/nixtlats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 04:07:11.000000 nixtlats-0.2.0/nixtlats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-22 04:07:11.000000 nixtlats-0.2.0/nixtlats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-22 04:07:11.000000 nixtlats-0.2.0/nixtlats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 04:07:11.515025 nixtlats-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-22 04:07:05.000000 nixtlats-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.102105 nixtlats-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-04-03 02:32:06.000000 nixtlats-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-03 02:32:11.102105 nixtlats-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-03 02:32:06.000000 nixtlats-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.094105 nixtlats-0.3.0/action_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:06.000000 nixtlats-0.3.0/action_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.094105 nixtlats-0.3.0/nixtlats/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20917 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47299 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.098105 nixtlats-0.3.0/nixtlats/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/api_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/client_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/jsonable_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/core/remove_none_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/date_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.098105 nixtlats-0.3.0/nixtlats/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/distributed/nixtla_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.098105 nixtlats-0.3.0/nixtlats/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/errors/unprocessable_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62656 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/nixtla_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.102105 nixtlats-0.3.0/nixtlats/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_anomaly_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/multi_series_insample_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/single_series_insample_forecast_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/types/validation_error_loc_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-03 02:32:06.000000 nixtlats-0.3.0/nixtlats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:32:11.102105 nixtlats-0.3.0/nixtlats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 02:32:11.000000 nixtlats-0.3.0/nixtlats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:32:11.102105 nixtlats-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 02:32:06.000000 nixtlats-0.3.0/setup.py
```

### Comparing `nixtlats-0.2.0/LICENSE` & `nixtlats-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/PKG-INFO` & `nixtlats-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nixtlats
-Version: 0.2.0
-Summary: TimeGPT SDK
+Version: 0.3.0
+Summary: Python SDK for Nixtla API (TimeGPT)
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -81,16 +81,16 @@
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 df = pd.read_csv('https://raw.githubusercontent.com/Nixtla/transfer-learning-time-series/main/datasets/electricity-short.csv')
 
-from nixtlats import TimeGPT
-timegpt = TimeGPT(
-    # defaults to os.environ.get("TIMEGPT_TOKEN")
-    token = 'my_token_provided_by_nixtla'
+from nixtlats import NixtlaClient
+nixtla = NixtlaClient(
+    # defaults to os.environ.get("NIXTLA_API_KEY")
+    api_key = 'my_api_key_provided_by_nixtla'
 )
-fcst_df = timegpt.forecast(df, h=24, level=[80, 90])
+fcst_df = nixtla.forecast(df, h=24, level=[80, 90])
 ```
 
 ![](./nbs/img/forecast_readme.png)
```

### Comparing `nixtlats-0.2.0/README.md` & `nixtlats-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 df = pd.read_csv('https://raw.githubusercontent.com/Nixtla/transfer-learning-time-series/main/datasets/electricity-short.csv')
 
-from nixtlats import TimeGPT
-timegpt = TimeGPT(
-    # defaults to os.environ.get("TIMEGPT_TOKEN")
-    token = 'my_token_provided_by_nixtla'
+from nixtlats import NixtlaClient
+nixtla = NixtlaClient(
+    # defaults to os.environ.get("NIXTLA_API_KEY")
+    api_key = 'my_api_key_provided_by_nixtla'
 )
-fcst_df = timegpt.forecast(df, h=24, level=[80, 90])
+fcst_df = nixtla.forecast(df, h=24, level=[80, 90])
 ```
 
 ![](./nbs/img/forecast_readme.png)
```

### Comparing `nixtlats-0.2.0/nixtlats/client.py` & `nixtlats-0.3.0/nixtlats/client.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/core/__init__.py` & `nixtlats-0.3.0/nixtlats/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/core/client_wrapper.py` & `nixtlats-0.3.0/nixtlats/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/core/datetime_utils.py` & `nixtlats-0.3.0/nixtlats/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/core/jsonable_encoder.py` & `nixtlats-0.3.0/nixtlats/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/date_features.py` & `nixtlats-0.3.0/nixtlats/date_features.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/distributed/timegpt.py` & `nixtlats-0.3.0/nixtlats/distributed/nixtla_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/distributed.timegpt.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/distributed.nixtla_client.ipynb.
 
 # %% auto 0
 __all__ = []
 
-# %% ../../nbs/distributed.timegpt.ipynb 2
+# %% ../../nbs/distributed.nixtla_client.ipynb 2
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 import fugue
 import fugue.api as fa
 from fugue import transform, DataFrame, FugueWorkflow, ExecutionEngine
 from fugue.collections.yielded import Yielded
 from fugue.constants import FUGUE_CONF_WORKFLOW_EXCEPTION_INJECT
 from fugue.execution.factory import make_execution_engine
 from triad import Schema
 
-# %% ../../nbs/distributed.timegpt.ipynb 3
+# %% ../../nbs/distributed.nixtla_client.ipynb 3
 def _cotransform(
     df1: Any,
     df2: Any,
     using: Any,
     schema: Any = None,
     params: Any = None,
     partition: Any = None,
@@ -41,27 +41,27 @@
     tdf.yield_dataframe_as("result", as_local=as_local)
     dag.run(engine, conf=engine_conf)
     result = dag.yields["result"].result  # type:ignore
     if force_output_fugue_dataframe or isinstance(df1, (DataFrame, Yielded)):
         return result
     return result.as_pandas() if result.is_local else result.native  # type:ignore
 
-# %% ../../nbs/distributed.timegpt.ipynb 4
-class _DistributedTimeGPT:
+# %% ../../nbs/distributed.nixtla_client.ipynb 4
+class _DistributedNixtlaClient:
 
     def __init__(
         self,
-        token: Optional[str] = None,
-        environment: Optional[str] = None,
+        api_key: Optional[str] = None,
+        base_url: Optional[str] = None,
         max_retries: int = 6,
         retry_interval: int = 10,
         max_wait_time: int = 60,
     ):
-        self.token = token
-        self.environment = environment
+        self.api_key = api_key
+        self.base_url = base_url
         self.max_retries = max_retries
         self.retry_interval = retry_interval
         self.max_wait_time = max_wait_time
 
     def _distribute_method(
         self,
         method: Callable,
@@ -122,36 +122,36 @@
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         X_df: Optional[fugue.AnyDataFrame] = None,
         level: Optional[List[Union[int, float]]] = None,
         quantiles: Optional[List[float]] = None,
-        fewshot_steps: int = 0,
-        fewshot_loss: str = "default",
+        finetune_steps: int = 0,
+        finetune_loss: str = "default",
         clean_ex_first: bool = True,
-        validate_token: bool = False,
+        validate_api_key: bool = False,
         add_history: bool = False,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         num_partitions: Optional[int] = None,
     ) -> fugue.AnyDataFrame:
         kwargs = dict(
             h=h,
             freq=freq,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             level=level,
             quantiles=quantiles,
-            fewshot_steps=fewshot_steps,
-            fewshot_loss=fewshot_loss,
+            finetune_steps=finetune_steps,
+            finetune_loss=finetune_loss,
             clean_ex_first=clean_ex_first,
-            validate_token=validate_token,
+            validate_api_key=validate_api_key,
             add_history=add_history,
             date_features=date_features,
             date_features_to_one_hot=date_features_to_one_hot,
             model=model,
         )
         schema = self._get_forecast_schema(
             id_col=id_col,
@@ -175,28 +175,28 @@
         df: pd.DataFrame,
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         level: Union[int, float] = 99,
         clean_ex_first: bool = True,
-        validate_token: bool = False,
+        validate_api_key: bool = False,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         num_partitions: Optional[int] = None,
     ) -> fugue.AnyDataFrame:
         kwargs = dict(
             freq=freq,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             level=level,
             clean_ex_first=clean_ex_first,
-            validate_token=validate_token,
+            validate_api_key=validate_api_key,
             date_features=date_features,
             date_features_to_one_hot=date_features_to_one_hot,
             model=model,
         )
         schema = self._get_anomalies_schema(id_col=id_col, time_col=time_col)
         anomalies_df = self._distribute_method(
             method=self._detect_anomalies,
@@ -215,37 +215,37 @@
         h: int,
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         level: Optional[List[Union[int, float]]] = None,
         quantiles: Optional[List[float]] = None,
-        fewshot_steps: int = 0,
-        fewshot_loss: str = "default",
+        finetune_steps: int = 0,
+        finetune_loss: str = "default",
         clean_ex_first: bool = True,
-        validate_token: bool = False,
+        validate_api_key: bool = False,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         n_windows: int = 1,
         step_size: Optional[int] = None,
         num_partitions: Optional[int] = None,
     ) -> fugue.AnyDataFrame:
         kwargs = dict(
             h=h,
             freq=freq,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             level=level,
             quantiles=quantiles,
-            fewshot_steps=fewshot_steps,
-            fewshot_loss=fewshot_loss,
+            finetune_steps=finetune_steps,
+            finetune_loss=finetune_loss,
             clean_ex_first=clean_ex_first,
-            validate_token=validate_token,
+            validate_api_key=validate_api_key,
             date_features=date_features,
             date_features_to_one_hot=date_features_to_one_hot,
             model=model,
             n_windows=n_windows,
             step_size=step_size,
         )
         schema = self._get_forecast_schema(
@@ -261,58 +261,58 @@
             kwargs=kwargs,
             schema=schema,
             num_partitions=num_partitions,
             id_col=id_col,
         )
         return fcst_df
 
-    def _instantiate_timegpt(self):
-        from nixtlats.timegpt import _TimeGPT
+    def _instantiate_nixtla_client(self):
+        from nixtlats.nixtla_client import _NixtlaClient
 
-        timegpt = _TimeGPT(
-            token=self.token,
-            environment=self.environment,
+        nixtla_client = _NixtlaClient(
+            api_key=self.api_key,
+            base_url=self.base_url,
             max_retries=self.max_retries,
             retry_interval=self.retry_interval,
             max_wait_time=self.max_wait_time,
         )
-        return timegpt
+        return nixtla_client
 
     def _forecast(
         self,
         df: pd.DataFrame,
         kwargs,
     ) -> pd.DataFrame:
-        timegpt = self._instantiate_timegpt()
-        return timegpt._forecast(df=df, **kwargs)
+        nixtla_client = self._instantiate_nixtla_client()
+        return nixtla_client._forecast(df=df, **kwargs)
 
     def _forecast_x(
         self,
         df: pd.DataFrame,
         X_df: pd.DataFrame,
         kwargs,
     ) -> pd.DataFrame:
-        timegpt = self._instantiate_timegpt()
-        return timegpt._forecast(df=df, X_df=X_df, **kwargs)
+        nixtla_client = self._instantiate_nixtla_client()
+        return nixtla_client._forecast(df=df, X_df=X_df, **kwargs)
 
     def _detect_anomalies(
         self,
         df: pd.DataFrame,
         kwargs,
     ) -> pd.DataFrame:
-        timegpt = self._instantiate_timegpt()
-        return timegpt._detect_anomalies(df=df, **kwargs)
+        nixtla_client = self._instantiate_nixtla_client()
+        return nixtla_client._detect_anomalies(df=df, **kwargs)
 
     def _cross_validation(
         self,
         df: pd.DataFrame,
         kwargs,
     ) -> pd.DataFrame:
-        timegpt = self._instantiate_timegpt()
-        return timegpt._cross_validation(df=df, **kwargs)
+        nixtla_client = self._instantiate_nixtla_client()
+        return nixtla_client._cross_validation(df=df, **kwargs)
 
     @staticmethod
     def _get_forecast_schema(id_col, time_col, level, quantiles, cv=False):
         schema = f"{id_col}:string,{time_col}:datetime"
         if cv:
             schema = f"{schema},cutoff:datetime"
         schema = f"{schema},TimeGPT:double"
```

### Comparing `nixtlats-0.2.0/nixtlats/timegpt.py` & `nixtlats-0.3.0/nixtlats/nixtla_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/timegpt.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/nixtla_client.ipynb.
 
 # %% auto 0
 __all__ = ['main_logger', 'httpx_logger']
 
-# %% ../nbs/timegpt.ipynb 3
+# %% ../nbs/nixtla_client.ipynb 3
 import functools
 import inspect
 import json
 import logging
 import os
 import requests
 import warnings
@@ -43,38 +43,60 @@
 )
 
 logging.basicConfig(level=logging.INFO)
 main_logger = logging.getLogger(__name__)
 httpx_logger = logging.getLogger("httpx")
 httpx_logger.setLevel(logging.ERROR)
 
-# %% ../nbs/timegpt.ipynb 5
+# %% ../nbs/nixtla_client.ipynb 5
 def deprecated_argument(old_name, new_name):
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             if old_name in kwargs:
                 warnings.warn(
-                    f"'{old_name}' is deprecated; use '{new_name}' instead.",
+                    f"`'{old_name}'` is deprecated; use `'{new_name}'` instead.",
                     FutureWarning,
                 )
                 if new_name in kwargs:
                     raise TypeError(f"{new_name} argument duplicated")
                 kwargs[new_name] = kwargs.pop(old_name)
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
-# %% ../nbs/timegpt.ipynb 6
-deprecated_finetune_steps = deprecated_argument("finetune_steps", "fewshot_steps")
-deprecated_finetune_loss = deprecated_argument("finetune_loss", "fewshot_loss")
+# %% ../nbs/nixtla_client.ipynb 6
+def deprecated_method(new_method):
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            warnings.warn(
+                f"Method `{func.__name__}` is deprecated; "
+                f"use `{new_method}` instead.",
+                FutureWarning,
+            )
+            return getattr(self, new_method)(*args, **kwargs)
+
+        wrapper.__doc__ = func.__doc__
+        return wrapper
+
+    return decorator
+
+# %% ../nbs/nixtla_client.ipynb 7
+deprecated_fewshot_steps = deprecated_argument("fewshot_steps", "finetune_steps")
+deprecated_fewshot_loss = deprecated_argument("fewshot_loss", "finetune_loss")
+deprecated_token = deprecated_argument("token", "api_key")
+deprecated_environment = deprecated_argument("environment", "base_url")
+
+# %% ../nbs/nixtla_client.ipynb 8
+use_validate_api_key = deprecated_method(new_method="validate_api_key")
 
-# %% ../nbs/timegpt.ipynb 7
+# %% ../nbs/nixtla_client.ipynb 9
 date_features_by_freq = {
     # Daily frequencies
     "B": ["year", "month", "day", "weekday"],
     "C": ["year", "month", "day", "weekday"],
     "D": ["year", "month", "day", "weekday"],
     # Weekly
     "W": ["year", "week", "weekday"],
@@ -115,46 +137,46 @@
     # Microseconds
     "U": ["year", "month", "day", "hour", "minute", "second", "microsecond"],
     "us": ["year", "month", "day", "hour", "minute", "second", "microsecond"],
     # Nanoseconds
     "N": [],
 }
 
-# %% ../nbs/timegpt.ipynb 8
-class _TimeGPTModel:
+# %% ../nbs/nixtla_client.ipynb 10
+class _NixtlaClientModel:
 
     def __init__(
         self,
         client: Nixtla,
         h: int,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         freq: str = None,
         level: Optional[List[Union[int, float]]] = None,
         quantiles: Optional[List[float]] = None,
-        fewshot_steps: int = 0,
-        fewshot_loss: str = "default",
+        finetune_steps: int = 0,
+        finetune_loss: str = "default",
         clean_ex_first: bool = True,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         max_retries: int = 6,
         retry_interval: int = 10,
         max_wait_time: int = 6 * 60,
     ):
         self.client = client
         self.h = h
         self.id_col = id_col
         self.time_col = time_col
         self.target_col = target_col
         self.base_freq = freq
         self.level, self.quantiles = self._prepare_level_and_quantiles(level, quantiles)
-        self.fewshot_steps = fewshot_steps
-        self.fewshot_loss = fewshot_loss
+        self.finetune_steps = finetune_steps
+        self.finetune_loss = finetune_loss
         self.clean_ex_first = clean_ex_first
         self.date_features = date_features
         self.date_features_to_one_hot = date_features_to_one_hot
         self.model = model
         self.max_retries = max_retries
         self.retry_interval = retry_interval
         self.max_wait_time = max_wait_time
@@ -516,46 +538,46 @@
         if self.h > self.model_horizon:
             main_logger.warning(
                 'The specified horizon "h" exceeds the model horizon. '
                 "This may lead to less accurate forecasts. "
                 "Please consider using a smaller horizon."
             )
         # restrict input if
-        # - we dont want to fewshot
+        # - we dont want to finetune
         # - we dont have exogenous regegressors
         # - and we dont want to produce pred intervals
         # - no add history
         restrict_input = (
-            self.fewshot_steps == 0
+            self.finetune_steps == 0
             and X_df is None
             and self.level is not None
             and not add_history
         )
         if restrict_input:
             # add sufficient info to compute
             # conformal interval
             main_logger.info("Restricting input...")
             new_input_size = 3 * self.input_size + max(self.model_horizon, self.h)
             Y_df = Y_df.groupby("unique_id").tail(new_input_size)
             if X_df is not None:
                 X_df = X_df.groupby("unique_id").tail(
                     new_input_size + self.h
                 )  # history plus exogenous
-        if self.fewshot_steps > 0 or self.level is not None:
+        if self.finetune_steps > 0 or self.level is not None:
             self.validate_input_size(Y_df=Y_df)
         y, x = self.dataframes_to_dict(Y_df, X_df)
         main_logger.info("Calling Forecast Endpoint...")
         payload = MultiSeriesForecast(
             y=y,
             x=x,
             fh=self.h,
             freq=self.freq,
             level=self.level,
-            fewshot_steps=self.fewshot_steps,
-            fewshot_loss=self.fewshot_loss,
+            finetune_steps=self.finetune_steps,
+            finetune_loss=self.finetune_loss,
             clean_ex_first=self.clean_ex_first,
             model=self.model,
         )
         response_timegpt = self._call_api(
             self.client.forecast_multi_series,
             payload,
         )
@@ -683,22 +705,22 @@
         first_out_cols = ["unique_id", "ds", "cutoff", "y"]
         remaining_cols = [c for c in out.columns if c not in first_out_cols]
         fcst_cv_df = out[first_out_cols + remaining_cols]
         fcst_cv_df["ds"] = fcst_cv_df["ds"].astype(str)
         fcst_cv_df = self.transform_outputs(fcst_cv_df)
         return fcst_cv_df
 
-# %% ../nbs/timegpt.ipynb 9
+# %% ../nbs/nixtla_client.ipynb 11
 def validate_model_parameter(func):
     def wrapper(self, *args, **kwargs):
         if "model" in kwargs:
             model = kwargs["model"]
             rename_models_dict = {
-                "timegpt-1": "short-horizon",
-                "timegpt-1-long-horizon": "long-horizon",
+                "short-horizon": "timegpt-1",
+                "long-horizon": "timegpt-1-long-horizon",
             }
             if model in rename_models_dict.keys():
                 new_model = rename_models_dict[model]
                 warnings.warn(
                     f"'{model}' is deprecated; use '{new_model}' instead.",
                     FutureWarning,
                 )
@@ -708,25 +730,25 @@
                     f'unsupported model: {kwargs["model"]} '
                     f'supported models: {", ".join(self.supported_models)}'
                 )
         return func(self, *args, **kwargs)
 
     return wrapper
 
-# %% ../nbs/timegpt.ipynb 10
+# %% ../nbs/nixtla_client.ipynb 12
 def remove_unused_categories(df: pd.DataFrame, col: str):
     """Check if col exists in df and if it is a category column.
     In that case, it removes the unused levels."""
     if df is not None and col in df:
         if df[col].dtype == "category":
             df = df.copy()
             df[col] = df[col].cat.remove_unused_categories()
     return df
 
-# %% ../nbs/timegpt.ipynb 11
+# %% ../nbs/nixtla_client.ipynb 13
 def partition_by_uid(func):
     def wrapper(self, num_partitions, **kwargs):
         if num_partitions is None or num_partitions == 1:
             return func(self, **kwargs, num_partitions=1)
         df = kwargs.pop("df")
         X_df = kwargs.pop("X_df", None)
         id_col = kwargs["id_col"]
@@ -746,38 +768,40 @@
             results_uids = func(self, **kwargs_uids, num_partitions=1)
             results_df.append(results_uids)
         results_df = pd.concat(results_df).reset_index(drop=True)
         return results_df
 
     return wrapper
 
-# %% ../nbs/timegpt.ipynb 12
-class _TimeGPT:
+# %% ../nbs/nixtla_client.ipynb 14
+class _NixtlaClient:
     """
-    A class used to interact with the TimeGPT API.
+    A class used to interact with Nixtla API.
     """
 
+    @deprecated_token
+    @deprecated_environment
     def __init__(
         self,
-        token: Optional[str] = None,
-        environment: Optional[str] = None,
+        api_key: Optional[str] = None,
+        base_url: Optional[str] = None,
         max_retries: int = 6,
         retry_interval: int = 10,
         max_wait_time: int = 6 * 60,
     ):
         """
-        Constructs all the necessary attributes for the TimeGPT object.
+        Constructs all the necessary attributes for the NixtlaClient object.
 
         Parameters
         ----------
-        token : str, (default=None)
-            The authorization token interacts with the TimeGPT API.
-            If not provided, it will be inferred by the TIMEGPT_TOKEN environment variable.
-        environment : str, (default=None)
-            Custom environment. Pass only if provided.
+        api_key : str, (default=None)
+            The authorization api_key interacts with the Nixtla API.
+            If not provided, it will be inferred by the NIXTLA_API_KEY environment variable.
+        base_url : str, (default=None)
+            Custom base_url. Pass only if provided.
         max_retries : int, (default=6)
             The maximum number of attempts to make when calling the API before giving up.
             It defines how many times the client will retry the API call if it fails.
             Default value is 6, indicating the client will attempt the API call up to 6 times in total
         retry_interval : int, (default=10)
             The interval in seconds between consecutive retry attempts.
             This is the waiting period before the client tries to call the API again after a failed attempt.
@@ -787,35 +811,53 @@
             This sets an upper limit on the cumulative waiting time for all retry attempts.
             If this time is exceeded, the client will stop retrying and raise an exception.
             Default value is 360 seconds, meaning the client will cease retrying if the total time
             spent on retries exceeds 360 seconds.
             The client throws a ReadTimeout error after 60 seconds of inactivity. If you want to
             catch these errors, use max_wait_time >> 60.
         """
-        if token is None:
-            token = os.environ.get("TIMEGPT_TOKEN")
-        if token is None:
+        if api_key is None:
+            timegpt_token = os.environ.get("TIMEGPT_TOKEN")
+            if timegpt_token is not None:
+                warnings.warn(
+                    f"`TIMEGPT_TOKEN` environment variable is deprecated; "
+                    "use `NIXTLA_API_KEY` instead.",
+                    FutureWarning,
+                )
+            api_key = os.environ.get("NIXTLA_API_KEY", timegpt_token)
+        if api_key is None:
             raise Exception(
-                "The token must be set either by passing `token` "
-                "or by setting the TIMEGPT_TOKEN environment variable."
+                "The api_key must be set either by passing `api_key` "
+                "or by setting the `NIXTLA_API_KEY` environment variable."
             )
-        if environment is None:
-            environment = "https://dashboard.nixtla.io/api"
-        self.client = Nixtla(base_url=environment, token=token)
+        if base_url is None:
+            base_url = os.environ.get(
+                "NIXTLA_BASE_URL",
+                "https://dashboard.nixtla.io/api",
+            )
+        self.client = Nixtla(base_url=base_url, token=api_key)
         self.max_retries = max_retries
         self.retry_interval = retry_interval
         self.max_wait_time = max_wait_time
-        self.supported_models = ["short-horizon", "long-horizon"]
+        self.supported_models = ["timegpt-1", "timegpt-1-long-horizon"]
         # custom attr
         self.weights_x: pd.DataFrame = None
 
-    def validate_token(self, log: bool = True) -> bool:
-        """Returns True if your token is valid."""
-        validation = self.client.validate_token()
+    @use_validate_api_key
+    def validate_token(self):
+        """this is deprecated in favor of validate_api_key"""
+        pass
+
+    def validate_api_key(self, log: bool = True) -> bool:
+        """Returns True if your api_key is valid."""
         valid = False
+        try:
+            validation = self.client.validate_token()
+        except:
+            validation = dict()
         if "message" in validation:
             if validation["message"] == "success":
                 valid = True
         elif "detail" in validation:
             if "Forecasting! :)" in validation["detail"]:
                 valid = True
         if "support" in validation and log:
@@ -831,69 +873,71 @@
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         X_df: Optional[pd.DataFrame] = None,
         level: Optional[List[Union[int, float]]] = None,
         quantiles: Optional[List[float]] = None,
-        fewshot_steps: int = 0,
-        fewshot_loss: str = "default",
+        finetune_steps: int = 0,
+        finetune_loss: str = "default",
         clean_ex_first: bool = True,
-        validate_token: bool = False,
+        validate_api_key: bool = False,
         add_history: bool = False,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         num_partitions: int = 1,
     ):
-        if validate_token and not self.validate_token(log=False):
-            raise Exception("Token not valid, please email ops@nixtla.io")
-        timegpt_model = _TimeGPTModel(
+        if validate_api_key and not self.validate_api_key(log=False):
+            raise Exception("API Key not valid, please email ops@nixtla.io")
+        nixtla_client_model = _NixtlaClientModel(
             client=self.client,
             h=h,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             freq=freq,
             level=level,
             quantiles=quantiles,
-            fewshot_steps=fewshot_steps,
-            fewshot_loss=fewshot_loss,
+            finetune_steps=finetune_steps,
+            finetune_loss=finetune_loss,
             clean_ex_first=clean_ex_first,
             date_features=date_features,
             date_features_to_one_hot=date_features_to_one_hot,
             model=model,
             max_retries=self.max_retries,
             retry_interval=self.retry_interval,
             max_wait_time=self.max_wait_time,
         )
-        fcst_df = timegpt_model.forecast(df=df, X_df=X_df, add_history=add_history)
-        self.weights_x = timegpt_model.weights_x
+        fcst_df = nixtla_client_model.forecast(
+            df=df, X_df=X_df, add_history=add_history
+        )
+        self.weights_x = nixtla_client_model.weights_x
         return fcst_df
 
     @validate_model_parameter
     @partition_by_uid
     def _detect_anomalies(
         self,
         df: pd.DataFrame,
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         level: Union[int, float] = 99,
         clean_ex_first: bool = True,
-        validate_token: bool = False,
+        validate_api_key: bool = False,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         num_partitions: int = 1,
     ):
-        if validate_token and not self.validate_token(log=False):
-            raise Exception("Token not valid, please email ops@nixtla.io")
-        timegpt_model = _TimeGPTModel(
+        if validate_api_key and not self.validate_api_key(log=False):
+            raise Exception("API Key not valid, please email ops@nixtla.io")
+        nixtla_client_model = _NixtlaClientModel(
             client=self.client,
             h=None,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             freq=freq,
             level=level,
@@ -901,66 +945,66 @@
             date_features=date_features,
             date_features_to_one_hot=date_features_to_one_hot,
             model=model,
             max_retries=self.max_retries,
             retry_interval=self.retry_interval,
             max_wait_time=self.max_wait_time,
         )
-        anomalies_df = timegpt_model.detect_anomalies(df=df)
-        self.weights_x = timegpt_model.weights_x
+        anomalies_df = nixtla_client_model.detect_anomalies(df=df)
+        self.weights_x = nixtla_client_model.weights_x
         return anomalies_df
 
     @validate_model_parameter
     @partition_by_uid
     def _cross_validation(
         self,
         df: pd.DataFrame,
         h: int,
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         level: Optional[List[Union[int, float]]] = None,
         quantiles: Optional[List[float]] = None,
-        validate_token: bool = False,
+        validate_api_key: bool = False,
         n_windows: int = 1,
         step_size: Optional[int] = None,
-        fewshot_steps: int = 0,
-        fewshot_loss: str = "default",
+        finetune_steps: int = 0,
+        finetune_loss: str = "default",
         clean_ex_first: bool = True,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         num_partitions: int = 1,
     ):
-        if validate_token and not self.validate_token(log=False):
-            raise Exception("Token not valid, please email ops@nixtla.io")
-        timegpt_model = _TimeGPTModel(
+        if validate_api_key and not self.validate_api_key(log=False):
+            raise Exception("API Key not valid, please email ops@nixtla.io")
+        nixtla_client_model = _NixtlaClientModel(
             client=self.client,
             h=h,
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
             freq=freq,
             level=level,
             quantiles=quantiles,
-            fewshot_steps=fewshot_steps,
-            fewshot_loss=fewshot_loss,
+            finetune_steps=finetune_steps,
+            finetune_loss=finetune_loss,
             clean_ex_first=clean_ex_first,
             date_features=date_features,
             date_features_to_one_hot=date_features_to_one_hot,
             model=model,
             max_retries=self.max_retries,
             retry_interval=self.retry_interval,
             max_wait_time=self.max_wait_time,
         )
-        cv_df = timegpt_model.cross_validation(
+        cv_df = nixtla_client_model.cross_validation(
             df=df, n_windows=n_windows, step_size=step_size
         )
-        self.weights_x = timegpt_model.weights_x
+        self.weights_x = nixtla_client_model.weights_x
         return cv_df
 
     def plot(
         self,
         df: pd.DataFrame,
         forecasts_df: Optional[pd.DataFrame] = None,
         id_col: str = "unique_id",
@@ -1064,50 +1108,50 @@
             resampler_kwargs=resampler_kwargs,
             palette="tab20b",
             id_col=id_col,
             time_col=time_col,
             target_col=target_col,
         )
 
-# %% ../nbs/timegpt.ipynb 13
-class TimeGPT(_TimeGPT):
+# %% ../nbs/nixtla_client.ipynb 15
+class NixtlaClient(_NixtlaClient):
 
-    def _instantiate_distributed_timegpt(self):
-        from nixtlats.distributed.timegpt import _DistributedTimeGPT
+    def _instantiate_distributed_nixtla_client(self):
+        from nixtlats.distributed.nixtla_client import _DistributedNixtlaClient
 
-        dist_timegpt = _DistributedTimeGPT(
-            token=self.client._client_wrapper._token,
-            environment=self.client._client_wrapper._base_url,
+        dist_nixtla_client = _DistributedNixtlaClient(
+            api_key=self.client._client_wrapper._token,
+            base_url=self.client._client_wrapper._base_url,
             max_retries=self.max_retries,
             retry_interval=self.retry_interval,
             max_wait_time=self.max_wait_time,
         )
-        return dist_timegpt
+        return dist_nixtla_client
 
-    @deprecated_finetune_steps
-    @deprecated_finetune_loss
+    @deprecated_fewshot_loss
+    @deprecated_fewshot_steps
     def forecast(
         self,
         df: pd.DataFrame,
         h: int,
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         X_df: Optional[pd.DataFrame] = None,
         level: Optional[List[Union[int, float]]] = None,
         quantiles: Optional[List[float]] = None,
-        fewshot_steps: int = 0,
-        fewshot_loss: str = "default",
+        finetune_steps: int = 0,
+        finetune_loss: str = "default",
         clean_ex_first: bool = True,
-        validate_token: bool = False,
+        validate_api_key: bool = False,
         add_history: bool = False,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         num_partitions: Optional[int] = None,
     ):
         """Forecast your time series using TimeGPT.
 
         Parameters
         ----------
         df : pandas.DataFrame
@@ -1137,42 +1181,42 @@
             DataFrame with [`unique_id`, `ds`] columns and `df`'s future exogenous.
         level : List[float], optional (default=None)
             Confidence levels between 0 and 100 for prediction intervals.
         quantiles : List[float], optional (default=None)
             Quantiles to forecast, list between (0, 1).
             `level` and `quantiles` should not be used simultaneously.
             The output dataframe will have the quantile columns
-            formatted as TimeGPT-q-{int(100 * q)} for each q.
+            formatted as TimeGPT-q-(100 * q) for each q.
             100 * q represents percentiles but we choose this notation
-            to avoid handling __dots__ (.) in names.
-        fewshot_steps : int (default=0)
-            Number of steps used to fewshot learning TimeGPT in the
+            to avoid having dots in column names.
+        finetune_steps : int (default=0)
+            Number of steps used to finetune learning TimeGPT in the
             new data.
-        fewshot_loss : str (default='default')
+        finetune_loss : str (default='default')
             Loss function to use for finetuning. Options are: `default`, `mae`, `mse`, `rmse`, `mape`, and `smape`.
         clean_ex_first : bool (default=True)
             Clean exogenous signal before making forecasts
             using TimeGPT.
-        validate_token : bool (default=False)
-            If True, validates token before
+        validate_api_key : bool (default=False)
+            If True, validates api_key before
             sending requests.
         add_history : bool (default=False)
             Return fitted values of the model.
         date_features : bool or list of str or callable, optional (default=False)
             Features computed from the dates.
             Can be pandas date attributes or functions that will take the dates as input.
             If True automatically adds most used date features for the
             frequency of `df`.
         date_features_to_one_hot : bool or list of str (default=True)
             Apply one-hot encoding to these date features.
             If `date_features=True`, then all date features are
             one-hot encoded by default.
-        model : str (default='short-horizon')
-            Model to use as a string. Options are: `short-horizon`, and `long-horizon`.
-            We recommend using `long-horizon` for forecasting
+        model : str (default='timegpt-1')
+            Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon`.
+            We recommend using `timegpt-1-long-horizon` for forecasting
             if you want to predict more than one seasonal
             period given the frequency of your data.
         num_partitions : int (default=None)
             Number of partitions to use.
             If None, the number of partitions will be equal
             to the available parallel resources in distributed environments.
 
@@ -1189,40 +1233,40 @@
                 freq=freq,
                 id_col=id_col,
                 time_col=time_col,
                 target_col=target_col,
                 X_df=X_df,
                 level=level,
                 quantiles=quantiles,
-                fewshot_steps=fewshot_steps,
-                fewshot_loss=fewshot_loss,
+                finetune_steps=finetune_steps,
+                finetune_loss=finetune_loss,
                 clean_ex_first=clean_ex_first,
-                validate_token=validate_token,
+                validate_api_key=validate_api_key,
                 add_history=add_history,
                 date_features=date_features,
                 date_features_to_one_hot=date_features_to_one_hot,
                 model=model,
                 num_partitions=num_partitions,
             )
         else:
-            dist_timegpt = self._instantiate_distributed_timegpt()
-            return dist_timegpt.forecast(
+            dist_nixtla_client = self._instantiate_distributed_nixtla_client()
+            return dist_nixtla_client.forecast(
                 df=df,
                 h=h,
                 freq=freq,
                 id_col=id_col,
                 time_col=time_col,
                 target_col=target_col,
                 X_df=X_df,
                 level=level,
                 quantiles=quantiles,
-                fewshot_steps=fewshot_steps,
-                fewshot_loss=fewshot_loss,
+                finetune_steps=finetune_steps,
+                finetune_loss=finetune_loss,
                 clean_ex_first=clean_ex_first,
-                validate_token=validate_token,
+                validate_api_key=validate_api_key,
                 add_history=add_history,
                 date_features=date_features,
                 date_features_to_one_hot=date_features_to_one_hot,
                 model=model,
                 num_partitions=num_partitions,
             )
 
@@ -1231,18 +1275,18 @@
         df: pd.DataFrame,
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         level: Union[int, float] = 99,
         clean_ex_first: bool = True,
-        validate_token: bool = False,
+        validate_api_key: bool = False,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         num_partitions: Optional[int] = None,
     ):
         """Detect anomalies in your time series using TimeGPT.
 
         Parameters
         ----------
         df : pandas.DataFrame
@@ -1267,29 +1311,29 @@
         target_col : str (default='y')
             Column that contains the target.
         level : float (default=99)
             Confidence level between 0 and 100 for detecting the anomalies.
         clean_ex_first : bool (default=True)
             Clean exogenous signal before making forecasts
             using TimeGPT.
-        validate_token : bool (default=False)
-            If True, validates token before
+        validate_api_key : bool (default=False)
+            If True, validates api_key before
             sending requests.
         date_features : bool or list of str or callable, optional (default=False)
             Features computed from the dates.
             Can be pandas date attributes or functions that will take the dates as input.
             If True automatically adds most used date features for the
             frequency of `df`.
         date_features_to_one_hot : bool or list of str (default=True)
             Apply one-hot encoding to these date features.
             If `date_features=True`, then all date features are
             one-hot encoded by default.
-        model : str (default='short-horizon')
-            Model to use as a string. Options are: `short-horizon`, and `long-horizon`.
-            We recommend using `long-horizon` for forecasting
+        model : str (default='timegpt-1')
+            Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon`.
+            We recommend using `timegpt-1-long-horizon` for forecasting
             if you want to predict more than one seasonal
             period given the frequency of your data.
         num_partitions : int (default=None)
             Number of partitions to use.
             If None, the number of partitions will be equal
             to the available parallel resources in distributed environments.
 
@@ -1303,58 +1347,58 @@
                 df=df,
                 freq=freq,
                 id_col=id_col,
                 time_col=time_col,
                 target_col=target_col,
                 level=level,
                 clean_ex_first=clean_ex_first,
-                validate_token=validate_token,
+                validate_api_key=validate_api_key,
                 date_features=date_features,
                 date_features_to_one_hot=date_features_to_one_hot,
                 model=model,
                 num_partitions=num_partitions,
             )
         else:
-            dist_timegpt = self._instantiate_distributed_timegpt()
-            return dist_timegpt.detect_anomalies(
+            dist_nixtla_client = self._instantiate_distributed_nixtla_client()
+            return dist_nixtla_client.detect_anomalies(
                 df=df,
                 freq=freq,
                 id_col=id_col,
                 time_col=time_col,
                 target_col=target_col,
                 level=level,
                 clean_ex_first=clean_ex_first,
-                validate_token=validate_token,
+                validate_api_key=validate_api_key,
                 date_features=date_features,
                 date_features_to_one_hot=date_features_to_one_hot,
                 model=model,
                 num_partitions=num_partitions,
             )
 
-    @deprecated_finetune_steps
-    @deprecated_finetune_loss
+    @deprecated_fewshot_loss
+    @deprecated_fewshot_steps
     def cross_validation(
         self,
         df: pd.DataFrame,
         h: int,
         freq: Optional[str] = None,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
         level: Optional[List[Union[int, float]]] = None,
         quantiles: Optional[List[float]] = None,
-        validate_token: bool = False,
+        validate_api_key: bool = False,
         n_windows: int = 1,
         step_size: Optional[int] = None,
-        fewshot_steps: int = 0,
-        fewshot_loss: str = "default",
+        finetune_steps: int = 0,
+        finetune_loss: str = "default",
         clean_ex_first: bool = True,
         date_features: Union[bool, List[str]] = False,
         date_features_to_one_hot: Union[bool, List[str]] = True,
-        model: str = "short-horizon",
+        model: str = "timegpt-1",
         num_partitions: Optional[int] = None,
     ):
         """Perform cross validation in your time series using TimeGPT.
 
         Parameters
         ----------
         df : pandas.DataFrame
@@ -1382,44 +1426,44 @@
             Column that contains the target.
         level : float (default=99)
             Confidence level between 0 and 100 for prediction intervals.
         quantiles : List[float], optional (default=None)
             Quantiles to forecast, list between (0, 1).
             `level` and `quantiles` should not be used simultaneously.
             The output dataframe will have the quantile columns
-            formatted as TimeGPT-q-{int(100 * q)} for each q.
+            formatted as TimeGPT-q-(100 * q) for each q.
             100 * q represents percentiles but we choose this notation
-            to avoid handling __dots__ (.) in names.
-        validate_token : bool (default=False)
-            If True, validates token before
+            to avoid having dots in column names..
+        validate_api_key : bool (default=False)
+            If True, validates api_key before
             sending requests.
         n_windows : int (defaul=1)
             Number of windows to evaluate.
         step_size : int, optional (default=None)
             Step size between each cross validation window. If None it will be equal to `h`.
-        fewshot_steps : int (default=0)
-            Number of steps used to fewshot TimeGPT in the
+        finetune_steps : int (default=0)
+            Number of steps used to finetune TimeGPT in the
             new data.
-        fewshot_loss : str (default='default')
+        finetune_loss : str (default='default')
             Loss function to use for finetuning. Options are: `default`, `mae`, `mse`, `rmse`, `mape`, and `smape`.
         clean_ex_first : bool (default=True)
             Clean exogenous signal before making forecasts
             using TimeGPT.
         date_features : bool or list of str or callable, optional (default=False)
             Features computed from the dates.
             Can be pandas date attributes or functions that will take the dates as input.
             If True automatically adds most used date features for the
             frequency of `df`.
         date_features_to_one_hot : bool or list of str (default=True)
             Apply one-hot encoding to these date features.
             If `date_features=True`, then all date features are
             one-hot encoded by default.
-        model : str (default='short-horizon')
-            Model to use as a string. Options are: `short-horizon`, and `long-horizon`.
-            We recommend using `long-horizon` for forecasting
+        model : str (default='timegpt-1')
+            Model to use as a string. Options are: `timegpt-1`, and `timegpt-1-long-horizon`.
+            We recommend using `timegpt-1-long-horizon` for forecasting
             if you want to predict more than one seasonal
             period given the frequency of your data.
         num_partitions : int (default=None)
             Number of partitions to use.
             If None, the number of partitions will be equal
             to the available parallel resources in distributed environments.
 
@@ -1434,40 +1478,57 @@
                 h=h,
                 freq=freq,
                 id_col=id_col,
                 time_col=time_col,
                 target_col=target_col,
                 level=level,
                 quantiles=quantiles,
-                fewshot_steps=fewshot_steps,
-                fewshot_loss=fewshot_loss,
+                finetune_steps=finetune_steps,
+                finetune_loss=finetune_loss,
                 clean_ex_first=clean_ex_first,
-                validate_token=validate_token,
+                validate_api_key=validate_api_key,
                 date_features=date_features,
                 date_features_to_one_hot=date_features_to_one_hot,
                 model=model,
                 n_windows=n_windows,
                 step_size=step_size,
                 num_partitions=num_partitions,
             )
         else:
-            dist_timegpt = self._instantiate_distributed_timegpt()
-            return dist_timegpt.cross_validation(
+            dist_nixtla_client = self._instantiate_distributed_nixtla_client()
+            return dist_nixtla_client.cross_validation(
                 df=df,
                 h=h,
                 freq=freq,
                 id_col=id_col,
                 time_col=time_col,
                 target_col=target_col,
                 level=level,
                 quantiles=quantiles,
-                fewshot_steps=fewshot_steps,
-                fewshot_loss=fewshot_loss,
+                finetune_steps=finetune_steps,
+                finetune_loss=finetune_loss,
                 clean_ex_first=clean_ex_first,
-                validate_token=validate_token,
+                validate_api_key=validate_api_key,
                 date_features=date_features,
                 date_features_to_one_hot=date_features_to_one_hot,
                 model=model,
                 num_partitions=num_partitions,
                 n_windows=n_windows,
                 step_size=step_size,
             )
+
+# %% ../nbs/nixtla_client.ipynb 16
+class TimeGPT(NixtlaClient):
+    """
+    Class `TimeGPT` is deprecated; use `NixtlaClient` instead.
+
+    This class is deprecated and may be removed in future releases.
+    Please use `NixtlaClient` instead.
+
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        warnings.warn(
+            "Class `TimeGPT` is deprecated; use `NixtlaClient` instead.",
+            FutureWarning,
+        )
```

### Comparing `nixtlats-0.2.0/nixtlats/types/__init__.py` & `nixtlats-0.3.0/nixtlats/types/__init__.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/http_validation_error.py` & `nixtlats-0.3.0/nixtlats/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_anomaly.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_anomaly.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_anomaly_model.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_anomaly_model.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_cross_validation.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_cross_validation_fewshot_loss.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_fewshot_loss.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_cross_validation_finetune_loss.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_finetune_loss.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_cross_validation_model.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_cross_validation_model.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_forecast.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_forecast.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_forecast_fewshot_loss.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_forecast_fewshot_loss.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_forecast_finetune_loss.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_forecast_finetune_loss.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_forecast_model.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_forecast_model.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_input.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_input.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_insample_forecast.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_insample_forecast.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/multi_series_insample_forecast_model.py` & `nixtlats-0.3.0/nixtlats/types/multi_series_insample_forecast_model.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/single_series_forecast.py` & `nixtlats-0.3.0/nixtlats/types/single_series_forecast.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/single_series_forecast_fewshot_loss.py` & `nixtlats-0.3.0/nixtlats/types/single_series_forecast_fewshot_loss.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/single_series_forecast_finetune_loss.py` & `nixtlats-0.3.0/nixtlats/types/single_series_forecast_finetune_loss.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/single_series_forecast_model.py` & `nixtlats-0.3.0/nixtlats/types/single_series_forecast_model.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/single_series_insample_forecast.py` & `nixtlats-0.3.0/nixtlats/types/single_series_insample_forecast.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/single_series_insample_forecast_model.py` & `nixtlats-0.3.0/nixtlats/types/single_series_insample_forecast_model.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats/types/validation_error.py` & `nixtlats-0.3.0/nixtlats/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `nixtlats-0.2.0/nixtlats.egg-info/PKG-INFO` & `nixtlats-0.3.0/nixtlats.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nixtlats
-Version: 0.2.0
-Summary: TimeGPT SDK
+Version: 0.3.0
+Summary: Python SDK for Nixtla API (TimeGPT)
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -81,16 +81,16 @@
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 df = pd.read_csv('https://raw.githubusercontent.com/Nixtla/transfer-learning-time-series/main/datasets/electricity-short.csv')
 
-from nixtlats import TimeGPT
-timegpt = TimeGPT(
-    # defaults to os.environ.get("TIMEGPT_TOKEN")
-    token = 'my_token_provided_by_nixtla'
+from nixtlats import NixtlaClient
+nixtla = NixtlaClient(
+    # defaults to os.environ.get("NIXTLA_API_KEY")
+    api_key = 'my_api_key_provided_by_nixtla'
 )
-fcst_df = timegpt.forecast(df, h=24, level=[80, 90])
+fcst_df = nixtla.forecast(df, h=24, level=[80, 90])
 ```
 
 ![](./nbs/img/forecast_readme.png)
```

### Comparing `nixtlats-0.2.0/nixtlats.egg-info/SOURCES.txt` & `nixtlats-0.3.0/nixtlats.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 README.md
 setup.py
 action_files/__init__.py
 nixtlats/__init__.py
 nixtlats/_modidx.py
 nixtlats/client.py
 nixtlats/date_features.py
+nixtlats/nixtla_client.py
 nixtlats/py.typed
-nixtlats/timegpt.py
 nixtlats/utils.py
 nixtlats.egg-info/PKG-INFO
 nixtlats.egg-info/SOURCES.txt
 nixtlats.egg-info/dependency_links.txt
 nixtlats.egg-info/requires.txt
 nixtlats.egg-info/top_level.txt
 nixtlats/core/__init__.py
 nixtlats/core/api_error.py
 nixtlats/core/client_wrapper.py
 nixtlats/core/datetime_utils.py
 nixtlats/core/jsonable_encoder.py
 nixtlats/core/remove_none_from_dict.py
 nixtlats/distributed/__init__.py
-nixtlats/distributed/timegpt.py
+nixtlats/distributed/nixtla_client.py
 nixtlats/errors/__init__.py
 nixtlats/errors/unprocessable_entity_error.py
 nixtlats/types/__init__.py
 nixtlats/types/http_validation_error.py
 nixtlats/types/multi_series_anomaly.py
 nixtlats/types/multi_series_anomaly_model.py
 nixtlats/types/multi_series_cross_validation.py
```

### Comparing `nixtlats-0.2.0/setup.py` & `nixtlats-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 ]
 distributed = ["dask[dataframe]", "fugue[ray]>=0.8.7", "pyspark", "ray[serve-grpc]"]
 plotting = ["utilsforecast[plotting]>=0.0.5"]
 date_extras = ["holidays"]
 
 setuptools.setup(
     name="nixtlats",
-    version="0.2.0",
-    description="TimeGPT SDK",
+    version="0.3.0",
+    description="Python SDK for Nixtla API (TimeGPT)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nixtla/nixtla",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

