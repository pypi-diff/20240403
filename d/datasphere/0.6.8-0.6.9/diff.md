# Comparing `tmp/datasphere-0.6.8.tar.gz` & `tmp/datasphere-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasphere-0.6.8.tar", last modified: Mon Feb 19 12:50:26 2024, max compression
+gzip compressed data, was "datasphere-0.6.9.tar", last modified: Thu Mar  7 14:42:39 2024, max compression
```

## Comparing `datasphere-0.6.8.tar` & `datasphere-0.6.9.tar`

### file list

```diff
@@ -1,934 +1,934 @@
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.936635 datasphere-0.6.8/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      771 2024-02-19 12:50:26.935641 datasphere-0.6.8/PKG-INFO
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3760 2024-01-26 17:55:40.000000 datasphere-0.6.8/README.md
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.047369 datasphere-0.6.8/datasphere/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-09-06 08:57:07.000000 datasphere-0.6.8/datasphere/__init__.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.051530 datasphere-0.6.8/datasphere/api/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2252 2024-01-15 10:36:00.000000 datasphere-0.6.8/datasphere/api/__init__.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3294 2024-01-29 11:25:55.000000 datasphere-0.6.8/datasphere/auth.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1764 2023-12-15 12:37:42.000000 datasphere-0.6.8/datasphere/channel.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12263 2024-01-29 11:25:55.000000 datasphere-0.6.8/datasphere/client.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22481 2024-02-19 12:47:17.000000 datasphere-0.6.8/datasphere/config.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3390 2023-11-28 11:07:54.000000 datasphere-0.6.8/datasphere/files.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.056319 datasphere-0.6.8/datasphere/logs/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       22 2023-09-06 08:57:07.000000 datasphere-0.6.8/datasphere/logs/__init__.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1107 2024-01-24 15:46:34.000000 datasphere-0.6.8/datasphere/logs/config.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3048 2024-01-24 15:46:34.000000 datasphere-0.6.8/datasphere/logs/logging.yaml
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6495 2024-01-29 11:25:55.000000 datasphere-0.6.8/datasphere/main.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6445 2024-02-19 11:57:17.000000 datasphere-0.6.8/datasphere/pyenv.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8353 2024-01-29 11:25:55.000000 datasphere-0.6.8/datasphere/utils.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       18 2024-02-19 12:47:57.000000 datasphere-0.6.8/datasphere/version.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.934013 datasphere-0.6.8/datasphere.egg-info/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      771 2024-02-19 12:50:25.000000 datasphere-0.6.8/datasphere.egg-info/PKG-INFO
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    47475 2024-02-19 12:50:26.000000 datasphere-0.6.8/datasphere.egg-info/SOURCES.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        1 2024-02-19 12:50:25.000000 datasphere-0.6.8/datasphere.egg-info/dependency_links.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       52 2024-02-19 12:50:25.000000 datasphere-0.6.8/datasphere.egg-info/entry_points.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       91 2024-02-19 12:50:25.000000 datasphere-0.6.8/datasphere.egg-info/requires.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       18 2024-02-19 12:50:25.000000 datasphere-0.6.8/datasphere.egg-info/top_level.txt
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       90 2023-09-06 08:57:07.000000 datasphere-0.6.8/pyproject.toml
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       38 2024-02-19 12:50:26.936747 datasphere-0.6.8/setup.cfg
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1558 2024-01-26 17:55:40.000000 datasphere-0.6.8/setup.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.061566 datasphere-0.6.8/tests/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2509 2024-01-29 11:25:55.000000 datasphere-0.6.8/tests/test_auth.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24679 2024-02-19 12:47:17.000000 datasphere-0.6.8/tests/test_config.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4513 2023-12-07 15:17:05.000000 datasphere-0.6.8/tests/test_files.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22644 2024-01-26 17:55:40.000000 datasphere-0.6.8/tests/test_main.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7625 2024-02-19 11:57:17.000000 datasphere-0.6.8/tests/test_pyenv.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7045 2024-01-29 11:25:55.000000 datasphere-0.6.8/tests/test_utils.py
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.022742 datasphere-0.6.8/yandex/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.065079 datasphere-0.6.8/yandex/cloud/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.069377 datasphere-0.6.8/yandex/cloud/access/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6665 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/access/access_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11909 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/access/access_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/access/access_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/access/access_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.073529 datasphere-0.6.8/yandex/cloud/api/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1584 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/api/operation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1671 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/api/operation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/api/operation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/api/operation_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.078267 datasphere-0.6.8/yandex/cloud/api/tools/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5000 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/api/tools/options_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11122 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/api/tools/options_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/api/tools/options_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/api/tools/options_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.024195 datasphere-0.6.8/yandex/cloud/datasphere/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.114220 datasphere-0.6.8/yandex/cloud/datasphere/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2045 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/app_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      821 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/app_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2843 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1743 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4209 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/folder_budget_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4542 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/folder_budget_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4843 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2917 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1417 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1430 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/node_execution_error_details_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/node_execution_error_details_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3291 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/node_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3828 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/node_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4708 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2715 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/node_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3492 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_data_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4613 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_data_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5007 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3085 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2795 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6829 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20175 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24543 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23351 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11777 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v1/project_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.169963 datasphere-0.6.8/yandex/cloud/datasphere/v2/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2003 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/community_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2855 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/community_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/community_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/community_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14608 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/community_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13893 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/community_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19589 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/community_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9797 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/community_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3140 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6253 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4058 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1577 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4763 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2549 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2955 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/docker_image_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      957 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/docker_image_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3021 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1751 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.180478 datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6389 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/jobs_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17757 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/jobs_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/jobs_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/jobs_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12732 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21128 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22551 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11246 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4783 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13939 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26729 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    31987 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    30603 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15150 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/project_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1670 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/resource_types_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1807 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/resource_types_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/resource_types_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/resource_types_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3887 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/s3_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1497 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/s3_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4638 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2429 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2321 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/secret_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3858 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/secret_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/secret_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/secret_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1345 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/user_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1402 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/user_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/user_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/datasphere/v2/user_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.025009 datasphere-0.6.8/yandex/cloud/iam/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.221636 datasphere-0.6.8/yandex/cloud/iam/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1454 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/api_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1724 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/api_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/api_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/api_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9402 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/api_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11255 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/api_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11954 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6433 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/api_key_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.232472 datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1630 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2056 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10385 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11644 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13154 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7342 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3583 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/iam_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3354 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/iam_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4843 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2883 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1857 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3688 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9752 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12434 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11657 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6178 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1197 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/role_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1049 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/role_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/role_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/role_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3565 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/role_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3458 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/role_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4554 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/role_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2765 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/role_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.246521 datasphere-0.6.8/yandex/cloud/iam/v1/saml/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2669 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1911 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11417 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12211 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12556 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6849 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4080 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6061 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17091 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23042 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16385 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8694 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1954 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/service_account_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2904 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/service_account_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/service_account_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/service_account_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15230 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/service_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13993 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/service_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18212 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9895 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/service_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3278 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/user_account_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5440 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/user_account_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/user_account_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/user_account_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2382 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      884 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3160 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2115 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/user_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2508 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      872 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3259 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2162 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.252554 datasphere-0.6.8/yandex/cloud/operation/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2024 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/operation/operation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4080 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/operation/operation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/operation/operation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/operation/operation_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3268 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/operation/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1393 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/operation/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4786 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/operation/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3024 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/operation/operation_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.258342 datasphere-0.6.8/yandex/cloud/priv/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.261687 datasphere-0.6.8/yandex/cloud/priv/access/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7066 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/access/access_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11446 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/access/access_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/access/access_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/access/access_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.027698 datasphere-0.6.8/yandex/cloud/priv/ai/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.028021 datasphere-0.6.8/yandex/cloud/priv/ai/platform/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.285256 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5536 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9014 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20605 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24248 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28428 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11907 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1899 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      165 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6379 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2745 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2349 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2141 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11736 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10066 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16814 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7204 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.029163 datasphere-0.6.8/yandex/cloud/priv/console/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.295160 datasphere-0.6.8/yandex/cloud/priv/console/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3699 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/access_binding_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5113 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/access_binding_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/access_binding_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/access_binding_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5184 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/form_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13004 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/form_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/form_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/form_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2871 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/resource_settings_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2931 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/resource_settings_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/resource_settings_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v1/resource_settings_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.297983 datasphere-0.6.8/yandex/cloud/priv/console/v2/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6190 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v2/form_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17308 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v2/form_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v2/form_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/console/v2/form_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.030201 datasphere-0.6.8/yandex/cloud/priv/datasphere/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.314888 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2097 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      821 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2899 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1763 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5645 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6036 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8725 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3945 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3536 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4180 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5128 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2593 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4521 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10153 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23427 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24457 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26233 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11053 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.463348 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2838 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      962 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3226 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1694 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2882 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5227 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1800 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      822 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3158 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1646 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1686 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2016 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3674 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3576 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8935 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3974 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4134 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9069 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16228 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23223 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22907 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10010 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4239 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8474 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8160 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12559 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13504 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6158 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    36196 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    42316 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    66265 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27530 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5451 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11310 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12811 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12594 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19704 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8812 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3202 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5630 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13554 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13197 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32326 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13892 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2972 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5388 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19179 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19707 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27038 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11675 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4342 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9374 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5810 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8348 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11448 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5056 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3254 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6255 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9014 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11278 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15510 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7107 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3340 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4026 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3328 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1861 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6523 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/invite_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6288 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/invite_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11164 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5005 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.471464 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7866 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19928 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15958 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24725 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    31272 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14111 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3265 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6465 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10595 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12758 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14265 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6095 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8017 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12591 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12828 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5581 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.526157 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2416 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2305 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7269 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11522 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3311 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4141 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2948 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3912 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3297 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3667 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5885 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7671 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6997 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7955 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9379 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4317 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7713 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8926 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13689 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6257 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3245 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4143 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3192 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3008 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4098 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5192 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2414 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2364 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4896 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7237 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3577 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7160 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5486 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5379 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9310 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4332 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8729 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20154 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    57944 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    76840 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    82053 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    34476 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10588 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    29650 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_actions_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_actions_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10677 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_types_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22058 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_types_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_types_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_types_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2295 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1428 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2998 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1594 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3745 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7411 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14542 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17570 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23541 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9913 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2703 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4525 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9804 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8285 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16411 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7199 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1388 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1216 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3769 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3275 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8621 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3748 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.533493 datasphere-0.6.8/yandex/cloud/priv/iam/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.538765 datasphere-0.6.8/yandex/cloud/priv/iam/management/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1784 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/management/cache_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1445 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/management/cache_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3041 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1955 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6389 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/restriction_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9448 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/restriction_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/restriction_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/restriction_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.748996 datasphere-0.6.8/yandex/cloud/priv/iam/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19133 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/access_binding_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27602 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/access_binding_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13351 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5937 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1440 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1429 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10074 2024-01-16 12:00:38.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8328 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12365 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5282 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.763550 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1630 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1774 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12396 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10408 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15757 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7155 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3385 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2236 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3312 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1902 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4409 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3656 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1934 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.774223 datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6916 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9571 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5367 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2733 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4011 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5020 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3123 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1700 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.780086 datasphere-0.6.8/yandex/cloud/priv/iam/v1/compute/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9883 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12962 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8942 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4262 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.809170 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4533 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5387 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5722 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3541 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3095 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2151 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2956 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1546 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3652 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/membership_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3479 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/membership_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3063 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1807 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2055 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1469 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3007 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1751 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3751 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/role_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4457 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/role_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4893 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2507 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7263 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5820 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7360 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3649 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2357 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1090 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3238 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1890 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4637 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/gizmo_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3316 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/gizmo_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5144 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2463 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6007 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6689 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8930 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4121 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2832 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1932 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3144 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1680 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4472 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3231 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3115 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1924 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10719 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9114 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14946 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7494 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2183 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3524 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12899 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12279 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14022 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5847 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.812534 datasphere-0.6.8/yandex/cloud/priv/iam/v1/maintenance/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1727 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1995 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5007 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/membership_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5190 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/membership_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5169 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2870 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.825937 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.831378 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/console/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4346 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4923 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5480 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3599 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.840594 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3110 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4813 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23234 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21942 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23761 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12571 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2009 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      811 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3028 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1573 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2980 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5827 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9030 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9478 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15464 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8935 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2008 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4677 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14411 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13744 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12466 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5373 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1287 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1352 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7644 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7548 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10574 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4600 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2351 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/operation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      811 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/operation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2980 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1557 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1241 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1012 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5682 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5176 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6765 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3041 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1191 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      849 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6665 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6036 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10526 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4575 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3290 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4498 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6513 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5937 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8996 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4109 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2798 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      165 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8522 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3799 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1736 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      165 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6323 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2745 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3934 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2974 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3234 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1803 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6818 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7624 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5029 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2474 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1240 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1000 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9776 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9185 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14808 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6421 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1759 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1761 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12267 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12390 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12870 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5667 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2374 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4716 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16230 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17780 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17177 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7764 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1681 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/revoked_credential_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2218 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/revoked_credential_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/revoked_credential_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/revoked_credential_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1529 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2300 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13376 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14434 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19538 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7962 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3839 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/root_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2638 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/root_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5121 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2445 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.854433 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1745 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2780 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11660 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8638 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12943 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5824 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3012 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7238 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18643 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16533 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19103 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8272 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1941 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2390 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22310 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15517 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32314 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13669 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3133 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4947 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22839 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    25016 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28176 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11780 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1718 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1629 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7138 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8143 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10494 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4524 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1630 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2549 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18550 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27356 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16449 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8681 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.857371 datasphere-0.6.8/yandex/cloud/priv/iam/v1/token/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1685 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/token/iam_token_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1145 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/token/iam_token_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/token/iam_token_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/token/iam_token_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2118 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/token_agent_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1788 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/token_agent_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2788 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1610 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.887404 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3521 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1430 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7376 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3687 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2580 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1398 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3014 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1683 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2727 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1989 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3179 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1721 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4010 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3464 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3334 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1763 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5879 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5761 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13083 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5892 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2336 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2128 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3020 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1601 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4138 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4432 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7626 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3701 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6907 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7244 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11106 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4997 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.890027 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ts/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2451 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2269 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4241 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6737 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9753 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10498 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10807 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4729 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2283 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1839 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5561 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4221 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7412 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3638 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.893161 datasphere-0.6.8/yandex/cloud/priv/oauth/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7906 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/claims_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13350 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/claims_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/claims_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/claims_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.908901 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3704 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/claim_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5933 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/claim_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2871 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1515 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2098 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/cloud_user_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2574 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/cloud_user_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/cloud_user_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/cloud_user_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4341 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/login_history_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4256 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/login_history_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5062 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3272 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1781 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/oauth_request_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1316 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/oauth_request_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/oauth_request_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/oauth_request_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11693 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/session_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16752 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/session_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13682 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9834 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.911538 datasphere-0.6.8/yandex/cloud/priv/operation/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1999 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/operation/operation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2833 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/operation/operation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/operation/operation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/operation/operation_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.918565 datasphere-0.6.8/yandex/cloud/priv/quota/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6813 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/quota/quota_limit_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9901 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/quota/quota_limit_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/quota/quota_limit_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/quota/quota_limit_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6603 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/quota/quota_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11691 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/quota/quota_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/quota/quota_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/quota/quota_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.921863 datasphere-0.6.8/yandex/cloud/priv/reference/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1704 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/reference/reference_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2651 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/reference/reference_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/reference/reference_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/reference/reference_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1895 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/sensitive_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2594 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/sensitive_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/sensitive_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/sensitive_pb2_grpc.pyi
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.037842 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/
-drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-02-19 12:50:26.932121 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16394 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23875 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9486 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11394 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2116 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/resource_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1574 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/resource_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/resource_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/resource_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2053 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/validation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2603 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/validation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/validation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/priv/validation_pb2_grpc.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2074 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/validation_pb2.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2603 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/validation_pb2.pyi
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/validation_pb2_grpc.py
--rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.8/yandex/cloud/validation_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.424967 datasphere-0.6.9/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      771 2024-03-07 14:42:39.423998 datasphere-0.6.9/PKG-INFO
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3760 2024-03-06 11:19:25.000000 datasphere-0.6.9/README.md
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.573279 datasphere-0.6.9/datasphere/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2023-09-06 08:57:07.000000 datasphere-0.6.9/datasphere/__init__.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.580953 datasphere-0.6.9/datasphere/api/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2252 2024-01-15 10:36:00.000000 datasphere-0.6.9/datasphere/api/__init__.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3294 2024-01-29 11:25:55.000000 datasphere-0.6.9/datasphere/auth.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1764 2023-12-15 12:37:42.000000 datasphere-0.6.9/datasphere/channel.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12375 2024-03-07 08:46:57.000000 datasphere-0.6.9/datasphere/client.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22481 2024-02-19 12:47:17.000000 datasphere-0.6.9/datasphere/config.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3390 2023-11-28 11:07:54.000000 datasphere-0.6.9/datasphere/files.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.584648 datasphere-0.6.9/datasphere/logs/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       22 2023-09-06 08:57:07.000000 datasphere-0.6.9/datasphere/logs/__init__.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1107 2024-03-04 12:28:02.000000 datasphere-0.6.9/datasphere/logs/config.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3048 2024-01-24 15:46:34.000000 datasphere-0.6.9/datasphere/logs/logging.yaml
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6567 2024-03-07 08:46:57.000000 datasphere-0.6.9/datasphere/main.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6445 2024-02-19 11:57:17.000000 datasphere-0.6.9/datasphere/pyenv.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8353 2024-01-29 11:25:55.000000 datasphere-0.6.9/datasphere/utils.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       18 2024-03-07 14:36:53.000000 datasphere-0.6.9/datasphere/version.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.422714 datasphere-0.6.9/datasphere.egg-info/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      771 2024-03-07 14:42:38.000000 datasphere-0.6.9/datasphere.egg-info/PKG-INFO
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    47475 2024-03-07 14:42:38.000000 datasphere-0.6.9/datasphere.egg-info/SOURCES.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)        1 2024-03-07 14:42:38.000000 datasphere-0.6.9/datasphere.egg-info/dependency_links.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       52 2024-03-07 14:42:38.000000 datasphere-0.6.9/datasphere.egg-info/entry_points.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       91 2024-03-07 14:42:38.000000 datasphere-0.6.9/datasphere.egg-info/requires.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       18 2024-03-07 14:42:38.000000 datasphere-0.6.9/datasphere.egg-info/top_level.txt
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       90 2023-09-06 08:57:07.000000 datasphere-0.6.9/pyproject.toml
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)       38 2024-03-07 14:42:39.425081 datasphere-0.6.9/setup.cfg
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1558 2024-01-26 17:55:40.000000 datasphere-0.6.9/setup.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.593040 datasphere-0.6.9/tests/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2509 2024-01-29 11:25:55.000000 datasphere-0.6.9/tests/test_auth.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24679 2024-02-19 12:47:17.000000 datasphere-0.6.9/tests/test_config.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4513 2023-12-07 15:17:05.000000 datasphere-0.6.9/tests/test_files.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22658 2024-03-07 08:46:57.000000 datasphere-0.6.9/tests/test_main.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7625 2024-02-19 11:57:17.000000 datasphere-0.6.9/tests/test_pyenv.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7045 2024-01-29 11:25:55.000000 datasphere-0.6.9/tests/test_utils.py
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.532793 datasphere-0.6.9/yandex/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.598974 datasphere-0.6.9/yandex/cloud/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.605356 datasphere-0.6.9/yandex/cloud/access/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6665 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/access/access_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11909 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/access/access_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/access/access_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/access/access_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.611304 datasphere-0.6.9/yandex/cloud/api/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1584 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/api/operation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1671 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/api/operation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/api/operation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/api/operation_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.616102 datasphere-0.6.9/yandex/cloud/api/tools/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5000 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/api/tools/options_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11122 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/api/tools/options_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/api/tools/options_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/api/tools/options_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.535359 datasphere-0.6.9/yandex/cloud/datasphere/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.644655 datasphere-0.6.9/yandex/cloud/datasphere/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2045 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/app_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      821 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/app_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2843 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1743 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4209 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/folder_budget_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4542 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/folder_budget_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4843 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2917 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1417 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1430 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/node_execution_error_details_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/node_execution_error_details_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3291 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/node_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3828 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/node_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4708 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2715 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/node_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3492 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_data_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4613 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_data_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5007 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3085 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2795 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6829 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20175 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24543 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23351 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11777 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v1/project_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.688167 datasphere-0.6.9/yandex/cloud/datasphere/v2/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2003 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/community_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2855 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/community_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/community_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/community_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14608 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/community_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13893 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/community_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19589 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/community_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9797 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/community_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3140 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6253 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4058 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1577 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4763 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2549 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2955 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/docker_image_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      957 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/docker_image_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3021 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1751 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.696840 datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6389 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/jobs_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17757 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/jobs_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/jobs_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/jobs_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12732 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21128 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22551 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11246 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4783 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13939 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26729 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    31987 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    30603 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15150 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/project_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1670 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/resource_types_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1807 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/resource_types_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/resource_types_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/resource_types_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3887 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/s3_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1497 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/s3_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4638 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2429 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2321 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/secret_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3858 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/secret_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/secret_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/secret_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1345 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/user_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1402 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/user_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/user_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/datasphere/v2/user_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.536463 datasphere-0.6.9/yandex/cloud/iam/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.742404 datasphere-0.6.9/yandex/cloud/iam/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1454 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/api_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1724 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/api_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/api_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/api_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9402 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/api_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11255 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/api_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11954 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6433 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/api_key_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.751732 datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1630 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2056 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10385 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11644 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13154 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7342 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3583 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/iam_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3354 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/iam_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4843 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2883 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1857 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3688 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9752 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12434 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11657 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6178 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1197 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/role_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1049 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/role_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/role_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/role_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3565 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/role_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3458 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/role_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4554 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/role_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2765 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/role_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.767706 datasphere-0.6.9/yandex/cloud/iam/v1/saml/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2669 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1911 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11417 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12211 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12556 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6849 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4080 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6061 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17091 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23042 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16385 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8694 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1954 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/service_account_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2904 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/service_account_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/service_account_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/service_account_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15230 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/service_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13993 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18212 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9895 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/service_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3278 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/user_account_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5440 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/user_account_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/user_account_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/user_account_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2382 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      884 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3160 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2115 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/user_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2508 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      872 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3259 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2162 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.773687 datasphere-0.6.9/yandex/cloud/operation/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2024 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/operation/operation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4080 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/operation/operation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/operation/operation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/operation/operation_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3268 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/operation/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1393 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/operation/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4786 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/operation/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3024 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/operation/operation_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.780722 datasphere-0.6.9/yandex/cloud/priv/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.784017 datasphere-0.6.9/yandex/cloud/priv/access/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7066 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/access/access_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11446 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/access/access_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/access/access_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/access/access_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.539200 datasphere-0.6.9/yandex/cloud/priv/ai/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.539496 datasphere-0.6.9/yandex/cloud/priv/ai/platform/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.806762 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5536 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9014 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20605 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24248 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28428 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11907 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1899 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      165 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6379 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2745 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2349 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2141 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11736 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10066 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16814 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7204 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.540527 datasphere-0.6.9/yandex/cloud/priv/console/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.816933 datasphere-0.6.9/yandex/cloud/priv/console/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3699 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/access_binding_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5113 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/access_binding_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/access_binding_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/access_binding_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5184 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/form_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13004 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/form_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/form_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/form_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2871 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/resource_settings_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2931 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/resource_settings_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/resource_settings_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v1/resource_settings_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.820197 datasphere-0.6.9/yandex/cloud/priv/console/v2/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6190 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v2/form_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17308 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v2/form_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v2/form_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/console/v2/form_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.541946 datasphere-0.6.9/yandex/cloud/priv/datasphere/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.837763 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2097 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      821 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2899 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1763 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5645 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6036 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8725 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3945 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3536 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4180 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5128 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2593 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4521 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10153 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23427 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24457 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    26233 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11053 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.984295 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2838 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      962 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3226 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1694 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2882 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5227 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1800 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      822 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3158 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1646 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1686 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2016 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3674 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3576 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8935 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3974 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4134 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9069 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16228 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23223 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22907 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10010 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4239 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8474 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8160 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12559 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13504 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6158 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    36196 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    42316 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    66265 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27530 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5451 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11310 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12811 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12594 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19704 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8812 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3202 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5630 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13554 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13197 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32326 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13892 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2972 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5388 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19179 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19707 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27038 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11675 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4342 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9374 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5810 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8348 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11448 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5056 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3254 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6255 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9014 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11278 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15510 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7107 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3340 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4026 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3328 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1861 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6523 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/invite_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6288 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/invite_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11164 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5005 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.990453 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7866 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19928 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15958 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    24725 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    31272 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14111 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3265 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6465 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10595 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12758 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14265 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6095 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8017 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12591 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12828 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5581 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.041340 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2416 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2305 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7269 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11522 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3311 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4141 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2948 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3912 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3297 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3667 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5885 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7671 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6997 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7955 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9379 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4317 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7713 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8926 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13689 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6257 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3245 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4143 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3192 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3008 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4098 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5192 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2414 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2364 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4896 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7237 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3577 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7160 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5486 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5379 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9310 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4332 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8729 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    20154 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    57944 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    76840 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    82053 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    34476 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10588 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    29650 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_actions_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_actions_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10677 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_types_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22058 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_types_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_types_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_types_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2295 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1428 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2998 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1594 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3745 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7411 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14542 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17570 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23541 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9913 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2703 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4525 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9804 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8285 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16411 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7199 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1388 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1216 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3769 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3275 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8621 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3748 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.046527 datasphere-0.6.9/yandex/cloud/priv/iam/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.051328 datasphere-0.6.9/yandex/cloud/priv/iam/management/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1784 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/management/cache_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1445 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/management/cache_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3041 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1955 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6389 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/restriction_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9448 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/restriction_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/restriction_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/restriction_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.241447 datasphere-0.6.9/yandex/cloud/priv/iam/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19133 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/access_binding_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27602 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/access_binding_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13351 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5937 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1440 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1429 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10074 2024-01-16 12:00:38.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8328 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12365 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5282 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.259933 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1630 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1774 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12396 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10408 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15757 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7155 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3385 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2236 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3312 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1902 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4409 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3656 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1934 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.267997 datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6916 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9571 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5367 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2733 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4011 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5020 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3123 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1700 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.271483 datasphere-0.6.9/yandex/cloud/priv/iam/v1/compute/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9883 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12962 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8942 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4262 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.295905 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4533 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5387 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5722 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3541 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3095 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2151 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2956 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1546 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3652 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/membership_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3479 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/membership_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3063 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1807 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2055 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1469 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3007 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1751 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3751 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/role_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4457 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/role_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4893 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2507 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7263 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5820 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7360 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3649 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2357 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1090 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3238 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1890 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4637 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/gizmo_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3316 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/gizmo_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5144 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2463 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6007 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6689 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8930 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4121 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2832 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1932 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3144 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1680 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4472 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3231 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3115 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1924 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10719 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9114 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14946 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7494 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2183 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3524 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12899 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12279 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14022 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5847 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.299735 datasphere-0.6.9/yandex/cloud/priv/iam/v1/maintenance/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1727 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1995 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5007 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/membership_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5190 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/membership_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5169 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2870 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.312245 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.316533 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/console/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4346 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4923 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5480 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3599 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.323367 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3110 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4813 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23234 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    21942 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23761 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12571 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2009 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      811 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3028 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1573 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2980 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5827 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9030 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9478 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15464 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8935 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2008 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4677 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14411 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13744 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12466 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5373 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1287 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1352 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7644 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7548 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10574 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4600 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2351 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/operation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      811 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/operation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2980 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1557 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1241 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1012 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5682 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5176 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6765 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3041 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1191 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      849 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6665 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6036 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10526 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4575 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3290 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4498 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6513 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5937 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8996 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4109 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2798 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      165 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8522 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3799 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1736 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      165 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6323 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2745 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3934 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2974 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3234 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1803 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6818 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7624 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5029 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2474 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1240 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1000 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9776 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9185 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14808 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6421 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1759 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1761 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12267 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12390 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12870 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5667 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2374 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4716 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16230 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17780 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    17177 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7764 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1681 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/revoked_credential_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2218 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/revoked_credential_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/revoked_credential_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/revoked_credential_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1529 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2300 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13376 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    14434 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19538 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7962 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3839 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/root_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2638 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/root_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5121 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2445 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.336777 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1745 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2780 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11660 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8638 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    12943 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5824 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3012 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7238 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18643 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16533 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    19103 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8272 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1941 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2390 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22310 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    15517 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    32314 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13669 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3133 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4947 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    22839 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    25016 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    28176 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11780 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1718 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1629 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7138 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8143 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10494 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4524 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1630 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2549 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    18550 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    27356 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16449 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     8681 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.340152 datasphere-0.6.9/yandex/cloud/priv/iam/v1/token/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1685 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/token/iam_token_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1145 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/token/iam_token_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/token/iam_token_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/token/iam_token_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2118 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/token_agent_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1788 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/token_agent_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2788 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1610 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.369516 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3521 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1430 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7376 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3687 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2580 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1398 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3014 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1683 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2727 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1989 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3179 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1721 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4010 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3464 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3334 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1763 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5879 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5761 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13083 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5892 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2336 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2128 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3020 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1601 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4138 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4432 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7626 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3701 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6907 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7244 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11106 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4997 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.372501 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ts/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2451 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2269 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4241 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6737 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9753 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10498 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    10807 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4729 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2283 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1839 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5561 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4221 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7412 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3638 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.375582 datasphere-0.6.9/yandex/cloud/priv/oauth/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     7906 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/claims_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13350 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/claims_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/claims_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/claims_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.391633 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3704 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/claim_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5933 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/claim_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2871 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1515 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2098 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/cloud_user_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2574 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/cloud_user_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/cloud_user_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/cloud_user_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4341 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/login_history_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     4256 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/login_history_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     5062 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     3272 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1781 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/oauth_request_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1316 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/oauth_request_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/oauth_request_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/oauth_request_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11693 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/session_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16752 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/session_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    13682 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9834 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.396076 datasphere-0.6.9/yandex/cloud/priv/operation/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1999 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/operation/operation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2833 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/operation/operation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/operation/operation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/operation/operation_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.406932 datasphere-0.6.9/yandex/cloud/priv/quota/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6813 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/quota/quota_limit_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9901 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/quota/quota_limit_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/quota/quota_limit_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/quota/quota_limit_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     6603 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/quota/quota_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11691 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/quota/quota_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/quota/quota_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/quota/quota_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.411779 datasphere-0.6.9/yandex/cloud/priv/reference/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1704 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/reference/reference_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2651 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/reference/reference_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/reference/reference_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/reference/reference_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1895 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/sensitive_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2594 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/sensitive_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/sensitive_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/sensitive_pb2_grpc.pyi
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:38.556178 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/
+drwxr-xr-x   0 o-gulyaev (212751049) LD\Domain Users (593637566)        0 2024-03-07 14:42:39.421372 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    16394 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    23875 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     9486 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)    11394 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2116 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/resource_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     1574 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/resource_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/resource_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/resource_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2053 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/validation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2603 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/validation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/validation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/priv/validation_pb2_grpc.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2074 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/validation_pb2.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)     2603 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/validation_pb2.pyi
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      159 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/validation_pb2_grpc.py
+-rw-r--r--   0 o-gulyaev (212751049) LD\Domain Users (593637566)      400 2024-01-16 12:00:39.000000 datasphere-0.6.9/yandex/cloud/validation_pb2_grpc.pyi
```

### Comparing `datasphere-0.6.8/PKG-INFO` & `datasphere-0.6.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasphere
-Version: 0.6.8
+Version: 0.6.9
 Summary: Yandex Cloud DataSphere
 Author: Yandex LLC
 Author-email: cloud@support.yandex.ru
 License: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datasphere-0.6.8/README.md` & `datasphere-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere/api/__init__.py` & `datasphere-0.6.9/datasphere/api/__init__.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere/auth.py` & `datasphere-0.6.9/datasphere/auth.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere/channel.py` & `datasphere-0.6.9/datasphere/channel.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere/client.py` & `datasphere-0.6.9/datasphere/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,22 @@
         op = self._poll_operation(op, create_call)
         resp = job_service.CreateProjectJobResponse()
         op.response.Unpack(resp)
         upload_files(list(resp.upload_files), sha256_to_display_path)
         logger.info('created job `%s`', resp.job_id)
         return resp.job_id
 
-    def execute(self, job_id: str, std_logs_offset: int = 0) -> Tuple[operation.Operation, grpc.Call]:
-        self.read_logs(job_id, std_logs_offset)
+    def execute(
+            self,
+            job_id: str,
+            std_logs_offset: int = 0,
+            async_mode: bool = False,
+    ) -> Tuple[operation.Operation, grpc.Call]:
+        if not async_mode:
+            self.read_logs(job_id, std_logs_offset)
         logger.debug('executing job ...')
         return self.stub.Execute.with_call(job_service.ExecuteProjectJobRequest(job_id=job_id), metadata=self.md)
 
     def list(self, project_id: str) -> List[jobs.Job]:
         page_token = None
         jobs = []
         while True:
```

### Comparing `datasphere-0.6.8/datasphere/config.py` & `datasphere-0.6.9/datasphere/config.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere/files.py` & `datasphere-0.6.9/datasphere/files.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere/logs/config.py` & `datasphere-0.6.9/datasphere/logs/config.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere/logs/logging.yaml` & `datasphere-0.6.9/datasphere/logs/logging.yaml`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere/main.py` & `datasphere-0.6.9/datasphere/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     cfg = parse_config(args.config)
 
     py_env = None
     if cfg.env.python:
         logger.debug('defining python env ...')
         py_env = define_py_env(cfg.python_root_modules, cfg.env.python)
 
+    async_mode = args.async_
+
     with tempfile.TemporaryDirectory(prefix='datasphere_') as tmpdir:
         logger.debug('using tmp dir `%s` to prepare local files', tmpdir)
 
         if py_env:
             local_modules = [f.get_file() for f in prepare_local_modules(py_env, tmpdir)]
             # Preserve original local modules paths (before archiving).
             sha256_to_display_path = {f.sha256: p for f, p in zip(local_modules, py_env.local_modules_paths)}
@@ -42,18 +44,19 @@
         job_params = cfg.get_job_params(py_env, local_modules)
         if py_env:
             logger.debug('resulting conda.yaml:\n%s', job_params.env.python_env.conda_yaml)
 
         client = Client(args.token)
 
         job_id = client.create(job_params, cfg, args.project_id, sha256_to_display_path)
-        op, execute_call = client.execute(job_id)
+        op, execute_call = client.execute(job_id, async_mode=async_mode)
         logger.debug('operation `%s` executes the job', op.id)
 
-    client.wait_for_completion(op, execute_call)
+    if not async_mode:
+        client.wait_for_completion(op, execute_call)
 
 
 def attach(args):
     client = Client(args.token)
     # TODO: handle case of completed job, display DS job link with results.
     op, execute_call = client.execute(args.id, std_logs_offset=-1)
     client.wait_for_completion(op, execute_call)
@@ -117,14 +120,15 @@
 
     def add_job_id_argument(parser):
         parser.add_argument('--id', required=True, help='Job ID')
 
     parser_execute = subparsers_job.add_parser('execute', help='Execute job')
     add_project_id_argument(parser_execute)
     parser_execute.add_argument('-c', '--config', required=True, help='Config file', type=argparse.FileType('r'))
+    parser_execute.add_argument('--async', action='store_true', dest='async_', help='Async mode')
     parser_execute.set_defaults(func=execute)
 
     parser_attach = subparsers_job.add_parser('attach', help='Attach to the job execution')
     add_job_id_argument(parser_attach)
     parser_attach.set_defaults(func=attach)
 
     parser_list = subparsers_job.add_parser('list', help='List jobs')
@@ -147,30 +151,25 @@
 
 
 def main():
     arg_parser = build_arg_parser()
 
     args = arg_parser.parse_args()
 
-    if args.func == show_version:
-        args.func(args)
-        check_package_version()
-        return
-
     logs_file_path = configure_logging(args.log_level, args.log_config)
     logger.info('logs file path: %s', logs_file_path)
 
     try:
         args.func(args)
     except Exception as e:
         log_exception(e, logs_file_path)
+        print_logs_files(logs_file_path)
         raise
     finally:
         check_package_version()
-        print_logs_files(logs_file_path)
 
 
 def log_exception(e: Exception, logs_file_path: str):
     title = 'Error occurred'
     md = None
     if isinstance(e, grpc.RpcError):
         md = e.args[0].initial_metadata
```

### Comparing `datasphere-0.6.8/datasphere/pyenv.py` & `datasphere-0.6.9/datasphere/pyenv.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere/utils.py` & `datasphere-0.6.9/datasphere/utils.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/datasphere.egg-info/PKG-INFO` & `datasphere-0.6.9/datasphere.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasphere
-Version: 0.6.8
+Version: 0.6.9
 Summary: Yandex Cloud DataSphere
 Author: Yandex LLC
 Author-email: cloud@support.yandex.ru
 License: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datasphere-0.6.8/datasphere.egg-info/SOURCES.txt` & `datasphere-0.6.9/datasphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/setup.py` & `datasphere-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/tests/test_auth.py` & `datasphere-0.6.9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/tests/test_config.py` & `datasphere-0.6.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/tests/test_files.py` & `datasphere-0.6.9/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/tests/test_main.py` & `datasphere-0.6.9/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
 @fixture
 def system_error_op(execute_op_id, job_id, project_id, expected_download_files) -> operation.Operation:
     return get_op(execute_op_id, job_id, project_id, expected_download_files, OperationStatus.FAILURE)
 
 
 @fixture
 def args(cfg, project_id, oauth_token):
-    return Mock(config=cfg.absolute(), project_id=project_id, token=oauth_token)
+    return Mock(config=cfg.absolute(), project_id=project_id, token=oauth_token, async_=False)
 
 
 @fixture
 def common_logs(execute_op_id) -> List[tuple]:
     return [
         ('datasphere.utils', 10, '`python` is detected as Python interpreter path by common name'),
         ('datasphere.config', 10, '`main.py` is detected as Python main module'),
```

### Comparing `datasphere-0.6.8/tests/test_pyenv.py` & `datasphere-0.6.9/tests/test_pyenv.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/tests/test_utils.py` & `datasphere-0.6.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/access/access_pb2.py` & `datasphere-0.6.9/yandex/cloud/access/access_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/access/access_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/access/access_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/api/operation_pb2.py` & `datasphere-0.6.9/yandex/cloud/api/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/api/operation_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/api/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/api/tools/options_pb2.py` & `datasphere-0.6.9/yandex/cloud/api/tools/options_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/api/tools/options_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/api/tools/options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/app_token_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/app_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/app_token_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/app_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/app_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/folder_budget_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/folder_budget_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/folder_budget_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/folder_budget_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/folder_budget_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/node_execution_error_details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/node_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/node_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/node_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/node_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/node_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/node_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/node_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_data_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_data_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_data_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_data_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v1/project_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v1/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/community_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/community_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/community_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/community_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/community_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/community_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/community_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/community_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/community_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/community_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/community_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/community_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/dataset_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/docker_image_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/docker_image_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/docker_image_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/docker_image_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/docker_image_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/jobs_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/jobs_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/jobs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/project_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/project_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/project_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/project_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/project_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/project_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/resource_types_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/resource_types_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/resource_types_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/resource_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/s3_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/s3_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/s3_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/s3_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/s3_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/secret_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/secret_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/secret_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/user_pb2.py` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/user_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/datasphere/v2/user_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/datasphere/v2/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/api_key_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/api_key_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/api_key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/api_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/api_key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/api_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/api_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/api_key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/api_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/iam_token_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/iam_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/iam_token_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/iam_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/iam_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/key_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/key_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/role_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/role_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/role_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/role_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/role_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/role_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/role_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/role_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/role_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/role_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/role_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/role_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/certificate_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/saml/federation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/service_account_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/service_account_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/service_account_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/service_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/service_account_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/service_account_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/service_account_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/service_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/user_account_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/user_account_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/user_account_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/user_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/user_account_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/user_account_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/user_account_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/operation/operation_pb2.py` & `datasphere-0.6.9/yandex/cloud/operation/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/operation/operation_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/operation/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/operation/operation_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/operation/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/operation/operation_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/operation/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/operation/operation_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/operation/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/operation/operation_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/operation/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/access/access_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/access/access_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/access/access_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/access/access_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/quota_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/quota_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/ai/platform/v1/resource_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/console/v1/access_binding_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/console/v1/access_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/console/v1/access_binding_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/console/v1/access_binding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/console/v1/form_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/console/v1/form_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/console/v1/form_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/console/v1/form_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/console/v1/resource_settings_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/console/v1/resource_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/console/v1/resource_settings_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/console/v1/resource_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/console/v2/form_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/console/v2/form_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/console/v2/form_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/console/v2/form_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/app_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/app_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/operation_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/operation_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_data_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v1/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/access_binding_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/admin_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/alpha_flag_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/checkpoint_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_quota_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/community_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/data_proc_template_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/dataset_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/docker_image_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/feature_property_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/foundation_model_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/internal_storage_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/invite_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/invite_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/invite_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/invite_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/invite_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/jobs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/jobs/project_job_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/model_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/navigation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/navigation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/billing_spec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/docker_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/healthcheck_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/instance_spec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_alias_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_deployer_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/node_spec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/policies_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/runtime_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/servant_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/nodedeployer/triton_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_ide_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/project_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_actions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_types_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_types_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/resource_types_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/resource_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_keys_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/s3_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/secret_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/datasphere/v2/user_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/management/cache_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/management/cache_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/management/cache_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/management/cache_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/management/cache_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/restriction_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/restriction_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/restriction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/access_binding_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/access_binding_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/access_binding_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/access_binding_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/access_binding_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/api_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/access_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/delegation_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/awscompatibility/temporary_access_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/access_binding_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/backoffice/permission_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/compute/os_login_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/access_binding_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/membership_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/membership_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/membership_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/os_login_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/os_login_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/role_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/role_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/role_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/role_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/role_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/service_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/console/user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/gizmo_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/gizmo_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/gizmo_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/gizmo_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/gizmo_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_cookie_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_credential_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_credential_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_session_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_token_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_token_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/iam_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/maintenance/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/membership_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/membership_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/membership_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/console/totp_profile_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/hardware/totp_profile_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/mfa/totp_profile_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_client_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/oauth_scope_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/operation_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/operation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/operation_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/operation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/os_login_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/permission_stage_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_limit_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_limit_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/quota_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_issue_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/refresh_token_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/resource_type_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/restriction_type_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/revoked_credential_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/revoked_credential_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/revoked_credential_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/revoked_credential_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/role_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/root_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/root_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/root_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/root_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/root_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/certificate_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/saml/federation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/service_control_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/ssh_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/subject_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/token/iam_token_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/token/iam_token_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/token/iam_token_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/token/iam_token_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/token_agent_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/token_agent_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/token_agent_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/token_agent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/token_agent_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/agreement_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/auth_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/health_check_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/passport_federation_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/policy_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/roles_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/service_account_access_key_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/transitional/user_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/ts/iam_token_service_subject_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_cookie_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/iam/v1/yandex_passport_user_account_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/claims_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/oauth/claims_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/claims_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/oauth/claims_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/claim_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/claim_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/claim_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/claim_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/claim_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/cloud_user_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/cloud_user_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/cloud_user_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/cloud_user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/login_history_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/login_history_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/login_history_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/login_history_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/login_history_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/oauth_request_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/oauth_request_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/oauth_request_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/oauth_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/session_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/session_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/session_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/session_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/oauth/v1/session_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/operation/operation_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/operation/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/operation/operation_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/operation/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/quota/quota_limit_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/quota/quota_limit_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/quota/quota_limit_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/quota/quota_limit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/quota/quota_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/quota/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/quota/quota_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/quota/quota_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/reference/reference_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/reference/reference_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/reference/reference_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/reference/reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/sensitive_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/sensitive_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/sensitive_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/sensitive_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/access_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.py` & `datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.pyi` & `datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/access_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/resource_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/servicecontrol/v1/resource_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/servicecontrol/v1/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/validation_pb2.py` & `datasphere-0.6.9/yandex/cloud/priv/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/priv/validation_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/priv/validation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/validation_pb2.py` & `datasphere-0.6.9/yandex/cloud/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `datasphere-0.6.8/yandex/cloud/validation_pb2.pyi` & `datasphere-0.6.9/yandex/cloud/validation_pb2.pyi`

 * *Files identical despite different names*

