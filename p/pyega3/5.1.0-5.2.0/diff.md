# Comparing `tmp/pyega3-5.1.0.tar.gz` & `tmp/pyega3-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyega3-5.1.0.tar", last modified: Thu Oct 26 13:35:53 2023, max compression
+gzip compressed data, was "pyega3-5.2.0.tar", last modified: Wed Apr  3 08:37:28 2024, max compression
```

## Comparing `pyega3-5.1.0.tar` & `pyega3-5.2.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:35:53.963941 pyega3-5.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2022-01-10 16:11:49.000000 pyega3-5.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-02-10 00:47:36.000000 pyega3-5.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13543 2023-10-26 13:35:53.963941 pyega3-5.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12985 2023-02-10 00:47:36.000000 pyega3-5.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:35:53.959941 pyega3-5.1.0/pyega3/
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-10-26 13:27:04.000000 pyega3-5.1.0/pyega3/VERSION
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-10 16:11:49.000000 pyega3-5.1.0/pyega3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:35:53.960941 pyega3-5.1.0/pyega3/config/
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-01-10 16:11:49.000000 pyega3-5.1.0/pyega3/config/default_credential_file.json
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-08-10 15:52:25.000000 pyega3-5.1.0/pyega3/config/default_server_file.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:35:53.961941 pyega3-5.1.0/pyega3/libs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 00:34:25.000000 pyega3-5.1.0/pyega3/libs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2560 2023-10-25 17:11:47.000000 pyega3-5.1.0/pyega3/libs/auth_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3211 2023-02-10 00:47:36.000000 pyega3-5.1.0/pyega3/libs/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     1231 2023-02-10 00:34:25.000000 pyega3-5.1.0/pyega3/libs/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     4419 2023-10-25 17:11:47.000000 pyega3-5.1.0/pyega3/libs/data_client.py
--rw-rw-rw-   0 root         (0) root         (0)    16857 2023-10-13 14:54:03.000000 pyega3-5.1.0/pyega3/libs/data_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3766 2023-02-10 00:47:36.000000 pyega3-5.1.0/pyega3/libs/data_set.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-10-13 14:54:03.000000 pyega3-5.1.0/pyega3/libs/error.py
--rw-rw-rw-   0 root         (0) root         (0)     1733 2023-02-10 00:34:25.000000 pyega3-5.1.0/pyega3/libs/pretty_printing.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2023-08-10 15:16:56.000000 pyega3-5.1.0/pyega3/libs/server_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1835 2023-10-25 17:11:47.000000 pyega3-5.1.0/pyega3/libs/stats.py
--rw-rw-rw-   0 root         (0) root         (0)     3572 2023-02-10 00:34:25.000000 pyega3-5.1.0/pyega3/libs/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     7476 2023-10-12 16:50:18.000000 pyega3-5.1.0/pyega3/pyega3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:35:53.960941 pyega3-5.1.0/pyega3.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13543 2023-10-26 13:35:53.000000 pyega3-5.1.0/pyega3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1570 2023-10-26 13:35:53.000000 pyega3-5.1.0/pyega3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-26 13:35:53.000000 pyega3-5.1.0/pyega3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-10-26 13:35:53.000000 pyega3-5.1.0/pyega3.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-10-26 13:35:53.000000 pyega3-5.1.0/pyega3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-26 13:35:53.000000 pyega3-5.1.0/pyega3.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-10-26 13:35:53.964941 pyega3-5.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2024 2023-08-10 14:33:50.000000 pyega3-5.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:35:53.961941 pyega3-5.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:35:53.961941 pyega3-5.1.0/tests/functional/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/functional/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/functional/test_display_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1915 2023-02-13 12:03:29.000000 pyega3-5.1.0/tests/functional/test_download.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2023-02-13 12:03:29.000000 pyega3-5.1.0/tests/functional/test_htsget.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-02-13 12:03:29.000000 pyega3-5.1.0/tests/functional/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:35:53.963941 pyega3-5.1.0/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2023-10-25 17:11:47.000000 pyega3-5.1.0/tests/unit/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3804 2023-10-12 16:50:18.000000 pyega3-5.1.0/tests/unit/mock_data_server.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_client_ip.py
--rw-rw-rw-   0 root         (0) root         (0)     1136 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     5715 2023-10-12 16:50:18.000000 pyega3-5.1.0/tests/unit/test_delete_temporary_files.py
--rw-rw-rw-   0 root         (0) root         (0)     4146 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_download_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    14919 2023-10-25 17:11:47.000000 pyega3-5.1.0/tests/unit/test_download_file.py
--rw-rw-rw-   0 root         (0) root         (0)     7447 2023-02-13 12:03:29.000000 pyega3-5.1.0/tests/unit/test_download_file_slice.py
--rw-rw-rw-   0 root         (0) root         (0)     1376 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_generate_output_filename.py
--rw-rw-rw-   0 root         (0) root         (0)     2145 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_get_file_name_size_md5.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_list_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     1281 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_list_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1015 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_md5.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_merge_bin_files.py
--rw-rw-rw-   0 root         (0) root         (0)     2724 2023-10-25 17:11:47.000000 pyega3-5.1.0/tests/unit/test_openid.py
--rw-rw-rw-   0 root         (0) root         (0)     2060 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_pretty_printing.py
--rw-rw-rw-   0 root         (0) root         (0)     7462 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_save_to_with_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     6892 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_save_to_with_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1741 2023-10-12 09:41:48.000000 pyega3-5.1.0/tests/unit/test_server_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2197 2023-02-10 00:47:36.000000 pyega3-5.1.0/tests/unit/test_verify_output_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:37:28.948443 pyega3-5.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2022-01-10 16:11:49.000000 pyega3-5.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-02-10 00:48:40.000000 pyega3-5.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13656 2024-04-03 08:37:28.949442 pyega3-5.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13098 2024-03-19 14:41:13.000000 pyega3-5.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:37:28.877441 pyega3-5.2.0/pyega3/
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-04-02 16:35:12.000000 pyega3-5.2.0/pyega3/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-10 16:11:49.000000 pyega3-5.2.0/pyega3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:37:28.883441 pyega3-5.2.0/pyega3/config/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2022-01-10 16:11:49.000000 pyega3-5.2.0/pyega3/config/default_credential_file.json
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-08-10 15:52:25.000000 pyega3-5.2.0/pyega3/config/default_server_file.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:37:28.885441 pyega3-5.2.0/pyega3/libs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 00:34:59.000000 pyega3-5.2.0/pyega3/libs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2023-10-25 17:11:47.000000 pyega3-5.2.0/pyega3/libs/auth_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3211 2023-02-10 00:48:40.000000 pyega3-5.2.0/pyega3/libs/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2023-02-10 00:34:59.000000 pyega3-5.2.0/pyega3/libs/credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)     4419 2023-10-25 17:11:47.000000 pyega3-5.2.0/pyega3/libs/data_client.py
+-rw-rw-rw-   0 root         (0) root         (0)    17190 2024-04-02 15:56:21.000000 pyega3-5.2.0/pyega3/libs/data_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3766 2023-02-13 12:03:58.000000 pyega3-5.2.0/pyega3/libs/data_set.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-10-13 14:54:03.000000 pyega3-5.2.0/pyega3/libs/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2024-04-02 15:56:21.000000 pyega3-5.2.0/pyega3/libs/file_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2023-02-10 00:34:59.000000 pyega3-5.2.0/pyega3/libs/pretty_printing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-08-10 15:16:56.000000 pyega3-5.2.0/pyega3/libs/server_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1835 2023-10-25 17:11:47.000000 pyega3-5.2.0/pyega3/libs/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     3572 2023-02-10 00:34:59.000000 pyega3-5.2.0/pyega3/libs/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     7476 2023-10-12 16:50:19.000000 pyega3-5.2.0/pyega3/pyega3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:37:28.878441 pyega3-5.2.0/pyega3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13656 2024-04-03 08:37:28.000000 pyega3-5.2.0/pyega3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1628 2024-04-03 08:37:28.000000 pyega3-5.2.0/pyega3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:37:28.000000 pyega3-5.2.0/pyega3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-03 08:37:28.000000 pyega3-5.2.0/pyega3.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-03 08:37:28.000000 pyega3-5.2.0/pyega3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 08:37:28.000000 pyega3-5.2.0/pyega3.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-03 08:37:28.949442 pyega3-5.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2024 2023-08-10 14:34:19.000000 pyega3-5.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:37:28.885441 pyega3-5.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:37:28.945443 pyega3-5.2.0/tests/functional/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/functional/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/functional/test_display_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1915 2023-02-13 12:03:58.000000 pyega3-5.2.0/tests/functional/test_download.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2023-02-13 12:03:58.000000 pyega3-5.2.0/tests/functional/test_htsget.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-02-13 12:03:58.000000 pyega3-5.2.0/tests/functional/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:37:28.948443 pyega3-5.2.0/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2023-10-25 17:11:47.000000 pyega3-5.2.0/tests/unit/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2023-10-12 16:50:19.000000 pyega3-5.2.0/tests/unit/mock_data_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_client_ip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1136 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)     5715 2023-10-12 16:50:19.000000 pyega3-5.2.0/tests/unit/test_delete_temporary_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     4146 2023-02-13 12:03:58.000000 pyega3-5.2.0/tests/unit/test_download_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    14919 2023-10-25 17:11:47.000000 pyega3-5.2.0/tests/unit/test_download_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     7447 2023-02-13 12:03:58.000000 pyega3-5.2.0/tests/unit/test_download_file_slice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3108 2024-04-02 15:51:29.000000 pyega3-5.2.0/tests/unit/test_file_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_generate_output_filename.py
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_get_file_name_size_md5.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_list_datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_list_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_md5.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_merge_bin_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     2724 2023-10-25 17:11:47.000000 pyega3-5.2.0/tests/unit/test_openid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_pretty_printing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7462 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_save_to_with_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     6892 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_save_to_with_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1741 2023-10-12 09:41:48.000000 pyega3-5.2.0/tests/unit/test_server_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2023-02-10 00:48:40.000000 pyega3-5.2.0/tests/unit/test_verify_output_dir.py
```

### Comparing `pyega3-5.1.0/LICENSE` & `pyega3-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/PKG-INFO` & `pyega3-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyega3
-Version: 5.1.0
+Version: 5.2.0
 Summary: EGA python client
 Home-page: https://github.com/EGA-archive/ega-download-client
 Author: EGA team
 Author-email: ega-helpdesk@ebi.ac.uk
 License: Apache License, Version 2.0
 Keywords: EGA,archive
 Classifier: Development Status :: 3 - Alpha
@@ -340,7 +340,10 @@
 If, after troubleshooting an issue, you are still experiencing difficulties, please email EGA Helpdesk (helpdesk@ega-archive.org) with the following information:
 * Attach the log file (pyega3_output.log) located in the directory where pyEGA3 is running
 * Indicate the compute environment you are running pyEGA3 in: compute cluster, single machine, other (please describe).
 
 ## Attribution
 
 Parts of pyEGA3 are derived from [pyEGA](https://github.com/blachlylab/pyega) developed by James Blachly.
+
+## Development
+See guide in updating and releasing updates to client in the [Development](development.md) page.
```

### Comparing `pyega3-5.1.0/README.md` & `pyega3-5.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -323,7 +323,10 @@
 If, after troubleshooting an issue, you are still experiencing difficulties, please email EGA Helpdesk (helpdesk@ega-archive.org) with the following information:
 * Attach the log file (pyega3_output.log) located in the directory where pyEGA3 is running
 * Indicate the compute environment you are running pyEGA3 in: compute cluster, single machine, other (please describe).
 
 ## Attribution
 
 Parts of pyEGA3 are derived from [pyEGA](https://github.com/blachlylab/pyega) developed by James Blachly.
+
+## Development
+See guide in updating and releasing updates to client in the [Development](development.md) page.
```

### Comparing `pyega3-5.1.0/pyega3/libs/auth_client.py` & `pyega3-5.2.0/pyega3/libs/auth_client.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/libs/commands.py` & `pyega3-5.2.0/pyega3/libs/commands.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/libs/credentials.py` & `pyega3-5.2.0/pyega3/libs/credentials.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/libs/data_client.py` & `pyega3-5.2.0/pyega3/libs/data_client.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/libs/data_file.py` & `pyega3-5.2.0/pyega3/libs/data_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 import psutil
 from tqdm import tqdm
 
 from pyega3.libs import utils
 from pyega3.libs.error import DataFileError, SliceError, MD5MismatchError, MaxRetriesReachedError
 from pyega3.libs.stats import Stats
 
+from pyega3.libs.file_format import is_bam_or_cram_file, autocorrect_format_in_genomic_range_args
+
 DOWNLOAD_FILE_MEMORY_BUFFER_SIZE = 32 * 1024
 
+SUPPORTED_FILE_FORMATS = ["BAM", "CRAM", "VCF", "BCF"]
+
 
 class DataFile:
     DEFAULT_SLICE_SIZE = 100 * 1024 * 1024
     temporary_files_should_be_deleted = False
 
     def __init__(self, data_client, file_id,
                  display_file_name=None,
@@ -288,15 +292,18 @@
             self._check_and_warn_if_file_is_bigger_than_free_space()
             output_file = self.generate_output_filename(output_dir, genomic_range_args)
             temporary_directory = self._create_temp_dir(output_file)
 
             if self.does_file_exist(output_file):
                 DataFile.print_local_file_info('Local file exists:', output_file, self.unencrypted_checksum)
             elif DataFile.is_genomic_range(genomic_range_args):
-                self._download_htsget_slice(genomic_range_args, max_retries, output_file, retry_wait)
+                corrected_genomic_range_args = autocorrect_format_in_genomic_range_args(self.name,
+                                                                                        genomic_range_args,
+                                                                                        SUPPORTED_FILE_FORMATS)
+                self._download_htsget_slice(corrected_genomic_range_args, max_retries, output_file, retry_wait)
             else:
                 stats_list = self._download_whole_file(max_retries, max_slice_size, num_connections, output_file,
                                                        retry_wait, temporary_directory)
                 download_stats_list.extend(stats_list)
 
         return download_stats_list
 
@@ -310,15 +317,15 @@
             logging.warning(f"The size of the file that you want to download is bigger than your free space in this "
                             f"location")
 
     def _download_htsget_slice(self, genomic_range_args, max_retries, output_file, retry_wait):
         if self.data_client.api_version == 1:
             endpoint_type = "files"
         else:
-            endpoint_type = "htsget/reads" if self.is_bam_or_cram_file(self.name) else "htsget/variants"
+            endpoint_type = "htsget/reads" if is_bam_or_cram_file(self.name) else "htsget/variants"
         with open(output_file, 'wb') as output:
             htsget.get(
                 f"{self.data_client.htsget_url}/{endpoint_type}/{self.id}",
                 output,
                 reference_name=genomic_range_args[0], reference_md5=genomic_range_args[1],
                 start=genomic_range_args[2], end=genomic_range_args[3],
                 data_format=genomic_range_args[4],
@@ -382,15 +389,12 @@
     def _format_stats_error_reason(self, e):
         error_class_name = e.__class__.__name__
         error_reason = str(e)
         if isinstance(e, DataFileError):
             error_reason = e.message
         return error_class_name, error_reason
 
-    def is_bam_or_cram_file(self, name: str):
-        return re.search("\.bam", name, re.IGNORECASE) or re.search("\.cram", name, re.IGNORECASE)
-
     def delete_temporary_folder(self, temporary_directory):
         try:
             shutil.rmtree(temporary_directory)
         except FileNotFoundError as ex:
             logging.error(f'Could not delete the temporary folder: {ex}')
```

### Comparing `pyega3-5.1.0/pyega3/libs/data_set.py` & `pyega3-5.2.0/pyega3/libs/data_set.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/libs/error.py` & `pyega3-5.2.0/pyega3/libs/error.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/libs/pretty_printing.py` & `pyega3-5.2.0/pyega3/libs/pretty_printing.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/libs/server_config.py` & `pyega3-5.2.0/pyega3/libs/server_config.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/libs/stats.py` & `pyega3-5.2.0/pyega3/libs/stats.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/libs/utils.py` & `pyega3-5.2.0/pyega3/libs/utils.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3/pyega3.py` & `pyega3-5.2.0/pyega3/pyega3.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/pyega3.egg-info/PKG-INFO` & `pyega3-5.2.0/pyega3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyega3
-Version: 5.1.0
+Version: 5.2.0
 Summary: EGA python client
 Home-page: https://github.com/EGA-archive/ega-download-client
 Author: EGA team
 Author-email: ega-helpdesk@ebi.ac.uk
 License: Apache License, Version 2.0
 Keywords: EGA,archive
 Classifier: Development Status :: 3 - Alpha
@@ -340,7 +340,10 @@
 If, after troubleshooting an issue, you are still experiencing difficulties, please email EGA Helpdesk (helpdesk@ega-archive.org) with the following information:
 * Attach the log file (pyega3_output.log) located in the directory where pyEGA3 is running
 * Indicate the compute environment you are running pyEGA3 in: compute cluster, single machine, other (please describe).
 
 ## Attribution
 
 Parts of pyEGA3 are derived from [pyEGA](https://github.com/blachlylab/pyega) developed by James Blachly.
+
+## Development
+See guide in updating and releasing updates to client in the [Development](development.md) page.
```

### Comparing `pyega3-5.1.0/pyega3.egg-info/SOURCES.txt` & `pyega3-5.2.0/pyega3.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 pyega3/libs/auth_client.py
 pyega3/libs/commands.py
 pyega3/libs/credentials.py
 pyega3/libs/data_client.py
 pyega3/libs/data_file.py
 pyega3/libs/data_set.py
 pyega3/libs/error.py
+pyega3/libs/file_format.py
 pyega3/libs/pretty_printing.py
 pyega3/libs/server_config.py
 pyega3/libs/stats.py
 pyega3/libs/utils.py
 tests/__init__.py
 tests/functional/__init__.py
 tests/functional/test_display_info.py
@@ -38,14 +39,15 @@
 tests/unit/test_client_ip.py
 tests/unit/test_commands.py
 tests/unit/test_credentials.py
 tests/unit/test_delete_temporary_files.py
 tests/unit/test_download_dataset.py
 tests/unit/test_download_file.py
 tests/unit/test_download_file_slice.py
+tests/unit/test_file_format.py
 tests/unit/test_generate_output_filename.py
 tests/unit/test_get_file_name_size_md5.py
 tests/unit/test_list_datasets.py
 tests/unit/test_list_files.py
 tests/unit/test_md5.py
 tests/unit/test_merge_bin_files.py
 tests/unit/test_openid.py
```

### Comparing `pyega3-5.1.0/setup.py` & `pyega3-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/functional/test_download.py` & `pyega3-5.2.0/tests/functional/test_download.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/functional/test_htsget.py` & `pyega3-5.2.0/tests/functional/test_htsget.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/functional/util.py` & `pyega3-5.2.0/tests/functional/util.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/conftest.py` & `pyega3-5.2.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/mock_data_server.py` & `pyega3-5.2.0/tests/unit/mock_data_server.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_commands.py` & `pyega3-5.2.0/tests/unit/test_commands.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_credentials.py` & `pyega3-5.2.0/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_delete_temporary_files.py` & `pyega3-5.2.0/tests/unit/test_delete_temporary_files.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_download_dataset.py` & `pyega3-5.2.0/tests/unit/test_download_dataset.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_download_file.py` & `pyega3-5.2.0/tests/unit/test_download_file.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_download_file_slice.py` & `pyega3-5.2.0/tests/unit/test_download_file_slice.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_generate_output_filename.py` & `pyega3-5.2.0/tests/unit/test_generate_output_filename.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_get_file_name_size_md5.py` & `pyega3-5.2.0/tests/unit/test_get_file_name_size_md5.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_list_datasets.py` & `pyega3-5.2.0/tests/unit/test_list_datasets.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_list_files.py` & `pyega3-5.2.0/tests/unit/test_list_files.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_md5.py` & `pyega3-5.2.0/tests/unit/test_md5.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_merge_bin_files.py` & `pyega3-5.2.0/tests/unit/test_merge_bin_files.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_openid.py` & `pyega3-5.2.0/tests/unit/test_openid.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_pretty_printing.py` & `pyega3-5.2.0/tests/unit/test_pretty_printing.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_save_to_with_dataset.py` & `pyega3-5.2.0/tests/unit/test_save_to_with_dataset.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_save_to_with_file.py` & `pyega3-5.2.0/tests/unit/test_save_to_with_file.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_server_config.py` & `pyega3-5.2.0/tests/unit/test_server_config.py`

 * *Files identical despite different names*

### Comparing `pyega3-5.1.0/tests/unit/test_verify_output_dir.py` & `pyega3-5.2.0/tests/unit/test_verify_output_dir.py`

 * *Files identical despite different names*

