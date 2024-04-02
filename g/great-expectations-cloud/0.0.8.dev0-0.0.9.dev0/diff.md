# Comparing `tmp/great_expectations_cloud-0.0.8.dev0.tar.gz` & `tmp/great_expectations_cloud-0.0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-0.0.8.dev0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-0.0.9.dev0.tar", max compression
```

## Comparing `great_expectations_cloud-0.0.8.dev0.tar` & `great_expectations_cloud-0.0.9.dev0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1022 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/LICENSE
--rw-r--r--   0        0        0     2116 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/README.md
--rw-r--r--   0        0        0      114 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      114 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      576 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      697 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      280 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1334 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1328 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4132 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     2467 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2635 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     1066 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     1620 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py
--rw-r--r--   0        0        0    10744 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0     1320 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      423 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0     3761 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0        0 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9017 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5334 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     2402 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      158 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0     1841 2023-11-28 19:28:51.324452 great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/logging_cfg.py
--rw-r--r--   0        0        0     5850 2023-11-28 19:28:51.328452 great_expectations_cloud-0.0.8.dev0/pyproject.toml
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 great_expectations_cloud-0.0.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/LICENSE
+-rw-r--r--   0        0        0     2116 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/README.md
+-rw-r--r--   0        0        0      114 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      114 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      576 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      697 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      280 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1334 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1328 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4132 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     2467 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2635 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     1066 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     1620 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py
+-rw-r--r--   0        0        0    10744 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0     1320 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      423 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0     3761 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0        0 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9065 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5334 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     2402 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      158 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0     1841 2023-11-29 18:21:57.122602 great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/logging_cfg.py
+-rw-r--r--   0        0        0     5852 2023-11-29 18:21:57.126602 great_expectations_cloud-0.0.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 great_expectations_cloud-0.0.9.dev0/PKG-INFO
```

### Comparing `great_expectations_cloud-0.0.8.dev0/LICENSE` & `great_expectations_cloud-0.0.9.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/README.md` & `great_expectations_cloud-0.0.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/agent.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,16 @@
 
     def _build_client_parameters(self, url: str) -> pika.URLParameters:
         """Configure parameters used to connect to the broker."""
         parameters = pika.URLParameters(url)
         # only enable SSL if connection string calls for it
         if url.startswith("amqps://"):
             # SSL Context for TLS configuration of Amazon MQ for RabbitMQ
-            ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLSv1_2)
+            ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+            ssl_context.load_default_certs()
             ssl_context.set_ciphers("ECDHE+AESGCM:!ECDSA")
             parameters.ssl_options = pika.SSLOptions(context=ssl_context)
         return parameters
 
 
 class ClientError(Exception):
     ...
```

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/great_expectations_cloud/logging_cfg.py` & `great_expectations_cloud-0.0.9.dev0/great_expectations_cloud/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-0.0.8.dev0/pyproject.toml` & `great_expectations_cloud-0.0.9.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "0.0.8.dev0"
+version = "0.0.9.dev0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
@@ -38,21 +38,21 @@
     "redshift",
 ] }
 snowflake-sqlalchemy = ">=1.5.0"
 snowflake-connector-python = ">=3.3.1"
 
 [tool.poetry.group.dev.dependencies]
 invoke = "^2.2.0"
-mypy = "~1.6"
+mypy = "~1.7.1"
 pre-commit = "^3.3.3"
 pytest = "^7.4.0"
 pytest-icdiff = "*"
 pytest-mock = "*"
 responses = "^0.23.1"
-ruff = "^0.1.5"
+ruff = "^0.1.6"
 tenacity = "^8.2.3"
 tomlkit = "^0.12.1"
 typing_extensions = ">=4.4.0"
 types-requests = "^2.31"
 
 [tool.poetry.scripts]
 gx-agent = 'great_expectations_cloud.agent.cli:main'
```

### Comparing `great_expectations_cloud-0.0.8.dev0/PKG-INFO` & `great_expectations_cloud-0.0.9.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great-expectations-cloud
-Version: 0.0.8.dev0
+Version: 0.0.9.dev0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
```

