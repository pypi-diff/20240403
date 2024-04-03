# Comparing `tmp/galaxy-test-api-23.2.1.tar.gz` & `tmp/galaxy-test-api-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_api/dist/.tmp-qjkjv54x/galaxy-test-api-23.2.1.tar", last modified: Thu Feb 22 03:55:46 2024, max compression
+gzip compressed data, was "galaxy-test-api-24.0.0.tar", last modified: Wed Apr  3 02:46:08 2024, max compression
```

## Comparing `galaxy-test-api-23.2.1.tar` & `galaxy-test-api-24.0.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/galaxy_test/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/galaxy_test/api/cwl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/cwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/embed_test_1.gxwf.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/embed_test_1_tool.gxtool.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/sharable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_container_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    33392 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_dataset_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    38871 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_display_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_drs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19567 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_folder_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    42155 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    72077 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_history_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_history_contents_provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    53210 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_page_revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23398 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_short_term_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_tool_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   148182 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    46354 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_tools_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_tours.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    27506 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_workflow_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)   283097 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_workflows_cwl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/api/test_workflows_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/galaxy_test_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/galaxy_test_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/galaxy_test_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/galaxy_test_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/galaxy_test_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/galaxy_test_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-22 03:55:46.000000 galaxy-test-api-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-test-api-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.147843 galaxy-test-api-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    15479 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-03 02:46:08.147843 galaxy-test-api-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.135843 galaxy-test-api-24.0.0/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.143843 galaxy-test-api-24.0.0/galaxy_test/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.143843 galaxy-test-api-24.0.0/galaxy_test/api/cwl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/cwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/embed_test_1.gxwf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/embed_test_1_tool.gxtool.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/sharable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_container_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33392 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_dataset_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38871 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_display_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19567 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_folder_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51434 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78017 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_history_contents_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53965 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_page_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_short_term_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tool_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148593 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46383 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tools_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27526 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_workflow_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)   289951 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_workflows_cwl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_workflows_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.147843 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-03 02:46:08.147843 galaxy-test-api-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-test-api-23.2.1/HISTORY.rst` & `galaxy-test-api-24.0.0/HISTORY.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,56 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Only check access permissions in ``/api/{history_dataset_collection_id}/contents/{dataset_collection_id}`` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17444 <https://github.com/galaxyproject/galaxy/pull/17444>`_
+* Fix ``test_index_advanced_filter`` API test re-running by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17547 <https://github.com/galaxyproject/galaxy/pull/17547>`_
+* Limit new anon histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17657 <https://github.com/galaxyproject/galaxy/pull/17657>`_
+* Fix step type serialization for StoredWorkflowDetailed models by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17716 <https://github.com/galaxyproject/galaxy/pull/17716>`_
+* Fix histories API index_query serialization by `@davelopez <https://github.com/davelopez>`_ in `#17726 <https://github.com/galaxyproject/galaxy/pull/17726>`_
+* Fix source history update_time being updated when importing a public history by `@jmchilton <https://github.com/jmchilton>`_ in `#17728 <https://github.com/galaxyproject/galaxy/pull/17728>`_
+* Also set extension and metadata on copies of job outputs when finishing job by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17777 <https://github.com/galaxyproject/galaxy/pull/17777>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+* Fix archived histories mixing with active in histories list by `@davelopez <https://github.com/davelopez>`_ in `#17856 <https://github.com/galaxyproject/galaxy/pull/17856>`_
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Create pydantic model for the return of show operation -  get: `/api/jobs/{job_id}`  by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17153 <https://github.com/galaxyproject/galaxy/pull/17153>`_
+* Don't require admin user to list ``/api/tool_data`` by `@jozh2008 <https://github.com/jozh2008>`_ in `#17161 <https://github.com/galaxyproject/galaxy/pull/17161>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Reuse test instance during non-integration tests by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17234 <https://github.com/galaxyproject/galaxy/pull/17234>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Add ``__KEEP_SUCCESS_DATASETS__`` by `@lldelisle <https://github.com/lldelisle>`_ in `#17294 <https://github.com/galaxyproject/galaxy/pull/17294>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Combines legacy qv-pattern and advanced filter pattern in history index endpoint by `@guerler <https://github.com/guerler>`_ in `#17368 <https://github.com/galaxyproject/galaxy/pull/17368>`_
+* Cancel all active jobs when the user is deleted by `@davelopez <https://github.com/davelopez>`_ in `#17390 <https://github.com/galaxyproject/galaxy/pull/17390>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Purge `groups` and `roles` from DB (for real) by `@davelopez <https://github.com/davelopez>`_ in `#17411 <https://github.com/galaxyproject/galaxy/pull/17411>`_
+* Refactor Workflow API routes - Part 1 by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17463 <https://github.com/galaxyproject/galaxy/pull/17463>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+* Restore histories API behavior for `keys` query parameter by `@davelopez <https://github.com/davelopez>`_ in `#17779 <https://github.com/galaxyproject/galaxy/pull/17779>`_
+* Fix datasets API custom keys encoding by `@davelopez <https://github.com/davelopez>`_ in `#17793 <https://github.com/galaxyproject/galaxy/pull/17793>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-api-23.2.1/LICENSE` & `galaxy-test-api-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/PKG-INFO` & `galaxy-test-api-24.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: galaxy-test-api
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy API tests
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: driver
 License-File: LICENSE
+Requires-Dist: galaxy-test-base
+Requires-Dist: pytest
+Requires-Dist: python-dateutil
+Requires-Dist: requests
+Requires-Dist: tuspy
+Provides-Extra: driver
+Requires-Dist: galaxy-test-driver; extra == "driver"
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-api.svg
    :target: https://pypi.org/project/galaxy-test-api/
 
 
 
@@ -44,14 +50,57 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Only check access permissions in ``/api/{history_dataset_collection_id}/contents/{dataset_collection_id}`` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17444 <https://github.com/galaxyproject/galaxy/pull/17444>`_
+* Fix ``test_index_advanced_filter`` API test re-running by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17547 <https://github.com/galaxyproject/galaxy/pull/17547>`_
+* Limit new anon histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17657 <https://github.com/galaxyproject/galaxy/pull/17657>`_
+* Fix step type serialization for StoredWorkflowDetailed models by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17716 <https://github.com/galaxyproject/galaxy/pull/17716>`_
+* Fix histories API index_query serialization by `@davelopez <https://github.com/davelopez>`_ in `#17726 <https://github.com/galaxyproject/galaxy/pull/17726>`_
+* Fix source history update_time being updated when importing a public history by `@jmchilton <https://github.com/jmchilton>`_ in `#17728 <https://github.com/galaxyproject/galaxy/pull/17728>`_
+* Also set extension and metadata on copies of job outputs when finishing job by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17777 <https://github.com/galaxyproject/galaxy/pull/17777>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+* Fix archived histories mixing with active in histories list by `@davelopez <https://github.com/davelopez>`_ in `#17856 <https://github.com/galaxyproject/galaxy/pull/17856>`_
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Create pydantic model for the return of show operation -  get: `/api/jobs/{job_id}`  by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17153 <https://github.com/galaxyproject/galaxy/pull/17153>`_
+* Don't require admin user to list ``/api/tool_data`` by `@jozh2008 <https://github.com/jozh2008>`_ in `#17161 <https://github.com/galaxyproject/galaxy/pull/17161>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Reuse test instance during non-integration tests by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17234 <https://github.com/galaxyproject/galaxy/pull/17234>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Add ``__KEEP_SUCCESS_DATASETS__`` by `@lldelisle <https://github.com/lldelisle>`_ in `#17294 <https://github.com/galaxyproject/galaxy/pull/17294>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Combines legacy qv-pattern and advanced filter pattern in history index endpoint by `@guerler <https://github.com/guerler>`_ in `#17368 <https://github.com/galaxyproject/galaxy/pull/17368>`_
+* Cancel all active jobs when the user is deleted by `@davelopez <https://github.com/davelopez>`_ in `#17390 <https://github.com/galaxyproject/galaxy/pull/17390>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Purge `groups` and `roles` from DB (for real) by `@davelopez <https://github.com/davelopez>`_ in `#17411 <https://github.com/galaxyproject/galaxy/pull/17411>`_
+* Refactor Workflow API routes - Part 1 by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17463 <https://github.com/galaxyproject/galaxy/pull/17463>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+* Restore histories API behavior for `keys` query parameter by `@davelopez <https://github.com/davelopez>`_ in `#17779 <https://github.com/galaxyproject/galaxy/pull/17779>`_
+* Fix datasets API custom keys encoding by `@davelopez <https://github.com/davelopez>`_ in `#17793 <https://github.com/galaxyproject/galaxy/pull/17793>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/_framework.py` & `galaxy-test-api-24.0.0/galaxy_test/api/_framework.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/sharable.py` & `galaxy-test-api-24.0.0/galaxy_test/api/sharable.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_configuration.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_container_resolution.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_container_resolution.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_dataset_collections.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_dataset_collections.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_datasets.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_datatypes.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_display_applications.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_display_applications.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_drs.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_drs.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_folder_contents.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_folder_contents.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_folders.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_folders.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     @requires_new_library
     def test_create_without_name_raises_400(self):
         root_folder_id = self.library["root_folder_id"]
         data = {
             "description": "Description only",
         }
-        create_response = self._post(f"folders/{root_folder_id}", data=data, admin=True)
+        create_response = self._post(f"folders/{root_folder_id}", data=data, admin=True, json=True)
         self._assert_status_code_is(create_response, 400)
 
     @requires_new_library
     def test_permissions(self):
         folder = self._create_folder("Test Permissions Folder")
         folder_id = folder["id"]
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_framework.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_framework.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_group_roles.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_group_roles.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_group_users.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_group_users.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_groups.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_groups.py`

 * *Files 24% similar despite different names*

```diff
@@ -68,18 +68,18 @@
 
     def test_show_unknown_raises_400(self):
         group_id = "invalid-group-id"
         response = self._get(f"groups/{group_id}", admin=True)
         self._assert_status_code_is(response, 400)
 
     def test_update(self):
-        group = self.test_create_valid(group_name="group-test")
+        group = self.test_create_valid(group_name=f"group-test-{self.dataset_populator.get_random_name()}")
 
         group_id = group["id"]
-        updated_name = "group-test-updated"
+        updated_name = f"group-test-updated-{self.dataset_populator.get_random_name()}"
         update_payload = {
             "name": updated_name,
         }
         update_response = self._put(f"groups/{group_id}", data=update_payload, admin=True, json=True)
         self._assert_status_code_is_ok(update_response)
 
     def test_update_only_admin(self):
@@ -97,14 +97,63 @@
         updated_name = group_a["name"]
         update_payload = {
             "name": updated_name,
         }
         update_response = self._put(f"groups/{group_b_id}", data=update_payload, admin=True, json=True)
         self._assert_status_code_is(update_response, 409)
 
+    def test_delete(self):
+        group = self.test_create_valid()
+        group_id = group["id"]
+        delete_response = self._delete(f"groups/{group_id}", admin=True)
+        self._assert_status_code_is_ok(delete_response)
+
+    def test_delete_duplicating_name_raises_409(self):
+        group = self.test_create_valid()
+        group_id = group["id"]
+        group_name = group["name"]
+
+        delete_response = self._delete(f"groups/{group_id}", admin=True)
+        self._assert_status_code_is_ok(delete_response)
+
+        # Create a new group with the same name as the deleted one is not allowed
+        payload = self._build_valid_group_payload(group_name)
+        response = self._post("groups", payload, admin=True, json=True)
+        self._assert_status_code_is(response, 409)
+
+    def test_purge(self):
+        group = self.test_create_valid()
+        group_id = group["id"]
+
+        # Delete and purge the group
+        delete_response = self._delete(f"groups/{group_id}", admin=True)
+        self._assert_status_code_is_ok(delete_response)
+        purge_response = self._post(f"groups/{group_id}/purge", admin=True)
+        self._assert_status_code_is_ok(purge_response)
+
+        # The group is deleted and purged, so it cannot be found
+        response = self._get(f"groups/{group_id}", admin=True)
+        self._assert_status_code_is(response, 404)
+
+    def test_purge_can_reuse_name(self):
+        group = self.test_create_valid()
+        group_id = group["id"]
+        group_name = group["name"]
+
+        # Delete and purge the group
+        delete_response = self._delete(f"groups/{group_id}", admin=True)
+        self._assert_status_code_is_ok(delete_response)
+        purge_response = self._post(f"groups/{group_id}/purge", admin=True)
+        self._assert_status_code_is_ok(purge_response)
+
+        # Create a new group with the same name as the deleted one is allowed
+        payload = self._build_valid_group_payload(group_name)
+        response = self._post("groups", payload, admin=True, json=True)
+        self._assert_status_code_is(response, 200)
+
     def _assert_valid_group(self, group, assert_id=None):
         self._assert_has_keys(group, "id", "name", "model_class", "url")
         if assert_id is not None:
             assert group["id"] == assert_id
 
     def _build_valid_group_payload(self, name: Optional[str] = None):
         name = name or self.dataset_populator.get_random_name()
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_histories.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_histories.py`

 * *Files 13% similar despite different names*

```diff
@@ -102,14 +102,34 @@
         history_id = self._create_history("TestHistoryForUrls")["id"]
         show_response = self._show(history_id)
         self._assert_has_key(show_response, "id", "url", "contents_url")
 
         assert show_response["url"] == f"/api/histories/{history_id}"
         assert show_response["contents_url"] == f"/api/histories/{history_id}/contents"
 
+    def test_show_respects_view(self):
+        history_id = self._create_history(f"TestHistoryForShowView_{uuid4()}")["id"]
+        # By default the view is "detailed"
+        show_response = self._get(f"histories/{history_id}").json()
+        assert "state" in show_response
+
+        # Change the view to summary
+        show_response = self._get(f"histories/{history_id}", {"view": "summary"}).json()
+        assert "state" not in show_response
+
+        # Expect only specific keys
+        expected_keys = ["name"]
+        unexpected_keys = ["id", "deleted", "state"]
+        show_response = self._get(f"histories/{history_id}", {"keys": ",".join(expected_keys)}).json()
+        assert len(show_response) == len(expected_keys)
+        for key in expected_keys:
+            assert key in show_response
+        for key in unexpected_keys:
+            assert key not in show_response
+
     def test_show_most_recently_used(self):
         history_id = self._create_history("TestHistoryRecent")["id"]
         show_response = self._get("histories/most_recently_used").json()
         assert show_response["id"] == history_id
 
     def test_index_order(self):
         slightly_older_history_id = self._create_history("TestHistorySlightlyOlder")["id"]
@@ -136,14 +156,86 @@
         # Delete the history
         self._delete(f"histories/{expected_history_id}")
         # Now it should match the query
         index_response = self._get(f"histories{query}").json()
         assert len(index_response) == 1
         assert index_response[0]["name"] == expected_history_name
 
+    def test_index_views(self):
+        # Make sure there is at least one history
+        self._create_history(f"TestHistoryForViews_{uuid4()}")["id"]
+        # By default the view is summary
+        index_response = self._get("histories").json()
+        for history in index_response:
+            assert "state" not in history
+
+        # Change the view to detailed
+        index_response = self._get("histories?view=detailed").json()
+        for history in index_response:
+            assert "state" in history
+
+        # Expect only specific keys
+        expected_keys = ["nice_size", "contents_active", "contents_states"]
+        unexpected_keys = ["id", "deleted", "state"]
+        index_response = self._get(f"histories?keys={','.join(expected_keys)}").json()
+        for history in index_response:
+            assert len(history) == len(expected_keys)
+            for key in expected_keys:
+                assert key in history
+            for key in unexpected_keys:
+                assert key not in history
+
+        # Expect combination of view and keys
+        view = "summary"
+        expected_keys = ["create_time", "count"]
+        data = dict(view=view, keys=",".join(expected_keys))
+        index_response = self._get("histories", data=data).json()
+        for history in index_response:
+            for key in expected_keys:
+                assert key in history
+            self._assert_has_keys(history, "id", "name", "url", "update_time", "deleted", "purged", "tags")
+
+    def test_index_search_mode_views(self):
+        # Make sure there is at least one history
+        expected_name_contains = "SearchMode"
+        self._create_history(f"TestHistory{expected_name_contains}_{uuid4()}")["id"]
+        # By default the view is summary
+        data = dict(search=expected_name_contains, show_published=False)
+        index_response = self._get("histories", data=data).json()
+        for history in index_response:
+            assert "state" not in history
+
+        # Change the view to detailed
+        data = dict(search=expected_name_contains, show_published=False)
+        index_response = self._get("histories?view=detailed", data=data).json()
+        for history in index_response:
+            assert "state" in history
+
+        # Expect only specific keys
+        expected_keys = ["nice_size", "contents_active", "contents_states"]
+        unexpected_keys = ["id", "deleted", "state"]
+        data = dict(search=expected_name_contains, show_published=False, keys=",".join(expected_keys))
+        index_response = self._get("histories", data=data).json()
+        for history in index_response:
+            assert len(history) == len(expected_keys)
+            for key in expected_keys:
+                assert key in history
+            for key in unexpected_keys:
+                assert key not in history
+
+        # Expect combination of view and keys
+        view = "summary"
+        expected_keys = ["create_time", "count"]
+        data = dict(search=expected_name_contains, show_published=False, view=view, keys=",".join(expected_keys))
+        index_response = self._get("histories", data=data).json()
+        for history in index_response:
+            for key in expected_keys:
+                assert key in history
+            self._assert_has_keys(history, "id", "name", "url", "update_time", "deleted", "purged", "tags")
+
     def test_index_case_insensitive_contains_query(self):
         # Create the histories with a different user to ensure the test
         # is not conflicted with the current user's histories.
         with self._different_user(f"user_{uuid4()}@bx.psu.edu"):
             unique_id = uuid4()
             expected_history_name = f"Test History That Match Query_{unique_id}"
             self._create_history(expected_history_name)
@@ -172,14 +264,106 @@
             assert len(index_response) == 3
 
             name_contains = unique_id
             query = f"?q=name-contains&qv={name_contains}"
             index_response = self._get(f"histories{query}").json()
             assert len(index_response) == 3
 
+    def test_index_advanced_filter(self):
+        # Create the histories with a different user to ensure the test
+        # is not conflicted with the current user's histories.
+        with self._different_user(f"user_{uuid4()}@bx.psu.edu"):
+            unique_id = uuid4()
+            expected_history_name = f"Test History That Match Query_{unique_id}"
+            self._create_history(expected_history_name)
+            self._create_history(expected_history_name.upper())
+            history_0 = self._create_history(expected_history_name.lower())["id"]
+            history_1 = self._create_history(f"Another history_{uuid4()}")["id"]
+            self._delete(f"histories/{history_1}")
+
+            name_contains = "history"
+            data = dict(search=name_contains, show_published=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 3
+
+            name_contains = "history that match query"
+            data = dict(search=name_contains, show_published=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 3
+
+            name_contains = "ANOTHER"
+            data = dict(search=name_contains, show_published=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 0
+
+            data = dict(search="is:deleted", show_published=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 1
+
+            self._update(history_0, {"published": True})
+            data = dict(search=f"query_{unique_id} is:published")
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 1
+
+            archived_history_id = self._create_history(f"Archived history_{uuid4()}")["id"]
+            name_contains = "history"
+            data = dict(search=name_contains, show_published=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 4
+
+            # Archived histories should not be included by default
+            self.dataset_populator.archive_history(archived_history_id)
+            data = dict(search=name_contains, show_published=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 3
+
+            self._create_history_then_publish_and_archive_it(f"Public Archived history_{uuid4()}")
+            data = dict(search=name_contains, show_published=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 3
+
+            name_contains = "Archived"
+            data = dict(search=name_contains, show_published=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 0
+
+            # Archived public histories should be included when filtering by show_published and show_archived
+            data = dict(search="is:published", show_archived=True)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 2
+
+            # Searching all published histories will NOT include the archived if show_archived is not set
+            data = dict(search="is:published")
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 1
+
+            # Searching all published histories will include our own archived when show_own is false
+            # as long as they are published
+            data = dict(search="is:published", show_own=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 2
+
+            # Publish a history and archive it by a different user
+            with self._different_user(f"other_user_{uuid4()}@bx.psu.edu"):
+                self._create_history_then_publish_and_archive_it(f"Public Archived history_{uuid4()}")
+
+            # Searching all published histories will include archived from other users and our own
+            # as long as they are published
+            data = dict(search="is:published", show_own=False)
+            index_response = self._get("histories", data=data).json()
+            assert len(index_response) == 3
+
+    def _create_history_then_publish_and_archive_it(self, name):
+        history_id = self._create_history(name)["id"]
+        response = self._update(history_id, {"published": True})
+        self._assert_status_code_is_ok(response)
+        response = self.dataset_populator.archive_history(history_id)
+        self._assert_status_code_is_ok(response)
+        return history_id
+
     def test_delete(self):
         # Setup a history and ensure it is in the index
         history_id = self._create_history("TestHistoryForDelete")["id"]
         index_response = self._get("histories").json()
         assert index_response[0]["id"] == history_id
 
         show_response = self._show(history_id)
@@ -306,14 +490,18 @@
 
     def test_copy_history(self):
         history_id = self.dataset_populator.new_history()
         fetch_response = self.dataset_collection_populator.create_list_in_history(
             history_id, contents=["Hello", "World"], direct_upload=True
         )
         dataset_collection = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response.json())
+        history = self._show(history_id)
+        assert "update_time" in history
+        original_update_time = history["update_time"]
+
         copied_history_response = self.dataset_populator.copy_history(history_id)
         copied_history_response.raise_for_status()
         copied_history = copied_history_response.json()
         copied_collection = self.dataset_populator.get_history_collection_details(
             history_id=copied_history["id"], history_content_type="dataset_collection"
         )
         assert dataset_collection["name"] == copied_collection["name"]
@@ -326,14 +514,18 @@
         source_hda = source_element["object"]
         copied_hda = copied_element["object"]
         assert source_hda["name"] == copied_hda["name"] == "data0"
         assert source_hda["id"] != copied_hda["id"]
         assert source_hda["history_id"] != copied_hda["history_id"]
         assert source_hda["hid"] == copied_hda["hid"] == 2
 
+        history = self._show(history_id)
+        new_update_time = history["update_time"]
+        assert original_update_time == new_update_time
+
     # TODO: (CE) test_create_from_copy
     def test_import_from_model_store_dict(self):
         response = self.dataset_populator.create_from_store(store_dict=history_model_store_dict())
         assert_has_keys(response, "name", "id")
         assert response["name"] == TEST_HISTORY_NAME
         self._assert_history_length(response["id"], 1)
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_history_contents.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_history_contents.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,14 +180,176 @@
         contents_response = self._get(f"histories/{history_id}/contents?v=dev&details=,,{hda1['id']}")
         self._assert_status_code_is(contents_response, 400)
 
         # Invalid IDs should return 400
         contents_response = self._get(f"histories/{history_id}/contents?v=dev&details={hda1['id']}, ,{hda1['id']}")
         self._assert_status_code_is(contents_response, 400)
 
+    def test_view_and_keys_parameters_for_datasets(self, history_id):
+        created_hda = self.dataset_populator.new_dataset(history_id)
+        hda_id = created_hda["id"]
+        item_type = "dataset"
+
+        summary_view_keys = [
+            "id",
+            "name",
+            "history_id",
+            "hid",
+            "history_content_type",
+            "deleted",
+            "visible",
+            "type_id",
+            "type",
+            "create_time",
+            "update_time",
+            "url",
+            "tags",
+            "dataset_id",
+            "state",
+            "extension",
+            "purged",
+            "genome_build",
+        ]
+
+        detailed_view_only_keys = [
+            "created_from_basename",
+            "api_type",
+            "accessible",
+            "misc_info",
+            "resubmitted",
+            "misc_blurb",
+            "hda_ldda",
+            "file_size",
+            "hashes",
+            "drs_id",
+            "validated_state_message",
+            "creating_job",
+            "file_ext",
+            "copied_from_ldda_id",
+            "peek",
+            "validated_state",
+            "permissions",
+            "uuid",
+            "model_class",
+            "sources",
+            "annotation",
+            "display_apps",
+            "display_types",
+            "file_name",
+            "download_url",
+            "rerunnable",
+            "data_type",
+            "meta_files",
+        ]
+
+        detailed_view_keys = summary_view_keys + detailed_view_only_keys
+
+        # Expect summary view to be returned.
+        view = "summary"
+        keys = None
+        item = self._get_history_item_with_custom_serialization(history_id, hda_id, item_type, view, keys)
+        self._assert_has_keys(item, *summary_view_keys)
+        for key in detailed_view_only_keys:
+            assert key not in item
+        # Expect "dynamic" metadata fields to NOT be returned.
+        metadata_keys = [key for key in item.keys() if key.startswith("metadata_")]
+        assert len(metadata_keys) == 0
+
+        # Expect detailed view to be returned.
+        view = "detailed"
+        keys = None
+        item = self._get_history_item_with_custom_serialization(history_id, hda_id, item_type, view, keys)
+        self._assert_has_keys(item, *detailed_view_keys)
+        # Expect also "dynamic" metadata fields to be returned.
+        metadata_keys = [key for key in item.keys() if key.startswith("metadata_")]
+        assert len(metadata_keys) > 0
+
+        # Expect only specific keys to be returned.
+        view = None
+        keys = detailed_view_only_keys + ["id"]
+        item = self._get_history_item_with_custom_serialization(history_id, hda_id, item_type, view, keys)
+        self._assert_has_keys(item, *keys)
+        assert len(item) == len(keys)
+        # Make sure the id is encoded in the response.
+        assert isinstance(item["id"], str)
+        assert item["id"] == hda_id
+
+        # Expect combined view and keys to be returned.
+        view = "summary"
+        keys = ["file_size"]
+        item = self._get_history_item_with_custom_serialization(history_id, hda_id, item_type, view, keys)
+        self._assert_has_keys(item, *summary_view_keys, *keys)
+        assert "peek" not in item
+
+    def test_view_and_keys_parameters_for_collections(self, history_id):
+        fetch_response = self.dataset_collection_populator.create_list_in_history(history_id, direct_upload=True).json()
+        created_dataset_collection = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
+        hdca_id = created_dataset_collection["id"]
+        item_type = "dataset_collection"
+
+        # Collections seems to have 3 different views, "collection", "element" and "element-reference".
+        # We cannot use the keys parameter with collections, so we will only test the view parameter.
+        collection_view_keys = [
+            "hid",
+            "history_id",
+            "history_content_type",
+            "visible",
+            "deleted",
+            "job_source_id",
+            "job_source_type",
+            "job_state_summary",
+            "create_time",
+            "update_time",
+            "id",
+            "name",
+            "collection_id",
+            "collection_type",
+            "populated",
+            "populated_state",
+            "populated_state_message",
+            "element_count",
+            "elements_datatypes",
+            "type",
+            "model_class",
+            "tags",
+            "url",
+            "contents_url",
+        ]
+
+        element_view_only_keys = ["elements", "implicit_collection_jobs_id"]
+        element_view_keys = collection_view_keys + element_view_only_keys
+
+        # Expect summary view to be returned.
+        view = "collection"
+        item = self._get_history_item_with_custom_serialization(history_id, hdca_id, item_type, view)
+        self._assert_has_keys(item, *collection_view_keys)
+        for key in element_view_only_keys:
+            assert key not in item
+
+        # Expect detailed view to be returned.
+        view = "element"
+        item = self._get_history_item_with_custom_serialization(history_id, hdca_id, item_type, view)
+        self._assert_has_keys(item, *element_view_keys)
+        # The `elements` field should be populated for the "element" view.
+        assert len(item["elements"]) > 0
+
+    def _get_history_item_with_custom_serialization(
+        self,
+        history_id: str,
+        content_id: str,
+        item_type: str,
+        expected_view: Optional[str] = None,
+        expected_keys: Optional[List[str]] = None,
+    ):
+        view = f"&view={expected_view}" if expected_view else ""
+        keys = f"&keys={','.join(expected_keys)}" if expected_keys else ""
+        response = self._get(f"histories/{history_id}/contents/{item_type}s/{content_id}?v=dev{view}{keys}")
+        self._assert_status_code_is_ok(response)
+        return response.json()
+
     def test_show_hda(self, history_id):
         hda1 = self.dataset_populator.new_dataset(history_id)
         show_response = self.__show(history_id, hda1)
         self._assert_status_code_is(show_response, 200)
         self.__assert_matches_hda(hda1, show_response.json())
 
     def _create_copy(self, history_id: str):
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_history_contents_provenance.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_history_contents_provenance.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_item_tags.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_item_tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 )
 
 from galaxy_test.base.populators import (
     DatasetCollectionPopulator,
     DatasetPopulator,
     WorkflowPopulator,
 )
-from galaxy_test.driver import integration_util
+from ._framework import ApiTestCase
 
 
-class TestItemTagsApi(integration_util.IntegrationTestCase):
+class TestItemTagsApi(ApiTestCase):
     dataset_populator: DatasetPopulator
 
     @classmethod
     def handle_galaxy_config_kwds(cls, config):
         super().handle_galaxy_config_kwds(config)
 
     def setUp(self):
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_jobs.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,20 @@
         assert "__DATA_FETCH__" in map(itemgetter("tool_id"), jobs)
 
     @pytest.mark.require_new_history
     def test_system_details_admin_only(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs = self.__jobs_index(admin=False)
         job = jobs[0]
-        self._assert_not_has_keys(job, "external_id")
+        assert job["external_id"] is None
 
         jobs = self.__jobs_index(admin=True)
         job = jobs[0]
-        self._assert_has_keys(job, "command_line", "external_id")
+        assert job["command_line"]
+        assert job["external_id"]
 
     @pytest.mark.require_new_history
     def test_admin_job_list(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs_response = self._get("jobs?view=admin_job_list", admin=False)
         assert jobs_response.status_code == 403
         assert jobs_response.json()["err_msg"] == "Only admins can use the admin_job_list view"
@@ -349,23 +350,24 @@
         job_id = job["id"]
 
         job_lock_response = self._get("job_lock", admin=True)
         job_lock_response.raise_for_status()
         assert not job_lock_response.json()["active"]
 
         show_jobs_response = self._get(f"jobs/{job_id}", admin=False)
-        self._assert_not_has_keys(show_jobs_response.json(), "external_id")
+        assert show_jobs_response.json()["external_id"] is None
 
         # TODO: Re-activate test case when API accepts privacy settings
         # with self._different_user():
         #    show_jobs_response = self._get( "jobs/%s" % job_id, admin=False )
         #    self._assert_status_code_is( show_jobs_response, 200 )
 
         show_jobs_response = self._get(f"jobs/{job_id}", admin=True)
-        self._assert_has_keys(show_jobs_response.json(), "command_line", "external_id")
+        assert show_jobs_response.json()["external_id"] is not None
+        assert show_jobs_response.json()["command_line"] is not None
 
     def _run_detect_errors(self, history_id, inputs):
         payload = self.dataset_populator.run_tool_payload(
             tool_id="detect_errors_aggressive",
             inputs=inputs,
             history_id=history_id,
         )
@@ -735,14 +737,30 @@
         tool_response = self._job_search(tool_id="cat1", history_id=history_id, inputs=inputs)
         output_id = tool_response.json()["outputs"][0]["id"]
         delete_respone = self._delete(f"histories/{history_id}/contents/{output_id}")
         self._assert_status_code_is(delete_respone, 200)
         search_payload = self._search_payload(history_id=history_id, tool_id="cat1", inputs=inputs)
         self._search(search_payload, expected_search_count=0)
 
+    def test_implicit_collection_jobs(self, history_id):
+        run_response = self._run_map_over_error(history_id)
+        implicit_collection_id = run_response["implicit_collections"][0]["id"]
+        failed_hdca = self.dataset_populator.get_history_collection_details(
+            history_id=history_id,
+            content_id=implicit_collection_id,
+            assert_ok=False,
+        )
+        job_id = run_response["jobs"][0]["id"]
+        icj_id = failed_hdca["implicit_collection_jobs_id"]
+        assert icj_id
+        index = self.__jobs_index(data=dict(implicit_collection_jobs_id=icj_id))
+        assert len(index) == 1
+        assert index[0]["id"] == job_id
+        assert index[0]["state"] == "error", index
+
     @pytest.mark.require_new_history
     def test_search_with_hdca_list_input(self, history_id):
         list_id_a = self.__history_with_ok_collection(collection_type="list", history_id=history_id)
         list_id_b = self.__history_with_ok_collection(collection_type="list", history_id=history_id)
         inputs = json.dumps(
             {
                 "f1": {"src": "hdca", "id": list_id_a},
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_libraries.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_libraries.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_licenses.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_licenses.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_page_revisions.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_page_revisions.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_pages.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         response2 = self._create_valid_page_with_slug("indexdeletedpagedeleted")
         assert self._users_index_has_page_with_id(response1)
         assert self._users_index_has_page_with_id(response2)
         delete_response = self._delete(f"pages/{response2['id']}")
         delete_response.raise_for_status()
         assert self._users_index_has_page_with_id(response1)
         assert not self._users_index_has_page_with_id(response2)
-        assert self._users_index_has_page_with_id(response2, dict(deleted=True))
+        assert self._users_index_has_page_with_id(response2, dict(deleted=True, show_published=False))
 
     def test_index_user_id_security(self):
         user_id = self.dataset_populator.user_id()
         response1 = self._create_valid_page_with_slug("indexuseridsecurity")
         assert self._users_index_has_page_with_id(response1, dict(user_id=user_id))
         with self._different_user():
             response = self._index_raw()
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_roles.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_roles.py`

 * *Files 21% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         response = self._post("roles", payload, admin=True, json=True)
         assert_status_code_is(response, 400)
         assert_error_code_is(response, error_codes.error_codes_by_name["USER_REQUEST_MISSING_PARAMETER"].code)
         assert "description" in response.json()["err_msg"]
 
         # Test missing name
         payload_missing_name = {
-            "name": None,
             "description": description,
             "user_ids": [self.dataset_populator.user_id()],
         }
         response = self._post("roles", payload_missing_name, admin=True, json=True)
         assert_status_code_is(response, 400)
         assert_error_code_is(response, error_codes.error_codes_by_name["USER_REQUEST_MISSING_PARAMETER"].code)
         assert "name" in response.json()["err_msg"]
@@ -100,23 +99,15 @@
         assert "name" in response.json()["err_msg"]
         assert "validation_errors" in response.json()
 
     @requires_admin
     def test_create_valid(self):
         name = self.dataset_populator.get_random_name()
         description = "A test role."
-        payload = {
-            "name": name,
-            "description": description,
-            "user_ids": [self.dataset_populator.user_id()],
-        }
-        response = self._post("roles", payload, admin=True, json=True)
-        assert_status_code_is(response, 200)
-        role = response.json()
-        self.check_role_dict(role)
+        role = self._create_role(name=name, description=description)
 
         assert role["name"] == name
         assert role["description"] == description
 
         user_roles_response = self._get("roles")
         with self._different_user():
             different_user_roles_response = self._get("roles")
@@ -130,27 +121,98 @@
 
     @requires_admin
     def test_show_error_codes(self):
         # Bad role ids are 400.
         response = self._get("roles/badroleid")
         assert_status_code_is(response, 400)
 
-        # Trying to access roles are errors - should probably be 403 not 400 though?
+        # Trying to access others roles raise (not found) error
         with self._different_user():
             different_user_role_id = self.dataset_populator.user_private_role_id()
         response = self._get(f"roles/{different_user_role_id}")
-        assert_status_code_is(response, 400)
+        assert_status_code_is(response, 404)
 
     @requires_admin
     def test_create_only_admin(self):
         response = self._post("roles", json=True)
         assert_status_code_is(response, 403)
         response_err = response.json()
         assert response_err["err_code"] == 403006
         assert "administrator" in response_err["err_msg"]
 
+    @requires_admin
+    def test_delete(self):
+        role = self._create_role()
+        role_id = role["id"]
+        response = self._delete(f"roles/{role_id}", admin=True)
+        assert_status_code_is(response, 200)
+
+    @requires_admin
+    def test_delete_duplicating_name_raises_409(self):
+        role = self._create_role()
+        role_id = role["id"]
+        role_name = role["name"]
+
+        delete_response = self._delete(f"roles/{role_id}", admin=True)
+        self._assert_status_code_is_ok(delete_response)
+
+        # Create a new role with the same name as the deleted one is not allowed
+        payload = self._build_valid_role_payload(role_name)
+        response = self._post("roles", payload, admin=True, json=True)
+        self._assert_status_code_is(response, 409)
+
+    @requires_admin
+    def test_purge(self):
+        role = self._create_role()
+        role_id = role["id"]
+
+        # Delete and purge the role
+        delete_response = self._delete(f"roles/{role_id}", admin=True)
+        self._assert_status_code_is_ok(delete_response)
+        purge_response = self._post(f"roles/{role_id}/purge", admin=True)
+        self._assert_status_code_is_ok(purge_response)
+
+        # The role is deleted and purged, so it cannot be found
+        response = self._get(f"roles/{role_id}", admin=True)
+        self._assert_status_code_is(response, 404)
+
+    @requires_admin
+    def test_purge_can_reuse_name(self):
+        role = self._create_role()
+        role_id = role["id"]
+        role_name = role["name"]
+
+        # Delete and purge the role
+        delete_response = self._delete(f"roles/{role_id}", admin=True)
+        self._assert_status_code_is_ok(delete_response)
+        purge_response = self._post(f"roles/{role_id}/purge", admin=True)
+        self._assert_status_code_is_ok(purge_response)
+
+        # Create a new role with the same name as the deleted one is allowed
+        payload = self._build_valid_role_payload(role_name)
+        response = self._post("roles", payload, admin=True, json=True)
+        self._assert_status_code_is(response, 200)
+
+    def _create_role(self, name: Optional[str] = None, description: Optional[str] = None) -> Dict[str, Any]:
+        payload = self._build_valid_role_payload(name=name, description=description)
+        response = self._post("roles", payload, admin=True, json=True)
+        assert_status_code_is(response, 200)
+        role = response.json()
+        self.check_role_dict(role)
+        return role
+
+    def _build_valid_role_payload(self, name: Optional[str] = None, description: Optional[str] = None):
+        name = name or self.dataset_populator.get_random_name()
+        description = description or f"A test role with name: {name}."
+        payload = {
+            "name": name,
+            "description": description,
+            "user_ids": [self.dataset_populator.user_id()],
+        }
+        return payload
+
     @staticmethod
     def check_role_dict(role_dict: Dict[str, Any], assert_id: Optional[str] = None) -> None:
         assert_has_keys(role_dict, "id", "name", "model_class", "url")
         assert role_dict["model_class"] == "Role"
         if assert_id is not None:
             assert role_dict["id"] == assert_id
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_short_term_storage.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_short_term_storage.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_tags.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_tool_data.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_tool_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from galaxy.util import UNKNOWN
 from ._framework import ApiTestCase
 
 
 class TestToolDataApi(ApiTestCase):
     def test_admin_only(self):
         index_response = self._get("tool_data", admin=False)
-        self._assert_status_code_is(index_response, 403)
+        self._assert_status_code_is(index_response, 200)
 
     def test_list(self):
         index_response = self._get("tool_data", admin=True)
         self._assert_status_code_is(index_response, 200)
         print(index_response.content)
         index = index_response.json()
         assert "testalpha" in [operator.itemgetter("name")(_) for _ in index]
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_tools.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1392,19 +1392,25 @@
             "quality": 3,
         }
         create = self._run("qc_stdout", history_id, inputs, wait_for_job=True, assert_ok=True)
         assert "jobs" in create, create
         job_id = create["jobs"][0]["id"]
         details = self.dataset_populator.get_job_details(job_id, full=True).json()
         assert "job_messages" in details, details
+        # test autogenerated message (if regex defines no description attribute)
         qc_message = details["job_messages"][0]
         # assert qc_message["code_desc"] == "QC Metrics for Tool", qc_message
         assert qc_message["desc"] == "QC: Matched on Quality of sample is 30%."
         assert qc_message["match"] == "Quality of sample is 30%."
         assert qc_message["error_level"] == 1.1
+        # test message generated from the description containing a reference to group defined in the regex
+        qc_message = details["job_messages"][1]
+        assert qc_message["desc"] == "QC: Sample quality 30"
+        assert qc_message["match"] == "Quality of sample is 30%."
+        assert qc_message["error_level"] == 1.1
 
     @skip_without_tool("cat1")
     def test_multirun_cat1(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123")
         new_dataset2 = self.dataset_populator.new_dataset(history_id, content="456")
         datasets = [dataset_to_param(new_dataset1), dataset_to_param(new_dataset2)]
         inputs = {
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_tools_upload.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_tools_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -987,15 +987,15 @@
             }
             my_client = client.TusClient(url, headers={"x-api-key": api_key})
 
             # Upload a file to a tus server.
             uploader = my_client.uploader(path, metadata=metadata)
             uploader.upload()
             assert uploader.url
-            return uploader.url.rsplit("/", 1)[1]
+            return uploader.url.rsplit("/", 1)[1]  # type: ignore[unreachable]
 
         with self.dataset_populator.test_history() as history_id:
             session_id = upload_file(
                 url=urllib.parse.urljoin(self.url, "api/upload/resumable_upload"),
                 path=TestDataResolver().get_filename("1.fastqsanger.gz"),
                 api_key=self.galaxy_interactor.api_key,
                 history_id=history_id,
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_tours.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_tours.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_users.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_users.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from galaxy_test.api._framework import ApiTestCase
 from galaxy_test.base.api_asserts import assert_object_id_error
 from galaxy_test.base.decorators import (
     requires_admin,
+    requires_new_history,
     requires_new_user,
 )
-from galaxy_test.base.populators import skip_without_tool
+from galaxy_test.base.populators import (
+    DatasetPopulator,
+    skip_without_tool,
+)
 
 TEST_USER_EMAIL = "user_for_users_index_test@bx.psu.edu"
 TEST_USER_EMAIL_INDEX_DELETED = "user_for_users_index_deleted_test@bx.psu.edu"
 TEST_USER_EMAIL_DELETE = "user_for_delete_test@bx.psu.edu"
+TEST_USER_EMAIL_DELETE_CANCEL_JOBS = "user_for_delete_cancel_jobs_test@bx.psu.edu"
 TEST_USER_EMAIL_PURGE = "user_for_purge_test@bx.psu.edu"
 TEST_USER_EMAIL_UNDELETE = "user_for_undelete_test@bx.psu.edu"
 TEST_USER_EMAIL_SHOW = "user_for_show_test@bx.psu.edu"
 
 
 class TestUsersApi(ApiTestCase):
     @requires_admin
@@ -125,14 +130,53 @@
         payload = {"deleted": "True"}
         deleted_user = self._get(f"users/{user['id']}", payload, admin=True).json()
         assert deleted_user["deleted"] is True, deleted_user
         self._post(f"users/deleted/{user['id']}/undelete", admin=True)
         undeleted_user = self._get(f"users/{user['id']}", admin=True).json()
         assert undeleted_user["deleted"] is False, undeleted_user
 
+    @requires_admin
+    @requires_new_user
+    @requires_new_history
+    @skip_without_tool("cat_data_and_sleep")
+    def test_delete_user_cancel_all_jobs(self):
+        dataset_populator = DatasetPopulator(self.galaxy_interactor)
+        with self._different_user(TEST_USER_EMAIL_DELETE_CANCEL_JOBS):
+            user_id = self._get_current_user_id()
+            history_id = dataset_populator.new_history()
+            hda_id = dataset_populator.new_dataset(history_id)["id"]
+
+            inputs = {
+                "input1": {"src": "hda", "id": hda_id},
+                "sleep_time": 6000,
+            }
+            run_response = dataset_populator.run_tool_raw(
+                "cat_data_and_sleep",
+                inputs,
+                history_id,
+            )
+            self._assert_status_code_is_ok(run_response)
+
+            job_id = run_response.json()["jobs"][0]["id"]
+
+            # Wait a bit for the job to be ready
+            expected_job_states = ["new", "queued", "running"]
+            dataset_populator.wait_for_job(job_id, ok_states=expected_job_states)
+
+            # Get the job state
+            job_response = self._get(f"jobs/{job_id}").json()
+            assert job_response["state"] in expected_job_states, job_response
+
+            # Delete user will cancel all jobs
+            self._delete(f"users/{user_id}", admin=True)
+
+            # Get the job state again (this time as admin), it should be deleting
+            job_response = self._get(f"jobs/{job_id}", admin=True).json()
+            assert job_response["state"] == "deleting", job_response
+
     @requires_new_user
     def test_information(self):
         user = self._setup_user(TEST_USER_EMAIL)
         url = self.__url("information/inputs", user)
         response = self._get(url).json()
         assert response["username"] == user["username"]
         assert response["email"] == TEST_USER_EMAIL
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_visualizations.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_visualizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         for x in range(3):
             assert ids[x] in index_ids
         index_ids = self._index_ids(dict(search="visualization-filter-1"))
         assert ids[1] in index_ids
         self._update_viz(ids[1], dict(deleted=True))
         index_ids = self._index_ids(dict(search="visualization-filter-1"))
         assert ids[1] not in index_ids
-        index_ids = self._index_ids(dict(search="is:deleted"))
+        index_ids = self._index_ids(dict(search="is:deleted", show_published=False))
         assert ids[1] in index_ids
 
     def test_create(self):
         viz_id, viz_request = self._create_viz()
         self._show_viz(viz_id, assert_ok=True)
 
     def test_create_fails_without_title(self):
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_webhooks.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_workflow_extraction.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_workflow_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     def test_extract_copied_mapping_from_history_reimported(self, history_id):
         import unittest
 
         raise unittest.SkipTest(
             "Mapping connection for copied collections not yet implemented in history import/export"
         )
 
-        old_history_id = self.dataset_populator.new_history()
+        old_history_id = self.dataset_populator.new_history()  # type: ignore[unreachable]
         hdca, job_id1, job_id2 = self.__run_random_lines_mapped_over_singleton(old_history_id)
 
         old_contents = self._history_contents(old_history_id)
         for old_content in old_contents:
             self.__copy_content_to_history(history_id, old_content)
 
         def reimport_jobs_ids(new_history_id):
@@ -474,15 +474,15 @@
             response = self._post(f"histories/{history_id}/contents/dataset_collections", payload, json=True)
         self._assert_status_code_is(response, 200)
         return response.json()
 
     def __setup_and_run_cat1_workflow(self, history_id):
         workflow = self.workflow_populator.load_workflow(name="test_for_extract")
         workflow_request, history_id, workflow_id = self._setup_workflow_run(workflow, history_id=history_id)
-        run_workflow_response = self._post(f"workflows/{workflow_id}/invocations", data=workflow_request)
+        run_workflow_response = self._post(f"workflows/{workflow_id}/invocations", data=workflow_request, json=True)
         self._assert_status_code_is(run_workflow_response, 200)
         invocation_response = run_workflow_response.json()
         self.workflow_populator.wait_for_invocation_and_jobs(
             history_id=history_id, workflow_id=workflow_id, invocation_id=invocation_response["id"]
         )
         return self.__cat_job_id(history_id)
 
@@ -491,17 +491,15 @@
         collection_step = collection_steps[0]
         collection_step_state = loads(collection_step["tool_state"])
         assert collection_step_state["collection_type"] == "paired"
         collect_step_idx = collection_step["id"]
         return collect_step_idx
 
     def _extract_and_download_workflow(self, history_id: str, **extract_payload):
-        reimport_as = extract_payload.get("reimport_as")
-
-        if reimport_as:
+        if reimport_as := extract_payload.get("reimport_as"):
             history_name = reimport_as
             self.dataset_populator.wait_for_history(history_id)
             self.dataset_populator.rename_history(history_id, history_name)
 
             history_length = extract_payload.get("reimport_wait_on_history_length")
             if history_length is None:
                 # sometimes this won't be the same (i.e. datasets copied from outside the history
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_workflows.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,14 +324,23 @@
         workflow = show_response.json()
         self._assert_looks_like_instance_workflow_representation(workflow)
         assert len(workflow["steps"]) == 3
         # Can't reay say what the legacy IDs are but must be greater than 3 because dummy
         # workflow was created first in this instance.
         assert sorted(step["id"] for step in workflow["steps"].values()) != [0, 1, 2]
 
+    def test_show_subworkflow(self):
+        workflow_id = self.workflow_populator.upload_yaml_workflow(WORKFLOW_NESTED_SIMPLE)
+        workflow = self._get(f"workflows/{workflow_id}", {"style": "instance"}).json()
+        assert isinstance(workflow["id"], str)
+        subworkflow_step = workflow["steps"]["2"]
+        assert subworkflow_step["type"] == "subworkflow"
+        assert isinstance(subworkflow_step["workflow_id"], str)
+        self._get(f"workflows/{subworkflow_step['workflow_id']}", {"style": "instance"}).json()
+
     def test_show_invalid_key_is_400(self):
         show_response = self._get(f"workflows/{self._random_key()}")
         self._assert_status_code_is(show_response, 400)
 
     def test_cannot_show_private_workflow(self):
         workflow_id = self.workflow_populator.simple_workflow("test_not_importable")
         with self._different_user():
@@ -1993,15 +2002,15 @@
                 history_id=history_id,
             )
 
     def test_run_workflow_pick_value_bam_pja(self):
         # Makes sure that setting metadata on expression tool data outputs
         # doesn't break result evaluation.
         with self.dataset_populator.test_history() as history_id:
-            self._run_workflow(
+            summary = self._run_workflow(
                 """class: GalaxyWorkflow
 inputs:
   some_file:
     type: data
 steps:
   pick_value:
     tool_id: pick_value
@@ -2018,23 +2027,34 @@
         type_cond:
           __current_case__: 4
           param_type: data
           pick_from:
           - __index__: 0
             value:
               __class__: RuntimeValue
+outputs:
+  pick_out:
+    outputSource: pick_value/data_param
 """,
                 test_data="""
 some_file:
   value: 1.bam
   file_type: bam
   type: File
 """,
                 history_id=history_id,
             )
+        invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+        # Make sure metadata is actually available
+        pick_value_hda = invocation_details["outputs"]["pick_out"]
+        dataset_details = self.dataset_populator.get_history_dataset_details(
+            history_id=history_id, content_id=pick_value_hda["id"]
+        )
+        assert dataset_details["metadata_reference_names"]
+        assert dataset_details["metadata_bam_index"]
 
     def test_run_workflow_simple_conditional_step(self):
         with self.dataset_populator.test_history() as history_id:
             summary = self._run_workflow(
                 """class: GalaxyWorkflow
 inputs:
   should_run:
@@ -3251,14 +3271,136 @@
                 return [j for j in summary.jobs if j["tool_id"] == tool_id]
 
             assert len(filter_jobs_by_tool("exit_code_from_file")) == 2, jobs
             assert len(filter_jobs_by_tool("__FILTER_FAILED_DATASETS__")) == 1, jobs
             # Follow proves one job was filtered out of the result of cat1
             assert len(filter_jobs_by_tool("cat1")) == 1, jobs
 
+    def test_keep_success_mapping_error(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """
+class: GalaxyWorkflow
+inputs:
+  input_c: collection
+
+steps:
+  mixed_collection:
+    tool_id: exit_code_from_file
+    in:
+       input: input_c
+
+  filtered_collection:
+    tool_id: "__KEEP_SUCCESS_DATASETS__"
+    in:
+      input: mixed_collection/out_file1
+
+  cat:
+    tool_id: cat1
+    in:
+      input1: filtered_collection/output
+""",
+                test_data="""
+input_c:
+  collection_type: list
+  elements:
+    - identifier: i1
+      content: "0"
+    - identifier: i2
+      content: "1"
+""",
+                history_id=history_id,
+                wait=True,
+                assert_ok=False,
+            )
+            jobs = summary.jobs
+
+            def filter_jobs_by_tool(tool_id):
+                return [j for j in summary.jobs if j["tool_id"] == tool_id]
+
+            assert len(filter_jobs_by_tool("exit_code_from_file")) == 2, jobs
+            assert len(filter_jobs_by_tool("__KEEP_SUCCESS_DATASETS__")) == 1, jobs
+            # Follow proves one job was filtered out of the exit_code_from_file
+            # And a single one has been sent to cat1
+            assert len(filter_jobs_by_tool("cat1")) == 1, jobs
+
+    def test_keep_success_mapping_paused(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """
+class: GalaxyWorkflow
+inputs:
+  input_c: collection
+
+steps:
+  mixed_collection:
+    tool_id: exit_code_from_file
+    in:
+       input: input_c
+
+  cat:
+    tool_id: cat1
+    in:
+      input1: mixed_collection/out_file1
+
+  filtered_collection:
+    tool_id: "__KEEP_SUCCESS_DATASETS__"
+    in:
+      input: cat/out_file1
+""",
+                test_data="""
+input_c:
+  collection_type: list
+  elements:
+    - identifier: i1
+      content: "0"
+    - identifier: i2
+      content: "1"
+    - identifier: i3
+      content: "0"
+""",
+                history_id=history_id,
+                wait=True,
+                assert_ok=False,
+            )
+            jobs = summary.jobs
+
+            def filter_jobs_by_tool(tool_id):
+                return [j for j in summary.jobs if j["tool_id"] == tool_id]
+
+            # Get invocation to access output collections
+            invocation = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            # Check there are 3 exit_code_from_file
+            assert len(filter_jobs_by_tool("exit_code_from_file")) == 3, jobs
+            # Check output collection has 3 elements
+            output_mixed_collection_id = invocation["steps"][1]["output_collections"]["out_file1"]["id"]
+            mixed_collection = self.dataset_populator.get_history_collection_details(
+                history_id, content_id=output_mixed_collection_id, assert_ok=False
+            )
+            assert mixed_collection["element_count"] == 3, mixed_collection
+            # Check 3 jobs cat1 has been "scheduled":
+            assert len(filter_jobs_by_tool("cat1")) == 3, jobs
+            # Check 2 are 'ok' the other is 'paused'
+            output_cat_id = invocation["steps"][2]["output_collections"]["out_file1"]["id"]
+            cat_collection = self.dataset_populator.get_history_collection_details(
+                history_id, content_id=output_cat_id, assert_ok=False
+            )
+            assert cat_collection["element_count"] == 3, cat_collection
+            cat1_states = [e["object"]["state"] for e in cat_collection["elements"]]
+            assert "paused" in cat1_states, jobs
+            assert len([s for s in cat1_states if s == "ok"]) == 2, cat_collection
+            # Check the KEEP_SUCCESS_DATASETS have been run
+            assert len(filter_jobs_by_tool("__KEEP_SUCCESS_DATASETS__")) == 1, jobs
+            # Check the output has 2 elements
+            output_filtered_id = invocation["steps"][3]["output_collections"]["output"]["id"]
+            output_filtered = self.dataset_populator.get_history_collection_details(
+                history_id, content_id=output_filtered_id, assert_ok=False
+            )
+            assert output_filtered["element_count"] == 2, output_filtered
+
     def test_workflow_request(self):
         workflow = self.workflow_populator.load_workflow(name="test_for_queue")
         workflow_request, history_id, workflow_id = self._setup_workflow_run(workflow)
         run_workflow_response = self.workflow_populator.invoke_workflow_raw(
             workflow_id, workflow_request, assert_ok=True
         )
         invocation_id = run_workflow_response.json()["id"]
@@ -3854,14 +3996,44 @@
             hdca = self.dataset_populator.get_history_collection_details(history_id=jobs_summary.history_id, hid=4)
             assert hdca["collection_type"] == "list:paired"
             assert len(hdca["elements"][0]["object"]["elements"]) == 2
             forward, reverse = hdca["elements"][0]["object"]["elements"]
             assert forward["object"]["file_ext"] == "csv"
             assert reverse["object"]["file_ext"] == "csv"
 
+    @skip_without_tool("collection_split_on_column")
+    def test_change_datatype_discovered_outputs(self):
+        with self.dataset_populator.test_history() as history_id:
+            jobs_summary = self._run_workflow(
+                """
+class: GalaxyWorkflow
+inputs:
+  input: data
+steps:
+  split:
+    tool_id: collection_split_on_column
+    in:
+      input1: input
+    outputs:
+        split_output:
+          change_datatype: csv
+outputs:
+  output:
+    outputSource: split/split_output
+test_data:
+  input: "1\t2\t3"
+""",
+                history_id=history_id,
+            )
+            inv = self.workflow_populator.get_invocation(jobs_summary.invocation_id, step_details=True)
+            details = self.dataset_populator.get_history_collection_details(
+                history_id=history_id, content_id=inv["output_collections"]["output"]["id"]
+            )
+            assert details["elements"][0]["object"]["file_ext"] == "csv"
+
     @skip_without_tool("collection_type_source_map_over")
     def test_mapping_and_subcollection_mapping(self):
         with self.dataset_populator.test_history() as history_id:
             jobs_summary = self._run_workflow(
                 """
 class: GalaxyWorkflow
 inputs:
@@ -5168,30 +5340,30 @@
                     item_one["dataset_id"], item_two["dataset_id"], i + 1
                 )
 
     def test_cannot_run_inaccessible_workflow(self):
         workflow = self.workflow_populator.load_workflow(name="test_for_run_cannot_access")
         workflow_request, _, workflow_id = self._setup_workflow_run(workflow)
         with self._different_user():
-            run_workflow_response = self._post(f"workflows/{workflow_id}/invocations", data=workflow_request)
+            run_workflow_response = self._post(f"workflows/{workflow_id}/invocations", data=workflow_request, json=True)
             self._assert_status_code_is(run_workflow_response, 403)
 
     def test_400_on_invalid_workflow_id(self):
         workflow = self.workflow_populator.load_workflow(name="test_for_run_does_not_exist")
         workflow_request, _, _ = self._setup_workflow_run(workflow)
         run_workflow_response = self._post(f"workflows/{self._random_key()}/invocations", data=workflow_request)
         self._assert_status_code_is(run_workflow_response, 400)
 
     def test_cannot_run_against_other_users_history(self):
         workflow = self.workflow_populator.load_workflow(name="test_for_run_does_not_exist")
         workflow_request, history_id, workflow_id = self._setup_workflow_run(workflow)
         with self._different_user():
             other_history_id = self.dataset_populator.new_history()
         workflow_request["history"] = f"hist_id={other_history_id}"
-        run_workflow_response = self._post(f"workflows/{workflow_id}/invocations", data=workflow_request)
+        run_workflow_response = self._post(f"workflows/{workflow_id}/invocations", data=workflow_request, json=True)
         self._assert_status_code_is(run_workflow_response, 403)
 
     def test_cannot_run_bootstrap_admin_workflow(self):
         workflow = self.workflow_populator.load_workflow(name="test_bootstrap_admin_cannot_run")
         workflow_request, *_ = self._setup_workflow_run(workflow)
         run_workflow_response = self._post("workflows", data=workflow_request, key=self.master_api_key, json=True)
         self._assert_status_code_is(run_workflow_response, 400)
@@ -6534,15 +6706,15 @@
             }
             workflow_request = {
                 "history_id": history_id,
                 "batch": True,
                 "parameters_normalized": True,
                 "parameters": dumps(parameters),
             }
-            invocation_response = self._post(f"workflows/{workflow_id}/usage", data=workflow_request)
+            invocation_response = self._post(f"workflows/{workflow_id}/usage", data=workflow_request, json=True)
             self._assert_status_code_is(invocation_response, 200)
             time.sleep(5)
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
             r1 = "1 2 3\t1\n1 2 3\t2\n"
             r2 = "4 5 6\t1\n1 2 3\t2\n"
             r3 = "7 8 9\t1\n1 2 3\t2\n"
             r4 = "10 11 12\t1\n1 2 3\t2\n"
@@ -6586,15 +6758,15 @@
                 "history_id": history_id,
                 "batch": True,
                 "inputs": dumps(inputs),
                 "inputs_by": "name",
                 "parameters_normalized": True,
                 "parameters": dumps(parameters),
             }
-            invocation_response = self._post(f"workflows/{workflow_id}/usage", data=workflow_request)
+            invocation_response = self._post(f"workflows/{workflow_id}/usage", data=workflow_request, json=True)
             self._assert_status_code_is(invocation_response, 200)
             time.sleep(5)
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
             r1 = "1 2 3\t1\n1 2 3\t2\n"
             r2 = "4 5 6\t1\n1 2 3\t2\n"
             r3 = "7 8 9\t1\n1 2 3\t2\n"
             r4 = "10 11 12\t1\n1 2 3\t2\n"
@@ -6629,15 +6801,15 @@
         - text: "abd"
 """
             )
             workflow_request = dict(
                 history=f"hist_id={history_id}", parameters=dumps(dict(validation_repeat={"r2_0|text": ""}))
             )
             url = f"workflows/{workflow_id}/invocations"
-            invocation_response = self._post(url, data=workflow_request)
+            invocation_response = self._post(url, data=workflow_request, json=True)
             # Take a valid stat and make it invalid, assert workflow won't run.
             self._assert_status_code_is(invocation_response, 400)
 
     @skip_without_tool("validation_default")
     def test_parameter_substitution_validation_value_errors_1(self):
         substitions = dict(select_param='" ; echo "moo')
         run_workflow_response, history_id = self._run_validation_workflow_with_substitions(substitions)
@@ -7141,14 +7313,28 @@
         )
         run_workflow_dict = run_workflow_response.json()
         invocation_id = run_workflow_dict["id"]
         with self._different_user():
             usage_details_response = self._get(f"workflows/{workflow_id}/usage/{invocation_id}")
             self._assert_status_code_is(usage_details_response, 403)
 
+    def test_invocation_filtering_exclude_subworkflow(self):
+        with self.dataset_populator.test_history() as history_id:
+            self._run_workflow(
+                WORKFLOW_NESTED_SIMPLE,
+                test_data="""
+outer_input:
+  value: 1.bed
+  type: File
+""",
+                history_id=history_id,
+            )
+            assert len(self.workflow_populator.history_invocations(history_id)) == 2
+            assert len(self.workflow_populator.history_invocations(history_id, include_nested_invocations=False)) == 1
+
     def test_workflow_publishing(self):
         workflow_id = self.workflow_populator.simple_workflow("dummy")
         response = self._show_workflow(workflow_id)
         assert not response["published"]
         assert not response["importable"]
         published_worklow = self._put(f"workflows/{workflow_id}", data={"published": True}, json=True).json()
         assert published_worklow["published"]
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test/api/test_workflows_from_yaml.py` & `galaxy-test-api-24.0.0/galaxy_test/api/test_workflows_from_yaml.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/galaxy_test_api.egg-info/PKG-INFO` & `galaxy-test-api-24.0.0/galaxy_test_api.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: galaxy-test-api
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy API tests
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: driver
 License-File: LICENSE
+Requires-Dist: galaxy-test-base
+Requires-Dist: pytest
+Requires-Dist: python-dateutil
+Requires-Dist: requests
+Requires-Dist: tuspy
+Provides-Extra: driver
+Requires-Dist: galaxy-test-driver; extra == "driver"
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-api.svg
    :target: https://pypi.org/project/galaxy-test-api/
 
 
 
@@ -44,14 +50,57 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Only check access permissions in ``/api/{history_dataset_collection_id}/contents/{dataset_collection_id}`` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17444 <https://github.com/galaxyproject/galaxy/pull/17444>`_
+* Fix ``test_index_advanced_filter`` API test re-running by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17547 <https://github.com/galaxyproject/galaxy/pull/17547>`_
+* Limit new anon histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17657 <https://github.com/galaxyproject/galaxy/pull/17657>`_
+* Fix step type serialization for StoredWorkflowDetailed models by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17716 <https://github.com/galaxyproject/galaxy/pull/17716>`_
+* Fix histories API index_query serialization by `@davelopez <https://github.com/davelopez>`_ in `#17726 <https://github.com/galaxyproject/galaxy/pull/17726>`_
+* Fix source history update_time being updated when importing a public history by `@jmchilton <https://github.com/jmchilton>`_ in `#17728 <https://github.com/galaxyproject/galaxy/pull/17728>`_
+* Also set extension and metadata on copies of job outputs when finishing job by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17777 <https://github.com/galaxyproject/galaxy/pull/17777>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+* Fix archived histories mixing with active in histories list by `@davelopez <https://github.com/davelopez>`_ in `#17856 <https://github.com/galaxyproject/galaxy/pull/17856>`_
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Create pydantic model for the return of show operation -  get: `/api/jobs/{job_id}`  by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17153 <https://github.com/galaxyproject/galaxy/pull/17153>`_
+* Don't require admin user to list ``/api/tool_data`` by `@jozh2008 <https://github.com/jozh2008>`_ in `#17161 <https://github.com/galaxyproject/galaxy/pull/17161>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Reuse test instance during non-integration tests by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17234 <https://github.com/galaxyproject/galaxy/pull/17234>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Add ``__KEEP_SUCCESS_DATASETS__`` by `@lldelisle <https://github.com/lldelisle>`_ in `#17294 <https://github.com/galaxyproject/galaxy/pull/17294>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Combines legacy qv-pattern and advanced filter pattern in history index endpoint by `@guerler <https://github.com/guerler>`_ in `#17368 <https://github.com/galaxyproject/galaxy/pull/17368>`_
+* Cancel all active jobs when the user is deleted by `@davelopez <https://github.com/davelopez>`_ in `#17390 <https://github.com/galaxyproject/galaxy/pull/17390>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Purge `groups` and `roles` from DB (for real) by `@davelopez <https://github.com/davelopez>`_ in `#17411 <https://github.com/galaxyproject/galaxy/pull/17411>`_
+* Refactor Workflow API routes - Part 1 by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17463 <https://github.com/galaxyproject/galaxy/pull/17463>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+* Restore histories API behavior for `keys` query parameter by `@davelopez <https://github.com/davelopez>`_ in `#17779 <https://github.com/galaxyproject/galaxy/pull/17779>`_
+* Fix datasets API custom keys encoding by `@davelopez <https://github.com/davelopez>`_ in `#17793 <https://github.com/galaxyproject/galaxy/pull/17793>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-api-23.2.1/galaxy_test_api.egg-info/SOURCES.txt` & `galaxy-test-api-24.0.0/galaxy_test_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-23.2.1/setup.cfg` & `galaxy-test-api-24.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -5,44 +5,44 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy API tests
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-api
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-test-base
 	pytest
 	python-dateutil
 	requests
 	tuspy
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.extras_require]
 driver = 
 	galaxy-test-driver
 
 [options.packages.find]
 exclude =
```

