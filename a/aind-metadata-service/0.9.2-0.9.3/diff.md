# Comparing `tmp/aind_metadata_service-0.9.2.tar.gz` & `tmp/aind_metadata_service-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.9.2.tar", last modified: Fri Feb 16 22:56:15 2024, max compression
+gzip compressed data, was "aind_metadata_service-0.9.3.tar", last modified: Mon Feb 19 17:30:29 2024, max compression
```

## Comparing `aind_metadata_service-0.9.2.tar` & `aind_metadata_service-0.9.3.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.752637 aind_metadata_service-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.720637 aind_metadata_service-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.728637 aind_metadata_service-0.9.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.728637 aind_metadata_service-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-02-16 22:56:15.752637 aind_metadata_service-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.728637 aind_metadata_service-0.9.2/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.728637 aind_metadata_service-0.9.2/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 22:56:15.752637 aind_metadata_service-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.720637 aind_metadata_service-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.728637 aind_metadata_service-0.9.2/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.728637 aind_metadata_service-0.9.2/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.732637 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.732637 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70192 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    41586 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2019/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.732637 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   148119 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    74601 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2023/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.732637 aind_metadata_service-0.9.2/src/aind_metadata_service/slims/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/slims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/slims/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/slims/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.732637 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.732637 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/funding/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/funding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/funding/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/funding/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.732637 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/perfusions/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/perfusions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/perfusions/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/perfusions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.736636 aind_metadata_service-0.9.2/src/aind_metadata_service/tars/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/tars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/tars/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/src/aind_metadata_service/tars/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.748637 aind_metadata_service-0.9.2/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-02-16 22:56:15.000000 aind_metadata_service-0.9.2/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-02-16 22:56:15.000000 aind_metadata_service-0.9.2/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 22:56:15.000000 aind_metadata_service-0.9.2/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-16 22:56:15.000000 aind_metadata_service-0.9.2/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-16 22:56:15.000000 aind_metadata_service-0.9.2/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.736636 aind_metadata_service-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.736636 aind_metadata_service-0.9.2/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15915 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.724637 aind_metadata_service-0.9.2/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.736636 aind_metadata_service-0.9.2/tests/resources/json_responses/
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/json_responses/combined.json
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/json_responses/combined_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/json_responses/mapped_las_procedure.json
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/json_responses/mapped_las_procedure_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/json_responses/mapped_sp_procedure.json
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/json_responses/mapped_sp_procedure_invalid.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.724637 aind_metadata_service-0.9.2/tests/resources/sharepoint/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.736636 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.740636 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item19.json
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item20.json
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/nsb2019_string_entries.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.740636 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item19.json
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item20.json
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.740636 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.744636 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
--rw-r--r--   0 runner    (1001) docker     (127)     7510 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item18.json
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item19.json
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item20.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item21.json
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item22.json
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
--rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/nsb2023_string_entries.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.744636 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item18.json
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item19.json
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item20.json
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item21.json
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item22.json
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.744636 aind_metadata_service-0.9.2/tests/resources/slims/
--rw-r--r--   0 runner    (1001) docker     (127)    26365 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/slims/json_entity.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.744636 aind_metadata_service-0.9.2/tests/resources/smartsheet/
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/smartsheet/test_funding_sheet.json
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/smartsheet/test_perfusions_sheet.json
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/resources/smartsheet/test_sheet.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.744636 aind_metadata_service-0.9.2/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.748637 aind_metadata_service-0.9.2/tests/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/nsb2019/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/nsb2019/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/nsb2019/test_string_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.748637 aind_metadata_service-0.9.2/tests/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/nsb2023/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/nsb2023/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/nsb2023/test_string_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22331 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/sharepoint/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.748637 aind_metadata_service-0.9.2/tests/slims/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/slims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/slims/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/slims/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.748637 aind_metadata_service-0.9.2/tests/smartsheet/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/smartsheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/smartsheet/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/smartsheet/test_funding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/smartsheet/test_perfusions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:56:15.748637 aind_metadata_service-0.9.2/tests/tars/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/tars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/tars/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/tars/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-02-16 22:56:02.000000 aind_metadata_service-0.9.2/tests/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.212885 aind_metadata_service-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.176885 aind_metadata_service-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.184885 aind_metadata_service-0.9.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.184885 aind_metadata_service-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-02-19 17:30:29.212885 aind_metadata_service-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.184885 aind_metadata_service-0.9.3/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.184885 aind_metadata_service-0.9.3/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 17:30:29.212885 aind_metadata_service-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.176885 aind_metadata_service-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.184885 aind_metadata_service-0.9.3/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.188885 aind_metadata_service-0.9.3/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17372 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.188885 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.188885 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70192 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41586 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2019/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.188885 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148145 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74601 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2023/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.188885 aind_metadata_service-0.9.3/src/aind_metadata_service/slims/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/slims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/slims/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/slims/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.192885 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.192885 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/funding/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/funding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/funding/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/funding/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.192885 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/perfusions/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/perfusions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/perfusions/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/perfusions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.192885 aind_metadata_service-0.9.3/src/aind_metadata_service/tars/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/tars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/tars/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/src/aind_metadata_service/tars/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.208885 aind_metadata_service-0.9.3/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-02-19 17:30:29.000000 aind_metadata_service-0.9.3/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-02-19 17:30:29.000000 aind_metadata_service-0.9.3/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 17:30:29.000000 aind_metadata_service-0.9.3/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-19 17:30:29.000000 aind_metadata_service-0.9.3/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-19 17:30:29.000000 aind_metadata_service-0.9.3/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.192885 aind_metadata_service-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.192885 aind_metadata_service-0.9.3/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15915 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.180885 aind_metadata_service-0.9.3/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.196885 aind_metadata_service-0.9.3/tests/resources/json_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/json_responses/combined.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/json_responses/combined_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/json_responses/mapped_las_procedure.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/json_responses/mapped_las_procedure_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/json_responses/mapped_sp_procedure.json
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/json_responses/mapped_sp_procedure_invalid.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.180885 aind_metadata_service-0.9.3/tests/resources/sharepoint/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.196885 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.196885 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item20.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/nsb2019_string_entries.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.200885 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item20.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.200885 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.200885 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7510 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item18.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item20.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item21.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item22.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/nsb2023_string_entries.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.204885 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item18.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item20.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item21.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item22.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.204885 aind_metadata_service-0.9.3/tests/resources/slims/
+-rw-r--r--   0 runner    (1001) docker     (127)    26365 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/slims/json_entity.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.204885 aind_metadata_service-0.9.3/tests/resources/smartsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/smartsheet/test_funding_sheet.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/smartsheet/test_perfusions_sheet.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/resources/smartsheet/test_sheet.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.204885 aind_metadata_service-0.9.3/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.204885 aind_metadata_service-0.9.3/tests/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/nsb2019/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/nsb2019/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/nsb2019/test_string_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.208885 aind_metadata_service-0.9.3/tests/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/nsb2023/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/nsb2023/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/nsb2023/test_string_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/sharepoint/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.208885 aind_metadata_service-0.9.3/tests/slims/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/slims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/slims/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/slims/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.208885 aind_metadata_service-0.9.3/tests/smartsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/smartsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/smartsheet/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/smartsheet/test_funding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/smartsheet/test_perfusions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 17:30:29.208885 aind_metadata_service-0.9.3/tests/tars/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/tars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/tars/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14043 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/tars/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-02-19 17:30:16.000000 aind_metadata_service-0.9.3/tests/test_response_handler.py
```

### Comparing `aind_metadata_service-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.9.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/.github/workflows/ci.yml` & `aind_metadata_service-0.9.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/.github/workflows/publish.yml` & `aind_metadata_service-0.9.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/.gitignore` & `aind_metadata_service-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/Dockerfile` & `aind_metadata_service-0.9.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/LICENSE` & `aind_metadata_service-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/PKG-INFO` & `aind_metadata_service-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.9.2
+Version: 0.9.3
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_service-0.9.2/README.md` & `aind_metadata_service-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/doc_template/Makefile` & `aind_metadata_service-0.9.3/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/doc_template/make.bat` & `aind_metadata_service-0.9.3/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.9.3/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/doc_template/source/conf.py` & `aind_metadata_service-0.9.3/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/pyproject.toml` & `aind_metadata_service-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/client.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         domain : str
           url of the domain
         """
 
         self.domain = domain
         self.subject_url = f"{self.domain}/subject"
         self.procedures_url = f"{self.domain}/procedures"
+        self.injection_materials_url = f"{self.domain}/injection_materials"
 
     def get_subject(
         self, subject_id: str, pickle: bool = False
     ) -> requests.Response:
         """
         Retrieve a subject response from the server
         Parameters
```

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/labtracks/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
             columns = [column[0].lower() for column in column_names]
             fetched_rows = cursor.fetchall()
             cursor.close()
             self.close_session(session)
             results = []
             for row in fetched_rows:
                 results.append(dict(zip(columns, row)))
+            # TODO: return results
             lth = LabTracksResponseHandler()
             procedures = lth.map_response_to_procedures(
                 subject_id=subject_id, results=results
             )
             procedures = [] if procedures is None else [procedures]
             return ModelResponse(
                 aind_models=procedures, status_code=StatusCodes.DB_RESPONDED
```

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/response_handler.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/server.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,44 +20,34 @@
     SmartsheetSettings,
 )
 from aind_metadata_service.smartsheet.funding.mapping import FundingMapper
 from aind_metadata_service.smartsheet.perfusions.mapping import (
     PerfusionsMapper,
 )
 from aind_metadata_service.tars.client import AzureSettings, TarsClient
+from aind_metadata_service.tars.mapping import TarsResponseHandler
 
 SMARTSHEET_FUNDING_ID = os.getenv("SMARTSHEET_FUNDING_ID")
 SMARTSHEET_FUNDING_TOKEN = os.getenv("SMARTSHEET_FUNDING_TOKEN")
 
 SMARTSHEET_PERFUSIONS_ID = os.getenv("SMARTSHEET_PERFUSIONS_ID")
 SMARTSHEET_PERFUSIONS_TOKEN = os.getenv("SMARTSHEET_PERFUSIONS_TOKEN")
 
-TARS_TENANT_ID = os.getenv("TARS_TENANT_ID")
-TARS_CLIENT_ID = os.getenv("TARS_CLIENT_ID")
-TARS_CLIENT_SECRET = os.getenv("TARS_CLIENT_SECRET")
-TARS_SCOPE = os.getenv("TARS_SCOPE")
-TARS_RESOURCE = os.getenv("TARS_RESOURCE")
 
 # TODO: Move client instantiation when the server starts instead of creating
 #  one for each request?
 sharepoint_settings = SharepointSettings()
 labtracks_settings = LabTracksSettings()
 funding_smartsheet_settings = SmartsheetSettings(
     access_token=SMARTSHEET_FUNDING_TOKEN, sheet_id=SMARTSHEET_FUNDING_ID
 )
 perfusions_smartsheet_settings = SmartsheetSettings(
     access_token=SMARTSHEET_PERFUSIONS_TOKEN, sheet_id=SMARTSHEET_PERFUSIONS_ID
 )
-tars_settings = AzureSettings(
-    tenant_id=TARS_TENANT_ID,
-    client_id=TARS_CLIENT_ID,
-    client_secret=TARS_CLIENT_SECRET,
-    scope=TARS_SCOPE,
-    resource=TARS_RESOURCE,
-)
+tars_settings = AzureSettings()
 
 
 app = FastAPI()
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
@@ -72,14 +62,16 @@
     smartsheet_settings=perfusions_smartsheet_settings
 )
 
 funding_smart_sheet_client = SmartSheetClient(
     smartsheet_settings=funding_smartsheet_settings
 )
 
+tars_client = TarsClient(azure_settings=tars_settings)
+
 
 @app.get("/perfusions/{subject_id}")
 async def retrieve_perfusions(subject_id, pickle: bool = False):
     """Retrieves perfusion information from smartsheet"""
 
     # TODO: We can probably cache the response if it's 200
     smart_sheet_response = await run_in_threadpool(
@@ -132,19 +124,19 @@
 
 @app.get("/tars_injection_materials/{prep_lot_number}")
 async def retrieve_injection_materials(prep_lot_number, pickle: bool = False):
     """
     Retrieves injection materials from TARS server
     Returns pickled data if URL parameter pickle=True, else returns json
     """
-    tars_client = TarsClient(azure_settings=tars_settings)
     model_response = await run_in_threadpool(
         tars_client.get_injection_materials_info,
         prep_lot_number=prep_lot_number,
     )
+    # TODO: move molecules call to here
     if pickle:
         return model_response.map_to_pickled_response()
     else:
         return model_response.map_to_json_response()
 
 
 @app.get("/procedures/{subject_id}")
@@ -167,18 +159,29 @@
         sharepoint_client.get_procedure_info,
         subject_id=subject_id,
         list_title=sharepoint_settings.nsb_2023_list,
     )
     merged_response = sharepoint_client.merge_responses(
         [lb_response, sp2019_response, sp2023_response]
     )
+    mapper = TarsResponseHandler()
+    viruses = mapper.get_virus_strains(merged_response)
+    tars_mapping = {}
+    for virus_strain in viruses:
+        tars_response = await retrieve_injection_materials(
+            prep_lot_number=virus_strain
+        )
+        tars_mapping[virus_strain] = tars_response
+    integrated_response = mapper.integrate_injection_materials(
+        response=merged_response, tars_mapping=tars_mapping
+    )
     if pickle:
-        return merged_response.map_to_pickled_response()
+        return integrated_response.map_to_pickled_response()
     else:
-        return merged_response.map_to_json_response()
+        return integrated_response.map_to_json_response()
 
 
 @app.get(
     "/favicon.ico",
     include_in_schema=False,
     response_class=RedirectResponse,
     status_code=200,
```

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/client.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2019/mapping.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2019/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2019/models.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2019/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2019/procedures.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2019/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2023/mapping.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2023/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,18 +250,18 @@
 
     @staticmethod
     def _parse_datetime_to_date(dt: Optional[datetime]) -> Optional[date]:
         """Parse date from datetime"""
         return None if dt is None else dt.date()
 
     @staticmethod
-    def _parse_virus_strain_str(_: Optional[str]) -> Optional[str]:
+    def _parse_virus_strain_str(virus_strain_str: Optional[str]) -> Optional[str]:
         """Parse virus strain strings"""
-        # TODO: Figure out how to parse virus strain fields
-        return None
+        # TODO: Figure out how to parse virus strain field
+        return virus_strain_str
 
     @property
     def aind_age_at_injection(self) -> Optional[Decimal]:
         """Maps age_at_injection to aind model"""
         return self._parse_basic_decimal_str(self._nsb.age_at_injection)
 
     @property
```

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2023/models.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2023/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/sharepoint/nsb2023/procedures.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/sharepoint/nsb2023/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/slims/client.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/slims/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/slims/models.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/slims/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/client.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/funding/mapping.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/funding/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/mapper.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/mapper.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/models.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/perfusions/mapping.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/perfusions/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/smartsheet/perfusions/models.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/smartsheet/perfusions/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service/tars/client.py` & `aind_metadata_service-0.9.3/src/aind_metadata_service/tars/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 import logging
 from typing import List, Optional
 
 import requests
 from azure.identity import ClientSecretCredential
 from pydantic import Field, SecretStr
-from pydantic_settings import BaseSettings
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 from aind_metadata_service.response_handler import ModelResponse, StatusCodes
 from aind_metadata_service.tars.mapping import TarsResponseHandler
 
 
 class AzureSettings(BaseSettings):
     """Configuration class. Mostly a wrapper around AzureAuth
     class constructor arguments."""
 
+    model_config = SettingsConfigDict(env_prefix="TARS_")
+
     tenant_id: str = Field(
         ..., description="The ID of the AllenInstituteB2C Azure tenant."
     )
     client_id: str = Field(
         ..., description="Client ID of the service account accessing resource."
     )
     client_secret: SecretStr = Field(
```

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.9.3/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.9.2
+Version: 0.9.3
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_service-0.9.2/src/aind_metadata_service.egg-info/SOURCES.txt` & `aind_metadata_service-0.9.3/src/aind_metadata_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/labtracks/test_client.py` & `aind_metadata_service-0.9.3/tests/labtracks/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/labtracks/test_query_builder.py` & `aind_metadata_service-0.9.3/tests/labtracks/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/labtracks/test_response_handler.py` & `aind_metadata_service-0.9.3/tests/labtracks/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/json_responses/combined.json` & `aind_metadata_service-0.9.3/tests/resources/json_responses/combined.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/json_responses/combined_invalid.json` & `aind_metadata_service-0.9.3/tests/resources/json_responses/combined_invalid.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/json_responses/mapped_las_procedure.json` & `aind_metadata_service-0.9.3/tests/resources/json_responses/mapped_las_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/json_responses/mapped_las_procedure_invalid.json` & `aind_metadata_service-0.9.3/tests/resources/json_responses/mapped_las_procedure_invalid.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/json_responses/mapped_sp_procedure.json` & `aind_metadata_service-0.9.3/tests/resources/json_responses/mapped_sp_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/json_responses/mapped_sp_procedure_invalid.json` & `aind_metadata_service-0.9.3/tests/resources/json_responses/mapped_sp_procedure_invalid.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item20.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item20.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/nsb2019_string_entries.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/nsb2019_string_entries.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item1.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item12.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item19.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item19.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item2.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item20.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item20.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item3.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item4.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item5.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item6.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2019/raw/list_item7.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2019/raw/list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item19.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item19.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item20.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item20.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item21.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item21.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item22.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item22.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989177489177489%*

 * *Differences: {'0': "{'procedures': {0: {'injection_materials': [OrderedDict([('name', 'Premixied "*

 * *      "&quot;\\u200bdL+Cre&quot;'), ('material_type', 'Virus'), ('tars_identifiers', None), "*

 * *      "('addgene_id', None), ('titer', None), ('titer_unit', 'gc/mL')])]}}}"}*

```diff
@@ -25,15 +25,24 @@
                 "injection_coordinate_reference": "Bregma",
                 "injection_coordinate_unit": "millimeter",
                 "injection_current": "5",
                 "injection_current_unit": "microamps",
                 "injection_duration": null,
                 "injection_duration_unit": "minute",
                 "injection_hemisphere": "Right",
-                "injection_materials": [],
+                "injection_materials": [
+                    {
+                        "addgene_id": null,
+                        "material_type": "Virus",
+                        "name": "Premixied &quot;\u200bdL+Cre&quot;",
+                        "tars_identifiers": null,
+                        "titer": null,
+                        "titer_unit": "gc/mL"
+                    }
+                ],
                 "instrument_id": "Ionto #1",
                 "procedure_type": "Iontophoresis injection",
                 "recovery_time": null,
                 "recovery_time_unit": "minute",
                 "targeted_structure": null
             }
         ],
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/nsb2023_string_entries.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/nsb2023_string_entries.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item10.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item13.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.972972972972973%*

 * *Differences: {"'Burr2_x0020_Perform_x0020_During'": "'Initial Surgery'",*

 * * "'Burr3_x0020_Perform_x0020_During'": "'Initial Surgery'",*

 * * "'Burr4_x0020_Perform_x0020_During'": "'Initial Surgery'",*

 * * "'CraniotomyType'": "'5mm'",*

 * * "'Headpost_x0020_Perform_x0020_Dur'": "'Initial Surgery'",*

 * * "'ImplantIDCoverslipType'": "'5mm stacked coverslip'",*

 * * "'Inj1VirusStrain_rt'": 'None',*

 * * "'Inj4VirusStrain_rt'": 'None',*

 * * "'Procedure'": 'None',*

 * * "'Procedure_x0020_Family'": "'Headpost Only'",*

 * * 'delete': "['Burr1_x0020_Perform_x0020_During'] […]*

```diff
@@ -4,32 +4,31 @@
     "Attachments": false,
     "AuthorId": "187",
     "Behavior": "0",
     "Behavior_x0020_Complete": null,
     "Behavior_x0020_Type": "Select...",
     "Breg2Lamb": null,
     "Burr1_x0020_Injection_x0020_Devi": "Select...",
-    "Burr1_x0020_Perform_x0020_During": null,
     "Burr1_x0020_Virus_x0020_Biosafte": null,
     "Burr2_x0020_Injection_x0020_Devi": "Select...",
-    "Burr2_x0020_Perform_x0020_During": null,
+    "Burr2_x0020_Perform_x0020_During": "Initial Surgery",
     "Burr2_x0020_Status": null,
     "Burr2_x0020_Virus_x0020_Biosafte": "Select...",
     "Burr3_x0020_A_x002f_P": null,
     "Burr3_x0020_D_x002f_V": null,
     "Burr3_x0020_Injection_x0020_Devi": "Select...",
     "Burr3_x0020_M_x002f_L": null,
-    "Burr3_x0020_Perform_x0020_During": null,
+    "Burr3_x0020_Perform_x0020_During": "Initial Surgery",
     "Burr3_x0020_Status": null,
     "Burr3_x0020_Virus_x0020_Biosafet": "Select...",
     "Burr4_x0020_A_x002f_P": null,
     "Burr4_x0020_D_x002f_V": null,
     "Burr4_x0020_Injection_x0020_Devi": "Select...",
     "Burr4_x0020_M_x002f_L": null,
-    "Burr4_x0020_Perform_x0020_During": null,
+    "Burr4_x0020_Perform_x0020_During": "Initial Surgery",
     "Burr4_x0020_Status": null,
     "Burr4_x0020_Virus_x0020_Biosafte": null,
     "Burr5_x0020_Injection_x0020_Devi": "Select...",
     "Burr5_x0020_Perform_x0020_During": "Initial Surgery",
     "Burr5_x0020_Status": null,
     "Burr5_x0020_Virus_x0020_Biosafte": "Select...",
     "Burr6_x0020_Injection_x0020_Devi": "Select...",
@@ -80,15 +79,15 @@
     "ComDurotomy": "Complete",
     "ComSinusbleed": "Mild",
     "ComSwelling": "None",
     "ComWindow": "None",
     "ComplianceAssetId": null,
     "ContentTypeId": "0x010043A15BEFF52D264A9B0D7FB6BC1EC47B",
     "Contusion": "Central",
-    "CraniotomyType": "3mm",
+    "CraniotomyType": "5mm",
     "Craniotomy_x0020_Perform_x0020_D": "Initial Surgery",
     "Created": "2022-12-20T17:08:31Z",
     "DV2ndInj": null,
     "Date1stInjection": null,
     "DateRangeStart": "2023-01-02T08:00:00Z",
     "Date_x0020_of_x0020_Birth": "2022-11-09T08:00:00Z",
     "Date_x0020_of_x0020_Surgery": "2022-01-03T08:00:00Z",
@@ -112,28 +111,28 @@
     "FirstInjectionWeightBefor": null,
     "GUID": "cda0b241-be4f-4a14-a7ef-75a01939036a",
     "HPIsoLevel": "2",
     "HPRecovery": "25",
     "HPSurgeonComments": "Went very well",
     "Headpost": "Visual Ctx",
     "HeadpostType": "Mesoscope",
-    "Headpost_x0020_Perform_x0020_Dur": null,
+    "Headpost_x0020_Perform_x0020_Dur": "Initial Surgery",
     "Hemisphere2ndInj": "Select...",
     "HpWorkStation": "SWS 4",
     "IACUC_x0020_Protocol_x0020__x002": "2103",
     "ID": 190,
     "Id": 190,
-    "ImplantIDCoverslipType": "3mm stacked coverslip",
+    "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
     "Inj1Angle_v2": null,
     "Inj1Current": null,
     "Inj1IontoTime": null,
     "Inj1StorageLocation": "Select...",
     "Inj1Type": null,
-    "Inj1VirusStrain_rt": "Select...",
+    "Inj1VirusStrain_rt": null,
     "Inj2AlternatingTime": null,
     "Inj2Angle_v2": null,
     "Inj2Current": null,
     "Inj2IontoTime": null,
     "Inj2StorageLocation": null,
     "Inj2Type": "Select...",
     "Inj2VirusStrain_rt": null,
@@ -145,15 +144,15 @@
     "Inj3retSetting": "Off",
     "Inj3volperdepth": null,
     "Inj4AlternatingTime": null,
     "Inj4Current": null,
     "Inj4IontoTime": "Off",
     "Inj4StorageLocation": "Select...",
     "Inj4Type": null,
-    "Inj4VirusStrain_rt": "Select...",
+    "Inj4VirusStrain_rt": null,
     "Inj4retSetting": null,
     "Inj4volperdepth": null,
     "Inj5AlternatingTime": null,
     "Inj5Current": null,
     "Inj5IontoTime": null,
     "Inj5StorageLocation": null,
     "Inj5Type": "Select...",
@@ -187,16 +186,16 @@
     "NanojectNumberInj2": "Select...",
     "OData__ColorTag": null,
     "OData__UIVersionString": "1",
     "OData__x0023__x0020_of_x0020_Burr_x002": "1",
     "PIId": 166,
     "PIStringId": "166",
     "PedigreeName": "Gad2-IRES-Cre;Slc32a1-T2A-FlpO;Ai210-hyg",
-    "Procedure": "Visual Ctx 2P",
-    "Procedure_x0020_Family": "Cranial Window",
+    "Procedure": null,
+    "Procedure_x0020_Family": "Headpost Only",
     "Procedure_x0020_Slots": "Single surgical session",
     "Procedure_x0020_T2": "Select...",
     "ProjectID": "121-01-012-10 Learning mFISH",
     "Project_x0020_ID_x0020__x0028_te": "121-01-012-10 Learning mFISH",
     "Round1InjIsolevel": null,
     "ServerRedirectedEmbedUri": null,
     "ServerRedirectedEmbedUrl": "",
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item11.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item13.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item20.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9617117117117117%*

 * *Differences: {"'Burr1_x0020_Perform_x0020_During'": 'None',*

 * * "'Burr2_x0020_Perform_x0020_During'": 'None',*

 * * "'Burr3_x0020_Perform_x0020_During'": 'None',*

 * * "'Burr4_x0020_Perform_x0020_During'": 'None',*

 * * "'Craniotomy_x0020_Perform_x0020_D'": "'Follow up Surgery'",*

 * * "'Date1stInjection'": "'2022-01-03T08:00:00Z'",*

 * * "'FirstInjRecovery'": "'30'",*

 * * "'FirstInjectionIsoDuration'": "'1.5'",*

 * * "'FirstInjectionWeightAfter'": "'28.2'",*

 * * "'FirstInjectionWeightBefor'": "'25.2'",*

 * * "'Headpost_x0020_Perform_x0020_Dur'": "'Follow up Surger […]*

```diff
@@ -4,31 +4,32 @@
     "Attachments": false,
     "AuthorId": "187",
     "Behavior": "0",
     "Behavior_x0020_Complete": null,
     "Behavior_x0020_Type": "Select...",
     "Breg2Lamb": null,
     "Burr1_x0020_Injection_x0020_Devi": "Select...",
+    "Burr1_x0020_Perform_x0020_During": null,
     "Burr1_x0020_Virus_x0020_Biosafte": null,
     "Burr2_x0020_Injection_x0020_Devi": "Select...",
-    "Burr2_x0020_Perform_x0020_During": "Initial Surgery",
+    "Burr2_x0020_Perform_x0020_During": null,
     "Burr2_x0020_Status": null,
     "Burr2_x0020_Virus_x0020_Biosafte": "Select...",
     "Burr3_x0020_A_x002f_P": null,
     "Burr3_x0020_D_x002f_V": null,
     "Burr3_x0020_Injection_x0020_Devi": "Select...",
     "Burr3_x0020_M_x002f_L": null,
-    "Burr3_x0020_Perform_x0020_During": "Initial Surgery",
+    "Burr3_x0020_Perform_x0020_During": null,
     "Burr3_x0020_Status": null,
     "Burr3_x0020_Virus_x0020_Biosafet": "Select...",
     "Burr4_x0020_A_x002f_P": null,
     "Burr4_x0020_D_x002f_V": null,
     "Burr4_x0020_Injection_x0020_Devi": "Select...",
     "Burr4_x0020_M_x002f_L": null,
-    "Burr4_x0020_Perform_x0020_During": "Initial Surgery",
+    "Burr4_x0020_Perform_x0020_During": null,
     "Burr4_x0020_Status": null,
     "Burr4_x0020_Virus_x0020_Biosafte": null,
     "Burr5_x0020_Injection_x0020_Devi": "Select...",
     "Burr5_x0020_Perform_x0020_During": "Initial Surgery",
     "Burr5_x0020_Status": null,
     "Burr5_x0020_Virus_x0020_Biosafte": "Select...",
     "Burr6_x0020_Injection_x0020_Devi": "Select...",
@@ -80,18 +81,18 @@
     "ComSinusbleed": "Mild",
     "ComSwelling": "None",
     "ComWindow": "None",
     "ComplianceAssetId": null,
     "ContentTypeId": "0x010043A15BEFF52D264A9B0D7FB6BC1EC47B",
     "Contusion": "Central",
     "CraniotomyType": "5mm",
-    "Craniotomy_x0020_Perform_x0020_D": "Initial Surgery",
+    "Craniotomy_x0020_Perform_x0020_D": "Follow up Surgery",
     "Created": "2022-12-20T17:08:31Z",
     "DV2ndInj": null,
-    "Date1stInjection": null,
+    "Date1stInjection": "2022-01-03T08:00:00Z",
     "DateRangeStart": "2023-01-02T08:00:00Z",
     "Date_x0020_of_x0020_Birth": "2022-11-09T08:00:00Z",
     "Date_x0020_of_x0020_Surgery": "2022-01-03T08:00:00Z",
     "EditorId": "2846",
     "FiberImplant1DV": null,
     "FiberImplant2DV": null,
     "Fiber_x0020_Implant1_x0020_Lengt": "Select...",
@@ -101,25 +102,25 @@
     "Fiber_x0020_Implant4_x0020_D_x00": null,
     "Fiber_x0020_Implant4_x0020_Lengt": "Select...",
     "Fiber_x0020_Implant5_x0020_D_x00": null,
     "Fiber_x0020_Implant5_x0020_Lengt": "Select...",
     "Fiber_x0020_Implant6_x0020_D_x00": null,
     "Fiber_x0020_Implant6_x0020_Lengt": "Select...",
     "FileSystemObjectType": 0,
-    "FirstInjRecovery": null,
-    "FirstInjectionIsoDuration": null,
-    "FirstInjectionWeightAfter": null,
-    "FirstInjectionWeightBefor": null,
+    "FirstInjRecovery": "30",
+    "FirstInjectionIsoDuration": "1.5",
+    "FirstInjectionWeightAfter": "28.2",
+    "FirstInjectionWeightBefor": "25.2",
     "GUID": "cda0b241-be4f-4a14-a7ef-75a01939036a",
     "HPIsoLevel": "2",
     "HPRecovery": "25",
     "HPSurgeonComments": "Went very well",
     "Headpost": "Visual Ctx",
     "HeadpostType": "Mesoscope",
-    "Headpost_x0020_Perform_x0020_Dur": "Initial Surgery",
+    "Headpost_x0020_Perform_x0020_Dur": "Follow up Surgery",
     "Hemisphere2ndInj": "Select...",
     "HpWorkStation": "SWS 4",
     "IACUC_x0020_Protocol_x0020__x002": "2103",
     "ID": 190,
     "Id": 190,
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
@@ -186,21 +187,21 @@
     "NanojectNumberInj2": "Select...",
     "OData__ColorTag": null,
     "OData__UIVersionString": "1",
     "OData__x0023__x0020_of_x0020_Burr_x002": "1",
     "PIId": 166,
     "PIStringId": "166",
     "PedigreeName": "Gad2-IRES-Cre;Slc32a1-T2A-FlpO;Ai210-hyg",
-    "Procedure": null,
-    "Procedure_x0020_Family": "Headpost Only",
-    "Procedure_x0020_Slots": "Single surgical session",
+    "Procedure": "HP Only",
+    "Procedure_x0020_Family": "Injection",
+    "Procedure_x0020_Slots": "Initial surgery with follow up session",
     "Procedure_x0020_T2": "Select...",
     "ProjectID": "121-01-012-10 Learning mFISH",
     "Project_x0020_ID_x0020__x0028_te": "121-01-012-10 Learning mFISH",
-    "Round1InjIsolevel": null,
+    "Round1InjIsolevel": "2",
     "ServerRedirectedEmbedUri": null,
     "ServerRedirectedEmbedUrl": "",
     "Sex": "Male",
     "SurgeryStatus": "Ready for Feedback",
     "TEST_x0020_1st_x0020_Round_x0020Id": null,
     "TEST_x0020_1st_x0020_Round_x0020StringId": null,
     "Test1Id": 2846,
@@ -208,15 +209,15 @@
     "Title": "657849Visual Ctx 2P",
     "Virus_x0020_A_x002f_P": null,
     "Virus_x0020_D_x002f_V": null,
     "Virus_x0020_Hemisphere": "Select...",
     "Virus_x0020_M_x002f_L": null,
     "Weight_x0020_after_x0020_Surgery": "28.2",
     "Weight_x0020_before_x0020_Surger": "25.2",
-    "WorkStation1stInjection": "Select...",
+    "WorkStation1stInjection": "SWS 5",
     "inj1volperdepth": null,
     "inj2volperdepth": null,
     "inj3volperdepth": null,
     "inj5volperdepth": null,
     "inj6volperdepth": null,
     "retSetting0": "Off",
     "retSetting1": "Off"
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item14.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item15.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item15.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954954954954955%*

 * *Differences: {"'Inj1VirusStrain_rt'": 'None', "'Inj4VirusStrain_rt'": 'None'}*

```diff
@@ -125,15 +125,15 @@
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
     "Inj1Angle_v2": "0",
     "Inj1Current": null,
     "Inj1IontoTime": null,
     "Inj1StorageLocation": "Select...",
     "Inj1Type": "Nanoject (Pressure)",
-    "Inj1VirusStrain_rt": "Select...",
+    "Inj1VirusStrain_rt": null,
     "Inj2AlternatingTime": "7/7",
     "Inj2Angle_v2": "0",
     "Inj2Current": null,
     "Inj2IontoTime": null,
     "Inj2StorageLocation": null,
     "Inj2Type": "Iontophoresis",
     "Inj2VirusStrain_rt": null,
@@ -145,15 +145,15 @@
     "Inj3retSetting": "Off",
     "Inj3volperdepth": null,
     "Inj4AlternatingTime": "7/7",
     "Inj4Current": "5uA",
     "Inj4IontoTime": null,
     "Inj4StorageLocation": "Select...",
     "Inj4Type": "Iontophoresis",
-    "Inj4VirusStrain_rt": "Select...",
+    "Inj4VirusStrain_rt": null,
     "Inj4retSetting": null,
     "Inj4volperdepth": null,
     "Inj5AlternatingTime": null,
     "Inj5Current": null,
     "Inj5IontoTime": null,
     "Inj5StorageLocation": null,
     "Inj5Type": "Select...",
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item16.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item16.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954954954954955%*

 * *Differences: {"'Inj1VirusStrain_rt'": 'None', "'Inj4VirusStrain_rt'": 'None'}*

```diff
@@ -125,15 +125,15 @@
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
     "Inj1Angle_v2": 0.0,
     "Inj1Current": null,
     "Inj1IontoTime": null,
     "Inj1StorageLocation": "Select...",
     "Inj1Type": "Nanoject (Pressure)",
-    "Inj1VirusStrain_rt": "Select...",
+    "Inj1VirusStrain_rt": null,
     "Inj2AlternatingTime": "7/7",
     "Inj2Angle_v2": "0",
     "Inj2Current": null,
     "Inj2IontoTime": null,
     "Inj2StorageLocation": null,
     "Inj2Type": "Iontophoresis",
     "Inj2VirusStrain_rt": null,
@@ -145,15 +145,15 @@
     "Inj3retSetting": "Off",
     "Inj3volperdepth": null,
     "Inj4AlternatingTime": "7/7",
     "Inj4Current": "5uA",
     "Inj4IontoTime": null,
     "Inj4StorageLocation": "Select...",
     "Inj4Type": "Iontophoresis",
-    "Inj4VirusStrain_rt": "Select...",
+    "Inj4VirusStrain_rt": null,
     "Inj4retSetting": null,
     "Inj4volperdepth": null,
     "Inj5AlternatingTime": null,
     "Inj5Current": null,
     "Inj5IontoTime": null,
     "Inj5StorageLocation": null,
     "Inj5Type": "Select...",
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item17.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item17.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954954954954955%*

 * *Differences: {"'Inj1VirusStrain_rt'": 'None', "'Inj4VirusStrain_rt'": 'None'}*

```diff
@@ -125,15 +125,15 @@
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
     "Inj1Angle_v2": "0",
     "Inj1Current": null,
     "Inj1IontoTime": null,
     "Inj1StorageLocation": "Select...",
     "Inj1Type": "Nanoject (Pressure)",
-    "Inj1VirusStrain_rt": "Select...",
+    "Inj1VirusStrain_rt": null,
     "Inj2AlternatingTime": "7/7",
     "Inj2Angle_v2": "0",
     "Inj2Current": null,
     "Inj2IontoTime": null,
     "Inj2StorageLocation": null,
     "Inj2Type": "Iontophoresis",
     "Inj2VirusStrain_rt": null,
@@ -145,15 +145,15 @@
     "Inj3retSetting": "Off",
     "Inj3volperdepth": null,
     "Inj4AlternatingTime": "7/7",
     "Inj4Current": "5uA",
     "Inj4IontoTime": null,
     "Inj4StorageLocation": "Select...",
     "Inj4Type": "Iontophoresis",
-    "Inj4VirusStrain_rt": "Select...",
+    "Inj4VirusStrain_rt": null,
     "Inj4retSetting": null,
     "Inj4volperdepth": null,
     "Inj5AlternatingTime": null,
     "Inj5Current": null,
     "Inj5IontoTime": null,
     "Inj5StorageLocation": null,
     "Inj5Type": "Select...",
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item18.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item18.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928571428571429%*

 * *Differences: {"'Inj1VirusStrain_rt'": 'None', "'Inj4VirusStrain_rt'": 'None'}*

```diff
@@ -66,15 +66,15 @@
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
     "Inj1Angle_v2": null,
     "Inj1Current": null,
     "Inj1IontoTime": null,
     "Inj1StorageLocation": "Select...",
     "Inj1Type": null,
-    "Inj1VirusStrain_rt": "Select...",
+    "Inj1VirusStrain_rt": null,
     "Inj2AlternatingTime": null,
     "Inj2Angle_v2": null,
     "Inj2Current": null,
     "Inj2IontoTime": null,
     "Inj2StorageLocation": null,
     "Inj2Type": "Select...",
     "Inj2VirusStrain_rt": null,
@@ -85,15 +85,15 @@
     "Inj3Type": "Select...",
     "Inj3retSetting": "Off",
     "Inj4AlternatingTime": null,
     "Inj4Current": null,
     "Inj4IontoTime": "Off",
     "Inj4StorageLocation": "Select...",
     "Inj4Type": null,
-    "Inj4VirusStrain_rt": "Select...",
+    "Inj4VirusStrain_rt": null,
     "Inj4retSetting": null,
     "Inj4volperdepth": null,
     "InjVirusStrain_rt": null,
     "IontoNumberInj1": "Select...",
     "IontoNumberInj2": "Select...",
     "Iso_x0020_On": "1.5",
     "LIMStaskflow1": "MSP Learning & mFISH Development (Dox)",
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item19.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item19.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954954954954955%*

 * *Differences: {"'Inj1VirusStrain_rt'": 'None', "'Inj4VirusStrain_rt'": 'None'}*

```diff
@@ -125,15 +125,15 @@
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
     "Inj1Angle_v2": "0",
     "Inj1Current": null,
     "Inj1IontoTime": null,
     "Inj1StorageLocation": "Select...",
     "Inj1Type": "Nanoject (Pressure)",
-    "Inj1VirusStrain_rt": "Select...",
+    "Inj1VirusStrain_rt": null,
     "Inj2AlternatingTime": "7/7",
     "Inj2Angle_v2": "0",
     "Inj2Current": null,
     "Inj2IontoTime": null,
     "Inj2StorageLocation": null,
     "Inj2Type": "Iontophoresis",
     "Inj2VirusStrain_rt": null,
@@ -145,15 +145,15 @@
     "Inj3retSetting": "Off",
     "Inj3volperdepth": null,
     "Inj4AlternatingTime": "7/7",
     "Inj4Current": "5uA",
     "Inj4IontoTime": null,
     "Inj4StorageLocation": "Select...",
     "Inj4Type": "Iontophoresis",
-    "Inj4VirusStrain_rt": "Select...",
+    "Inj4VirusStrain_rt": null,
     "Inj4retSetting": null,
     "Inj4volperdepth": null,
     "Inj5AlternatingTime": null,
     "Inj5Current": null,
     "Inj5IontoTime": null,
     "Inj5StorageLocation": null,
     "Inj5Type": "Nanoject (Pressure)",
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item20.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item21.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954954954954955%*

 * *Differences: {"'Craniotomy_x0020_Perform_x0020_D'": "'null'", "'Headpost_x0020_Perform_x0020_Dur'": "'null'"}*

```diff
@@ -81,15 +81,15 @@
     "ComSinusbleed": "Mild",
     "ComSwelling": "None",
     "ComWindow": "None",
     "ComplianceAssetId": null,
     "ContentTypeId": "0x010043A15BEFF52D264A9B0D7FB6BC1EC47B",
     "Contusion": "Central",
     "CraniotomyType": "5mm",
-    "Craniotomy_x0020_Perform_x0020_D": "Follow up Surgery",
+    "Craniotomy_x0020_Perform_x0020_D": "null",
     "Created": "2022-12-20T17:08:31Z",
     "DV2ndInj": null,
     "Date1stInjection": "2022-01-03T08:00:00Z",
     "DateRangeStart": "2023-01-02T08:00:00Z",
     "Date_x0020_of_x0020_Birth": "2022-11-09T08:00:00Z",
     "Date_x0020_of_x0020_Surgery": "2022-01-03T08:00:00Z",
     "EditorId": "2846",
@@ -112,15 +112,15 @@
     "FirstInjectionWeightBefor": "25.2",
     "GUID": "cda0b241-be4f-4a14-a7ef-75a01939036a",
     "HPIsoLevel": "2",
     "HPRecovery": "25",
     "HPSurgeonComments": "Went very well",
     "Headpost": "Visual Ctx",
     "HeadpostType": "Mesoscope",
-    "Headpost_x0020_Perform_x0020_Dur": "Follow up Surgery",
+    "Headpost_x0020_Perform_x0020_Dur": "null",
     "Hemisphere2ndInj": "Select...",
     "HpWorkStation": "SWS 4",
     "IACUC_x0020_Protocol_x0020__x002": "2103",
     "ID": 190,
     "Id": 190,
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item21.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item22.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9932432432432432%*

 * *Differences: {"'Craniotomy_x0020_Perform_x0020_D'": 'None',*

 * * "'Headpost_x0020_Perform_x0020_Dur'": 'None',*

 * * "'Procedure'": "'Frontal Ctx 2P'"}*

```diff
@@ -81,15 +81,15 @@
     "ComSinusbleed": "Mild",
     "ComSwelling": "None",
     "ComWindow": "None",
     "ComplianceAssetId": null,
     "ContentTypeId": "0x010043A15BEFF52D264A9B0D7FB6BC1EC47B",
     "Contusion": "Central",
     "CraniotomyType": "5mm",
-    "Craniotomy_x0020_Perform_x0020_D": "null",
+    "Craniotomy_x0020_Perform_x0020_D": null,
     "Created": "2022-12-20T17:08:31Z",
     "DV2ndInj": null,
     "Date1stInjection": "2022-01-03T08:00:00Z",
     "DateRangeStart": "2023-01-02T08:00:00Z",
     "Date_x0020_of_x0020_Birth": "2022-11-09T08:00:00Z",
     "Date_x0020_of_x0020_Surgery": "2022-01-03T08:00:00Z",
     "EditorId": "2846",
@@ -112,15 +112,15 @@
     "FirstInjectionWeightBefor": "25.2",
     "GUID": "cda0b241-be4f-4a14-a7ef-75a01939036a",
     "HPIsoLevel": "2",
     "HPRecovery": "25",
     "HPSurgeonComments": "Went very well",
     "Headpost": "Visual Ctx",
     "HeadpostType": "Mesoscope",
-    "Headpost_x0020_Perform_x0020_Dur": "null",
+    "Headpost_x0020_Perform_x0020_Dur": null,
     "Hemisphere2ndInj": "Select...",
     "HpWorkStation": "SWS 4",
     "IACUC_x0020_Protocol_x0020__x002": "2103",
     "ID": 190,
     "Id": 190,
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
@@ -187,15 +187,15 @@
     "NanojectNumberInj2": "Select...",
     "OData__ColorTag": null,
     "OData__UIVersionString": "1",
     "OData__x0023__x0020_of_x0020_Burr_x002": "1",
     "PIId": 166,
     "PIStringId": "166",
     "PedigreeName": "Gad2-IRES-Cre;Slc32a1-T2A-FlpO;Ai210-hyg",
-    "Procedure": "HP Only",
+    "Procedure": "Frontal Ctx 2P",
     "Procedure_x0020_Family": "Injection",
     "Procedure_x0020_Slots": "Initial surgery with follow up session",
     "Procedure_x0020_T2": "Select...",
     "ProjectID": "121-01-012-10 Learning mFISH",
     "Project_x0020_ID_x0020__x0028_te": "121-01-012-10 Learning mFISH",
     "Round1InjIsolevel": "2",
     "ServerRedirectedEmbedUri": null,
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item22.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item9.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.990990990990991%*

 * *Differences: {"'Craniotomy_x0020_Perform_x0020_D'": "'Follow up Surgery'",*

 * * "'Headpost_x0020_Perform_x0020_Dur'": "'Initial Surgery'",*

 * * "'Inj1VirusStrain_rt'": 'None',*

 * * "'Inj4VirusStrain_rt'": 'None'}*

```diff
@@ -81,15 +81,15 @@
     "ComSinusbleed": "Mild",
     "ComSwelling": "None",
     "ComWindow": "None",
     "ComplianceAssetId": null,
     "ContentTypeId": "0x010043A15BEFF52D264A9B0D7FB6BC1EC47B",
     "Contusion": "Central",
     "CraniotomyType": "5mm",
-    "Craniotomy_x0020_Perform_x0020_D": null,
+    "Craniotomy_x0020_Perform_x0020_D": "Follow up Surgery",
     "Created": "2022-12-20T17:08:31Z",
     "DV2ndInj": null,
     "Date1stInjection": "2022-01-03T08:00:00Z",
     "DateRangeStart": "2023-01-02T08:00:00Z",
     "Date_x0020_of_x0020_Birth": "2022-11-09T08:00:00Z",
     "Date_x0020_of_x0020_Surgery": "2022-01-03T08:00:00Z",
     "EditorId": "2846",
@@ -112,28 +112,28 @@
     "FirstInjectionWeightBefor": "25.2",
     "GUID": "cda0b241-be4f-4a14-a7ef-75a01939036a",
     "HPIsoLevel": "2",
     "HPRecovery": "25",
     "HPSurgeonComments": "Went very well",
     "Headpost": "Visual Ctx",
     "HeadpostType": "Mesoscope",
-    "Headpost_x0020_Perform_x0020_Dur": null,
+    "Headpost_x0020_Perform_x0020_Dur": "Initial Surgery",
     "Hemisphere2ndInj": "Select...",
     "HpWorkStation": "SWS 4",
     "IACUC_x0020_Protocol_x0020__x002": "2103",
     "ID": 190,
     "Id": 190,
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
     "Inj1Angle_v2": null,
     "Inj1Current": null,
     "Inj1IontoTime": null,
     "Inj1StorageLocation": "Select...",
     "Inj1Type": null,
-    "Inj1VirusStrain_rt": "Select...",
+    "Inj1VirusStrain_rt": null,
     "Inj2AlternatingTime": null,
     "Inj2Angle_v2": null,
     "Inj2Current": null,
     "Inj2IontoTime": null,
     "Inj2StorageLocation": null,
     "Inj2Type": "Select...",
     "Inj2VirusStrain_rt": null,
@@ -145,15 +145,15 @@
     "Inj3retSetting": "Off",
     "Inj3volperdepth": null,
     "Inj4AlternatingTime": null,
     "Inj4Current": null,
     "Inj4IontoTime": "Off",
     "Inj4StorageLocation": "Select...",
     "Inj4Type": null,
-    "Inj4VirusStrain_rt": "Select...",
+    "Inj4VirusStrain_rt": null,
     "Inj4retSetting": null,
     "Inj4volperdepth": null,
     "Inj5AlternatingTime": null,
     "Inj5Current": null,
     "Inj5IontoTime": null,
     "Inj5StorageLocation": null,
     "Inj5Type": "Select...",
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item8.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/sharepoint/nsb2023/raw/list_item9.json` & `aind_metadata_service-0.9.3/tests/resources/sharepoint/nsb2023/raw/list_item10.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.963963963963964%*

 * *Differences: {"'CraniotomyType'": "'3mm'",*

 * * "'Craniotomy_x0020_Perform_x0020_D'": "'Initial Surgery'",*

 * * "'Date1stInjection'": 'None',*

 * * "'FirstInjRecovery'": 'None',*

 * * "'FirstInjectionIsoDuration'": 'None',*

 * * "'FirstInjectionWeightAfter'": 'None',*

 * * "'FirstInjectionWeightBefor'": 'None',*

 * * "'Headpost_x0020_Perform_x0020_Dur'": 'None',*

 * * "'ImplantIDCoverslipType'": "'3mm stacked coverslip'",*

 * * "'Inj1VirusStrain_rt'": 'None',*

 * * "'Inj4VirusStrain_rt'": 'None',*

 * * "'Procedure'": "'Visual Ctx 2P'",*

 * * "'Procedure_x0020_Family'": "'Crani […]*

```diff
@@ -80,19 +80,19 @@
     "ComDurotomy": "Complete",
     "ComSinusbleed": "Mild",
     "ComSwelling": "None",
     "ComWindow": "None",
     "ComplianceAssetId": null,
     "ContentTypeId": "0x010043A15BEFF52D264A9B0D7FB6BC1EC47B",
     "Contusion": "Central",
-    "CraniotomyType": "5mm",
-    "Craniotomy_x0020_Perform_x0020_D": "Follow up Surgery",
+    "CraniotomyType": "3mm",
+    "Craniotomy_x0020_Perform_x0020_D": "Initial Surgery",
     "Created": "2022-12-20T17:08:31Z",
     "DV2ndInj": null,
-    "Date1stInjection": "2022-01-03T08:00:00Z",
+    "Date1stInjection": null,
     "DateRangeStart": "2023-01-02T08:00:00Z",
     "Date_x0020_of_x0020_Birth": "2022-11-09T08:00:00Z",
     "Date_x0020_of_x0020_Surgery": "2022-01-03T08:00:00Z",
     "EditorId": "2846",
     "FiberImplant1DV": null,
     "FiberImplant2DV": null,
     "Fiber_x0020_Implant1_x0020_Lengt": "Select...",
@@ -102,38 +102,38 @@
     "Fiber_x0020_Implant4_x0020_D_x00": null,
     "Fiber_x0020_Implant4_x0020_Lengt": "Select...",
     "Fiber_x0020_Implant5_x0020_D_x00": null,
     "Fiber_x0020_Implant5_x0020_Lengt": "Select...",
     "Fiber_x0020_Implant6_x0020_D_x00": null,
     "Fiber_x0020_Implant6_x0020_Lengt": "Select...",
     "FileSystemObjectType": 0,
-    "FirstInjRecovery": "30",
-    "FirstInjectionIsoDuration": "1.5",
-    "FirstInjectionWeightAfter": "28.2",
-    "FirstInjectionWeightBefor": "25.2",
+    "FirstInjRecovery": null,
+    "FirstInjectionIsoDuration": null,
+    "FirstInjectionWeightAfter": null,
+    "FirstInjectionWeightBefor": null,
     "GUID": "cda0b241-be4f-4a14-a7ef-75a01939036a",
     "HPIsoLevel": "2",
     "HPRecovery": "25",
     "HPSurgeonComments": "Went very well",
     "Headpost": "Visual Ctx",
     "HeadpostType": "Mesoscope",
-    "Headpost_x0020_Perform_x0020_Dur": "Initial Surgery",
+    "Headpost_x0020_Perform_x0020_Dur": null,
     "Hemisphere2ndInj": "Select...",
     "HpWorkStation": "SWS 4",
     "IACUC_x0020_Protocol_x0020__x002": "2103",
     "ID": 190,
     "Id": 190,
-    "ImplantIDCoverslipType": "5mm stacked coverslip",
+    "ImplantIDCoverslipType": "3mm stacked coverslip",
     "Inj1AlternatingTime": null,
     "Inj1Angle_v2": null,
     "Inj1Current": null,
     "Inj1IontoTime": null,
     "Inj1StorageLocation": "Select...",
     "Inj1Type": null,
-    "Inj1VirusStrain_rt": "Select...",
+    "Inj1VirusStrain_rt": null,
     "Inj2AlternatingTime": null,
     "Inj2Angle_v2": null,
     "Inj2Current": null,
     "Inj2IontoTime": null,
     "Inj2StorageLocation": null,
     "Inj2Type": "Select...",
     "Inj2VirusStrain_rt": null,
@@ -145,15 +145,15 @@
     "Inj3retSetting": "Off",
     "Inj3volperdepth": null,
     "Inj4AlternatingTime": null,
     "Inj4Current": null,
     "Inj4IontoTime": "Off",
     "Inj4StorageLocation": "Select...",
     "Inj4Type": null,
-    "Inj4VirusStrain_rt": "Select...",
+    "Inj4VirusStrain_rt": null,
     "Inj4retSetting": null,
     "Inj4volperdepth": null,
     "Inj5AlternatingTime": null,
     "Inj5Current": null,
     "Inj5IontoTime": null,
     "Inj5StorageLocation": null,
     "Inj5Type": "Select...",
@@ -187,21 +187,21 @@
     "NanojectNumberInj2": "Select...",
     "OData__ColorTag": null,
     "OData__UIVersionString": "1",
     "OData__x0023__x0020_of_x0020_Burr_x002": "1",
     "PIId": 166,
     "PIStringId": "166",
     "PedigreeName": "Gad2-IRES-Cre;Slc32a1-T2A-FlpO;Ai210-hyg",
-    "Procedure": "Frontal Ctx 2P",
-    "Procedure_x0020_Family": "Injection",
-    "Procedure_x0020_Slots": "Initial surgery with follow up session",
+    "Procedure": "Visual Ctx 2P",
+    "Procedure_x0020_Family": "Cranial Window",
+    "Procedure_x0020_Slots": "Single surgical session",
     "Procedure_x0020_T2": "Select...",
     "ProjectID": "121-01-012-10 Learning mFISH",
     "Project_x0020_ID_x0020__x0028_te": "121-01-012-10 Learning mFISH",
-    "Round1InjIsolevel": "2",
+    "Round1InjIsolevel": null,
     "ServerRedirectedEmbedUri": null,
     "ServerRedirectedEmbedUrl": "",
     "Sex": "Male",
     "SurgeryStatus": "Ready for Feedback",
     "TEST_x0020_1st_x0020_Round_x0020Id": null,
     "TEST_x0020_1st_x0020_Round_x0020StringId": null,
     "Test1Id": 2846,
@@ -209,15 +209,15 @@
     "Title": "657849Visual Ctx 2P",
     "Virus_x0020_A_x002f_P": null,
     "Virus_x0020_D_x002f_V": null,
     "Virus_x0020_Hemisphere": "Select...",
     "Virus_x0020_M_x002f_L": null,
     "Weight_x0020_after_x0020_Surgery": "28.2",
     "Weight_x0020_before_x0020_Surger": "25.2",
-    "WorkStation1stInjection": "SWS 5",
+    "WorkStation1stInjection": "Select...",
     "inj1volperdepth": null,
     "inj2volperdepth": null,
     "inj3volperdepth": null,
     "inj5volperdepth": null,
     "inj6volperdepth": null,
     "retSetting0": "Off",
     "retSetting1": "Off"
```

### Comparing `aind_metadata_service-0.9.2/tests/resources/slims/json_entity.json` & `aind_metadata_service-0.9.3/tests/resources/slims/json_entity.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/smartsheet/test_funding_sheet.json` & `aind_metadata_service-0.9.3/tests/resources/smartsheet/test_funding_sheet.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/smartsheet/test_perfusions_sheet.json` & `aind_metadata_service-0.9.3/tests/resources/smartsheet/test_perfusions_sheet.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/resources/smartsheet/test_sheet.json` & `aind_metadata_service-0.9.3/tests/resources/smartsheet/test_sheet.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/sharepoint/nsb2019/test_mapping.py` & `aind_metadata_service-0.9.3/tests/sharepoint/nsb2019/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/sharepoint/nsb2019/test_models.py` & `aind_metadata_service-0.9.3/tests/sharepoint/nsb2019/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/sharepoint/nsb2019/test_string_parsing.py` & `aind_metadata_service-0.9.3/tests/sharepoint/nsb2019/test_string_parsing.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/sharepoint/nsb2023/test_mapping.py` & `aind_metadata_service-0.9.3/tests/sharepoint/nsb2023/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/sharepoint/nsb2023/test_models.py` & `aind_metadata_service-0.9.3/tests/sharepoint/nsb2023/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/sharepoint/nsb2023/test_string_parsing.py` & `aind_metadata_service-0.9.3/tests/sharepoint/nsb2023/test_string_parsing.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/sharepoint/test_client.py` & `aind_metadata_service-0.9.3/tests/sharepoint/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,17 @@
     DIR_RAW_2023 / str(f) for f in LIST_ITEM_FILE_NAMES_2023
 ]
 MAPPED_ITEM_FILE_NAMES_2023 = os.listdir(DIR_MAP_2023)
 sorted(MAPPED_ITEM_FILE_NAMES_2023)
 MAPPED_FILE_PATHS_2023 = [
     DIR_MAP_2023 / str(f) for f in MAPPED_ITEM_FILE_NAMES_2023
 ]
+INJECTION_MATERIALS_PATH = (
+    TEST_DIR / "resources" / "tars" / "mapped_materials.json"
+)
 
 
 class TestSharepointSettings(unittest.TestCase):
     """Class to test methods for SharepointSettings."""
 
     EXAMPLE_ENV_VAR1 = {
         "NSB_SHAREPOINT_URL": "some_url",
```

### Comparing `aind_metadata_service-0.9.2/tests/slims/test_client.py` & `aind_metadata_service-0.9.3/tests/slims/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/slims/test_models.py` & `aind_metadata_service-0.9.3/tests/slims/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/smartsheet/test_client.py` & `aind_metadata_service-0.9.3/tests/smartsheet/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/smartsheet/test_funding.py` & `aind_metadata_service-0.9.3/tests/smartsheet/test_funding.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/smartsheet/test_perfusions.py` & `aind_metadata_service-0.9.3/tests/smartsheet/test_perfusions.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/tars/test_client.py` & `aind_metadata_service-0.9.3/tests/tars/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from aind_metadata_service.tars.client import AzureSettings, TarsClient
 
 
 class TestAzureSettings(unittest.TestCase):
     """Class to test methods for AzureSettings."""
 
     EXAMPLE_ENV_VAR1 = {
-        "TENANT_ID": "some_tenant",
-        "CLIENT_ID": "some_client",
-        "RESOURCE": "some_resource",
-        "CLIENT_SECRET": "some_secret",
-        "SCOPE": "some_scope",
+        "TARS_TENANT_ID": "some_tenant",
+        "TARS_CLIENT_ID": "some_client",
+        "TARS_RESOURCE": "some_resource",
+        "TARS_CLIENT_SECRET": "some_secret",
+        "TARS_SCOPE": "some_scope",
     }
 
     @patch.dict(os.environ, EXAMPLE_ENV_VAR1, clear=True)
     def test_settings_set_from_env_vars(self):
         """Tests that the settings can be set from env vars."""
         settings1 = AzureSettings()
```

### Comparing `aind_metadata_service-0.9.2/tests/test_client.py` & `aind_metadata_service-0.9.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.9.2/tests/test_response_handler.py` & `aind_metadata_service-0.9.3/tests/test_response_handler.py`

 * *Files identical despite different names*

