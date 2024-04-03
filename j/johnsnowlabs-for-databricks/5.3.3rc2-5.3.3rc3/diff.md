# Comparing `tmp/johnsnowlabs_for_databricks-5.3.3rc2.tar.gz` & `tmp/johnsnowlabs_for_databricks-5.3.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs_for_databricks-5.3.3rc2.tar", last modified: Tue Mar 19 22:22:04 2024, max compression
+gzip compressed data, was "johnsnowlabs_for_databricks-5.3.3rc3.tar", last modified: Wed Apr  3 02:29:14 2024, max compression
```

## Comparing `johnsnowlabs_for_databricks-5.3.3rc2.tar` & `johnsnowlabs_for_databricks-5.3.3rc3.tar`

### file list

```diff
@@ -1,153 +1,163 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/.github/workflows/
--rw-rw-r--   0 root         (0) root         (0)     3388 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc2/.github/workflows/create_search_index.yml
--rw-rw-r--   0 root         (0) root         (0)     5379 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc2/.gitignore
--rw-rw-r--   0 root         (0) root         (0)    11356 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9336 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/PKG-INFO
--r--r--r--   0 root         (0) root         (0)     8310 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/docker/johnsnowlabs_fastapi/
--rw-rw-r--   0 root         (0) root         (0)     1178 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc2/docker/johnsnowlabs_fastapi/Dockerfile
--rw-rw-r--   0 root         (0) root         (0)     1075 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc2/docker/johnsnowlabs_fastapi/README.md
--rw-rw-r--   0 root         (0) root         (0)      372 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc2/docker/johnsnowlabs_fastapi/docker-compose.yaml
--rw-rw-r--   0 root         (0) root         (0)     1566 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc2/docker/johnsnowlabs_fastapi/fastapi_app.py
--rw-rw-r--   0 root         (0) root         (0)       34 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc2/docker/johnsnowlabs_fastapi/license.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/
--rw-rw-r--   0 root         (0) root         (0)      962 2024-03-05 00:51:18.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/abstract_base/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      395 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 root         (0) root         (0)     9794 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 root         (0) root         (0)      733 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 root         (0) root         (0)     9326 2024-03-13 13:11:15.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/abstract_base/software_product.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2680 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 root         (0) root         (0)    28916 2024-03-05 00:53:21.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)    20854 2024-03-12 00:24:49.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 root         (0) root         (0)     7591 2024-03-05 00:51:18.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/marketplace.py
--rw-rw-r--   0 root         (0) root         (0)    21829 2024-03-05 00:51:18.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/marketplace_offering.py
--rw-rw-r--   0 root         (0) root         (0)    12197 2024-03-05 00:51:18.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/emr/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/emr/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      376 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/emr/enums.py
--rw-rw-r--   0 root         (0) root         (0)    11474 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/emr/install_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1850 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/emr/utils.py
--rw-rw-r--   0 root         (0) root         (0)     4164 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/emr/work_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.257865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/glue/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/glue/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2806 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/glue/install_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3191 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/glue/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        1 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/benchmark_test.py
--rw-rw-r--   0 root         (0) root         (0)     6100 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/endpoint_test.py
--rw-rw-r--   0 root         (0) root         (0)      690 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/generate_test.py
--rw-rw-r--   0 root         (0) root         (0)      832 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 root         (0) root         (0)      317 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/load_predict_test.py
--rw-rw-r--   0 root         (0) root         (0)      908 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 root         (0) root         (0)     2124 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 root         (0) root         (0)     3496 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 root         (0) root         (0)    20831 2024-03-07 23:48:39.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 root         (0) root         (0)    11362 2024-03-13 13:15:47.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 root         (0) root         (0)    12178 2024-03-05 14:57:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/jsl_home.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 root         (0) root         (0)      124 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2061 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 root         (0) root         (0)     3192 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 root         (0) root         (0)     2105 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 root         (0) root         (0)     9118 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/offline_install.py
--rw-rw-r--   0 root         (0) root         (0)     9133 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 root         (0) root         (0)     5619 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/finance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 00:51:18.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/embedding_retrieval/
--rw-rw-r--   0 root         (0) root         (0)      547 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/embedding_retrieval/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18435 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py
--rw-rw-r--   0 root         (0) root         (0)    14001 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py
--rw-rw-r--   0 root         (0) root         (0)     6757 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/embedding_retrieval/utils.py
--rw-rw-r--   0 root         (0) root         (0)      212 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/lab.py
--rw-rw-r--   0 root         (0) root         (0)     5560 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/legal.py
--rw-rw-r--   0 root         (0) root         (0)       56 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/llm.py
--rw-rw-r--   0 root         (0) root         (0)     5440 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/medical.py
--rw-rw-r--   0 root         (0) root         (0)     1608 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/nlp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-05 00:51:18.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4945 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 root         (0) root         (0)    34057 2024-03-05 00:51:41.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 root         (0) root         (0)     4168 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 root         (0) root         (0)        2 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 root         (0) root         (0)      128 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 root         (0) root         (0)     2077 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 root         (0) root         (0)     2978 2024-03-19 22:21:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      997 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/boto_utils.py
--rw-rw-r--   0 root         (0) root         (0)     6668 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 root         (0) root         (0)     4594 2024-03-05 00:51:18.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 root         (0) root         (0)      759 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1005 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 root         (0) root         (0)     3326 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 root         (0) root         (0)    10596 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 root         (0) root         (0)    10654 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 root         (0) root         (0)     5856 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 root         (0) root         (0)      982 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 root         (0) root         (0)     4371 2024-03-05 00:51:18.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 root         (0) root         (0)     3109 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/s3_utils.py
--rw-rw-r--   0 root         (0) root         (0)     8495 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/sparksession_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4050 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 root         (0) root         (0)     1778 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 root         (0) root         (0)     1132 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 root         (0) root         (0)     3460 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 root         (0) root         (0)     4353 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1332 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/visual.py
--rw-rw-r--   0 root         (0) root         (0)      408 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs_for_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9336 2024-03-19 22:22:04.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs_for_databricks.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4927 2024-03-19 22:22:04.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs_for_databricks.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-03-19 22:22:04.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs_for_databricks.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      129 2024-03-19 22:22:04.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs_for_databricks.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2024-03-19 22:22:04.000000 johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs_for_databricks.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/notebooks/
--rw-rw-r--   0 root         (0) root         (0)     6777 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/notebooks/create_databricks_cluster.ipynb
--rw-rw-r--   0 root         (0) root         (0)     8273 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/notebooks/create_emr_cluster.ipynb
--rw-rw-r--   0 root         (0) root         (0)   145269 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/notebooks/databricks_endpoints_tutorial.ipynb
--rw-rw-r--   0 root         (0) root         (0)    19726 2024-03-05 00:51:18.000000 johnsnowlabs_for_databricks-5.3.3rc2/notebooks/databricks_model_marketplace.ipynb
--rw-rw-r--   0 root         (0) root         (0)    41449 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/notebooks/haystack_with_johnsnowlabs.ipynb
--rw-rw-r--   0 root         (0) root         (0)    11963 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/notebooks/langchain_with_johnsnowlabs.ipynb
--rw-rw-r--   0 root         (0) root         (0)     3685 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/notebooks/parameterized_nb_example.ipynb
--rw-rw-r--   0 root         (0) root         (0)     7837 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/notebooks/setup_glue_notebook.ipynb
--rw-rw-r--   0 root         (0) root         (0)      251 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc2/pytest.ini
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2074 2024-02-23 06:25:49.000000 johnsnowlabs_for_databricks-5.3.3rc2/setup_johnsnowlabs.py
--rw-rw-r--   0 root         (0) root         (0)     2028 2024-02-23 06:25:49.000000 johnsnowlabs_for_databricks-5.3.3rc2/setup_johnsnowlabs_for_databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6699 2024-03-11 05:43:30.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/auto_install.py
--rw-rw-r--   0 root         (0) root         (0)     1527 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/backward_compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1599 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/db_infos_test.py
--rw-rw-r--   0 root         (0) root         (0)    13529 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/db_test_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4385 2024-02-23 06:25:49.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/endpoint_tests.py
--rw-rw-r--   0 root         (0) root         (0)      724 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/hdfs_tests.py
--rw-rw-r--   0 root         (0) root         (0)     2543 2024-03-11 05:39:03.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/install_tests.py
--rw-rw-r--   0 root         (0) root         (0)     3531 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/parameterized_nb_example.ipynb
--rw-rw-r--   0 root         (0) root         (0)     1003 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/sample.ipynb
--rw-rw-r--   0 root         (0) root         (0)     4533 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/submit_tests.py
--rw-rw-r--   0 root         (0) root         (0)      948 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/file_models.py
--rw-rw-r--   0 root         (0) root         (0)     3158 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/install.py
--rw-rw-r--   0 root         (0) root         (0)     3368 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/jsl_dependency_resolver.py
--rw-rw-r--   0 root         (0) root         (0)     2986 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/jsl_secrets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:22:04.261865 johnsnowlabs_for_databricks-5.3.3rc2/tests/llm_frameworks/
--rw-rw-r--   0 root         (0) root         (0)     2696 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/llm_frameworks/test_haystack.py
--rw-rw-r--   0 root         (0) root         (0)     3057 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/llm_frameworks/test_langchain.py
--rw-rw-r--   0 root         (0) root         (0)     1648 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/markdown_tests.py
--rw-rw-r--   0 root         (0) root         (0)     2272 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/notebook_tests.py
--rw-rw-r--   0 root         (0) root         (0)     9066 2024-03-05 02:16:51.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/spark_session.py
--rw-rw-r--   0 root         (0) root         (0)     1798 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc2/tests/venv_wrapper_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.971811 johnsnowlabs_for_databricks-5.3.3rc3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.959811 johnsnowlabs_for_databricks-5.3.3rc3/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/.github/workflows/
+-rw-rw-r--   0 root         (0) root         (0)     3388 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc3/.github/workflows/create_search_index.yml
+-rw-rw-r--   0 root         (0) root         (0)     5379 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc3/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)    11356 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9336 2024-04-03 02:29:14.971811 johnsnowlabs_for_databricks-5.3.3rc3/PKG-INFO
+-r--r--r--   0 root         (0) root         (0)     8310 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.959811 johnsnowlabs_for_databricks-5.3.3rc3/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/docker/johnsnowlabs_fastapi/
+-rw-rw-r--   0 root         (0) root         (0)     1178 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc3/docker/johnsnowlabs_fastapi/Dockerfile
+-rw-rw-r--   0 root         (0) root         (0)     1075 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc3/docker/johnsnowlabs_fastapi/README.md
+-rw-rw-r--   0 root         (0) root         (0)      372 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc3/docker/johnsnowlabs_fastapi/docker-compose.yaml
+-rw-rw-r--   0 root         (0) root         (0)     1566 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc3/docker/johnsnowlabs_fastapi/fastapi_app.py
+-rw-rw-r--   0 root         (0) root         (0)       34 2024-02-14 23:45:57.000000 johnsnowlabs_for_databricks-5.3.3rc3/docker/johnsnowlabs_fastapi/license.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/
+-rw-rw-r--   0 root         (0) root         (0)     1042 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      395 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 root         (0) root         (0)     9794 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 root         (0) root         (0)      733 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 root         (0) root         (0)     9326 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/abstract_base/software_product.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2680 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 root         (0) root         (0)    28916 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)    20814 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     7591 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/marketplace.py
+-rw-rw-r--   0 root         (0) root         (0)    21829 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/marketplace_offering.py
+-rw-rw-r--   0 root         (0) root         (0)    12197 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/docker/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/docker/build/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-25 19:19:42.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/docker/build/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4191 2024-04-02 21:27:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/docker/build/app.py
+-rw-rw-r--   0 root         (0) root         (0)     1347 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/docker/build/installer.py
+-rw-rw-r--   0 root         (0) root         (0)     1109 2024-03-27 17:30:09.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/docker/build/test_qucik.py
+-rw-rw-r--   0 root         (0) root         (0)       84 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/docker/docker_template.py
+-rw-rw-r--   0 root         (0) root         (0)    13278 2024-04-01 23:43:48.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/docker/work_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/emr/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/emr/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      376 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/emr/enums.py
+-rw-rw-r--   0 root         (0) root         (0)    11474 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/emr/install_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1850 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/emr/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4164 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/emr/work_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.963811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/glue/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/glue/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2806 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/glue/install_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3191 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/glue/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.967811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/benchmark_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6100 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/endpoint_test.py
+-rw-rw-r--   0 root         (0) root         (0)      690 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/generate_test.py
+-rw-rw-r--   0 root         (0) root         (0)      832 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/load_predict_test.py
+-rw-rw-r--   0 root         (0) root         (0)      908 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2124 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3496 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 root         (0) root         (0)    20668 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 root         (0) root         (0)    11362 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 root         (0) root         (0)    12178 2024-03-05 14:57:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/jsl_home.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.967811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 root         (0) root         (0)      124 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2061 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 root         (0) root         (0)     3192 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 root         (0) root         (0)     2105 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 root         (0) root         (0)     9118 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/offline_install.py
+-rw-rw-r--   0 root         (0) root         (0)     9133 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 root         (0) root         (0)     5619 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/finance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.967811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.967811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/embedding_retrieval/
+-rw-rw-r--   0 root         (0) root         (0)      547 2024-03-25 19:19:32.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/embedding_retrieval/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    18435 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py
+-rw-rw-r--   0 root         (0) root         (0)    14001 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py
+-rw-rw-r--   0 root         (0) root         (0)     6757 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/embedding_retrieval/utils.py
+-rw-rw-r--   0 root         (0) root         (0)      212 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/lab.py
+-rw-rw-r--   0 root         (0) root         (0)     5560 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/legal.py
+-rw-rw-r--   0 root         (0) root         (0)       56 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/llm.py
+-rw-rw-r--   0 root         (0) root         (0)     5440 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/medical.py
+-rw-rw-r--   0 root         (0) root         (0)     1712 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/nlp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.967811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4945 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 root         (0) root         (0)    34057 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 root         (0) root         (0)     4168 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 root         (0) root         (0)        2 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 root         (0) root         (0)      128 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 root         (0) root         (0)     2077 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 root         (0) root         (0)      121 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/serve.py
+-rw-rw-r--   0 root         (0) root         (0)     2938 2024-04-03 02:29:02.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.967811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      997 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/boto_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     6668 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     4845 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      759 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1005 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 root         (0) root         (0)     3326 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 root         (0) root         (0)    10596 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 root         (0) root         (0)    10654 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 root         (0) root         (0)     5856 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      982 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 root         (0) root         (0)     4953 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 root         (0) root         (0)     3109 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/s3_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     8495 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/sparksession_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.967811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4050 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 root         (0) root         (0)     1778 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 root         (0) root         (0)     1132 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 root         (0) root         (0)     3460 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 root         (0) root         (0)     4353 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1332 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/visual.py
+-rw-rw-r--   0 root         (0) root         (0)      408 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.967811 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs_for_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9336 2024-04-03 02:29:14.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs_for_databricks.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5295 2024-04-03 02:29:14.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs_for_databricks.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-03 02:29:14.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs_for_databricks.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      126 2024-04-03 02:29:14.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs_for_databricks.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2024-04-03 02:29:14.000000 johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs_for_databricks.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.967811 johnsnowlabs_for_databricks-5.3.3rc3/notebooks/
+-rw-rw-r--   0 root         (0) root         (0)     6777 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/notebooks/create_databricks_cluster.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     8273 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/notebooks/create_emr_cluster.ipynb
+-rw-rw-r--   0 root         (0) root         (0)   145269 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/notebooks/databricks_endpoints_tutorial.ipynb
+-rw-rw-r--   0 root         (0) root         (0)    19726 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/notebooks/databricks_model_marketplace.ipynb
+-rw-rw-r--   0 root         (0) root         (0)    41449 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/notebooks/haystack_with_johnsnowlabs.ipynb
+-rw-rw-r--   0 root         (0) root         (0)    11963 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/notebooks/langchain_with_johnsnowlabs.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     3685 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/notebooks/parameterized_nb_example.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     7837 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/notebooks/setup_glue_notebook.ipynb
+-rw-rw-r--   0 root         (0) root         (0)      251 2024-02-14 23:45:59.000000 johnsnowlabs_for_databricks-5.3.3rc3/pytest.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 02:29:14.971811 johnsnowlabs_for_databricks-5.3.3rc3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2216 2024-04-01 23:43:41.000000 johnsnowlabs_for_databricks-5.3.3rc3/setup_johnsnowlabs.py
+-rw-rw-r--   0 root         (0) root         (0)     2028 2024-02-23 06:25:49.000000 johnsnowlabs_for_databricks-5.3.3rc3/setup_johnsnowlabs_for_databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.971811 johnsnowlabs_for_databricks-5.3.3rc3/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6986 2024-04-02 01:23:42.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/auto_install.py
+-rw-rw-r--   0 root         (0) root         (0)     1527 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/backward_compat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.971811 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1599 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/db_infos_test.py
+-rw-rw-r--   0 root         (0) root         (0)    13529 2024-03-05 01:02:38.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/db_test_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4385 2024-02-23 06:25:49.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/endpoint_tests.py
+-rw-rw-r--   0 root         (0) root         (0)      724 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/hdfs_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     2541 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/install_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     3531 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/parameterized_nb_example.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     1003 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/sample.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     4533 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/submit_tests.py
+-rw-rw-r--   0 root         (0) root         (0)      948 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/file_models.py
+-rw-rw-r--   0 root         (0) root         (0)     3158 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/install.py
+-rw-rw-r--   0 root         (0) root         (0)     3368 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/jsl_dependency_resolver.py
+-rw-rw-r--   0 root         (0) root         (0)     2986 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/jsl_secrets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:29:14.971811 johnsnowlabs_for_databricks-5.3.3rc3/tests/llm_frameworks/
+-rw-rw-r--   0 root         (0) root         (0)     2696 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/llm_frameworks/test_haystack.py
+-rw-rw-r--   0 root         (0) root         (0)     3057 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/llm_frameworks/test_langchain.py
+-rw-rw-r--   0 root         (0) root         (0)     1648 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/markdown_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     2272 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/notebook_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     9066 2024-03-23 03:19:52.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/spark_session.py
+-rw-rw-r--   0 root         (0) root         (0)     1798 2024-02-15 00:31:00.000000 johnsnowlabs_for_databricks-5.3.3rc3/tests/venv_wrapper_tests.py
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/.github/workflows/create_search_index.yml` & `johnsnowlabs_for_databricks-5.3.3rc3/.github/workflows/create_search_index.yml`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/.gitignore` & `johnsnowlabs_for_databricks-5.3.3rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/LICENSE` & `johnsnowlabs_for_databricks-5.3.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/PKG-INFO` & `johnsnowlabs_for_databricks-5.3.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs_for_databricks
-Version: 5.3.3rc2
+Version: 5.3.3rc3
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 License: UNKNOWN
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Platform: UNKNOWN
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/README.md` & `johnsnowlabs_for_databricks-5.3.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/docker/johnsnowlabs_fastapi/Dockerfile` & `johnsnowlabs_for_databricks-5.3.3rc3/docker/johnsnowlabs_fastapi/Dockerfile`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/docker/johnsnowlabs_fastapi/README.md` & `johnsnowlabs_for_databricks-5.3.3rc3/docker/johnsnowlabs_fastapi/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/docker/johnsnowlabs_fastapi/fastapi_app.py` & `johnsnowlabs_for_databricks-5.3.3rc3/docker/johnsnowlabs_fastapi/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/endpoints.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/endpoints.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 
 def install_license_to_cluster(install_suite: InstallSuite, db: DatabricksAPI, ):
     lic = {
         "SECRET": install_suite.secrets.HC_SECRET,
         "SPARK_OCR_SECRET": install_suite.secrets.OCR_SECRET,
         "SPARK_NLP_LICENSE": install_suite.secrets.HC_LICENSE,
+        "SPARK_OCR_LICENSE": install_suite.secrets.OCR_LICENSE,
     }
     lic = {k: v for k, v in lic.items() if v is not None}
 
     put_file_on_dbfs(db, settings.dbfs_license_path, lic, overwrite=True)
     return settings.dbfs_license_path
 
 
@@ -112,40 +113,40 @@
     else:
         user_spark_env_vars.update(default_spark_env_vars)
         spark_env_vars = user_spark_env_vars
     return spark_env_vars
 
 
 def create_cluster(
-        databricks_host: str,
-        databricks_token: str,
-        medical_nlp,
-        spark_nlp,
-        visual,
-        install_suite: InstallSuite = None,
-        num_workers=1,
-        cluster_name=settings.db_cluster_name,
-        node_type_id=settings.db_node_type_id,
-        driver_node_type_id=settings.db_driver_node_type,
-        spark_env_vars=None,
-        autotermination_minutes=60,
-        spark_version=settings.db_spark_version,
-        spark_conf=None,
-        auto_scale=None,
-        aws_attributes=None,
-        ssh_public_keys=None,
-        custom_tags=None,
-        cluster_log_conf=None,
-        enable_elastic_disk=None,
-        cluster_source=None,
-        instance_pool_id=None,
-        headers=None,
-        block_till_cluster_ready: bool = True,
-        write_db_credentials: bool = True,
-        extra_pip_installs: Optional[List[str]] = None,
+    databricks_host: str,
+    databricks_token: str,
+    medical_nlp,
+    spark_nlp,
+    visual,
+    install_suite: InstallSuite = None,
+    num_workers=1,
+    cluster_name=settings.db_cluster_name,
+    node_type_id=settings.db_node_type_id,
+    driver_node_type_id=settings.db_driver_node_type,
+    spark_env_vars=None,
+    autotermination_minutes=60,
+    spark_version=settings.db_spark_version,
+    spark_conf=None,
+    auto_scale=None,
+    aws_attributes=None,
+    ssh_public_keys=None,
+    custom_tags=None,
+    cluster_log_conf=None,
+    enable_elastic_disk=None,
+    cluster_source=None,
+    instance_pool_id=None,
+    headers=None,
+    block_till_cluster_ready: bool = True,
+    write_db_credentials: bool = True,
+    extra_pip_installs: Optional[List[str]] = None,
 ) -> str:
     db = get_db_client_for_token(databricks_host, databricks_token)
 
     if not install_suite:
         install_suite = jsl_home.get_install_suite_from_jsl_home()
 
     install_license_to_cluster(install_suite, db)
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/marketplace.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/marketplace.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/marketplace_offering.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/marketplace_offering.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/emr/install_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/emr/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/emr/utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/emr/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/emr/work_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/emr/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/glue/install_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/glue/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/glue/utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/glue/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/endpoint_test.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/endpoint_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/generate_test.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/generate_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/install_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from johnsnowlabs import settings
 from johnsnowlabs.auto_install.databricks.dbfs import dbfs_rm
 from johnsnowlabs.auto_install.databricks.install_utils import (
     create_cluster,
     get_db_client_for_token,
     install_jsl_suite_to_cluster,
-    install_list_of_pypi_ref_to_cluster, install_to_existing_cluster,
+    install_list_of_pypi_ref_to_cluster,
 )
 from johnsnowlabs.auto_install.emr.install_utils import create_emr_cluster
 from johnsnowlabs.auto_install.glue.install_utils import (
     create_glue_bucket,
     upload_pylibs_jars_to_glue_bucket,
 )
 from johnsnowlabs.auto_install.glue.utils import get_printable_glue_notebook_commands
@@ -228,72 +228,72 @@
             visual=visual,
             spark_nlp=spark_nlp,
             enterpise_nlp=nlp,
         )
 
 
 def install_to_databricks(
-        # -- JSL-Auth Flows --
-        # Browser Auth
-        browser_login: bool = True,
-        force_browser: bool = False,
-        # JWT Token Auth
-        access_token: Optional[str] = None,
-        # JSON file Auth
-        json_license_path: Optional[str] = None,
-        # Manual License specification Auth
-        med_license: Optional[str] = None,
-        enterprise_nlp_secret: Optional[str] = None,
-        ocr_secret: Optional[str] = None,
-        ocr_license: Optional[str] = None,
-        fin_license: Optional[str] = None,
-        leg_license: Optional[str] = None,
-        aws_access_key: Optional[str] = None,
-        aws_key_id: Optional[str] = None,
-        # -- Databricks auth flows & Install Target --
-        databricks_cluster_id: Optional[str] = None,
-        databricks_token: Optional[str] = None,
-        databricks_host: Optional[str] = None,
-        databricks_password: Optional[str] = None,
-        databricks_email: Optional[str] = None,
-        # -- Install Params --
-        product: Optional[str] = ProductName.jsl_full.value,
-        nlp: bool = True,
-        spark_nlp: bool = True,
-        visual: bool = False,
-        # License usage & Caching
-        local_license_number: int = 0,
-        remote_license_number: int = 0,
-        store_in_jsl_home: bool = True,
-        # Install File Types
-        hardware_platform: str = JvmHardwareTarget.cpu.value,
-        py_install_type: str = PyInstallTypes.wheel.value,
-        refresh_install: bool = False,
-        # -- Databricks Cluster Creation Params --
-        block_till_cluster_ready=True,
-        num_workers=1,
-        cluster_name=settings.db_cluster_name,
-        node_type_id=settings.db_node_type_id,
-        driver_node_type_id=settings.db_driver_node_type,
-        spark_env_vars=None,
-        autotermination_minutes=60,
-        spark_version=settings.db_spark_version,
-        spark_conf=None,
-        auto_scale=None,
-        aws_attributes=None,
-        ssh_public_keys=None,
-        custom_tags=None,
-        cluster_log_conf=None,
-        enable_elastic_disk=None,
-        cluster_source=None,
-        instance_pool_id=None,
-        headers=None,
-        clean_cluster=True,
-        write_db_credentials=True,
-        extra_pip_installs: Optional[List[str]] = None,
+    # -- JSL-Auth Flows --
+    # Browser Auth
+    browser_login: bool = True,
+    force_browser: bool = False,
+    # JWT Token Auth
+    access_token: Optional[str] = None,
+    # JSON file Auth
+    json_license_path: Optional[str] = None,
+    # Manual License specification Auth
+    med_license: Optional[str] = None,
+    enterprise_nlp_secret: Optional[str] = None,
+    ocr_secret: Optional[str] = None,
+    ocr_license: Optional[str] = None,
+    fin_license: Optional[str] = None,
+    leg_license: Optional[str] = None,
+    aws_access_key: Optional[str] = None,
+    aws_key_id: Optional[str] = None,
+    # -- Databricks auth flows & Install Target --
+    databricks_cluster_id: Optional[str] = None,
+    databricks_token: Optional[str] = None,
+    databricks_host: Optional[str] = None,
+    databricks_password: Optional[str] = None,
+    databricks_email: Optional[str] = None,
+    # -- Install Params --
+    product: Optional[str] = ProductName.jsl_full.value,
+    nlp: bool = True,
+    spark_nlp: bool = True,
+    visual: bool = False,
+    # License usage & Caching
+    local_license_number: int = 0,
+    remote_license_number: int = 0,
+    store_in_jsl_home: bool = True,
+    # Install File Types
+    hardware_platform: str = JvmHardwareTarget.cpu.value,
+    py_install_type: str = PyInstallTypes.wheel.value,
+    refresh_install: bool = False,
+    # -- Databricks Cluster Creation Params --
+    block_till_cluster_ready=True,
+    num_workers=1,
+    cluster_name=settings.db_cluster_name,
+    node_type_id=settings.db_node_type_id,
+    driver_node_type_id=settings.db_driver_node_type,
+    spark_env_vars=None,
+    autotermination_minutes=60,
+    spark_version=settings.db_spark_version,
+    spark_conf=None,
+    auto_scale=None,
+    aws_attributes=None,
+    ssh_public_keys=None,
+    custom_tags=None,
+    cluster_log_conf=None,
+    enable_elastic_disk=None,
+    cluster_source=None,
+    instance_pool_id=None,
+    headers=None,
+    clean_cluster=True,
+    write_db_credentials=True,
+    extra_pip_installs: Optional[List[str]] = None,
 ):
     if refresh_install and os.path.exists(settings.root_dir):
         print("🧹 Cleaning up old JSL Home in ", settings.root_dir)
         shutil.rmtree(settings.root_dir)
     if clean_cluster and databricks_host:
         dbfs_rm(
             get_db_client_for_token(databricks_host, databricks_token),
@@ -336,33 +336,38 @@
             visual=visual,
             nlp=nlp,
             spark_nlp=spark_nlp,
         )
 
     # Databricks Install
     if not databricks_host and databricks_token:
-        raise Exception('databricks_host and databricks_token must be specified.')
+        raise Exception()
     suite = get_install_suite_from_jsl_home(
         jvm_hardware_target=hardware_platform,
         visual=visual,
         nlp=nlp,
         spark_nlp=spark_nlp,
     )
     if databricks_cluster_id:
-        # Install to existing cluster. Licenses, P4j and relevant directories
-        install_to_existing_cluster(
+        # Install to existing cluster
+        install_jsl_suite_to_cluster(
+            db=get_db_client_for_token(databricks_host, databricks_token),
             install_suite=suite,
-            databricks_cluster_id=databricks_cluster_id,
+            cluster_id=databricks_cluster_id,
             medical_nlp=nlp,
             spark_nlp=spark_nlp,
             visual=visual,
-            databricks_host=databricks_host,
-            databricks_token=databricks_token,
-            extra_pip_installs=extra_pip_installs,
         )
+        if extra_pip_installs:
+            install_list_of_pypi_ref_to_cluster(
+                db=get_db_client_for_token(databricks_host, databricks_token),
+                cluster_id=databricks_cluster_id,
+                pip_installs=extra_pip_installs,
+            )
+
     else:
         # Create new cluster
         return create_cluster(
             medical_nlp=nlp,
             spark_nlp=spark_nlp,
             visual=visual,
             databricks_host=databricks_host,
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/finance.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/finance.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/embedding_retrieval/__init__.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/embedding_retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/frameworks/embedding_retrieval/utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/frameworks/embedding_retrieval/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/legal.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/legal.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/medical.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/medical.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/nlp.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/nlp.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,20 @@
     install,
     install_to_emr,
     install_to_glue,
     install_to_databricks,
 )
 from .utils.sparksession_utils import start
 
+from johnsnowlabs.auto_install.docker.work_utils import (
+    build_image,
+    serve_container,
+)
+
+
 if try_import_lib("sparknlp"):
     import sparknlp
     from sparknlp import annotation
     from sparknlp.annotator import *
     from sparknlp.base import *
     from sparknlp.functions import *
     from sparknlp.pretrained import PretrainedPipeline, ResourceDownloader
@@ -48,7 +54,11 @@
     import warnings
 
     warnings.filterwarnings("ignore")
 
 if try_import_lib("nlu"):
     import nlu as nlu
     from nlu import autocomplete_pipeline, load, to_nlu_pipe, to_pretty_df
+
+
+
+
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/settings.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     set_py4j_logger_to_error_on_databricks,
 )
 
 # These versions are used for auto-installs and version  checks
 
 
 
-raw_version_jsl_lib = "5.3.3rc2"
+raw_version_jsl_lib = "5.3.3rc3"
 
 
 raw_version_nlp = "5.3.1"
 
-raw_version_nlu = "5.3.1rc3"
+raw_version_nlu = "5.3.0"
 
 
 raw_version_pyspark = "3.4.0"
 raw_version_nlp_display = "5.0"
 
 raw_version_medical = "5.3.0"
 raw_version_secret_medical = "5.3.0"
@@ -68,17 +68,14 @@
 py_info_file = os.path.join(py_dir, "info.json")
 creds_info_file = os.path.join(license_dir, "info.json")
 
 # databricks paths
 dbfs_home_dir = "dbfs:/johnsnowlabs"
 dbfs_java_dir = f"{dbfs_home_dir}/java_installs"
 dbfs_py_dir = f"{dbfs_home_dir}/py_installs"
-# dbfs_license_path = "/johnsnowlabs/license.json"
-dbfs_license_path = f"{dbfs_home_dir}/license.json"
-dbfs_info_path = f"{dbfs_home_dir}/info.json"
 db_py_jobs_dir = f"{dbfs_home_dir}/py_jobs"
 db_py_notebook_dir = f"{dbfs_home_dir}/py_notebook_jobs"
 db_jar_jobs_dir = f"{dbfs_home_dir}/jar_jobs"
 
 db_cluster_name = "John-Snow-Labs-Databricks-Auto-Cluster🚀"
 db_driver_node_type = "i3.xlarge"
 db_node_type_id = "i3.xlarge"
@@ -99,7 +96,12 @@
 emr_default_instance_profile = "EMR_EC2_DefaultRole"
 emr_default_service_role = "EMR_DefaultRole"
 emr_volume_size = 100
 
 # Local Spark mode
 spark_session_name = "John-Snow-Labs-Spark-Session 🚀"
 
+
+### Docker Settings
+
+docker_image_name = "johnsnowlabs_image"
+docker_container_name = "johnsnowlabs_container"
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/boto_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/boto_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/enums.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/env_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ast
 import importlib
+import inspect
 import os
 import site
 import subprocess
 from typing import List
 
 logged_imports = []
 
@@ -135,7 +136,17 @@
 
         from pyspark.sql import SparkSession
 
         logger = SparkSession.builder.getOrCreate()._jvm.org.apache.log4j
         logging.getLogger("py4j.java_gateway").setLevel(logging.ERROR)
     except:
         pass
+
+
+def get_folder_of_func(func):
+    # Get the file path where the function is defined
+    func_file = inspect.getfile(func)
+
+    # Get the directory name from the file path
+    func_dir = os.path.dirname(func_file)
+
+    return func_dir
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/functional.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/py_process.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/py_process.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,74 @@
 import subprocess
 import sys
 from pathlib import Path
 from typing import List, Callable
 
 import colorama
 import pandas as pd
-from sparknlp.pretrained import PretrainedPipeline
 
 import johnsnowlabs.utils.testing.test_settings
 from johnsnowlabs.utils.file_utils import str_to_file
 
 Path(johnsnowlabs.utils.testing.test_settings.tmp_markdown_dir).mkdir(
     exist_ok=True, parents=True
 )
 
 
 def run_cmd_and_check_succ(
     args: List[str],
     log=True,
     suc_print=johnsnowlabs.utils.testing.test_settings.success_worker_print,
     return_pipes=False,
+    shell=False,
+    raise_on_fail=False,
+    use_code=False,
 ) -> bool:
-    print(f"👷 Executing {colorama.Fore.LIGHTGREEN_EX}{args}{colorama.Fore.RESET}")
-    r = subprocess.run(args, capture_output=True)
-    was_suc = process_was_suc(r)
-    if was_suc:
-        print(
-            f"{colorama.Fore.LIGHTGREEN_EX}✅ Success running {args}{colorama.Fore.RESET}"
-        )
-    else:
-        print(
-            f"{colorama.Fore.LIGHTRED_EX}❌ Failure running {args}{colorama.Fore.LIGHTGREEN_EX}"
-        )
+    if log:
+        if len(args) == 1:
+            print(
+                f"👷 Executing {colorama.Fore.LIGHTGREEN_EX}{args[0]}{colorama.Fore.RESET}"
+            )
+        else:
+            print(
+                f"👷 Executing {colorama.Fore.LIGHTGREEN_EX}{args}{colorama.Fore.RESET}"
+            )
+
+    r = subprocess.run(args, capture_output=True, shell=shell)
+    was_suc = process_was_suc(r, suc_print=suc_print, use_code=use_code)
+    if log:
+        if was_suc:
+            print(
+                f"{colorama.Fore.LIGHTGREEN_EX}✅ Success running {args}{colorama.Fore.RESET}"
+            )
+        else:
+            print(
+                f"{colorama.Fore.LIGHTRED_EX}❌ Failure running {args}{colorama.Fore.LIGHTGREEN_EX}"
+            )
+
     if log:
         log_process(r)
+    if raise_on_fail and not was_suc:
+        raise ValueError(f"Failed running {args}")
     if return_pipes:
         return was_suc, r
     return was_suc
 
 
 def process_was_suc(
     result: subprocess.CompletedProcess,
     suc_print=johnsnowlabs.utils.testing.test_settings.success_worker_print,
+    use_code=False,
 ) -> bool:
-    return suc_print in result.stdout.decode()
+    if use_code and result.returncode != 0:
+        return False
+    elif use_code and result.returncode == 0:
+        return True
+    else:
+        return suc_print in result.stdout.decode()
 
 
 def log_process(result: subprocess.CompletedProcess):
     print("______________STDOUT:")
     print(result.stdout.decode())
     print("______________STDERR:")
     print(result.stderr.decode())
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/s3_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs/visual.py` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs_for_databricks.egg-info/PKG-INFO` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs_for_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs-for-databricks
-Version: 5.3.3rc2
+Version: 5.3.3rc3
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 License: UNKNOWN
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Platform: UNKNOWN
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/johnsnowlabs_for_databricks.egg-info/SOURCES.txt` & `johnsnowlabs_for_databricks-5.3.3rc3/johnsnowlabs_for_databricks.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 johnsnowlabs/__init__.py
 johnsnowlabs/finance.py
 johnsnowlabs/lab.py
 johnsnowlabs/legal.py
 johnsnowlabs/llm.py
 johnsnowlabs/medical.py
 johnsnowlabs/nlp.py
+johnsnowlabs/serve.py
 johnsnowlabs/settings.py
 johnsnowlabs/visual.py
 johnsnowlabs/viz.py
 johnsnowlabs/abstract_base/__init__.py
 johnsnowlabs/abstract_base/base_enum.py
 johnsnowlabs/abstract_base/lib_resolver.py
 johnsnowlabs/abstract_base/pydantic_model.py
@@ -34,14 +35,21 @@
 johnsnowlabs/auto_install/databricks/__init__.py
 johnsnowlabs/auto_install/databricks/dbfs.py
 johnsnowlabs/auto_install/databricks/endpoints.py
 johnsnowlabs/auto_install/databricks/install_utils.py
 johnsnowlabs/auto_install/databricks/marketplace.py
 johnsnowlabs/auto_install/databricks/marketplace_offering.py
 johnsnowlabs/auto_install/databricks/work_utils.py
+johnsnowlabs/auto_install/docker/__init__.py
+johnsnowlabs/auto_install/docker/docker_template.py
+johnsnowlabs/auto_install/docker/work_utils.py
+johnsnowlabs/auto_install/docker/build/__init__.py
+johnsnowlabs/auto_install/docker/build/app.py
+johnsnowlabs/auto_install/docker/build/installer.py
+johnsnowlabs/auto_install/docker/build/test_qucik.py
 johnsnowlabs/auto_install/emr/__init__.py
 johnsnowlabs/auto_install/emr/enums.py
 johnsnowlabs/auto_install/emr/install_utils.py
 johnsnowlabs/auto_install/emr/utils.py
 johnsnowlabs/auto_install/emr/work_utils.py
 johnsnowlabs/auto_install/glue/__init__.py
 johnsnowlabs/auto_install/glue/install_utils.py
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/notebooks/create_databricks_cluster.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/notebooks/create_databricks_cluster.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/notebooks/create_emr_cluster.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/notebooks/create_emr_cluster.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/notebooks/databricks_endpoints_tutorial.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/notebooks/databricks_endpoints_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/notebooks/databricks_model_marketplace.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/notebooks/databricks_model_marketplace.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/notebooks/haystack_with_johnsnowlabs.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/notebooks/haystack_with_johnsnowlabs.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/notebooks/langchain_with_johnsnowlabs.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/notebooks/langchain_with_johnsnowlabs.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/notebooks/parameterized_nb_example.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/notebooks/parameterized_nb_example.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/notebooks/setup_glue_notebook.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/notebooks/setup_glue_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/setup_johnsnowlabs.py` & `johnsnowlabs_for_databricks-5.3.3rc3/setup_johnsnowlabs_for_databricks.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 REQUIRED_PKGS = [
-    f"pyspark=={johnsnowlabs.settings.raw_version_pyspark}",
     f"spark-nlp=={johnsnowlabs.settings.raw_version_nlp}",
     f"nlu=={johnsnowlabs.settings.raw_version_nlu}",
     f"spark-nlp-display=={johnsnowlabs.settings.raw_version_nlp_display}",
     "numpy",
     "dataclasses",
     "requests",
     "databricks-api",
     f"pydantic=={johnsnowlabs.settings.raw_version_pydantic}",
     "colorama",
     "boto3",
 ]
 
 setup(
     version=johnsnowlabs.settings.raw_version_jsl_lib,
-    name="johnsnowlabs",
+    name="johnsnowlabs_for_databricks",
     description="The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for "
     "Finance, Legal and Medical domains. Easily scalable to Spark Cluster ",
     long_description=long_description,
     install_requires=REQUIRED_PKGS,
     long_description_content_type="text/markdown",
     url="https://www.johnsnowlabs.com/",
     author="John Snow Labs",
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/setup_johnsnowlabs_for_databricks.py` & `johnsnowlabs_for_databricks-5.3.3rc3/setup_johnsnowlabs.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 REQUIRED_PKGS = [
+    f"pyspark=={johnsnowlabs.settings.raw_version_pyspark}",
     f"spark-nlp=={johnsnowlabs.settings.raw_version_nlp}",
     f"nlu=={johnsnowlabs.settings.raw_version_nlu}",
     f"spark-nlp-display=={johnsnowlabs.settings.raw_version_nlp_display}",
     "numpy",
     "dataclasses",
     "requests",
     "databricks-api",
     f"pydantic=={johnsnowlabs.settings.raw_version_pydantic}",
     "colorama",
     "boto3",
 ]
 
 setup(
     version=johnsnowlabs.settings.raw_version_jsl_lib,
-    name="johnsnowlabs_for_databricks",
+    name="johnsnowlabs",
     description="The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for "
     "Finance, Legal and Medical domains. Easily scalable to Spark Cluster ",
     long_description=long_description,
     install_requires=REQUIRED_PKGS,
     long_description_content_type="text/markdown",
     url="https://www.johnsnowlabs.com/",
     author="John Snow Labs",
@@ -45,8 +46,11 @@
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
     ],
     keywords="Spark NLP OCR Finance Legal Medical John Snow Labs  ",
     packages=find_packages(exclude=["test*", "tmp*"]),  # exclude=['test']
     include_package_data=True,
+    data_files=[("/johnsnowlabs/auto_install/docker/build",
+                 ["./johnsnowlabs/auto_install/docker/build/base_dockerfile"])],
+
 )
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/auto_install.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/auto_install.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 
 class AutoInstallTestCase(unittest.TestCase):
     venv_creation_dir = "/home/ckl/old_home/ckl/Documents/freelance/johnsnowlabs_lib/tmp/venv/tmp_test_venv"
     zip_dir = "/home/ckl/Documents/freelance/jsl/johnsnowlabs/tmp/offline"
 
 
     def test_install_to_current_env_browser_pop_up(self):
-        nlp.install(force_browser=False, visual=True, remote_license_number=2)
-
+        nlp.install(browser_login=False,visual=True)
 
     def test_install_pr_secret(self):
         settings.enforce_versions = False
         nlp.install(enterprise_nlp_secret=secrets.pr_secret)
 
     def test_install_to_current_env(self):
         settings.enforce_versions = False
-        nlp.install(json_license_path=sct.old_lic, refresh_install=True)
+        nlp.install(json_license_path='/home/ckl/Documents/freelance/jsl/endpoints/endpoints/creds/license_airgap.json', refresh_install=True)
         # import sparknlp
 
     def test_install_to_different_python_env(self):
         # Install to env which is not the one we are currently running
         os.system(f"rm -r {self.venv_creation_dir} ")
         f = "/home/ckl/old_home/ckl/Documents/freelance/johnsnowlabs_lib/tmp/licenses/ocr_40.json"
         VenvWrapper.create_venv(self.venv_creation_dir)
@@ -95,30 +94,34 @@
         new_secret = secrets.random_secret
         from johnsnowlabs import settings
 
         settings.enforce_versions = False
         nlp.install(enterprise_nlp_secret=new_secret)
 
     def test_json_license_install(self):
-        # nlp.install(json_license_path=sct.latest_lic,visual=True)
-        nlp.install(json_license_path='/home/ckl/Documents/freelance/jsl/johnsnowlabs_latest_2024/tests/lic.json',visual=True)
+        nlp.install(json_license_path=sct.latest_lic,visual=True)
 
 
     def test_json_license_install_outdated(self):
         nlp.settings.enforce_versions = False
         nlp.install(json_license_path=sct.old_lic)
 
 
     def test_create_and_install_cluster(self):
         install_suite = get_install_suite_from_jsl_home()
         print(install_suite)
 
     def test_uninstall_all(self):
-        os.system(f"{sys.executable} -m pip uninstall spark-nlp-jsl -y")
-        os.system(f"{sys.executable} -m pip uninstall spark-ocr -y")
+        # os.system(old_lic'{sys.py_executable} -py_executable pip uninstall spark-nlp -y')
+        # os.system(old_lic'{sys.py_executable} -py_executable pip uninstall spark-nlp-display -y')
+        # os.system(old_lic'{sys.py_executable} -py_executable pip uninstall nlu -y')
+
+        # os.system(f"{sys.executable} -m pip uninstall spark-nlp-jsl -y")
+        # os.system(f"{sys.executable} -m pip uninstall spark-ocr -y")
+        # os.system(old_lic'{sys.py_executable} -py_executable pip uninstall jsl_tmp -y')
         os.system(f"{sys.executable} -m pip uninstall spark-nlp-internal -y")
 
     def test_install_to_emr(self):
         # Make sure correct aws credentials are configured
         nlp.install_to_emr(
             "us-east-1",
             bootstrap_bucket="ksh-emr-bucket",
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/backward_compat.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/backward_compat.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/db_infos_test.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/db_infos_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/db_test_utils.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/db_test_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/endpoint_tests.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/hdfs_tests.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/hdfs_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/install_tests.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/install_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             parameters=[arg1, arg2],
         )
     )
 
 
 
 
-# @db_marketplace_cloud_node_params
+@db_marketplace_cloud_node_params
 def test_install_to_existing_cluster(creds, node_type):
     lic, host, token = creds
     print(lic, host, token)
     # Create a cluster with no installs
     db = DatabricksAPI(host=host, token=token)
     cluster_id = db.cluster.create_cluster(
         driver_node_type_id=node_type,
```

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/parameterized_nb_example.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/parameterized_nb_example.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/sample.ipynb` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/sample.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/databricks/submit_tests.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/databricks/submit_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/file_models.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/file_models.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/install.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/jsl_dependency_resolver.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/jsl_dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/jsl_secrets.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/llm_frameworks/test_haystack.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/llm_frameworks/test_haystack.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/llm_frameworks/test_langchain.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/llm_frameworks/test_langchain.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/markdown_tests.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/markdown_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/notebook_tests.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/notebook_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/spark_session.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/spark_session.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs_for_databricks-5.3.3rc2/tests/venv_wrapper_tests.py` & `johnsnowlabs_for_databricks-5.3.3rc3/tests/venv_wrapper_tests.py`

 * *Files identical despite different names*

