# Comparing `tmp/arize-7.8.1.tar.gz` & `tmp/arize-7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.8.1.tar", last modified: Tue Dec 19 04:58:51 2023, max compression
+gzip compressed data, was "arize-7.9.0.tar", last modified: Thu Dec 28 20:00:43 2023, max compression
```

## Comparing `arize-7.8.1.tar` & `arize-7.9.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.027353 arize-7.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-19 04:58:29.000000 arize-7.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-19 04:58:29.000000 arize-7.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13735 2023-12-19 04:58:51.027353 arize-7.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2023-12-19 04:58:29.000000 arize-7.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.019353 arize-7.8.1/arize/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-19 04:58:29.000000 arize-7.8.1/arize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40947 2023-12-19 04:58:29.000000 arize-7.8.1/arize/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-12-19 04:58:29.000000 arize-7.8.1/arize/bounded_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.019353 arize-7.8.1/arize/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:29.000000 arize-7.8.1/arize/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-12-19 04:58:29.000000 arize-7.8.1/arize/examples/bulk_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-12-19 04:58:29.000000 arize-7.8.1/arize/examples/bulk_client_shap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2023-12-19 04:58:29.000000 arize-7.8.1/arize/examples/client_shap_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2023-12-19 04:58:29.000000 arize-7.8.1/arize/examples/log_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2023-12-19 04:58:29.000000 arize-7.8.1/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2023-12-19 04:58:29.000000 arize-7.8.1/arize/examples/preproduction_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.019353 arize-7.8.1/arize/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.019353 arize-7.8.1/arize/exporter/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11599 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/core/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/core/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/publicexporter_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.019353 arize-7.8.1/arize/exporter/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/utils/schema_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-12-19 04:58:29.000000 arize-7.8.1/arize/exporter/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.019353 arize-7.8.1/arize/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.023353 arize-7.8.1/arize/pandas/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/embeddings/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/embeddings/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.023353 arize-7.8.1/arize/pandas/generative/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.023353 arize-7.8.1/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12178 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    21795 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.023353 arize-7.8.1/arize/pandas/surrogate_explainer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.023353 arize-7.8.1/arize/pandas/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28393 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)   104885 2023-12-19 04:58:29.000000 arize-7.8.1/arize/pandas/validation/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    63949 2023-12-19 04:58:29.000000 arize-7.8.1/arize/public_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.023353 arize-7.8.1/arize/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:29.000000 arize-7.8.1/arize/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-12-19 04:58:29.000000 arize-7.8.1/arize/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2023-12-19 04:58:29.000000 arize-7.8.1/arize/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-12-19 04:58:29.000000 arize-7.8.1/arize/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2023-12-19 04:58:29.000000 arize-7.8.1/arize/utils/model_mapping.json
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2023-12-19 04:58:29.000000 arize-7.8.1/arize/utils/proto.py
--rw-r--r--   0 runner    (1001) docker     (127)    34860 2023-12-19 04:58:29.000000 arize-7.8.1/arize/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2023-12-19 04:58:29.000000 arize-7.8.1/arize/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.023353 arize-7.8.1/arize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13735 2023-12-19 04:58:51.000000 arize-7.8.1/arize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-12-19 04:58:51.000000 arize-7.8.1/arize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 04:58:51.000000 arize-7.8.1/arize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-19 04:58:51.000000 arize-7.8.1/arize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-19 04:58:51.000000 arize-7.8.1/arize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-19 04:58:29.000000 arize-7.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-19 04:58:51.031353 arize-7.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 04:58:51.023353 arize-7.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    83846 2023-12-19 04:58:29.000000 arize-7.8.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-19 04:58:29.000000 arize-7.8.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.797476 arize-7.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-28 20:00:25.000000 arize-7.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-28 20:00:25.000000 arize-7.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13735 2023-12-28 20:00:43.797476 arize-7.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2023-12-28 20:00:25.000000 arize-7.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.785476 arize-7.9.0/arize/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-28 20:00:25.000000 arize-7.9.0/arize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44382 2023-12-28 20:00:25.000000 arize-7.9.0/arize/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-12-28 20:00:25.000000 arize-7.9.0/arize/bounded_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.789476 arize-7.9.0/arize/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:25.000000 arize-7.9.0/arize/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-12-28 20:00:25.000000 arize-7.9.0/arize/examples/bulk_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-12-28 20:00:25.000000 arize-7.9.0/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2023-12-28 20:00:25.000000 arize-7.9.0/arize/examples/client_shap_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2023-12-28 20:00:25.000000 arize-7.9.0/arize/examples/log_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2023-12-28 20:00:25.000000 arize-7.9.0/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2023-12-28 20:00:25.000000 arize-7.9.0/arize/examples/preproduction_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.789476 arize-7.9.0/arize/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.789476 arize-7.9.0/arize/exporter/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11599 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/core/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/core/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/publicexporter_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.789476 arize-7.9.0/arize/exporter/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/utils/schema_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2023-12-28 20:00:25.000000 arize-7.9.0/arize/exporter/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.789476 arize-7.9.0/arize/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.789476 arize-7.9.0/arize/pandas/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.789476 arize-7.9.0/arize/pandas/generative/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.789476 arize-7.9.0/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12178 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21795 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.789476 arize-7.9.0/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.793476 arize-7.9.0/arize/pandas/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28393 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104891 2023-12-28 20:00:25.000000 arize-7.9.0/arize/pandas/validation/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65363 2023-12-28 20:00:25.000000 arize-7.9.0/arize/public_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.793476 arize-7.9.0/arize/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:25.000000 arize-7.9.0/arize/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-12-28 20:00:25.000000 arize-7.9.0/arize/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2023-12-28 20:00:25.000000 arize-7.9.0/arize/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-12-28 20:00:25.000000 arize-7.9.0/arize/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2023-12-28 20:00:25.000000 arize-7.9.0/arize/utils/model_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2023-12-28 20:00:25.000000 arize-7.9.0/arize/utils/proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42686 2023-12-28 20:00:25.000000 arize-7.9.0/arize/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2023-12-28 20:00:25.000000 arize-7.9.0/arize/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.793476 arize-7.9.0/arize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13735 2023-12-28 20:00:43.000000 arize-7.9.0/arize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-12-28 20:00:43.000000 arize-7.9.0/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 20:00:43.000000 arize-7.9.0/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-28 20:00:43.000000 arize-7.9.0/arize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-28 20:00:43.000000 arize-7.9.0/arize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-28 20:00:25.000000 arize-7.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-28 20:00:43.797476 arize-7.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 20:00:43.793476 arize-7.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    88866 2023-12-28 20:00:25.000000 arize-7.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-28 20:00:25.000000 arize-7.9.0/tests/test_utils.py
```

### Comparing `arize-7.8.1/LICENSE.md` & `arize-7.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/PKG-INFO` & `arize-7.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.8.1
+Version: 7.9.0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.8.1/README.md` & `arize-7.9.0/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/api.py` & `arize-7.9.0/arize/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 from .utils.types import (
     CATEGORICAL_MODEL_TYPES,
     NUMERIC_MODEL_TYPES,
     Embedding,
     Environments,
     LLMRunMetadata,
     ModelTypes,
+    MultiClassActualLabel,
+    MultiClassPredictionLabel,
     ObjectDetectionLabel,
     RankingActualLabel,
     RankingPredictionLabel,
     _PromptOrResponseText,
     is_list_of,
 )
 from .utils.utils import (
@@ -62,23 +64,25 @@
     str,
     bool,
     int,
     float,
     Tuple[str, float],
     ObjectDetectionLabel,
     RankingPredictionLabel,
+    MultiClassPredictionLabel,
 ]
 ActualLabelTypes = Union[
     str,
     bool,
     int,
     float,
     Tuple[str, float],
     ObjectDetectionLabel,
     RankingActualLabel,
+    MultiClassActualLabel,
 ]
 
 
 class Client:
     """
     Arize API Client to log model predictions and actuals to the Arize AI platform
     """
@@ -174,21 +178,21 @@
                 and actuals for a given model_id to track and compare changes. Defaults to None.
             prediction_id (str, int, or float, optional): A unique string to identify a
                 prediction event. This value is used to match a prediction to delayed actuals in Arize. If
                 prediction id is not provided, Arize will, when possible, create a random prediction
                 id on the server side.
             prediction_timestamp (int, optional): Unix timestamp in seconds. If None, prediction
                 uses current timestamp. Defaults to None.
-            prediction_label (bool, int, float, str, Tuple(str, float), ObjectDetectionLabel or
-                RankingPredictionLabel; optional): The predicted value for a given model input. Defaults to
-                None.
-            actual_label (bool, int, float, str, Tuple[str, float], ObjectDetectionLabel or
-                RankingActualLabel; optional): The ground truth value for a given model input. This will be
-                be matched to the prediction with the same prediction_id as the one in this call. Defaults
-                to None.
+            prediction_label (bool, int, float, str, Tuple(str, float), ObjectDetectionLabel,
+                RankingPredictionLabel or MultiClassPredictionLabel; optional):
+                The predicted value for a given model input. Defaults to None.
+            actual_label (bool, int, float, str, Tuple[str, float], ObjectDetectionLabel,
+                RankingActualLabel or MultiClassActualLabel; optional):
+                The ground truth value for a given model input. This will be matched to the
+                prediction with the same prediction_id as the one in this call. Defaults to None.
             features (Dict[str, Union[str, bool, float, int]], optional): Dictionary containing
                 human readable and debuggable model features. Defaults to None.
             embedding_features (Dict[str, Embedding], optional): Dictionary containing model
                 embedding features. Keys must be strings. Values must be of type Embedding. Defaults to
                 None.
             shap_values (Dict[str, float], optional): Dictionary containing human readable and
                 debuggable model features keys, along with SHAP feature importance values. Defaults to None.
@@ -544,27 +548,31 @@
         bool,
         int,
         float,
         Tuple[Union[str, bool], float],
         ObjectDetectionLabel,
         RankingPredictionLabel,
         RankingActualLabel,
+        MultiClassPredictionLabel,
+        MultiClassActualLabel,
     ],
     embedding_features: Dict[str, Embedding],
 ):
     if model_type in NUMERIC_MODEL_TYPES:
         _validate_numeric_label(model_type, label)
     elif model_type in CATEGORICAL_MODEL_TYPES:
         _validate_categorical_label(model_type, label)
     elif model_type == ModelTypes.OBJECT_DETECTION:
         _validate_object_detection_label(prediction_or_actual, label, embedding_features)
     elif model_type == ModelTypes.RANKING:
         _validate_ranking_label(label)
     elif model_type == ModelTypes.GENERATIVE_LLM:
         _validate_generative_llm_label(label)
+    elif model_type == ModelTypes.MULTI_CLASS:
+        _validate_multi_class_label(label)
     else:
         raise InvalidValueType("model_type", model_type, "arize.utils.ModelTypes")
 
 
 def _validate_numeric_label(
     model_type: ModelTypes,
     label: Union[str, bool, int, float, Tuple[Union[str, bool], float]],
@@ -641,37 +649,53 @@
         raise InvalidValueType(
             f"label {label}",
             label,
             f"one of: bool, int, float, str for model type {ModelTypes.GENERATIVE_LLM}",
         )
 
 
+def _validate_multi_class_label(
+    label: Union[MultiClassPredictionLabel, MultiClassActualLabel],
+):
+    if not isinstance(label, (MultiClassPredictionLabel, MultiClassActualLabel)):
+        raise InvalidValueType(
+            f"label {label}",
+            label,
+            f"MultiClassPredictionLabel or MultiClassActualLabel for model type {ModelTypes.MULTI_CLASS}",
+        )
+    label.validate()
+
+
 def _get_label(
     prediction_or_actual: str,
     value: Union[
         str,
         bool,
         int,
         float,
         Tuple[str, float],
         ObjectDetectionLabel,
         RankingPredictionLabel,
         RankingActualLabel,
+        MultiClassPredictionLabel,
+        MultiClassActualLabel,
     ],
     model_type: ModelTypes,
 ) -> Union[pb2.PredictionLabel, pb2.ActualLabel]:
     value = convert_element(value)
     if model_type in NUMERIC_MODEL_TYPES:
         return _get_numeric_label(prediction_or_actual, value)
     elif model_type in CATEGORICAL_MODEL_TYPES or model_type == ModelTypes.GENERATIVE_LLM:
         return _get_score_categorical_label(prediction_or_actual, value)
     elif model_type == ModelTypes.OBJECT_DETECTION:
         return _get_object_detection_label(prediction_or_actual, value)
     elif model_type == ModelTypes.RANKING:
         return _get_ranking_label(value)
+    elif model_type == ModelTypes.MULTI_CLASS:
+        return _get_multi_class_label(value)
     raise ValueError(
         f"model_type must be one of: {[mt.prediction_or_actual for mt in ModelTypes]} "
         f"Got "
         f"{model_type} instead."
     )
 
 
@@ -797,14 +821,63 @@
         if value.relevance_labels is not None:
             ra.category.values.extend(value.relevance_labels)
         if value.relevance_score is not None:
             ra.relevance_score.value = value.relevance_score
         return pb2.ActualLabel(ranking=ra)
 
 
+def _get_multi_class_label(
+    value: Union[MultiClassPredictionLabel, MultiClassActualLabel]
+) -> Union[pb2.PredictionLabel, pb2.ActualLabel]:
+    if not isinstance(value, (MultiClassPredictionLabel, MultiClassActualLabel)):
+        raise InvalidValueType(
+            "multi class label",
+            value,
+            f"MultiClassPredictionLabel or MultiClassActualLabel for model type {ModelTypes.MULTI_CLASS}",
+        )
+    if isinstance(value, MultiClassPredictionLabel):
+        mc_pred = pb2.MultiClassPrediction()
+        # threshold score map is not None in multi-label case
+        if value.threshold_scores is not None:
+            prediction_threshold_scores = {}
+            # Validations checked prediction score map is not None
+            for class_name, p_score in value.prediction_scores.items():
+                # Validations checked threshold map contains all classes so safe to index w class_name
+                multi_label_scores = pb2.MultiClassPrediction.MultiLabel.MultiLabelScores(
+                    prediction_score=DoubleValue(value=p_score),
+                    threshold_score=DoubleValue(value=value.threshold_scores[class_name]),
+                )
+                prediction_threshold_scores[class_name] = multi_label_scores
+            multi_label = pb2.MultiClassPrediction.MultiLabel(
+                prediction_threshold_scores=prediction_threshold_scores
+            )
+            mc_pred = pb2.MultiClassPrediction(multi_label=multi_label)
+        else:
+            prediction_scores_double_values = {}
+            # Validations checked prediction score map is not None
+            for class_name, p_score in value.prediction_scores.items():
+                prediction_scores_double_values[class_name] = DoubleValue(value=p_score)
+            single_label = pb2.MultiClassPrediction.SingleLabel(
+                prediction_scores=prediction_scores_double_values,
+            )
+            mc_pred = pb2.MultiClassPrediction(single_label=single_label)
+        p_label = pb2.PredictionLabel(multi_class=mc_pred)
+        return p_label
+    elif isinstance(value, MultiClassActualLabel):
+        # Validations checked actual score map is not None
+        actual_labels = []  # list of class names with actual score of 1
+        for class_name, score in value.actual_scores.items():
+            if float(score) == 1.0:
+                actual_labels.append(class_name)
+        mc_act = pb2.MultiClassActual(
+            actual_labels=actual_labels,
+        )
+        return pb2.ActualLabel(multi_class=mc_act)
+
+
 def _validate_mapping_key(key_name: str, name: str):
     if not isinstance(key_name, str):
         raise ValueError(
             f"{name} dictionary key {key_name} must be named with string, type used: {type(key_name)}"
         )
     if key_name.endswith("_shap"):
         raise ValueError(
```

### Comparing `arize-7.8.1/arize/bounded_executor.py` & `arize-7.9.0/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/examples/bulk_client.py` & `arize-7.9.0/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/examples/bulk_client_shap.py` & `arize-7.9.0/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/examples/client_shap_values.py` & `arize-7.9.0/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/examples/log_client.py` & `arize-7.9.0/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/examples/log_pandas_dataframe.py` & `arize-7.9.0/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/examples/preproduction_client.py` & `arize-7.9.0/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/exporter/core/client.py` & `arize-7.9.0/arize/exporter/core/client.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/exporter/core/query.py` & `arize-7.9.0/arize/exporter/core/query.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/exporter/core/session.py` & `arize-7.9.0/arize/exporter/core/session.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/exporter/publicexporter_pb2.py` & `arize-7.9.0/arize/exporter/publicexporter_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/exporter/utils/constants.py` & `arize-7.9.0/arize/exporter/utils/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/exporter/utils/errors.py` & `arize-7.9.0/arize/exporter/utils/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/exporter/utils/schema_parser.py` & `arize-7.9.0/arize/exporter/utils/schema_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 # Ranking columns:
 get_pred_group_id = _get_colname("predictionGroupID")
 get_ranking_category = _get_colname("ranking:category")
 get_ranking_relevance = _get_colname("ranking:relevance")
 get_ranking_label = _get_colname("ranking:label")
 get_rank = _get_colname("ranking:rank")
 
+# TODO: Multi Class columns
+
 
 def get_tags(df_columns: Iterable) -> List[str]:
     return [c for c in df_columns if is_tag(c)]
 
 
 def get_embedding_dict(
     vector_col_name: str, df_columns: Iterable[str]
```

### Comparing `arize-7.8.1/arize/exporter/utils/validation.py` & `arize-7.9.0/arize/exporter/utils/validation.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/embeddings/auto_generator.py` & `arize-7.9.0/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/embeddings/base_generators.py` & `arize-7.9.0/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/embeddings/constants.py` & `arize-7.9.0/arize/pandas/embeddings/constants.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/embeddings/cv_generators.py` & `arize-7.9.0/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/embeddings/errors.py` & `arize-7.9.0/arize/pandas/embeddings/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/embeddings/nlp_generators.py` & `arize-7.9.0/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/embeddings/tabular_generators.py` & `arize-7.9.0/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.9.0/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/logger.py` & `arize-7.9.0/arize/pandas/logger.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.9.0/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/validation/errors.py` & `arize-7.9.0/arize/pandas/validation/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/pandas/validation/validator.py` & `arize-7.9.0/arize/pandas/validation/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
         # in the dataframe, it will be caught by _check_missing_columns
         if col is not None and col in dataframe.columns:
             if any(
                 not is_dict_of(
                     val,
                     key_allowed_types=str,
                     value_allowed_types=(bool, int, float, str),
-                    list_allowed_types=str,
+                    value_list_allowed_types=str,
                 )
                 for val in dataframe[col]
             ):
                 return [
                     err.InvalidTypeColumns(
                         wrong_type_columns=[col],
                         expected_types=["Dict[str, (bool, int, float, string or list[str])]"],
```

### Comparing `arize-7.8.1/arize/public_pb2.py` & `arize-7.9.0/arize/public_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpublic.proto\x12\x06public\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x98\x01\n\nBulkRecord\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x1f\n\x07records\x18\x05 \x03(\x0b\x32\x0e.public.Record\x12\x11\n\tspace_key\x18\x06 \x01(\tJ\x04\x08\x04\x10\x05R\ttimestamp\"\xd7\x05\n\x06Record\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rprediction_id\x18\x03 \x01(\t\x12&\n\nprediction\x18\x08 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\t \x01(\x0b\x32\x0e.public.Actual\x12\x37\n\x13\x66\x65\x61ture_importances\x18\n \x01(\x0b\x32\x1a.public.FeatureImportances\x12:\n\x15prediction_and_actual\x18\x0b \x01(\x0b\x32\x1b.public.PredictionAndActual\x12\x11\n\tspace_key\x18\x0c \x01(\t\x12<\n\x12\x65nvironment_params\x18\r \x01(\x0b\x32 .public.Record.EnvironmentParams\x12<\n\x18is_generative_llm_record\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\xa1\x02\n\x11\x45nvironmentParams\x12=\n\x08training\x18\x01 \x01(\x0b\x32).public.Record.EnvironmentParams.TrainingH\x00\x12\x41\n\nvalidation\x18\x02 \x01(\x0b\x32+.public.Record.EnvironmentParams.ValidationH\x00\x12\x41\n\nproduction\x18\x03 \x01(\x0b\x32+.public.Record.EnvironmentParams.ProductionH\x00\x1a\n\n\x08Training\x1a\x1e\n\nValidation\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x1a\x0c\n\nProductionB\r\n\x0b\x65nvironmentJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xae\x02\n\x13PreProductionRecord\x12\x45\n\x0ftraining_record\x18\x01 \x01(\x0b\x32*.public.PreProductionRecord.TrainingRecordH\x00\x12I\n\x11validation_record\x18\x02 \x01(\x0b\x32,.public.PreProductionRecord.ValidationRecordH\x00\x1a\x44\n\x10ValidationRecord\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x1e\n\x06record\x18\x02 \x01(\x0b\x32\x0e.public.Record\x1a\x30\n\x0eTrainingRecord\x12\x1e\n\x06record\x18\x01 \x01(\x0b\x32\x0e.public.RecordB\r\n\x0brecord_type\"\x86\x03\n\x10ScoreCategorical\x12\x17\n\x0b\x63\x61tegorical\x18\x01 \x01(\tB\x02\x18\x01\x12\x11\n\x05score\x18\x02 \x01(\x01\x42\x02\x18\x01\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0b\x32!.public.ScoreCategorical.CategoryH\x00\x12@\n\x0escore_category\x18\x04 \x01(\x0b\x32&.public.ScoreCategorical.ScoreCategoryH\x00\x12:\n\x0bscore_value\x18\x05 \x01(\x0b\x32#.public.ScoreCategorical.ScoreValueH\x00\x1a\x1c\n\x08\x43\x61tegory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x1a\x1b\n\nScoreValue\x12\r\n\x05value\x18\x01 \x01(\x01\x1aN\n\rScoreCategory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x1c\n\x10numeric_sequence\x18\x03 \x03(\x01\x42\x02\x18\x01\x42\x06\n\x04type\"\xb1\x01\n\x0fObjectDetection\x12;\n\x0e\x62ounding_boxes\x18\x01 \x03(\x0b\x32#.public.ObjectDetection.BoundingBox\x1a\x61\n\x0b\x42oundingBox\x12\x13\n\x0b\x63oordinates\x18\x01 \x03(\x01\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12+\n\x05score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x85\x01\n\x11RankingPrediction\x12\x1b\n\x13prediction_group_id\x18\x01 \x01(\t\x12\x0c\n\x04rank\x18\x02 \x01(\x03\x12\x36\n\x10prediction_score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\r\n\x05label\x18\x04 \x01(\t\"l\n\rRankingActual\x12$\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32\x12.public.MultiValue\x12\x35\n\x0frelevance_score\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xde\x05\n\x14MultiClassPrediction\x12>\n\x0bmulti_label\x18\x01 \x01(\x0b\x32\'.public.MultiClassPrediction.MultiLabelH\x00\x12@\n\x0csingle_label\x18\x02 \x01(\x0b\x32(.public.MultiClassPrediction.SingleLabelH\x00\x1a\xf9\x02\n\nMultiLabel\x12k\n\x1bprediction_threshold_scores\x18\x01 \x03(\x0b\x32\x46.public.MultiClassPrediction.MultiLabel.PredictionThresholdScoresEntry\x1a\x81\x01\n\x10MultiLabelScores\x12\x36\n\x10prediction_score\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0fthreshold_score\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1az\n\x1ePredictionThresholdScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12G\n\x05value\x18\x02 \x01(\x0b\x32\x38.public.MultiClassPrediction.MultiLabel.MultiLabelScores:\x02\x38\x01\x1a\xbf\x01\n\x0bSingleLabel\x12Y\n\x11prediction_scores\x18\x01 \x03(\x0b\x32>.public.MultiClassPrediction.SingleLabel.PredictionScoresEntry\x1aU\n\x15PredictionScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue:\x02\x38\x01\x42\x06\n\x04type\")\n\x10MultiClassActual\x12\x15\n\ractual_labels\x18\x01 \x03(\t\"\x82\x01\n\x05Label\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x42\x06\n\x04\x64\x61ta\"\xa4\x02\n\x0fPredictionLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12,\n\x07ranking\x18\x05 \x01(\x0b\x32\x19.public.RankingPredictionH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x12\x33\n\x0bmulti_class\x18\x07 \x01(\x0b\x32\x1c.public.MultiClassPredictionH\x00\x42\x06\n\x04\x64\x61ta\"\x98\x02\n\x0b\x41\x63tualLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12(\n\x07ranking\x18\x05 \x01(\x0b\x32\x15.public.RankingActualH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x12/\n\x0bmulti_class\x18\x07 \x01(\x0b\x32\x18.public.MultiClassActualH\x00\x42\x06\n\x04\x64\x61ta\"\xd1\x01\n\tLLMFields\x12\x16\n\x0ellm_model_name\x18\x01 \x01(\t\x12\x34\n\nllm_params\x18\x02 \x03(\x0b\x32 .public.LLMFields.LlmParamsEntry\x12\x17\n\x0fprompt_template\x18\x03 \x01(\t\x12\x1c\n\x14prompt_template_name\x18\x04 \x01(\t\x1a?\n\x0eLlmParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\xca\x03\n\nPrediction\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12 \n\x05label\x18\x03 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12\x32\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32 .public.Prediction.FeaturesEntry\x12*\n\x04tags\x18\x05 \x03(\x0b\x32\x1c.public.Prediction.TagsEntry\x12\x31\n\x10prediction_label\x18\x06 \x01(\x0b\x32\x17.public.PredictionLabel\x12%\n\nllm_fields\x18\x07 \x01(\x0b\x32\x11.public.LLMFields\x12\x1e\n\x16retrieved_document_ids\x18\x08 \x03(\t\x1a>\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\x95\x01\n\x05Value\x12\x10\n\x06string\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x10\n\x06\x64ouble\x18\x03 \x01(\x01H\x00\x12)\n\x0bmulti_value\x18\x04 \x01(\x0b\x32\x12.public.MultiValueH\x00\x12&\n\tembedding\x18\x05 \x01(\x0b\x32\x11.public.EmbeddingH\x00\x42\x06\n\x04\x64\x61ta\"\x1c\n\nMultiValue\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xed\x01\n\tEmbedding\x12\x0e\n\x06vector\x18\x01 \x03(\x01\x12\x32\n\x0clink_to_data\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x08raw_data\x18\x04 \x01(\x0b\x32\x19.public.Embedding.RawData\x1aK\n\x07RawData\x12\x32\n\ntokenArray\x18\x02 \x01(\x0b\x32\x1c.public.Embedding.TokenArrayH\x00\x42\x06\n\x04typeJ\x04\x08\x01\x10\x02\x1a\x1c\n\nTokenArray\x12\x0e\n\x06tokens\x18\x01 \x03(\tJ\x04\x08\x02\x10\x03\"\xe8\x01\n\x06\x41\x63tual\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x05label\x18\x02 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12&\n\x04tags\x18\x03 \x03(\x0b\x32\x18.public.Actual.TagsEntry\x12)\n\x0c\x61\x63tual_label\x18\x04 \x01(\x0b\x32\x13.public.ActualLabel\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\xe6\x01\n\x12\x46\x65\x61tureImportances\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12O\n\x13\x66\x65\x61ture_importances\x18\x03 \x03(\x0b\x32\x32.public.FeatureImportances.FeatureImportancesEntry\x1a\x39\n\x17\x46\x65\x61tureImportancesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"]\n\x13PredictionAndActual\x12&\n\nprediction\x18\x01 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x0e.public.Actual\"\x97\x01\n\nFileHeader\x12\x33\n\x0b\x65nvironment\x18\x01 \x01(\x0e\x32\x1e.public.FileHeader.Environment\"T\n\x0b\x45nvironment\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\x12\n\n\x06\x43ORPUS\x10\x04\"\xb0\x31\n\x06Schema\x12+\n\tconstants\x18\x01 \x01(\x0b\x32\x18.public.Schema.Constants\x12<\n\x11\x61rize_conclusions\x18\x02 \x01(\x0b\x32\x1f.public.Schema.ArizeConclusionsH\x00\x12>\n\x12\x61rize_explanations\x18\x03 \x01(\x0b\x32 .public.Schema.ArizeExplanationsH\x00\x12\x32\n\x0c\x61rrow_schema\x18\x04 \x01(\x0b\x32\x1a.public.Schema.ArrowSchemaH\x00\x12\x36\n\x0egeneric_schema\x18\x05 \x01(\x0b\x32\x1c.public.Schema.GenericSchemaH\x00\x12K\n\x19\x61rize_conclusion_pointers\x18\x06 \x01(\x0b\x32&.public.Schema.ArizeConclusionPointersH\x00\x12M\n\x1a\x61rize_explanation_pointers\x18\x07 \x01(\x0b\x32\'.public.Schema.ArizeExplanationPointersH\x00\x12\x30\n\x0b\x61rize_spans\x18\x08 \x01(\x0b\x32\x19.public.Schema.ArizeSpansH\x00\x1a\xa5\x01\n\tConstants\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61tch_id\x18\x03 \x01(\t\x12/\n\x0b\x65nvironment\x18\x04 \x01(\x0e\x32\x1a.public.Schema.Environment\x12,\n\nmodel_type\x18\x05 \x01(\x0e\x32\x18.public.Schema.ModelType\x1a\x12\n\x10\x41rizeConclusions\x1a\x13\n\x11\x41rizeExplanations\x1a\x19\n\x17\x41rizeConclusionPointers\x1a\x1a\n\x18\x41rizeExplanationPointers\x1a\x0c\n\nArizeSpans\x1a\x84\x0b\n\x0b\x41rrowSchema\x12!\n\x19prediction_id_column_name\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_column_names\x18\x02 \x03(\t\x12\x1d\n\x15timestamp_column_name\x18\x03 \x01(\t\x12$\n\x1cprediction_label_column_name\x18\x04 \x01(\t\x12$\n\x1cprediction_score_column_name\x18\x05 \x01(\t\x12 \n\x18\x61\x63tual_label_column_name\x18\x06 \x01(\t\x12 \n\x18\x61\x63tual_score_column_name\x18\x07 \x01(\t\x12W\n\x18shap_values_column_names\x18\x08 \x03(\x0b\x32\x35.public.Schema.ArrowSchema.ShapValuesColumnNamesEntry\x12\x18\n\x10tag_column_names\x18\t \x03(\t\x12/\n#actual_numeric_sequence_column_name\x18\n \x01(\tB\x02\x18\x01\x12O\n\x1e\x65mbedding_feature_column_names\x18\x0b \x03(\x0b\x32#.public.Schema.EmbeddingColumnNamesB\x02\x18\x01\x12%\n\x1dmodel_environment_column_name\x18\x0c \x01(\t\x12!\n\x19model_version_column_name\x18\r \x01(\t\x12\x1c\n\x14\x62\x61tch_id_column_name\x18\x0e \x01(\t\x12\'\n\x1fprediction_group_id_column_name\x18\x0f \x01(\t\x12\x18\n\x10rank_column_name\x18\x10 \x01(\t\x12j\n\"embedding_feature_column_names_map\x18\x11 \x03(\x0b\x32>.public.Schema.ArrowSchema.EmbeddingFeatureColumnNamesMapEntry\x12\x66\n.prediction_object_detection_label_column_names\x18\x12 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x12\x62\n*actual_object_detection_label_column_names\x18\x13 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x12N\n\x1cprompt_template_column_names\x18\x14 \x01(\x0b\x32(.public.Schema.PromptTemplateColumnNames\x12\x44\n\x17llm_config_column_names\x18\x15 \x01(\x0b\x32#.public.Schema.LLMConfigColumnNames\x12\x41\n\x15\x64ocument_column_names\x18\x16 \x01(\x0b\x32\".public.Schema.DocumentColumnNames\x12*\n\"retrieved_document_ids_column_name\x18\x17 \x01(\t\x1a<\n\x1aShapValuesColumnNamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aj\n#EmbeddingFeatureColumnNamesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.public.Schema.EmbeddingColumnNames:\x02\x38\x01\x1a\x89\x01\n\x13\x44ocumentColumnNames\x12\x16\n\x0eid_column_name\x18\x01 \x01(\t\x12=\n\x10text_column_name\x18\x02 \x01(\x0b\x32#.public.Schema.EmbeddingColumnNames\x12\x1b\n\x13version_column_name\x18\x03 \x01(\t\x1a_\n\x19PromptTemplateColumnNames\x12\x1c\n\x14template_column_name\x18\x01 \x01(\t\x12$\n\x1ctemplate_version_column_name\x18\x02 \x01(\t\x1aQ\n\x14LLMConfigColumnNames\x12\x19\n\x11model_column_name\x18\x01 \x01(\t\x12\x1e\n\x16params_map_column_name\x18\x02 \x01(\t\x1a\x93\x01\n\x1fObjectDetectionLabelColumnNames\x12&\n\x1e\x62\x62oxes_coordinates_column_name\x18\x01 \x01(\t\x12%\n\x1d\x62\x62oxes_categories_column_name\x18\x02 \x01(\t\x12!\n\x19\x62\x62oxes_scores_column_name\x18\x03 \x01(\t\x1an\n\x14\x45mbeddingColumnNames\x12\x1a\n\x12vector_column_name\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61ta_column_name\x18\x02 \x01(\t\x12 \n\x18link_to_data_column_name\x18\x03 \x01(\t\x1a\xb6\x19\n\rGenericSchema\x12\x43\n\rprediction_id\x18\x01 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\ttimestamp\x18\x03 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_label\x18\x04 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_score\x18\x05 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_label\x18\x06 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_score\x18\x07 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x0bshap_values\x18\x08 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\x04tags\x18\t \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12G\n\x11model_environment\x18\n \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rmodel_version\x18\x0b \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12>\n\x08\x62\x61tch_id\x18\x0c \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12=\n\x07\x65xclude\x18\r \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12Q\n\x17\x61\x63tual_numeric_sequence\x18\x0e \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptorB\x02\x18\x01\x12Q\n\x12\x65mbedding_features\x18\x0f \x01(\x0b\x32\x35.public.Schema.GenericSchema.EmbeddingFieldDescriptor\x12I\n\x13prediction_group_id\x18\x10 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12:\n\x04rank\x18\x11 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12k\n!prediction_object_detection_label\x18\x12 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12g\n\x1d\x61\x63tual_object_detection_label\x18\x13 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12\x46\n\x10\x63hange_timestamp\x18\x14 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rfeatures_list\x18\x15 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12?\n\ttags_list\x18\x16 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x45\n\x0fprompt_template\x18\x17 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12M\n\x17prompt_template_version\x18\x18 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x44\n\x0ellm_model_name\x18\x19 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12@\n\nllm_params\x18\x1a \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12O\n\rreserved_tags\x18\x1b \x01(\x0b\x32\x38.public.Schema.GenericSchema.ReservedNameFieldDescriptor\x1a%\n\x0f\x46ieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x1a\x41\n\x14GroupFieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x12\x15\n\rcapture_group\x18\x02 \x01(\t\x1a\xba\x03\n\x18\x45mbeddingFieldDescriptor\x12Y\n\nproperties\x18\x01 \x03(\x0b\x32\x45.public.Schema.GenericSchema.EmbeddingFieldDescriptor.PropertiesEntry\x1a\xc3\x01\n\x14\x45mbeddingPropertyMap\x12u\n\x0eproperties_map\x18\x01 \x03(\x0b\x32].public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a}\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0b\x32J.public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap:\x02\x38\x01\x1a\x89\x04\n#ObjectDetectionLabelFieldDescriptor\x12\x64\n\nproperties\x18\x01 \x03(\x0b\x32P.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.PropertiesEntry\x1a\xe5\x01\n\x1fObjectDetectionLabelPropertyMap\x12\x8b\x01\n\x0eproperties_map\x18\x01 \x03(\x0b\x32s.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x93\x01\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12o\n\x05value\x18\x02 \x01(\x0b\x32`.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap:\x02\x38\x01\x1a\xb8\x01\n\x1bReservedNameFieldDescriptor\x12\x63\n\x0eproperties_map\x18\x01 \x03(\x0b\x32K.public.Schema.GenericSchema.ReservedNameFieldDescriptor.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"m\n\x0b\x45nvironment\x12\x17\n\x13UNKNOWN_ENVIRONMENT\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\x12\n\n\x06\x43ORPUS\x10\x04\x12\x0b\n\x07TRACING\x10\x05\"\xab\x01\n\tModelType\x12\x15\n\x11UNKNOWN_MODELTYPE\x10\x00\x12\n\n\x06\x42INARY\x10\x01\x12\x0b\n\x07NUMERIC\x10\x02\x12\x0f\n\x0b\x43\x41TEGORICAL\x10\x03\x12\x15\n\x11SCORE_CATEGORICAL\x10\x04\x12\x0b\n\x07RANKING\x10\x05\x12\x14\n\x10OBJECT_DETECTION\x10\x06\x12\x12\n\x0eGENERATIVE_LLM\x10\x07\x12\x0f\n\x0bMULTI_CLASS\x10\x08\x42\x08\n\x06schema\"I\n\x17\x41rrowFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x1f\n\x17real_time_ingestion_uri\x18\x02 \x01(\t\":\n\x16UserFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x11\n\tfile_uuid\x18\x02 \x01(\tBO\n\x12\x63om.arize.protocolZ9github.com/Arize-ai/arize/go/pkg/receiver/protocol/publicb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpublic.proto\x12\x06public\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x98\x01\n\nBulkRecord\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x1f\n\x07records\x18\x05 \x03(\x0b\x32\x0e.public.Record\x12\x11\n\tspace_key\x18\x06 \x01(\tJ\x04\x08\x04\x10\x05R\ttimestamp\"\xd7\x05\n\x06Record\x12\x1c\n\x10organization_key\x18\x01 \x01(\tB\x02\x18\x01\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\rprediction_id\x18\x03 \x01(\t\x12&\n\nprediction\x18\x08 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\t \x01(\x0b\x32\x0e.public.Actual\x12\x37\n\x13\x66\x65\x61ture_importances\x18\n \x01(\x0b\x32\x1a.public.FeatureImportances\x12:\n\x15prediction_and_actual\x18\x0b \x01(\x0b\x32\x1b.public.PredictionAndActual\x12\x11\n\tspace_key\x18\x0c \x01(\t\x12<\n\x12\x65nvironment_params\x18\r \x01(\x0b\x32 .public.Record.EnvironmentParams\x12<\n\x18is_generative_llm_record\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\xa1\x02\n\x11\x45nvironmentParams\x12=\n\x08training\x18\x01 \x01(\x0b\x32).public.Record.EnvironmentParams.TrainingH\x00\x12\x41\n\nvalidation\x18\x02 \x01(\x0b\x32+.public.Record.EnvironmentParams.ValidationH\x00\x12\x41\n\nproduction\x18\x03 \x01(\x0b\x32+.public.Record.EnvironmentParams.ProductionH\x00\x1a\n\n\x08Training\x1a\x1e\n\nValidation\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x1a\x0c\n\nProductionB\r\n\x0b\x65nvironmentJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xae\x02\n\x13PreProductionRecord\x12\x45\n\x0ftraining_record\x18\x01 \x01(\x0b\x32*.public.PreProductionRecord.TrainingRecordH\x00\x12I\n\x11validation_record\x18\x02 \x01(\x0b\x32,.public.PreProductionRecord.ValidationRecordH\x00\x1a\x44\n\x10ValidationRecord\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x1e\n\x06record\x18\x02 \x01(\x0b\x32\x0e.public.Record\x1a\x30\n\x0eTrainingRecord\x12\x1e\n\x06record\x18\x01 \x01(\x0b\x32\x0e.public.RecordB\r\n\x0brecord_type\"\x86\x03\n\x10ScoreCategorical\x12\x17\n\x0b\x63\x61tegorical\x18\x01 \x01(\tB\x02\x18\x01\x12\x11\n\x05score\x18\x02 \x01(\x01\x42\x02\x18\x01\x12\x35\n\x08\x63\x61tegory\x18\x03 \x01(\x0b\x32!.public.ScoreCategorical.CategoryH\x00\x12@\n\x0escore_category\x18\x04 \x01(\x0b\x32&.public.ScoreCategorical.ScoreCategoryH\x00\x12:\n\x0bscore_value\x18\x05 \x01(\x0b\x32#.public.ScoreCategorical.ScoreValueH\x00\x1a\x1c\n\x08\x43\x61tegory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x1a\x1b\n\nScoreValue\x12\r\n\x05value\x18\x01 \x01(\x01\x1aN\n\rScoreCategory\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x1c\n\x10numeric_sequence\x18\x03 \x03(\x01\x42\x02\x18\x01\x42\x06\n\x04type\"\xb1\x01\n\x0fObjectDetection\x12;\n\x0e\x62ounding_boxes\x18\x01 \x03(\x0b\x32#.public.ObjectDetection.BoundingBox\x1a\x61\n\x0b\x42oundingBox\x12\x13\n\x0b\x63oordinates\x18\x01 \x03(\x01\x12\x10\n\x08\x63\x61tegory\x18\x02 \x01(\t\x12+\n\x05score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x85\x01\n\x11RankingPrediction\x12\x1b\n\x13prediction_group_id\x18\x01 \x01(\t\x12\x0c\n\x04rank\x18\x02 \x01(\x03\x12\x36\n\x10prediction_score\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\r\n\x05label\x18\x04 \x01(\t\"l\n\rRankingActual\x12$\n\x08\x63\x61tegory\x18\x01 \x01(\x0b\x32\x12.public.MultiValue\x12\x35\n\x0frelevance_score\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xde\x05\n\x14MultiClassPrediction\x12>\n\x0bmulti_label\x18\x01 \x01(\x0b\x32\'.public.MultiClassPrediction.MultiLabelH\x00\x12@\n\x0csingle_label\x18\x02 \x01(\x0b\x32(.public.MultiClassPrediction.SingleLabelH\x00\x1a\xf9\x02\n\nMultiLabel\x12k\n\x1bprediction_threshold_scores\x18\x01 \x03(\x0b\x32\x46.public.MultiClassPrediction.MultiLabel.PredictionThresholdScoresEntry\x1a\x81\x01\n\x10MultiLabelScores\x12\x36\n\x10prediction_score\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0fthreshold_score\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1az\n\x1ePredictionThresholdScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12G\n\x05value\x18\x02 \x01(\x0b\x32\x38.public.MultiClassPrediction.MultiLabel.MultiLabelScores:\x02\x38\x01\x1a\xbf\x01\n\x0bSingleLabel\x12Y\n\x11prediction_scores\x18\x01 \x03(\x0b\x32>.public.MultiClassPrediction.SingleLabel.PredictionScoresEntry\x1aU\n\x15PredictionScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue:\x02\x38\x01\x42\x06\n\x04type\")\n\x10MultiClassActual\x12\x15\n\ractual_labels\x18\x01 \x03(\t\"\x82\x01\n\x05Label\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x42\x06\n\x04\x64\x61ta\"\xa4\x02\n\x0fPredictionLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12,\n\x07ranking\x18\x05 \x01(\x0b\x32\x19.public.RankingPredictionH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x12\x33\n\x0bmulti_class\x18\x07 \x01(\x0b\x32\x1c.public.MultiClassPredictionH\x00\x42\x06\n\x04\x64\x61ta\"\x98\x02\n\x0b\x41\x63tualLabel\x12\x10\n\x06\x62inary\x18\x01 \x01(\x08H\x00\x12\x15\n\x0b\x63\x61tegorical\x18\x02 \x01(\tH\x00\x12\x11\n\x07numeric\x18\x03 \x01(\x01H\x00\x12\x35\n\x11score_categorical\x18\x04 \x01(\x0b\x32\x18.public.ScoreCategoricalH\x00\x12(\n\x07ranking\x18\x05 \x01(\x0b\x32\x15.public.RankingActualH\x00\x12\x33\n\x10object_detection\x18\x06 \x01(\x0b\x32\x17.public.ObjectDetectionH\x00\x12/\n\x0bmulti_class\x18\x07 \x01(\x0b\x32\x18.public.MultiClassActualH\x00\x42\x06\n\x04\x64\x61ta\"\xd1\x01\n\tLLMFields\x12\x16\n\x0ellm_model_name\x18\x01 \x01(\t\x12\x34\n\nllm_params\x18\x02 \x03(\x0b\x32 .public.LLMFields.LlmParamsEntry\x12\x17\n\x0fprompt_template\x18\x03 \x01(\t\x12\x1c\n\x14prompt_template_name\x18\x04 \x01(\t\x1a?\n\x0eLlmParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\xca\x03\n\nPrediction\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12 \n\x05label\x18\x03 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12\x32\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32 .public.Prediction.FeaturesEntry\x12*\n\x04tags\x18\x05 \x03(\x0b\x32\x1c.public.Prediction.TagsEntry\x12\x31\n\x10prediction_label\x18\x06 \x01(\x0b\x32\x17.public.PredictionLabel\x12%\n\nllm_fields\x18\x07 \x01(\x0b\x32\x11.public.LLMFields\x12\x1e\n\x16retrieved_document_ids\x18\x08 \x03(\t\x1a>\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\xc6\x01\n\x05Value\x12\x10\n\x06string\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x10\n\x06\x64ouble\x18\x03 \x01(\x01H\x00\x12)\n\x0bmulti_value\x18\x04 \x01(\x0b\x32\x12.public.MultiValueH\x00\x12&\n\tembedding\x18\x05 \x01(\x0b\x32\x11.public.EmbeddingH\x00\x12/\n\ndictionary\x18\x06 \x01(\x0b\x32\x19.public.NumericDictionaryH\x00\x42\x06\n\x04\x64\x61ta\"\x97\x01\n\x11NumericDictionary\x12\x35\n\x06values\x18\x01 \x03(\x0b\x32%.public.NumericDictionary.ValuesEntry\x1aK\n\x0bValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue:\x02\x38\x01\"\x1c\n\nMultiValue\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xed\x01\n\tEmbedding\x12\x0e\n\x06vector\x18\x01 \x03(\x01\x12\x32\n\x0clink_to_data\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x08raw_data\x18\x04 \x01(\x0b\x32\x19.public.Embedding.RawData\x1aK\n\x07RawData\x12\x32\n\ntokenArray\x18\x02 \x01(\x0b\x32\x1c.public.Embedding.TokenArrayH\x00\x42\x06\n\x04typeJ\x04\x08\x01\x10\x02\x1a\x1c\n\nTokenArray\x12\x0e\n\x06tokens\x18\x01 \x03(\tJ\x04\x08\x02\x10\x03\"\xe8\x01\n\x06\x41\x63tual\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12 \n\x05label\x18\x02 \x01(\x0b\x32\r.public.LabelB\x02\x18\x01\x12&\n\x04tags\x18\x03 \x03(\x0b\x32\x18.public.Actual.TagsEntry\x12)\n\x0c\x61\x63tual_label\x18\x04 \x01(\x0b\x32\x13.public.ActualLabel\x1a:\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.public.Value:\x02\x38\x01\"\xe6\x01\n\x12\x46\x65\x61tureImportances\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12O\n\x13\x66\x65\x61ture_importances\x18\x03 \x03(\x0b\x32\x32.public.FeatureImportances.FeatureImportancesEntry\x1a\x39\n\x17\x46\x65\x61tureImportancesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01:\x02\x38\x01\"]\n\x13PredictionAndActual\x12&\n\nprediction\x18\x01 \x01(\x0b\x32\x12.public.Prediction\x12\x1e\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x0e.public.Actual\"\x97\x01\n\nFileHeader\x12\x33\n\x0b\x65nvironment\x18\x01 \x01(\x0e\x32\x1e.public.FileHeader.Environment\"T\n\x0b\x45nvironment\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\x12\n\n\x06\x43ORPUS\x10\x04\"\xb0\x31\n\x06Schema\x12+\n\tconstants\x18\x01 \x01(\x0b\x32\x18.public.Schema.Constants\x12<\n\x11\x61rize_conclusions\x18\x02 \x01(\x0b\x32\x1f.public.Schema.ArizeConclusionsH\x00\x12>\n\x12\x61rize_explanations\x18\x03 \x01(\x0b\x32 .public.Schema.ArizeExplanationsH\x00\x12\x32\n\x0c\x61rrow_schema\x18\x04 \x01(\x0b\x32\x1a.public.Schema.ArrowSchemaH\x00\x12\x36\n\x0egeneric_schema\x18\x05 \x01(\x0b\x32\x1c.public.Schema.GenericSchemaH\x00\x12K\n\x19\x61rize_conclusion_pointers\x18\x06 \x01(\x0b\x32&.public.Schema.ArizeConclusionPointersH\x00\x12M\n\x1a\x61rize_explanation_pointers\x18\x07 \x01(\x0b\x32\'.public.Schema.ArizeExplanationPointersH\x00\x12\x30\n\x0b\x61rize_spans\x18\x08 \x01(\x0b\x32\x19.public.Schema.ArizeSpansH\x00\x1a\xa5\x01\n\tConstants\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61tch_id\x18\x03 \x01(\t\x12/\n\x0b\x65nvironment\x18\x04 \x01(\x0e\x32\x1a.public.Schema.Environment\x12,\n\nmodel_type\x18\x05 \x01(\x0e\x32\x18.public.Schema.ModelType\x1a\x12\n\x10\x41rizeConclusions\x1a\x13\n\x11\x41rizeExplanations\x1a\x19\n\x17\x41rizeConclusionPointers\x1a\x1a\n\x18\x41rizeExplanationPointers\x1a\x0c\n\nArizeSpans\x1a\x84\x0b\n\x0b\x41rrowSchema\x12!\n\x19prediction_id_column_name\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_column_names\x18\x02 \x03(\t\x12\x1d\n\x15timestamp_column_name\x18\x03 \x01(\t\x12$\n\x1cprediction_label_column_name\x18\x04 \x01(\t\x12$\n\x1cprediction_score_column_name\x18\x05 \x01(\t\x12 \n\x18\x61\x63tual_label_column_name\x18\x06 \x01(\t\x12 \n\x18\x61\x63tual_score_column_name\x18\x07 \x01(\t\x12W\n\x18shap_values_column_names\x18\x08 \x03(\x0b\x32\x35.public.Schema.ArrowSchema.ShapValuesColumnNamesEntry\x12\x18\n\x10tag_column_names\x18\t \x03(\t\x12/\n#actual_numeric_sequence_column_name\x18\n \x01(\tB\x02\x18\x01\x12O\n\x1e\x65mbedding_feature_column_names\x18\x0b \x03(\x0b\x32#.public.Schema.EmbeddingColumnNamesB\x02\x18\x01\x12%\n\x1dmodel_environment_column_name\x18\x0c \x01(\t\x12!\n\x19model_version_column_name\x18\r \x01(\t\x12\x1c\n\x14\x62\x61tch_id_column_name\x18\x0e \x01(\t\x12\'\n\x1fprediction_group_id_column_name\x18\x0f \x01(\t\x12\x18\n\x10rank_column_name\x18\x10 \x01(\t\x12j\n\"embedding_feature_column_names_map\x18\x11 \x03(\x0b\x32>.public.Schema.ArrowSchema.EmbeddingFeatureColumnNamesMapEntry\x12\x66\n.prediction_object_detection_label_column_names\x18\x12 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x12\x62\n*actual_object_detection_label_column_names\x18\x13 \x01(\x0b\x32..public.Schema.ObjectDetectionLabelColumnNames\x12N\n\x1cprompt_template_column_names\x18\x14 \x01(\x0b\x32(.public.Schema.PromptTemplateColumnNames\x12\x44\n\x17llm_config_column_names\x18\x15 \x01(\x0b\x32#.public.Schema.LLMConfigColumnNames\x12\x41\n\x15\x64ocument_column_names\x18\x16 \x01(\x0b\x32\".public.Schema.DocumentColumnNames\x12*\n\"retrieved_document_ids_column_name\x18\x17 \x01(\t\x1a<\n\x1aShapValuesColumnNamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aj\n#EmbeddingFeatureColumnNamesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.public.Schema.EmbeddingColumnNames:\x02\x38\x01\x1a\x89\x01\n\x13\x44ocumentColumnNames\x12\x16\n\x0eid_column_name\x18\x01 \x01(\t\x12=\n\x10text_column_name\x18\x02 \x01(\x0b\x32#.public.Schema.EmbeddingColumnNames\x12\x1b\n\x13version_column_name\x18\x03 \x01(\t\x1a_\n\x19PromptTemplateColumnNames\x12\x1c\n\x14template_column_name\x18\x01 \x01(\t\x12$\n\x1ctemplate_version_column_name\x18\x02 \x01(\t\x1aQ\n\x14LLMConfigColumnNames\x12\x19\n\x11model_column_name\x18\x01 \x01(\t\x12\x1e\n\x16params_map_column_name\x18\x02 \x01(\t\x1a\x93\x01\n\x1fObjectDetectionLabelColumnNames\x12&\n\x1e\x62\x62oxes_coordinates_column_name\x18\x01 \x01(\t\x12%\n\x1d\x62\x62oxes_categories_column_name\x18\x02 \x01(\t\x12!\n\x19\x62\x62oxes_scores_column_name\x18\x03 \x01(\t\x1an\n\x14\x45mbeddingColumnNames\x12\x1a\n\x12vector_column_name\x18\x01 \x01(\t\x12\x18\n\x10\x64\x61ta_column_name\x18\x02 \x01(\t\x12 \n\x18link_to_data_column_name\x18\x03 \x01(\t\x1a\xb6\x19\n\rGenericSchema\x12\x43\n\rprediction_id\x18\x01 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\x08\x66\x65\x61tures\x18\x02 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\ttimestamp\x18\x03 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_label\x18\x04 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x10prediction_score\x18\x05 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_label\x18\x06 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x42\n\x0c\x61\x63tual_score\x18\x07 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x46\n\x0bshap_values\x18\x08 \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12?\n\x04tags\x18\t \x01(\x0b\x32\x31.public.Schema.GenericSchema.GroupFieldDescriptor\x12G\n\x11model_environment\x18\n \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rmodel_version\x18\x0b \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12>\n\x08\x62\x61tch_id\x18\x0c \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12=\n\x07\x65xclude\x18\r \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12Q\n\x17\x61\x63tual_numeric_sequence\x18\x0e \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptorB\x02\x18\x01\x12Q\n\x12\x65mbedding_features\x18\x0f \x01(\x0b\x32\x35.public.Schema.GenericSchema.EmbeddingFieldDescriptor\x12I\n\x13prediction_group_id\x18\x10 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12:\n\x04rank\x18\x11 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12k\n!prediction_object_detection_label\x18\x12 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12g\n\x1d\x61\x63tual_object_detection_label\x18\x13 \x01(\x0b\x32@.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor\x12\x46\n\x10\x63hange_timestamp\x18\x14 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x43\n\rfeatures_list\x18\x15 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12?\n\ttags_list\x18\x16 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x45\n\x0fprompt_template\x18\x17 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12M\n\x17prompt_template_version\x18\x18 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12\x44\n\x0ellm_model_name\x18\x19 \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12@\n\nllm_params\x18\x1a \x01(\x0b\x32,.public.Schema.GenericSchema.FieldDescriptor\x12O\n\rreserved_tags\x18\x1b \x01(\x0b\x32\x38.public.Schema.GenericSchema.ReservedNameFieldDescriptor\x1a%\n\x0f\x46ieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x1a\x41\n\x14GroupFieldDescriptor\x12\x12\n\nproperties\x18\x01 \x03(\t\x12\x15\n\rcapture_group\x18\x02 \x01(\t\x1a\xba\x03\n\x18\x45mbeddingFieldDescriptor\x12Y\n\nproperties\x18\x01 \x03(\x0b\x32\x45.public.Schema.GenericSchema.EmbeddingFieldDescriptor.PropertiesEntry\x1a\xc3\x01\n\x14\x45mbeddingPropertyMap\x12u\n\x0eproperties_map\x18\x01 \x03(\x0b\x32].public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a}\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0b\x32J.public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap:\x02\x38\x01\x1a\x89\x04\n#ObjectDetectionLabelFieldDescriptor\x12\x64\n\nproperties\x18\x01 \x03(\x0b\x32P.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.PropertiesEntry\x1a\xe5\x01\n\x1fObjectDetectionLabelPropertyMap\x12\x8b\x01\n\x0eproperties_map\x18\x01 \x03(\x0b\x32s.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x93\x01\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12o\n\x05value\x18\x02 \x01(\x0b\x32`.public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap:\x02\x38\x01\x1a\xb8\x01\n\x1bReservedNameFieldDescriptor\x12\x63\n\x0eproperties_map\x18\x01 \x03(\x0b\x32K.public.Schema.GenericSchema.ReservedNameFieldDescriptor.PropertiesMapEntry\x1a\x34\n\x12PropertiesMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"m\n\x0b\x45nvironment\x12\x17\n\x13UNKNOWN_ENVIRONMENT\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x0e\n\nPRODUCTION\x10\x03\x12\n\n\x06\x43ORPUS\x10\x04\x12\x0b\n\x07TRACING\x10\x05\"\xab\x01\n\tModelType\x12\x15\n\x11UNKNOWN_MODELTYPE\x10\x00\x12\n\n\x06\x42INARY\x10\x01\x12\x0b\n\x07NUMERIC\x10\x02\x12\x0f\n\x0b\x43\x41TEGORICAL\x10\x03\x12\x15\n\x11SCORE_CATEGORICAL\x10\x04\x12\x0b\n\x07RANKING\x10\x05\x12\x14\n\x10OBJECT_DETECTION\x10\x06\x12\x12\n\x0eGENERATIVE_LLM\x10\x07\x12\x0f\n\x0bMULTI_CLASS\x10\x08\x42\x08\n\x06schema\"I\n\x17\x41rrowFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x1f\n\x17real_time_ingestion_uri\x18\x02 \x01(\t\":\n\x16UserFileUploadResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x11\n\tfile_uuid\x18\x02 \x01(\tBO\n\x12\x63om.arize.protocolZ9github.com/Arize-ai/arize/go/pkg/receiver/protocol/publicb\x06proto3')
 
 
 
 _BULKRECORD = DESCRIPTOR.message_types_by_name['BulkRecord']
 _RECORD = DESCRIPTOR.message_types_by_name['Record']
 _RECORD_ENVIRONMENTPARAMS = _RECORD.nested_types_by_name['EnvironmentParams']
 _RECORD_ENVIRONMENTPARAMS_TRAINING = _RECORD_ENVIRONMENTPARAMS.nested_types_by_name['Training']
@@ -49,14 +49,16 @@
 _ACTUALLABEL = DESCRIPTOR.message_types_by_name['ActualLabel']
 _LLMFIELDS = DESCRIPTOR.message_types_by_name['LLMFields']
 _LLMFIELDS_LLMPARAMSENTRY = _LLMFIELDS.nested_types_by_name['LlmParamsEntry']
 _PREDICTION = DESCRIPTOR.message_types_by_name['Prediction']
 _PREDICTION_FEATURESENTRY = _PREDICTION.nested_types_by_name['FeaturesEntry']
 _PREDICTION_TAGSENTRY = _PREDICTION.nested_types_by_name['TagsEntry']
 _VALUE = DESCRIPTOR.message_types_by_name['Value']
+_NUMERICDICTIONARY = DESCRIPTOR.message_types_by_name['NumericDictionary']
+_NUMERICDICTIONARY_VALUESENTRY = _NUMERICDICTIONARY.nested_types_by_name['ValuesEntry']
 _MULTIVALUE = DESCRIPTOR.message_types_by_name['MultiValue']
 _EMBEDDING = DESCRIPTOR.message_types_by_name['Embedding']
 _EMBEDDING_RAWDATA = _EMBEDDING.nested_types_by_name['RawData']
 _EMBEDDING_TOKENARRAY = _EMBEDDING.nested_types_by_name['TokenArray']
 _ACTUAL = DESCRIPTOR.message_types_by_name['Actual']
 _ACTUAL_TAGSENTRY = _ACTUAL.nested_types_by_name['TagsEntry']
 _FEATUREIMPORTANCES = DESCRIPTOR.message_types_by_name['FeatureImportances']
@@ -341,14 +343,29 @@
 Value = _reflection.GeneratedProtocolMessageType('Value', (_message.Message,), {
   'DESCRIPTOR' : _VALUE,
   '__module__' : 'public_pb2'
   # @@protoc_insertion_point(class_scope:public.Value)
   })
 _sym_db.RegisterMessage(Value)
 
+NumericDictionary = _reflection.GeneratedProtocolMessageType('NumericDictionary', (_message.Message,), {
+
+  'ValuesEntry' : _reflection.GeneratedProtocolMessageType('ValuesEntry', (_message.Message,), {
+    'DESCRIPTOR' : _NUMERICDICTIONARY_VALUESENTRY,
+    '__module__' : 'public_pb2'
+    # @@protoc_insertion_point(class_scope:public.NumericDictionary.ValuesEntry)
+    })
+  ,
+  'DESCRIPTOR' : _NUMERICDICTIONARY,
+  '__module__' : 'public_pb2'
+  # @@protoc_insertion_point(class_scope:public.NumericDictionary)
+  })
+_sym_db.RegisterMessage(NumericDictionary)
+_sym_db.RegisterMessage(NumericDictionary.ValuesEntry)
+
 MultiValue = _reflection.GeneratedProtocolMessageType('MultiValue', (_message.Message,), {
   'DESCRIPTOR' : _MULTIVALUE,
   '__module__' : 'public_pb2'
   # @@protoc_insertion_point(class_scope:public.MultiValue)
   })
 _sym_db.RegisterMessage(MultiValue)
 
@@ -678,14 +695,16 @@
   _LLMFIELDS_LLMPARAMSENTRY._serialized_options = b'8\001'
   _PREDICTION_FEATURESENTRY._options = None
   _PREDICTION_FEATURESENTRY._serialized_options = b'8\001'
   _PREDICTION_TAGSENTRY._options = None
   _PREDICTION_TAGSENTRY._serialized_options = b'8\001'
   _PREDICTION.fields_by_name['label']._options = None
   _PREDICTION.fields_by_name['label']._serialized_options = b'\030\001'
+  _NUMERICDICTIONARY_VALUESENTRY._options = None
+  _NUMERICDICTIONARY_VALUESENTRY._serialized_options = b'8\001'
   _ACTUAL_TAGSENTRY._options = None
   _ACTUAL_TAGSENTRY._serialized_options = b'8\001'
   _ACTUAL.fields_by_name['label']._options = None
   _ACTUAL.fields_by_name['label']._serialized_options = b'\030\001'
   _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._options = None
   _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._serialized_options = b'8\001'
   _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY._options = None
@@ -769,95 +788,99 @@
   _PREDICTION._serialized_start=3802
   _PREDICTION._serialized_end=4260
   _PREDICTION_FEATURESENTRY._serialized_start=4138
   _PREDICTION_FEATURESENTRY._serialized_end=4200
   _PREDICTION_TAGSENTRY._serialized_start=4202
   _PREDICTION_TAGSENTRY._serialized_end=4260
   _VALUE._serialized_start=4263
-  _VALUE._serialized_end=4412
-  _MULTIVALUE._serialized_start=4414
-  _MULTIVALUE._serialized_end=4442
-  _EMBEDDING._serialized_start=4445
-  _EMBEDDING._serialized_end=4682
-  _EMBEDDING_RAWDATA._serialized_start=4571
-  _EMBEDDING_RAWDATA._serialized_end=4646
-  _EMBEDDING_TOKENARRAY._serialized_start=4648
-  _EMBEDDING_TOKENARRAY._serialized_end=4676
-  _ACTUAL._serialized_start=4685
-  _ACTUAL._serialized_end=4917
+  _VALUE._serialized_end=4461
+  _NUMERICDICTIONARY._serialized_start=4464
+  _NUMERICDICTIONARY._serialized_end=4615
+  _NUMERICDICTIONARY_VALUESENTRY._serialized_start=4540
+  _NUMERICDICTIONARY_VALUESENTRY._serialized_end=4615
+  _MULTIVALUE._serialized_start=4617
+  _MULTIVALUE._serialized_end=4645
+  _EMBEDDING._serialized_start=4648
+  _EMBEDDING._serialized_end=4885
+  _EMBEDDING_RAWDATA._serialized_start=4774
+  _EMBEDDING_RAWDATA._serialized_end=4849
+  _EMBEDDING_TOKENARRAY._serialized_start=4851
+  _EMBEDDING_TOKENARRAY._serialized_end=4879
+  _ACTUAL._serialized_start=4888
+  _ACTUAL._serialized_end=5120
   _ACTUAL_TAGSENTRY._serialized_start=4202
   _ACTUAL_TAGSENTRY._serialized_end=4260
-  _FEATUREIMPORTANCES._serialized_start=4920
-  _FEATUREIMPORTANCES._serialized_end=5150
-  _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._serialized_start=5093
-  _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._serialized_end=5150
-  _PREDICTIONANDACTUAL._serialized_start=5152
-  _PREDICTIONANDACTUAL._serialized_end=5245
-  _FILEHEADER._serialized_start=5248
-  _FILEHEADER._serialized_end=5399
-  _FILEHEADER_ENVIRONMENT._serialized_start=5315
-  _FILEHEADER_ENVIRONMENT._serialized_end=5399
-  _SCHEMA._serialized_start=5402
-  _SCHEMA._serialized_end=11722
-  _SCHEMA_CONSTANTS._serialized_start=5898
-  _SCHEMA_CONSTANTS._serialized_end=6063
-  _SCHEMA_ARIZECONCLUSIONS._serialized_start=6065
-  _SCHEMA_ARIZECONCLUSIONS._serialized_end=6083
-  _SCHEMA_ARIZEEXPLANATIONS._serialized_start=6085
-  _SCHEMA_ARIZEEXPLANATIONS._serialized_end=6104
-  _SCHEMA_ARIZECONCLUSIONPOINTERS._serialized_start=6106
-  _SCHEMA_ARIZECONCLUSIONPOINTERS._serialized_end=6131
-  _SCHEMA_ARIZEEXPLANATIONPOINTERS._serialized_start=6133
-  _SCHEMA_ARIZEEXPLANATIONPOINTERS._serialized_end=6159
-  _SCHEMA_ARIZESPANS._serialized_start=6161
-  _SCHEMA_ARIZESPANS._serialized_end=6173
-  _SCHEMA_ARROWSCHEMA._serialized_start=6176
-  _SCHEMA_ARROWSCHEMA._serialized_end=7588
-  _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY._serialized_start=7420
-  _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY._serialized_end=7480
-  _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY._serialized_start=7482
-  _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY._serialized_end=7588
-  _SCHEMA_DOCUMENTCOLUMNNAMES._serialized_start=7591
-  _SCHEMA_DOCUMENTCOLUMNNAMES._serialized_end=7728
-  _SCHEMA_PROMPTTEMPLATECOLUMNNAMES._serialized_start=7730
-  _SCHEMA_PROMPTTEMPLATECOLUMNNAMES._serialized_end=7825
-  _SCHEMA_LLMCONFIGCOLUMNNAMES._serialized_start=7827
-  _SCHEMA_LLMCONFIGCOLUMNNAMES._serialized_end=7908
-  _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES._serialized_start=7911
-  _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES._serialized_end=8058
-  _SCHEMA_EMBEDDINGCOLUMNNAMES._serialized_start=8060
-  _SCHEMA_EMBEDDINGCOLUMNNAMES._serialized_end=8170
-  _SCHEMA_GENERICSCHEMA._serialized_start=8173
-  _SCHEMA_GENERICSCHEMA._serialized_end=11427
-  _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR._serialized_start=10167
-  _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR._serialized_end=10204
-  _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR._serialized_start=10206
-  _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR._serialized_end=10271
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR._serialized_start=10274
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR._serialized_end=10716
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP._serialized_start=10394
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP._serialized_end=10589
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY._serialized_start=10537
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY._serialized_end=10589
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_start=10591
-  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_end=10716
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR._serialized_start=10719
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR._serialized_end=11240
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP._serialized_start=10861
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP._serialized_end=11090
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY._serialized_start=10537
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY._serialized_end=10589
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_start=11093
-  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_end=11240
-  _SCHEMA_GENERICSCHEMA_RESERVEDNAMEFIELDDESCRIPTOR._serialized_start=11243
-  _SCHEMA_GENERICSCHEMA_RESERVEDNAMEFIELDDESCRIPTOR._serialized_end=11427
-  _SCHEMA_GENERICSCHEMA_RESERVEDNAMEFIELDDESCRIPTOR_PROPERTIESMAPENTRY._serialized_start=10537
-  _SCHEMA_GENERICSCHEMA_RESERVEDNAMEFIELDDESCRIPTOR_PROPERTIESMAPENTRY._serialized_end=10589
-  _SCHEMA_ENVIRONMENT._serialized_start=11429
-  _SCHEMA_ENVIRONMENT._serialized_end=11538
-  _SCHEMA_MODELTYPE._serialized_start=11541
-  _SCHEMA_MODELTYPE._serialized_end=11712
-  _ARROWFILEUPLOADRESPONSE._serialized_start=11724
-  _ARROWFILEUPLOADRESPONSE._serialized_end=11797
-  _USERFILEUPLOADRESPONSE._serialized_start=11799
-  _USERFILEUPLOADRESPONSE._serialized_end=11857
+  _FEATUREIMPORTANCES._serialized_start=5123
+  _FEATUREIMPORTANCES._serialized_end=5353
+  _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._serialized_start=5296
+  _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY._serialized_end=5353
+  _PREDICTIONANDACTUAL._serialized_start=5355
+  _PREDICTIONANDACTUAL._serialized_end=5448
+  _FILEHEADER._serialized_start=5451
+  _FILEHEADER._serialized_end=5602
+  _FILEHEADER_ENVIRONMENT._serialized_start=5518
+  _FILEHEADER_ENVIRONMENT._serialized_end=5602
+  _SCHEMA._serialized_start=5605
+  _SCHEMA._serialized_end=11925
+  _SCHEMA_CONSTANTS._serialized_start=6101
+  _SCHEMA_CONSTANTS._serialized_end=6266
+  _SCHEMA_ARIZECONCLUSIONS._serialized_start=6268
+  _SCHEMA_ARIZECONCLUSIONS._serialized_end=6286
+  _SCHEMA_ARIZEEXPLANATIONS._serialized_start=6288
+  _SCHEMA_ARIZEEXPLANATIONS._serialized_end=6307
+  _SCHEMA_ARIZECONCLUSIONPOINTERS._serialized_start=6309
+  _SCHEMA_ARIZECONCLUSIONPOINTERS._serialized_end=6334
+  _SCHEMA_ARIZEEXPLANATIONPOINTERS._serialized_start=6336
+  _SCHEMA_ARIZEEXPLANATIONPOINTERS._serialized_end=6362
+  _SCHEMA_ARIZESPANS._serialized_start=6364
+  _SCHEMA_ARIZESPANS._serialized_end=6376
+  _SCHEMA_ARROWSCHEMA._serialized_start=6379
+  _SCHEMA_ARROWSCHEMA._serialized_end=7791
+  _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY._serialized_start=7623
+  _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY._serialized_end=7683
+  _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY._serialized_start=7685
+  _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY._serialized_end=7791
+  _SCHEMA_DOCUMENTCOLUMNNAMES._serialized_start=7794
+  _SCHEMA_DOCUMENTCOLUMNNAMES._serialized_end=7931
+  _SCHEMA_PROMPTTEMPLATECOLUMNNAMES._serialized_start=7933
+  _SCHEMA_PROMPTTEMPLATECOLUMNNAMES._serialized_end=8028
+  _SCHEMA_LLMCONFIGCOLUMNNAMES._serialized_start=8030
+  _SCHEMA_LLMCONFIGCOLUMNNAMES._serialized_end=8111
+  _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES._serialized_start=8114
+  _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES._serialized_end=8261
+  _SCHEMA_EMBEDDINGCOLUMNNAMES._serialized_start=8263
+  _SCHEMA_EMBEDDINGCOLUMNNAMES._serialized_end=8373
+  _SCHEMA_GENERICSCHEMA._serialized_start=8376
+  _SCHEMA_GENERICSCHEMA._serialized_end=11630
+  _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR._serialized_start=10370
+  _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR._serialized_end=10407
+  _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR._serialized_start=10409
+  _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR._serialized_end=10474
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR._serialized_start=10477
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR._serialized_end=10919
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP._serialized_start=10597
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP._serialized_end=10792
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY._serialized_start=10740
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY._serialized_end=10792
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_start=10794
+  _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_end=10919
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR._serialized_start=10922
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR._serialized_end=11443
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP._serialized_start=11064
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP._serialized_end=11293
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY._serialized_start=10740
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY._serialized_end=10792
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_start=11296
+  _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY._serialized_end=11443
+  _SCHEMA_GENERICSCHEMA_RESERVEDNAMEFIELDDESCRIPTOR._serialized_start=11446
+  _SCHEMA_GENERICSCHEMA_RESERVEDNAMEFIELDDESCRIPTOR._serialized_end=11630
+  _SCHEMA_GENERICSCHEMA_RESERVEDNAMEFIELDDESCRIPTOR_PROPERTIESMAPENTRY._serialized_start=10740
+  _SCHEMA_GENERICSCHEMA_RESERVEDNAMEFIELDDESCRIPTOR_PROPERTIESMAPENTRY._serialized_end=10792
+  _SCHEMA_ENVIRONMENT._serialized_start=11632
+  _SCHEMA_ENVIRONMENT._serialized_end=11741
+  _SCHEMA_MODELTYPE._serialized_start=11744
+  _SCHEMA_MODELTYPE._serialized_end=11915
+  _ARROWFILEUPLOADRESPONSE._serialized_start=11927
+  _ARROWFILEUPLOADRESPONSE._serialized_end=12000
+  _USERFILEUPLOADRESPONSE._serialized_start=12002
+  _USERFILEUPLOADRESPONSE._serialized_end=12060
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arize-7.8.1/arize/utils/constants.py` & `arize-7.9.0/arize/utils/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 MAX_PROMPT_TEMPLATE_LENGTH_TRUNCATION = 5_000
 # The maximum number of character for prompt template version
 MAX_PROMPT_TEMPLATE_VERSION_LENGTH = 20_000
 MAX_PROMPT_TEMPLATE_VERSION_LENGTH_TRUNCATION = 50
 # The maximum number of embeddings
 MAX_NUMBER_OF_EMBEDDINGS = 30
 MAX_EMBEDDING_DIMENSIONALITY = 20_000
+# The maximum number of classes for multi class
+MAX_NUMBER_OF_MULTI_CLASS_CLASSES = 100
+MAX_MULTI_CLASS_NAME_LENGTH = 50
 
 # Arize generated columns
 GENERATED_PREDICTION_LABEL_COL = "arize_generated_prediction_label"
 GENERATED_LLM_PARAMS_JSON_COL = "arize_generated_llm_params_json"
 
 # reserved columns for LLM run metadata
 LLM_RUN_METADATA_TOTAL_TOKEN_COUNT_TAG_NAME = "total_token_count"
```

### Comparing `arize-7.8.1/arize/utils/errors.py` & `arize-7.9.0/arize/utils/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/utils/logging.py` & `arize-7.9.0/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/utils/model_mapping.json` & `arize-7.9.0/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/utils/proto.py` & `arize-7.9.0/arize/utils/proto.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize/utils/types.py` & `arize-7.9.0/arize/utils/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import math
 from dataclasses import asdict, dataclass, replace
 from enum import Enum, unique
 from typing import Dict, List, NamedTuple, Optional, Sequence, Set, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 from arize.utils.constants import (
+    MAX_MULTI_CLASS_NAME_LENGTH,
+    MAX_NUMBER_OF_MULTI_CLASS_CLASSES,
     MAX_PREDICTION_ID_LEN,
     MAX_RAW_DATA_CHARACTERS,
     MAX_RAW_DATA_CHARACTERS_TRUNCATION,
     MIN_PREDICTION_ID_LEN,
 )
 from arize.utils.errors import InvalidValueType
 from arize.utils.logging import get_truncation_warning_message, logger
@@ -19,14 +22,15 @@
     NUMERIC = 1
     SCORE_CATEGORICAL = 2
     RANKING = 3
     BINARY_CLASSIFICATION = 4
     REGRESSION = 5
     OBJECT_DETECTION = 6
     GENERATIVE_LLM = 7
+    MULTI_CLASS = 8
 
     @classmethod
     def list_types(cls):
         return [t.name for t in cls]
 
 
 NUMERIC_MODEL_TYPES = [ModelTypes.NUMERIC, ModelTypes.REGRESSION]
@@ -414,14 +418,158 @@
                 raise ValueError(
                     "Object Detection Labels must contain the same number of bounding boxes and "
                     f"confidence scores. Found {n_bounding_boxes} bounding boxes and {n_scores} "
                     "scores."
                 )
 
 
+class MultiClassPredictionLabel(NamedTuple):
+    prediction_scores: Dict[str, Union[float, int]]
+    threshold_scores: Dict[str, Union[float, int]] = None
+    """
+    Used to log multi class prediction label
+    Arguments:
+    ----------
+    MultiClassPredictionLabel
+        prediction_scores (Dict[str, Union[float, int]]): the prediction scores of the classes.
+        threshold_scores (Optional[Dict[str, Union[float, int]]]): the threshold scores of the classes.
+            Only Multi Label will have threshold scores.
+    """
+
+    def validate(self):
+        # Validate scores
+        self._validate_prediction_scores()
+        self._validate_threshold_scores()
+
+    def _validate_prediction_scores(self):
+        # prediction dictionary validations
+        if not is_dict_of(
+            self.prediction_scores, key_allowed_types=str, value_allowed_types=(int, float)
+        ):
+            raise ValueError(
+                "Multi-Class Prediction Scores must be a dictionary with keys of type str "
+                "and values must be a numeric type (int or float)."
+            )
+        # validate length of prediction scores
+        n_prediction_scores = len(self.prediction_scores)
+        if n_prediction_scores == 0 or n_prediction_scores > MAX_NUMBER_OF_MULTI_CLASS_CLASSES:
+            raise ValueError(
+                f"Multi-Class Prediction Scores dictionary must contain at least 1 class and "
+                f"can contain at most {MAX_NUMBER_OF_MULTI_CLASS_CLASSES} classes. "
+                f"Found {n_prediction_scores} classes."
+            )
+
+        for class_name, score in self.prediction_scores.items():
+            if class_name == "":
+                raise ValueError(
+                    "Found at least one class name as an empty string in the Multi-Class Prediction Scores "
+                    "dictionary. All class names (keys in dictionary) must be non-empty strings."
+                )
+            if len(class_name) > MAX_MULTI_CLASS_NAME_LENGTH:
+                raise ValueError(
+                    f"Found at least one class name with more characters than the limit allowed: "
+                    f"{MAX_MULTI_CLASS_NAME_LENGTH} characters. "
+                    f"The class name '{class_name}' has {len(class_name)} characters."
+                )
+            if score > 1 or score < 0:
+                raise ValueError(
+                    "Found at least one score in the Multi-Class Prediction Scores dictionary that was "
+                    "invalid. All scores (values in dictionary) must be between 0 and 1, inclusive."
+                )
+
+    def _validate_threshold_scores(self):
+        if self.threshold_scores is None or len(self.threshold_scores) == 0:
+            return
+        if not is_dict_of(
+            self.threshold_scores, key_allowed_types=str, value_allowed_types=(int, float)
+        ):
+            raise ValueError(
+                "Multi-Class Threshold Scores must be a dictionary with keys of type str "
+                "and values must be a numeric type (int or float)."
+            )
+
+        # validate there are the same number of thresholds as predictions
+        if len(self.threshold_scores) != len(self.prediction_scores):
+            raise ValueError(
+                "Multi-Class Prediction Scores and Threshold Scores Dictionaries must contain the same number"
+                f" of number of classes. Found Prediction Scores Dictionary contains "
+                f"{len(self.prediction_scores)} classes and Threshold Scores Dictionary contains "
+                f"{len(self.threshold_scores)} classes."
+            )
+
+        # validate prediction scores and threshold scores dictionaries contain same classes
+        prediction_class_set = set(self.prediction_scores.keys())
+        threshold_class_set = set(self.threshold_scores.keys())
+        if prediction_class_set != threshold_class_set:
+            raise ValueError(
+                "Multi-Class Prediction Scores and Threshold Scores Dictionaries must contain the same "
+                f"classes. The following classes of the Prediction Scores Dictionary are not in the "
+                f"Threshold Scores Dictionary: {prediction_class_set.difference(threshold_class_set)} \n"
+                "The following classes of the Threshold Scores Dictionary are not in the Prediction Scores "
+                f"Dictionary: {threshold_class_set.difference(prediction_class_set)}"
+            )
+
+        for class_name, t_score in self.threshold_scores.items():
+            if math.isnan(t_score) or t_score > 1 or t_score < 0:
+                raise ValueError(
+                    "Found at least one score in the Multi-Class Threshold Scores dictionary that was "
+                    "invalid. All scores (values) must be between 0 and 1, inclusive. "
+                    f"Found class '{class_name}' has score {t_score}"
+                )
+
+
+class MultiClassActualLabel(NamedTuple):
+    actual_scores: Dict[str, Union[float, int]]
+    """
+    Used to log multi class actual label
+    Arguments:
+    ----------
+    MultiClassActualLabel
+        actual_scores (Dict[str, Union[float, int]]): the actual scores of the classes.
+        Any class in actual_scores with a score of 1 will be sent to arize
+    """
+
+    def validate(self):
+        # Validate scores
+        self._validate_actual_scores()
+
+    def _validate_actual_scores(self):
+        if not is_dict_of(
+            self.actual_scores, key_allowed_types=str, value_allowed_types=(int, float)
+        ):
+            raise ValueError(
+                "Multi-Class Actual Scores must be a dictionary with keys of type str "
+                "and values must be a numeric type (int or float)."
+            )
+        n_actual_scores = len(self.actual_scores)
+        if n_actual_scores == 0 or n_actual_scores > MAX_NUMBER_OF_MULTI_CLASS_CLASSES:
+            raise ValueError(
+                f"Multi-Class Actual Scores dictionary must contain at least 1 class and "
+                f"can contain at most {MAX_NUMBER_OF_MULTI_CLASS_CLASSES} classes. "
+                f"Found {n_actual_scores} classes."
+            )
+        for class_name, score in self.actual_scores.items():
+            if class_name == "":
+                raise ValueError(
+                    "Found at least one class name as an empty string in the Multi-Class Actual Scores "
+                    "dictionary. All class names (keys) must be non-empty strings."
+                )
+            if len(class_name) > MAX_MULTI_CLASS_NAME_LENGTH:
+                raise ValueError(
+                    f"Found at least one class name with more characters than the limit allowed: "
+                    f"{MAX_MULTI_CLASS_NAME_LENGTH} characters. "
+                    f"The class name '{class_name}' has {len(class_name)} characters."
+                )
+            if score != 1 and score != 0:
+                raise ValueError(
+                    "Found at least one score in the Multi-Class Actual Scores dictionary that was invalid. "
+                    f"All scores (values) must be either 0 or 1. Found class '{class_name}' has score {score}"
+                )
+
+
 class RankingPredictionLabel(NamedTuple):
     group_id: str
     rank: int
     score: Optional[float] = None
     label: Optional[str] = None
 
     def validate(self):
@@ -798,26 +946,41 @@
     return isinstance(lst, list) and all(isinstance(x, tp) for x in lst)
 
 
 def is_dict_of(
     d: Dict[object, object],
     key_allowed_types: (T),
     value_allowed_types: (T) = (),
-    list_allowed_types: (T) = (),
+    value_list_allowed_types: (T) = (),
 ) -> bool:
-    if list_allowed_types and not isinstance(list_allowed_types, tuple):
-        list_allowed_types = (list_allowed_types,)
+    """
+    Method to check types are valid for dictionary.
+
+    Arguments:
+    ----------
+        d (Dict[object, object]): dictionary itself
+        key_allowed_types (T): all allowed types for keys of dictionary
+        value_allowed_types (T): all allowed types for values of dictionary
+        value_list_allowed_types (T): if value is a list, these are the allowed types for value list
+
+    Returns:
+    --------
+        True if the data types of dictionary match the types specified by the arguments, false otherwise
+    """
+    if value_list_allowed_types and not isinstance(value_list_allowed_types, tuple):
+        value_list_allowed_types = (value_list_allowed_types,)
 
     return (
         isinstance(d, dict)
         and all(isinstance(k, key_allowed_types) for k in d.keys())
         and all(
-            isinstance(v, value_allowed_types) or any(is_list_of(v, t) for t in list_allowed_types)
+            isinstance(v, value_allowed_types)
+            or any(is_list_of(v, t) for t in value_list_allowed_types)
             for v in d.values()
-            if value_allowed_types or list_allowed_types
+            if value_allowed_types or value_list_allowed_types
         )
     )
 
 
 def count_characters_raw_data(data: Union[str, List[str]]) -> int:
     character_count = 0
     if isinstance(data, str):
```

### Comparing `arize-7.8.1/arize/utils/utils.py` & `arize-7.9.0/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/arize.egg-info/PKG-INFO` & `arize-7.9.0/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.8.1
+Version: 7.9.0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.8.1/arize.egg-info/SOURCES.txt` & `arize-7.9.0/arize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/setup.cfg` & `arize-7.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arize-7.8.1/tests/test_api.py` & `arize-7.9.0/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     SPACE_KEY_ENVVAR_NAME,
 )
 from arize.utils.types import (
     Embedding,
     Environments,
     LLMRunMetadata,
     ModelTypes,
+    MultiClassActualLabel,
+    MultiClassPredictionLabel,
     ObjectDetectionLabel,
     RankingActualLabel,
     RankingPredictionLabel,
 )
 from arize.utils.utils import convert_dictionary, get_python_version
 from google.protobuf.wrappers_pb2 import BoolValue, DoubleValue, StringValue
 
@@ -58,14 +60,17 @@
     "label_str": STR_VAL,
     "label_int": INT_VAL,
     "label_float": FLOAT_VAL,
     "label_tuple": (STR_VAL, FLOAT_VAL),
     "object_detection_bounding_boxes": [[0.1, 0.2, 0.3, 0.4], [0.5, 0.6, 0.7, 0.8]],
     "object_detection_categories": ["dog", "cat"],
     "object_detection_scores": [0.8, 0.4],
+    "multi_class_prediction_scores": {"class1": 0.2, "class2": 0.1, "class3": 0.4},
+    "multi_class_threshold_scores": {"class1": 0.1, "class2": 0.2, "class3": 0.3},
+    "multi_class_actual_scores": {"class1": 0, "class2": 0, "class3": 1},
     "ranking_group_id": "a",
     "ranking_rank": 1,
     "ranking_prediction_score": 1.0,
     "ranking_label": "click",
     "ranking_relevance_labels": ["click", "save"],
     "ranking_relevance_score": 0.5,
     "space_key": "test_space",
@@ -220,14 +225,32 @@
                 )
             )
         od.bounding_boxes.extend(bounding_boxes)
         return pb2.Prediction(
             prediction_label=pb2.PredictionLabel(object_detection=od),
             model_version=inputs["model_version"],
         )
+    elif type == "multi_class":
+        prediction_scores = inputs["multi_class_prediction_scores"]
+        threshold_scores = inputs["multi_class_threshold_scores"]
+        prediction_threshold_scores = {}
+        for class_name, prediction_score in prediction_scores.items():
+            multi_label_scores = pb2.MultiClassPrediction.MultiLabel.MultiLabelScores(
+                prediction_score=DoubleValue(value=prediction_score),
+                threshold_score=DoubleValue(value=threshold_scores[class_name]),
+            )
+            prediction_threshold_scores[class_name] = multi_label_scores
+        multi_label = pb2.MultiClassPrediction.MultiLabel(
+            prediction_threshold_scores=prediction_threshold_scores,
+        )
+        mc_pred = pb2.MultiClassPrediction(multi_label=multi_label)
+        return pb2.Prediction(
+            prediction_label=pb2.PredictionLabel(multi_class=mc_pred),
+            model_version=inputs["model_version"],
+        )
     elif type == "ranking":
         rp = pb2.RankingPrediction()
         rp.rank = inputs["ranking_rank"]
         rp.prediction_group_id = inputs["ranking_group_id"]
         rp.prediction_score.value = inputs["ranking_prediction_score"]
         rp.label = inputs["ranking_label"]
         return pb2.Prediction(
@@ -287,14 +310,25 @@
             bounding_boxes.append(
                 pb2.ObjectDetection.BoundingBox(coordinates=coordinates, category=category)
             )
         od.bounding_boxes.extend(bounding_boxes)
         return pb2.Actual(
             actual_label=pb2.ActualLabel(object_detection=od),
         )
+    elif type == "multi_class":
+        actual_labels = []
+        for class_name, score in inputs["multi_class_actual_scores"].items():
+            if score == 1:
+                actual_labels.append(class_name)
+        mc = pb2.MultiClassActual(
+            actual_labels=actual_labels,
+        )
+        return pb2.Actual(
+            actual_label=pb2.ActualLabel(multi_class=mc),
+        )
     elif type == "ranking":
         ra = pb2.RankingActual()
         ra.category.values.extend(inputs["ranking_relevance_labels"])
         ra.relevance_score.value = inputs["ranking_relevance_score"]
         return pb2.Actual(
             actual_label=pb2.ActualLabel(ranking=ra),
         )
@@ -737,14 +771,98 @@
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
     #   Add props to prediction according to this test
     a.MergeFrom(_attach_tags_to_actual())
     #   Build expected record using built prediction
     expected_record = _build_expected_record(p=p, a=a, ep=ep)
+    #   Check result is as expected
+    assert record == expected_record
+
+
+def test_build_pred_and_actual_label_multi_class_multi_label():
+    pred_label = MultiClassPredictionLabel(
+        prediction_scores=inputs["multi_class_prediction_scores"],
+        threshold_scores=inputs["multi_class_threshold_scores"],
+    )
+    act_label = MultiClassActualLabel(
+        actual_scores=inputs["multi_class_actual_scores"],
+    )
+    c = get_stubbed_client()
+    record = c.log(
+        model_id=inputs["model_id"],
+        model_version=inputs["model_version"],
+        environment=Environments.PRODUCTION,
+        model_type=ModelTypes.MULTI_CLASS,
+        prediction_id=inputs["prediction_id"],
+        prediction_label=pred_label,
+        actual_label=act_label,
+        features=inputs["features"],
+        tags=inputs["tags"],
+    )
+
+    #   Get environment in proto format
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
+    #   Start constructing expected result by building the prediction
+    p = _build_basic_prediction("multi_class")
+    a = _build_basic_actual("multi_class")
+    #   Add props to prediction according to this test
+    p.MergeFrom(_attach_features_to_prediction())
+    p.MergeFrom(_attach_tags_to_prediction())
+    #   Add props to prediction according to this test
+    a.MergeFrom(_attach_tags_to_actual())
+    #   Build expected record using built prediction
+    expected_record = _build_expected_record(p=p, a=a, ep=ep)
+    #   Check result is as expected
+    assert record == expected_record
+
+
+def test_build_pred_and_actual_label_multi_class_single_label():
+    pred_label = MultiClassPredictionLabel(
+        prediction_scores=inputs["multi_class_prediction_scores"],
+    )
+    act_label = MultiClassActualLabel(
+        actual_scores=inputs["multi_class_actual_scores"],
+    )
+    c = get_stubbed_client()
+    record = c.log(
+        model_id=inputs["model_id"],
+        model_version=inputs["model_version"],
+        environment=Environments.PRODUCTION,
+        model_type=ModelTypes.MULTI_CLASS,
+        prediction_id=inputs["prediction_id"],
+        prediction_label=pred_label,
+        actual_label=act_label,
+        features=inputs["features"],
+        tags=inputs["tags"],
+    )
+
+    #   Get environment in proto format
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
+    #   Start constructing expected result by building the prediction
+    prediction_scores_with_double_value = {}
+    for class_name, score in inputs["multi_class_prediction_scores"].items():
+        prediction_scores_with_double_value[class_name] = DoubleValue(value=score)
+    single_label = pb2.MultiClassPrediction.SingleLabel(
+        prediction_scores=prediction_scores_with_double_value,
+    )
+    p = pb2.Prediction(
+        prediction_label=pb2.PredictionLabel(
+            multi_class=pb2.MultiClassPrediction(single_label=single_label)
+        ),
+        model_version=inputs["model_version"],
+    )
+    a = _build_basic_actual("multi_class")
+    #   Add props to prediction according to this test
+    p.MergeFrom(_attach_features_to_prediction())
+    p.MergeFrom(_attach_tags_to_prediction())
+    #   Add props to prediction according to this test
+    a.MergeFrom(_attach_tags_to_actual())
+    #   Build expected record using built prediction
+    expected_record = _build_expected_record(p=p, a=a, ep=ep)
     #   Check result is as expected
     assert record == expected_record
 
 
 def test_build_wrong_timestamp():
     c = get_stubbed_client()
     wrong_min_time = int(time.time()) - (MAX_PAST_YEARS_FROM_CURRENT_TIME * 365 * 24 * 60 * 60 + 1)
```

### Comparing `arize-7.8.1/tests/test_utils.py` & `arize-7.9.0/tests/test_utils.py`

 * *Files identical despite different names*

