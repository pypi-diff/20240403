# Comparing `tmp/adsdatahub-0.0.2.tar.gz` & `tmp/adsdatahub-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsdatahub-0.0.2.tar", max compression
+gzip compressed data, was "adsdatahub-0.0.3.tar", max compression
```

## Comparing `adsdatahub-0.0.2.tar` & `adsdatahub-0.0.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0      292 2024-04-02 08:41:16.592272 adsdatahub-0.0.2/README.md
--rw-r--r--   0        0        0     1241 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      206 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/__init__.py
--rw-r--r--   0        0        0     2188 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/_helpers.py
--rw-r--r--   0        0        0      137 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/client.py
--rw-r--r--   0        0        0        0 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/customer/__init__.py
--rw-r--r--   0        0        0      888 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/customer/customer.py
--rw-r--r--   0        0        0     2209 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/customer/mock_customer.py
--rw-r--r--   0        0        0     2756 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/customer/real_customer.py
--rw-r--r--   0        0        0      450 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/mock_client.py
--rw-r--r--   0        0        0     1969 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/parameters/__init__.py
--rw-r--r--   0        0        0     3165 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/parameters/primitive_parameters.py
--rw-r--r--   0        0        0     4213 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/parameters/pydantic_parameters.py
--rw-r--r--   0        0        0        0 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_job/__init__.py
--rw-r--r--   0        0        0      272 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_job/mock_query_job.py
--rw-r--r--   0        0        0      148 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_job/query_job.py
--rw-r--r--   0        0        0      310 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_job/real_query_job.py
--rw-r--r--   0        0        0     1101 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_result.py
--rw-r--r--   0        0        0     1114 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/real_client.py
--rw-r--r--   0        0        0     4135 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/py.typed
--rw-r--r--   0        0        0      137 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/__init__.py
--rw-r--r--   0        0        0     4149 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/client.py
--rw-r--r--   0        0        0      137 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/http/__init__.py
--rw-r--r--   0        0        0     2117 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/http/client.py
--rw-r--r--   0        0        0     2663 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/http/mock_client.py
--rw-r--r--   0        0        0     1783 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/http/real_client.py
--rw-r--r--   0        0        0     2305 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/mock_client.py
--rw-r--r--   0        0        0     4849 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/real_client.py
--rw-r--r--   0        0        0        0 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/__init__.py
--rw-r--r--   0        0        0     6040 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/__init__.py
--rw-r--r--   0        0        0     1450 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/list.py
--rw-r--r--   0        0        0     1203 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/start_transient.py
--rw-r--r--   0        0        0     3634 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/validate.py
--rw-r--r--   0        0        0     5065 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_query/__init__.py
--rw-r--r--   0        0        0     1105 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_query/start.py
--rw-r--r--   0        0        0     6604 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operation/__init__.py
--rw-r--r--   0        0        0      727 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operation/wait.py
--rw-r--r--   0        0        0     2909 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operations/__init__.py
--rw-r--r--   0        0        0      911 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operations/list.py
--rw-r--r--   0        0        0        0 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/__init__.py
--rw-r--r--   0        0        0      234 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/_model.py
--rw-r--r--   0        0        0     1743 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_queries_start.py
--rw-r--r--   0        0        0    12487 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_query.py
--rw-r--r--   0        0        0     1180 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_query_metadata.py
--rw-r--r--   0        0        0      214 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column.py
--rw-r--r--   0        0        0      735 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column_info.py
--rw-r--r--   0        0        0      671 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column_summary_rule.py
--rw-r--r--   0        0        0     1422 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/date.py
--rw-r--r--   0        0        0     2450 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/destination_table_info.py
--rw-r--r--   0        0        0     1364 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/field_type.py
--rw-r--r--   0        0        0      936 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/filtered_row_summary.py
--rw-r--r--   0        0        0     1202 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_column.py
--rw-r--r--   0        0        0      442 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_spec.py
--rw-r--r--   0        0        0      636 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_type.py
--rw-r--r--   0        0        0      677 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/noise_impact.py
--rw-r--r--   0        0        0     3132 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/operation.py
--rw-r--r--   0        0        0      661 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/output_artifacts.py
--rw-r--r--   0        0        0     1188 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/parameter_type.py
--rw-r--r--   0        0        0     1012 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/parameter_value.py
--rw-r--r--   0        0        0      508 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/privacy_message.py
--rw-r--r--   0        0        0     2349 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/privacy_message_type.py
--rw-r--r--   0        0        0     3861 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_execution_spec.py
--rw-r--r--   0        0        0     2565 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_metadata.py
--rw-r--r--   0        0        0      977 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_performance_info.py
--rw-r--r--   0        0        0     1995 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_response.py
--rw-r--r--   0        0        0      504 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_share.py
--rw-r--r--   0        0        0      536 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_state.py
--rw-r--r--   0        0        0      567 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_type.py
--rw-r--r--   0        0        0      559 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/share_type.py
--rw-r--r--   0        0        0     1680 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/status.py
--rw-r--r--   0        0        0      661 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/summary_type.py
--rw-r--r--   0        0        0     1015 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/table_noise_impact.py
--rw-r--r--   0        0        0     2411 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/temp_table.py
--rw-r--r--   0        0        0      562 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/types.py
--rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 adsdatahub-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      292 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/README.md
+-rw-r--r--   0        0        0     1241 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      206 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/__init__.py
+-rw-r--r--   0        0        0     2188 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/_helpers.py
+-rw-r--r--   0        0        0      137 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/client.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/customer/__init__.py
+-rw-r--r--   0        0        0      888 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/customer/customer.py
+-rw-r--r--   0        0        0     2209 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/customer/mock_customer.py
+-rw-r--r--   0        0        0     2756 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/customer/real_customer.py
+-rw-r--r--   0        0        0      450 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/mock_client.py
+-rw-r--r--   0        0        0     1969 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/parameters/__init__.py
+-rw-r--r--   0        0        0     3165 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/parameters/primitive_parameters.py
+-rw-r--r--   0        0        0     4213 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/parameters/pydantic_parameters.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/query_job/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-03 12:36:32.942427 adsdatahub-0.0.3/src/adsdatahub/client/query_job/mock_query_job.py
+-rw-r--r--   0        0        0      148 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/client/query_job/query_job.py
+-rw-r--r--   0        0        0      310 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/client/query_job/real_query_job.py
+-rw-r--r--   0        0        0     1101 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/client/query_result.py
+-rw-r--r--   0        0        0     1114 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/client/real_client.py
+-rw-r--r--   0        0        0     4135 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/py.typed
+-rw-r--r--   0        0        0      137 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/__init__.py
+-rw-r--r--   0        0        0     4149 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/client.py
+-rw-r--r--   0        0        0      137 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/http/__init__.py
+-rw-r--r--   0        0        0     2117 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/http/client.py
+-rw-r--r--   0        0        0     2663 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/http/mock_client.py
+-rw-r--r--   0        0        0     1783 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/http/real_client.py
+-rw-r--r--   0        0        0     2305 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/mock_client.py
+-rw-r--r--   0        0        0     4849 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/real_client.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/__init__.py
+-rw-r--r--   0        0        0     6040 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_queries/__init__.py
+-rw-r--r--   0        0        0     1450 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_queries/list.py
+-rw-r--r--   0        0        0     1203 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_queries/start_transient.py
+-rw-r--r--   0        0        0     3634 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_queries/validate.py
+-rw-r--r--   0        0        0     5065 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_query/__init__.py
+-rw-r--r--   0        0        0     1105 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_query/start.py
+-rw-r--r--   0        0        0     6604 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/operation/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/operation/wait.py
+-rw-r--r--   0        0        0     2909 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/operations/__init__.py
+-rw-r--r--   0        0        0      911 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/resources/operations/list.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/__init__.py
+-rw-r--r--   0        0        0      234 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/_model.py
+-rw-r--r--   0        0        0     1743 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/analysis_queries_start.py
+-rw-r--r--   0        0        0    12487 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/analysis_query.py
+-rw-r--r--   0        0        0     1180 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/analysis_query_metadata.py
+-rw-r--r--   0        0        0      214 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/column.py
+-rw-r--r--   0        0        0      735 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/column_info.py
+-rw-r--r--   0        0        0      671 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/column_summary_rule.py
+-rw-r--r--   0        0        0     1422 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/date.py
+-rw-r--r--   0        0        0     2450 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/destination_table_info.py
+-rw-r--r--   0        0        0     1364 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/field_type.py
+-rw-r--r--   0        0        0      936 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/filtered_row_summary.py
+-rw-r--r--   0        0        0     1202 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/merge_column.py
+-rw-r--r--   0        0        0      442 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/merge_spec.py
+-rw-r--r--   0        0        0      636 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/merge_type.py
+-rw-r--r--   0        0        0      677 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/noise_impact.py
+-rw-r--r--   0        0        0     3132 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/operation.py
+-rw-r--r--   0        0        0      661 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/output_artifacts.py
+-rw-r--r--   0        0        0     1188 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/parameter_type.py
+-rw-r--r--   0        0        0     1012 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/parameter_value.py
+-rw-r--r--   0        0        0      508 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/privacy_message.py
+-rw-r--r--   0        0        0     2349 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/privacy_message_type.py
+-rw-r--r--   0        0        0     3861 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_execution_spec.py
+-rw-r--r--   0        0        0     2565 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_metadata.py
+-rw-r--r--   0        0        0      977 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_performance_info.py
+-rw-r--r--   0        0        0     1995 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_response.py
+-rw-r--r--   0        0        0      504 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_share.py
+-rw-r--r--   0        0        0      536 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_state.py
+-rw-r--r--   0        0        0      567 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_type.py
+-rw-r--r--   0        0        0      559 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/share_type.py
+-rw-r--r--   0        0        0     1680 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/status.py
+-rw-r--r--   0        0        0      661 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/summary_type.py
+-rw-r--r--   0        0        0     1015 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/table_noise_impact.py
+-rw-r--r--   0        0        0     2411 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/temp_table.py
+-rw-r--r--   0        0        0      562 2024-04-03 12:36:32.946426 adsdatahub-0.0.3/src/adsdatahub/types.py
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 adsdatahub-0.0.3/PKG-INFO
```

### Comparing `adsdatahub-0.0.2/pyproject.toml` & `adsdatahub-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adsdatahub"
-version = "0.0.2"
+version = "0.0.3"
 description = "Ads Data Hub API client for Python"
 authors = ["yassun7010 <yassun7010@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "adsdatahub", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `adsdatahub-0.0.2/src/adsdatahub/_helpers.py` & `adsdatahub-0.0.3/src/adsdatahub/_helpers.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/client/client.py` & `adsdatahub-0.0.3/src/adsdatahub/client/client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/client/customer/customer.py` & `adsdatahub-0.0.3/src/adsdatahub/client/customer/customer.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/client/customer/mock_customer.py` & `adsdatahub-0.0.3/src/adsdatahub/client/customer/mock_customer.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/client/customer/real_customer.py` & `adsdatahub-0.0.3/src/adsdatahub/client/customer/real_customer.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/client/parameters/__init__.py` & `adsdatahub-0.0.3/src/adsdatahub/client/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/client/parameters/primitive_parameters.py` & `adsdatahub-0.0.3/src/adsdatahub/client/parameters/primitive_parameters.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/client/parameters/pydantic_parameters.py` & `adsdatahub-0.0.3/src/adsdatahub/client/parameters/pydantic_parameters.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/client/query_result.py` & `adsdatahub-0.0.3/src/adsdatahub/client/query_result.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/client/real_client.py` & `adsdatahub-0.0.3/src/adsdatahub/client/real_client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/exceptions.py` & `adsdatahub-0.0.3/src/adsdatahub/exceptions.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/client.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/http/client.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/http/client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/http/mock_client.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/http/mock_client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/http/real_client.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/http/real_client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/mock_client.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/mock_client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/real_client.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/real_client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/__init__.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/list.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_queries/list.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/start_transient.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_queries/start_transient.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/validate.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_queries/validate.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_query/__init__.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_query/__init__.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_query/start.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/analysis_query/start.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operation/__init__.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operation/wait.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/operation/wait.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operations/__init__.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operations/list.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/resources/operations/list.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_queries_start.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/analysis_queries_start.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_query.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/analysis_query.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_query_metadata.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/analysis_query_metadata.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column_info.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/column_info.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column_summary_rule.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/column_summary_rule.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/date.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/date.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/destination_table_info.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/destination_table_info.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/field_type.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/field_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/filtered_row_summary.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/filtered_row_summary.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_column.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/merge_column.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_type.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/merge_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/noise_impact.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/noise_impact.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/operation.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/operation.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/output_artifacts.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/output_artifacts.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/parameter_type.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/parameter_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/parameter_value.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/parameter_value.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/privacy_message_type.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/privacy_message_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_execution_spec.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_execution_spec.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_metadata.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_metadata.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_performance_info.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_performance_info.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_response.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_response.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_state.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_state.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_type.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/query_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/share_type.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/share_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/status.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/status.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/summary_type.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/summary_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/table_noise_impact.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/table_noise_impact.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/temp_table.py` & `adsdatahub-0.0.3/src/adsdatahub/restapi/schemas/temp_table.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/src/adsdatahub/types.py` & `adsdatahub-0.0.3/src/adsdatahub/types.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.2/PKG-INFO` & `adsdatahub-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsdatahub
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ads Data Hub API client for Python
 Author: yassun7010
 Author-email: yassun7010@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

