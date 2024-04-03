# Comparing `tmp/galaxy-tool-shed-23.2.1.tar.gz` & `tmp/galaxy-tool-shed-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/tool_shed/dist/.tmp-36jn6k_k/galaxy-tool-shed-23.2.1.tar", last modified: Thu Feb 22 03:57:51 2024, max compression
+gzip compressed data, was "galaxy-tool-shed-24.0.0.tar", last modified: Wed Apr  3 02:47:09 2024, max compression
```

## Comparing `galaxy-tool-shed-23.2.1.tar` & `galaxy-tool-shed-24.0.0.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/galaxy_tool_shed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/galaxy_tool_shed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/galaxy_tool_shed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/galaxy_tool_shed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/galaxy_tool_shed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/galaxy_tool_shed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12708 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/dependencies/attribute_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/dependencies/repository/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/dependencies/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31129 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/dependencies/repository/relation_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/dependencies/tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/dependencies/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/dependencies/tool/tag_attribute_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/galaxy_install/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/galaxy_install/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/grids/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/grids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18716 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/grids/admin_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/grids/repository_grid_filter_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    69671 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/grids/repository_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/grids/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/managers/categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/managers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    25998 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/managers/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/managers/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/managers/trs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/managers/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59689 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/metadata/repository_metadata_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/repository_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/repository_types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/repository_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/repository_types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/repository_types/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/repository_types/repository_suite_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/repository_types/tool_dependency_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/repository_types/unrestricted.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/repository_types/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/structured_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/test/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/api_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/playwrightbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/populators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/test_db_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/twillbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)    98650 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/base/twilltestcase.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    21271 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0000_basic_repository_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0010_repository_with_tool_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0020_basic_repository_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0030_repository_dependency_revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0040_repository_circular_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0050_circular_dependencies_4_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0070_invalid_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0080_advanced_circular_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0090_tool_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0100_complex_repository_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0110_invalid_simple_repository_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0120_simple_repository_dependency_multiple_owners.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0140_tool_help_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0150_prior_installation_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0160_circular_prior_installation_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0170_complex_prior_installation_required.py
--rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0300_reset_all_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0310_hg_api_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0420_citable_urls_for_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0430_browse_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0440_deleting_dependency_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18294 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0460_upload_to_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0470_tool_dependency_repository_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0480_tool_dependency_xml_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0530_repository_admin_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0550_metadata_updated_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1000_install_basic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1010_install_repository_with_tool_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1020_install_repository_with_repository_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1030_install_repository_with_dependency_revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1040_install_repository_basic_circular_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    20271 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1050_circular_dependencies_4_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1070_invalid_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1080_advanced_circular_dependency_installation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1090_repository_dependency_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1100_install_updated_repository_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1120_install_repository_with_complex_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1130_install_repository_with_invalid_repository_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1140_simple_repository_dependency_multiple_owners.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1160_tool_help_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1170_prior_installation_required.py
--rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1180_circular_prior_installation_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1190_complex_prior_installation_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1200_uninstall_and_reinstall_basic_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1210_uninstall_reinstall_repository_with_tool_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1230_uninstall_reinstall_repository_with_dependency_revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20413 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1300_reset_all_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1410_update_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1430_repair_installed_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1460_data_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1470_updating_installed_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_frontend_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_galaxy_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/test/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/test/test_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/tools/data_table_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/tools/tool_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/tools/tool_version_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47907 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/admin_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/basic_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/commit_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/common_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/container_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/encoding_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/hg_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/hgweb_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/metadata_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/readme_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/repository_content_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    26140 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/repository_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/search_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/shed_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/shed_util_common.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/tool_dependency_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/tool_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/web_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/util/xml_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/utility_containers/
--rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/utility_containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    32202 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/repository_revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/
--rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19574 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/buildapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25230 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/hg.py
--rw-r--r--   0 runner    (1001) docker     (127)   138380 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    24342 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/fast_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/fast_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/framework/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/framework/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/framework/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/framework/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/framework/middleware/remoteuser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/graphql/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/model/
--rw-r--r--   0 runner    (1001) docker     (127)    28428 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/model/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/model/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/model/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/model/migrations/dbscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/model/migrations/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/search/repo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/search/tool_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/security/
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:51.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/util/ratings_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-02-22 03:50:43.000000 galaxy-tool-shed-23.2.1/tool_shed/webapp/util/shed_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.856792 galaxy-tool-shed-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-03 02:47:09.856792 galaxy-tool-shed-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.856792 galaxy-tool-shed-24.0.0/galaxy_tool_shed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-03 02:47:09.000000 galaxy-tool-shed-24.0.0/galaxy_tool_shed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-03 02:47:09.000000 galaxy-tool-shed-24.0.0/galaxy_tool_shed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:47:09.000000 galaxy-tool-shed-24.0.0/galaxy_tool_shed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 02:47:09.000000 galaxy-tool-shed-24.0.0/galaxy_tool_shed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 02:47:09.000000 galaxy-tool-shed-24.0.0/galaxy_tool_shed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-03 02:47:09.856792 galaxy-tool-shed-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.824791 galaxy-tool-shed-24.0.0/tool_shed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.824791 galaxy-tool-shed-24.0.0/tool_shed/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/dependencies/attribute_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.824791 galaxy-tool-shed-24.0.0/tool_shed/dependencies/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/dependencies/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31113 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/dependencies/repository/relation_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.824791 galaxy-tool-shed-24.0.0/tool_shed/dependencies/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/dependencies/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/dependencies/tool/tag_attribute_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.824791 galaxy-tool-shed-24.0.0/tool_shed/galaxy_install/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/galaxy_install/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.828791 galaxy-tool-shed-24.0.0/tool_shed/grids/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/grids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18716 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/grids/admin_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/grids/repository_grid_filter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69626 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/grids/repository_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/grids/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.828791 galaxy-tool-shed-24.0.0/tool_shed/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/managers/categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/managers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26037 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/managers/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/managers/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/managers/trs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/managers/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.828791 galaxy-tool-shed-24.0.0/tool_shed/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59667 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/metadata/repository_metadata_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/repository_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.828791 galaxy-tool-shed-24.0.0/tool_shed/repository_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/repository_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/repository_types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/repository_types/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/repository_types/repository_suite_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/repository_types/tool_dependency_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/repository_types/unrestricted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/repository_types/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/structured_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.828791 galaxy-tool-shed-24.0.0/tool_shed/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.832791 galaxy-tool-shed-24.0.0/tool_shed/test/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/api_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/playwrightbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18823 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/populators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/test_db_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/twillbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98752 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/base/twilltestcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.840792 galaxy-tool-shed-24.0.0/tool_shed/test/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21267 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0000_basic_repository_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0010_repository_with_tool_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0020_basic_repository_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0030_repository_dependency_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0040_repository_circular_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0050_circular_dependencies_4_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0070_invalid_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0080_advanced_circular_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0090_tool_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0100_complex_repository_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0110_invalid_simple_repository_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0120_simple_repository_dependency_multiple_owners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0140_tool_help_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0150_prior_installation_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0160_circular_prior_installation_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0170_complex_prior_installation_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27835 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0300_reset_all_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0310_hg_api_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0420_citable_urls_for_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0430_browse_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0440_deleting_dependency_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18294 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0460_upload_to_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0470_tool_dependency_repository_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0480_tool_dependency_xml_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0530_repository_admin_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0550_metadata_updated_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1000_install_basic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1010_install_repository_with_tool_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1020_install_repository_with_repository_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1030_install_repository_with_dependency_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1040_install_repository_basic_circular_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20271 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1050_circular_dependencies_4_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1070_invalid_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1080_advanced_circular_dependency_installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1090_repository_dependency_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1100_install_updated_repository_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1120_install_repository_with_complex_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1130_install_repository_with_invalid_repository_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1140_simple_repository_dependency_multiple_owners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1160_tool_help_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1170_prior_installation_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1180_circular_prior_installation_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1190_complex_prior_installation_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1200_uninstall_and_reinstall_basic_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1210_uninstall_reinstall_repository_with_tool_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1230_uninstall_reinstall_repository_with_dependency_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20413 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1300_reset_all_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1410_update_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1430_repair_installed_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1460_data_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1470_updating_installed_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_frontend_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_galaxy_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.844792 galaxy-tool-shed-24.0.0/tool_shed/test/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/test/test_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.844792 galaxy-tool-shed-24.0.0/tool_shed/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/tools/data_table_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/tools/tool_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/tools/tool_version_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.844792 galaxy-tool-shed-24.0.0/tool_shed/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47907 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/admin_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/basic_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/commit_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/common_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/container_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/encoding_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/hg_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/hgweb_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/metadata_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/readme_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/repository_content_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26140 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/repository_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/search_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/shed_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/shed_util_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/tool_dependency_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/tool_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/web_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/util/xml_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.848792 galaxy-tool-shed-24.0.0/tool_shed/utility_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/utility_containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.848792 galaxy-tool-shed-24.0.0/tool_shed/webapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.848792 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32179 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/repository_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.848792 galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19300 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/buildapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.852792 galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25170 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/hg.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138132 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24342 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/fast_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/fast_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.852792 galaxy-tool-shed-24.0.0/tool_shed/webapp/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/framework/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.852792 galaxy-tool-shed-24.0.0/tool_shed/webapp/framework/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/framework/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/framework/middleware/remoteuser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.852792 galaxy-tool-shed-24.0.0/tool_shed/webapp/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/graphql/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.852792 galaxy-tool-shed-24.0.0/tool_shed/webapp/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    28413 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/model/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.852792 galaxy-tool-shed-24.0.0/tool_shed/webapp/model/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/model/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/model/migrations/dbscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/model/migrations/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.852792 galaxy-tool-shed-24.0.0/tool_shed/webapp/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/search/repo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/search/tool_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.852792 galaxy-tool-shed-24.0.0/tool_shed/webapp/security/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:09.852792 galaxy-tool-shed-24.0.0/tool_shed/webapp/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/util/ratings_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-03 02:43:42.000000 galaxy-tool-shed-24.0.0/tool_shed/webapp/util/shed_statistics.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-tool-shed-23.2.1/LICENSE` & `galaxy-tool-shed-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/galaxy_tool_shed.egg-info/SOURCES.txt` & `galaxy-tool-shed-24.0.0/galaxy_tool_shed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/setup.cfg` & `galaxy-tool-shed-24.0.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -5,40 +5,41 @@
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
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy auth framework and implementations
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-tool-shed
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-web-stack
 	galaxy-web-apps
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/context.py` & `galaxy-tool-shed-24.0.0/tool_shed/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,36 +77,30 @@
     @abc.abstractproperty
     def repositories_hostname(self) -> str:
         """Provide access to hostname used by target mercurial server."""
 
 
 class SessionRequestContext(ProvidesRepositoriesContext, Protocol):
     @abc.abstractmethod
-    def get_galaxy_session(self) -> Optional[GalaxySession]:
-        ...
+    def get_galaxy_session(self) -> Optional[GalaxySession]: ...
 
     @abc.abstractmethod
-    def set_galaxy_session(self, galaxy_session: GalaxySession):
-        ...
+    def set_galaxy_session(self, galaxy_session: GalaxySession): ...
 
     @abc.abstractproperty
-    def request(self) -> GalaxyAbstractRequest:
-        ...
+    def request(self) -> GalaxyAbstractRequest: ...
 
     @abc.abstractproperty
-    def response(self) -> GalaxyAbstractResponse:
-        ...
+    def response(self) -> GalaxyAbstractResponse: ...
 
     @abc.abstractmethod
-    def url_builder(self):
-        ...
+    def url_builder(self): ...
 
     @abc.abstractproperty
-    def session_csrf_token(self) -> str:
-        ...
+    def session_csrf_token(self) -> str: ...
 
 
 class SessionRequestContextImpl(SessionRequestContext):
     _app: ToolShedApp
     _user: Optional[User]
     _galaxy_session: Optional[GalaxySession]
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/dependencies/attribute_handlers.py` & `galaxy-tool-shed-24.0.0/tool_shed/dependencies/attribute_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     Optional,
     Tuple,
     TYPE_CHECKING,
 )
 
 from galaxy.util import (
     asbool,
-    etree,
+    Element,
+    SubElement,
 )
 from tool_shed.dependencies.tool import tag_attribute_handler
 from tool_shed.repository_types.util import (
     REPOSITORY_DEPENDENCY_DEFINITION_FILENAME,
     TOOL_DEPENDENCY_DEFINITION_FILENAME,
 )
 from tool_shed.util import (
@@ -224,49 +225,49 @@
         return altered, new_root, error_message
 
 
 def _create_element(
     tag: str,
     attributes: Optional[Dict[str, str]] = None,
     sub_elements: Optional[Dict[str, List[Tuple[str, str]]]] = None,
-) -> Optional[etree.Element]:
+) -> Optional[Element]:
     """
     Create a new element whose tag is the value of the received tag, and whose attributes are all
     key / value pairs in the received attributes and sub_elements.
     """
     if tag:
-        elem = etree.Element(tag)
+        elem = Element(tag)
         if attributes:
             # The received attributes is an odict to preserve ordering.
             for k, attribute_value in attributes.items():
                 elem.set(k, attribute_value)
         if sub_elements:
             # The received attributes is an odict.  These handle information that tends to be
             # long text including paragraphs (e.g., description and long_description.
             for k, v in sub_elements.items():
                 # Don't include fields that are blank.
                 if v:
                     if k == "packages":
                         # The received sub_elements is an odict whose key is 'packages' and whose
-                        # value is a list of ( name, version ) tuples.
+                        # value is a list of (name, version) tuples.
                         for v_tuple in v:
-                            sub_elem = etree.SubElement(elem, "package")
+                            sub_elem = SubElement(elem, "package")
                             sub_elem_name, sub_elem_version = v_tuple
                             sub_elem.set("name", sub_elem_name)
                             sub_elem.set("version", sub_elem_version)
                     elif isinstance(v, list):
-                        sub_elem = etree.SubElement(elem, k)
+                        sub_elem = SubElement(elem, k)
                         # If v is a list, then it must be a list of tuples where the first
                         # item is the tag and the second item is the text value.
                         for v_tuple in v:
                             if len(v_tuple) == 2:
                                 v_tag = v_tuple[0]
                                 v_text = v_tuple[1]
                                 # Don't include fields that are blank.
                                 if v_text:
-                                    v_elem = etree.SubElement(sub_elem, v_tag)
+                                    v_elem = SubElement(sub_elem, v_tag)
                                     v_elem.text = v_text
                     else:
-                        sub_elem = etree.SubElement(elem, k)
+                        sub_elem = SubElement(elem, k)
                         sub_elem.text = v
         return elem
     return None
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/dependencies/repository/relation_builder.py` & `galaxy-tool-shed-24.0.0/tool_shed/dependencies/repository/relation_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,16 +152,15 @@
         self.tool_shed_url/repository_name/repository_owner/changeset_revision
         and the values are lists of repository_dependency tuples consisting of:
         ( self.tool_shed_url, repository_name, repository_owner, changeset_revision ).
         This method ensures that all required repositories to the nth degree are returned.
         """
         # Assume the current repository does not have repository dependencies defined for it.
         current_repository_key = None
-        metadata = self.repository_metadata.metadata
-        if metadata:
+        if metadata := self.repository_metadata.metadata:
             # The value of self.tool_shed_url must include the port, but doesn't have to include
             # the protocol.
             if "repository_dependencies" in metadata:
                 current_repository_key = self.get_key_for_repository_changeset_revision()
                 repository_dependencies_dict = metadata["repository_dependencies"]
                 if not self.all_repository_dependencies:
                     self.initialize_all_repository_dependencies(current_repository_key, repository_dependencies_dict)
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/dependencies/tool/tag_attribute_handler.py` & `galaxy-tool-shed-24.0.0/tool_shed/dependencies/tool/tag_attribute_handler.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/grids/admin_grids.py` & `galaxy-tool-shed-24.0.0/tool_shed/grids/admin_grids.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/grids/repository_grid_filter_manager.py` & `galaxy-tool-shed-24.0.0/tool_shed/grids/repository_grid_filter_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/grids/repository_grids.py` & `galaxy-tool-shed-24.0.0/tool_shed/grids/repository_grids.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,17 +348,16 @@
         UserColumn("Owner", model_class=model.User, attach_popup=False),
     ]
     operations = [grids.GridOperation("Install to Galaxy", allow_multiple=True)]
     num_rows_per_page = 50
     use_paging = False
 
     def build_initial_query(self, trans, **kwd):
-        match_tuples = kwd.get("match_tuples", [])
         clause_list = []
-        if match_tuples:
+        if match_tuples := kwd.get("match_tuples", []):
             for match_tuple in match_tuples:
                 repository_id, changeset_revision = match_tuple
                 clause_list.append(
                     and_(
                         model.RepositoryMetadata.repository_id == int(repository_id),
                         model.RepositoryMetadata.changeset_revision == changeset_revision,
                     )
@@ -852,16 +851,15 @@
             # At the time this grid is displayed we know that the received repository will have invalid tools in its latest changeset revision
             # that has associated metadata.
             val = ""
             repository_metadata = grids_util.get_latest_repository_metadata_if_it_includes_invalid_tools(
                 trans, repository
             )
             metadata = repository_metadata.metadata
-            invalid_tools = metadata.get("invalid_tools", [])
-            if invalid_tools:
+            if invalid_tools := metadata.get("invalid_tools", []):
                 for invalid_tool_config in invalid_tools:
                     href_str = '<a href="load_invalid_tool?repository_id={}&tool_config={}&changeset_revision={}">{}</a>'.format(
                         trans.security.encode_id(repository.id),
                         invalid_tool_config,
                         repository_metadata.changeset_revision,
                         invalid_tool_config,
                     )
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/grids/util.py` & `galaxy-tool-shed-24.0.0/tool_shed/grids/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/managers/categories.py` & `galaxy-tool-shed-24.0.0/tool_shed/managers/categories.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/managers/groups.py` & `galaxy-tool-shed-24.0.0/tool_shed/managers/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Manager and Serializer for TS groups.
 """
+
 import logging
 
 from sqlalchemy import (
     false,
     select,
     true,
 )
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/managers/repositories.py` & `galaxy-tool-shed-24.0.0/tool_shed/managers/repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Manager and Serializer for TS repositories.
 """
+
 import json
 import logging
 from collections import namedtuple
 from time import strftime
 from typing import (
     Any,
     Callable,
@@ -380,15 +381,17 @@
     ):
         metadata = get_current_repository_metadata_for_changeset_revision(app, repository, changehash)
         if metadata is None:
             continue
         metadata_dict = metadata.to_dict(
             value_mapper={"id": app.security.encode_id, "repository_id": app.security.encode_id}
         )
-        metadata_dict["repository"] = repository.to_dict(value_mapper={"id": app.security.encode_id})
+        metadata_dict["repository"] = repository.to_dict(
+            value_mapper={"id": app.security.encode_id, "user_id": app.security.encode_id}
+        )
         if metadata.has_repository_dependencies and recursive:
             metadata_dict["repository_dependencies"] = get_all_dependencies(
                 app, metadata, processed_dependency_links=[]
             )
         else:
             metadata_dict["repository_dependencies"] = []
         if metadata.includes_tools:
@@ -454,16 +457,15 @@
 
 def create_repository(trans: ProvidesUserContext, request: CreateRepositoryRequest) -> Repository:
     app: ToolShedApp = trans.app
     user = trans.user
     assert user
     category_ids = listify(request.category_ids)
     name = request.name
-    invalid_message = validate_repository_name(app, name, user)
-    if invalid_message:
+    if invalid_message := validate_repository_name(app, name, user):
         raise RequestParameterInvalidException(invalid_message)
 
     repo, _ = low_level_create_repository(
         app=app,
         name=name,
         type=request.type_,
         description=request.synopsis,
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/managers/tools.py` & `galaxy-tool-shed-24.0.0/tool_shed/managers/tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/managers/trs.py` & `galaxy-tool-shed-24.0.0/tool_shed/managers/trs.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,16 @@
         name=organization_name,
     )
     service_type = ServiceType(
         group="org.ga4gh",
         artifact="trs",
         version="2.1.0",
     )
-    environment = config.ga4gh_service_environment
     extra_kwds = {}
-    if environment:
+    if environment := config.ga4gh_service_environment:
         extra_kwds["environment"] = environment
     return Service(
         id=organization_id + ".trs",
         name=TRS_SERVICE_NAME,
         description=TRS_SERVICE_DESCRIPTION,
         organization=organization,
         type=service_type,
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/managers/users.py` & `galaxy-tool-shed-24.0.0/tool_shed/managers/users.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/metadata/repository_metadata_manager.py` & `galaxy-tool-shed-24.0.0/tool_shed/metadata/repository_metadata_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -914,18 +914,17 @@
                     session.commit()
 
     def reset_metadata_on_selected_repositories(self, **kwd):
         """
         Inspect the repository changelog to reset metadata for all appropriate changeset revisions.
         This method is called from both Galaxy and the Tool Shed.
         """
-        repository_ids = util.listify(kwd.get("repository_ids", None))
         message = ""
         status = "done"
-        if repository_ids:
+        if repository_ids := util.listify(kwd.get("repository_ids", None)):
             successful_count = 0
             unsuccessful_count = 0
             for repository_id in repository_ids:
                 try:
                     repository = repository_util.get_repository_in_tool_shed(self.app, repository_id)
                     self.set_repository(repository)
                     self.resetting_all_metadata_on_repository = True
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/repository_registry.py` & `galaxy-tool-shed-24.0.0/tool_shed/repository_registry.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/repository_types/metadata.py` & `galaxy-tool-shed-24.0.0/tool_shed/repository_types/metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/repository_types/repository_suite_definition.py` & `galaxy-tool-shed-24.0.0/tool_shed/repository_types/repository_suite_definition.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/repository_types/tool_dependency_definition.py` & `galaxy-tool-shed-24.0.0/tool_shed/repository_types/tool_dependency_definition.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/repository_types/unrestricted.py` & `galaxy-tool-shed-24.0.0/tool_shed/repository_types/unrestricted.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/repository_types/util.py` & `galaxy-tool-shed-24.0.0/tool_shed/repository_types/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/structured_app.py` & `galaxy-tool-shed-24.0.0/tool_shed/structured_app.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/api.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,16 +86,16 @@
 
     @classmethod
     def tearDownClass(cls):
         """Shutdown Galaxy server and cleanup temp directory."""
         pass
 
     @pytest.fixture(autouse=True)
-    def _get_driver(self, tool_shed_test_driver):
-        self._test_driver = tool_shed_test_driver
+    def _get_driver(self, embedded_driver):
+        self._test_driver = embedded_driver
 
 
 class ShedGalaxyInteractorApi(GalaxyInteractorApi):
     def __init__(self, galaxy_url: str):
         interactor_kwds: Dict[str, Any] = {}
         interactor_kwds["galaxy_url"] = galaxy_url
         interactor_kwds["master_api_key"] = get_galaxy_admin_api_key()
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/api_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/api_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/browser.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/browser.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/common.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/common.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/driver.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/driver.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/playwrightbrowser.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/playwrightbrowser.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/populators.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/populators.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             if end and index >= end:
                 break
 
             commit_message = f"Updating {test_data_path} with index {index} with tar {repo_tar}"
             response = self.upload_revision_raw(repository_id, repo_tar, commit_message)
             if assert_ok:
                 api_asserts.assert_status_code_is_ok(response)
-                assert RepositoryUpdate(__root__=response.json()).is_ok
+                assert RepositoryUpdate(root=response.json()).is_ok
         return repository_id
 
     def setup_test_data_repo(
         self,
         test_data_path: str,
         repository: Optional[Repository] = None,
         assert_ok=True,
@@ -183,15 +183,15 @@
         repo = revision_metadata.repository
         request = GetInstallInfoRequest(
             owner=repo.owner,
             name=repo.name,
             changeset_revision=revision_metadata.changeset_revision,
         )
         revisions_response = self._api_interactor.get(
-            "repositories/get_repository_revision_install_info", params=request.dict()
+            "repositories/get_repository_revision_install_info", params=request.model_dump()
         )
         api_asserts.assert_status_code_is_ok(revisions_response)
         return from_legacy_install_info(revisions_response.json())
 
     def update_column_maker_repo(self, repository: HasRepositoryId) -> requests.Response:
         response = self.upload_revision(
             repository,
@@ -204,15 +204,15 @@
     ) -> requests.Response:
         body = RepositoryUpdateRequest(
             commit_message=commit_message,
         )
         files = {"file": path.open("rb")}
         repository_id = self._repository_id(repository)
         response = self._api_interactor.post(
-            f"repositories/{repository_id}/changeset_revision", params=body.dict(), files=files
+            f"repositories/{repository_id}/changeset_revision", params=body.model_dump(), files=files
         )
         return response
 
     def upload_revision(
         self, repository: HasRepositoryId, path: Traversable, commit_message: str = DEFAULT_COMMIT_MESSAGE
     ):
         response = self.upload_revision_raw(repository, path, commit_message=commit_message)
@@ -225,43 +225,43 @@
                 pass
             if response_json and "err_msg" in response_json:
                 err_msg = response_json["err_msg"]
             if err_msg and "No changes" in err_msg:
                 assert_msg = f"Updating repository [{repository}] with path [{path}] and commit_message {commit_message} failed to update repository contents, no changes found. Response: [{response_json}]"
                 raise AssertionError(assert_msg)
             api_asserts.assert_status_code_is_ok(response)
-        return RepositoryUpdate(__root__=response.json())
+        return RepositoryUpdate(root=response.json())
 
     def new_repository(self, category_ids: Union[List[str], str], prefix: str = DEFAULT_PREFIX) -> Repository:
         name = random_name(prefix=prefix)
         synopsis = random_name(prefix=prefix)
         request = CreateRepositoryRequest(
             name=name,
             synopsis=synopsis,
             category_ids=category_ids,
         )
         return self.create_repository(request)
 
     def create_repository(self, request: CreateRepositoryRequest) -> Repository:
-        response = self._api_interactor.post("repositories", json=request.dict(by_alias=True))
+        response = self._api_interactor.post("repositories", json=request.model_dump(by_alias=True))
         api_asserts.assert_status_code_is_ok(response)
         return Repository(**response.json())
 
     def reindex(self) -> BuildSearchIndexResponse:
         index_response = self._admin_api_interactor.put("tools/build_search_index")
         index_response.raise_for_status()
         return BuildSearchIndexResponse(**index_response.json())
 
     def new_category(
         self, name: Optional[str] = None, description: Optional[str] = None, prefix=DEFAULT_PREFIX
     ) -> Category:
         category_name = name or random_name(prefix=prefix)
         category_description = description or "testcreaterepo"
         request = CreateCategoryRequest(name=category_name, description=category_description)
-        response = self._admin_api_interactor.post("categories", json=request.dict())
+        response = self._admin_api_interactor.post("categories", json=request.model_dump())
         response.raise_for_status()
         return Category(**response.json())
 
     def get_categories(self) -> List[Category]:
         response = self._api_interactor.get("categories")
         response.raise_for_status()
         return [Category(**c) for c in response.json()]
@@ -286,37 +286,37 @@
         category_repos = self.repositories_by_category(category_id)
         assert category_repos.repository_count == n
         assert len(category_repos.repositories) == n
 
     def get_ordered_installable_revisions(self, owner: str, name: str) -> OrderedInstallableRevisions:
         request = GetOrderedInstallableRevisionsRequest(owner=owner, name=name)
         revisions_response = self._api_interactor.get(
-            "repositories/get_ordered_installable_revisions", params=request.dict()
+            "repositories/get_ordered_installable_revisions", params=request.model_dump()
         )
         api_asserts.assert_status_code_is_ok(revisions_response)
-        return OrderedInstallableRevisions(__root__=revisions_response.json())
+        return OrderedInstallableRevisions(root=revisions_response.json())
 
     def assert_has_n_installable_revisions(self, repository: Repository, n: int):
         revisions = self.get_ordered_installable_revisions(repository.owner, repository.name)
-        actual_n = len(revisions.__root__)
+        actual_n = len(revisions.root)
         assert actual_n == n, f"Expected {n} repository revisions, found {actual_n} for {repository}"
 
     def get_repository_for(self, owner: str, name: str, deleted: str = "false") -> Optional[Repository]:
         request = RepositoryIndexRequest(
             owner=owner,
             name=name,
             deleted=deleted,
         )
         index = self.repository_index(request)
-        return index.__root__[0] if index.__root__ else None
+        return index.root[0] if index.root else None
 
     def repository_index(self, request: Optional[RepositoryIndexRequest]) -> RepositoryIndexResponse:
-        repository_response = self._api_interactor.get("repositories", params=(request.dict() if request else {}))
+        repository_response = self._api_interactor.get("repositories", params=(request.model_dump() if request else {}))
         api_asserts.assert_status_code_is_ok(repository_response)
-        return RepositoryIndexResponse(__root__=repository_response.json())
+        return RepositoryIndexResponse(root=repository_response.json())
 
     def get_usernames_allowed_to_push(self, repository: HasRepositoryId) -> List[str]:
         repository_id = self._repository_id(repository)
         show_response = self._api_interactor.get(f"repositories/{repository_id}/allow_push")
         show_response.raise_for_status()
         as_list = show_response.json()
         assert isinstance(as_list, list)
@@ -369,33 +369,35 @@
 
     def get_metadata(self, repository: HasRepositoryId, downloadable_only=True) -> RepositoryMetadata:
         repository_id = self._repository_id(repository)
         metadata_response = self._api_interactor.get(
             f"repositories/{repository_id}/metadata?downloadable_only={downloadable_only}"
         )
         api_asserts.assert_status_code_is_ok(metadata_response)
-        return RepositoryMetadata(__root__=metadata_response.json())
+        return RepositoryMetadata(root=metadata_response.json())
 
     def reset_metadata(self, repository: HasRepositoryId) -> ResetMetadataOnRepositoryResponse:
         repository_id = self._repository_id(repository)
         request = ResetMetadataOnRepositoryRequest(repository_id=repository_id)
-        reset_response = self._api_interactor.post("repositories/reset_metadata_on_repository", json=request.dict())
+        reset_response = self._api_interactor.post(
+            "repositories/reset_metadata_on_repository", json=request.model_dump()
+        )
         api_asserts.assert_status_code_is_ok(reset_response)
         return ResetMetadataOnRepositoryResponse(**reset_response.json())
 
     def version(self) -> Version:
         version_response = self._admin_api_interactor.get("version")
         api_asserts.assert_status_code_is_ok(version_response)
         return Version(**version_response.json())
 
     def tool_search_query(self, query: str) -> ToolSearchResults:
         return self.tool_search(ToolSearchRequest(q=query))
 
     def tool_search(self, search_request: ToolSearchRequest) -> ToolSearchResults:
-        search_response = self._api_interactor.get("tools", params=search_request.dict())
+        search_response = self._api_interactor.get("tools", params=search_request.model_dump())
         api_asserts.assert_status_code_is_ok(search_response)
         return ToolSearchResults(**search_response.json())
 
     def tool_guid(
         self, shed_host: HostsTestToolShed, repository: Repository, tool_id: str, tool_version: Optional[str] = None
     ) -> str:
         owner = repository.owner
@@ -411,15 +413,15 @@
         else:
             return f"{tool_id_base}/{tool_version}"
 
     def repo_search_query(self, query: str) -> RepositorySearchResults:
         return self.repo_search(RepositorySearchRequest(q=query))
 
     def repo_search(self, repo_search_request: RepositorySearchRequest) -> RepositorySearchResults:
-        search_response = self._api_interactor.get("repositories", params=repo_search_request.dict())
+        search_response = self._api_interactor.get("repositories", params=repo_search_request.model_dump())
         api_asserts.assert_status_code_is_ok(search_response)
         return RepositorySearchResults(**search_response.json())
 
     def delete_api_key(self) -> None:
         response = self._api_interactor.delete("users/current/api_key")
         response.raise_for_status()
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/test_db_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/test_db_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/twillbrowser.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/twillbrowser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from galaxy.util import smart_str
 from .browser import (
     FormValueType,
     ShedBrowser,
 )
 
 tc.options["equiv_refresh_interval"] = 0
+# Resetting all repository metadata can take a really long time
+tc.timeout(240)
 
 
 def visit_url(url: str, allowed_codes: List[int]) -> str:
     new_url = tc.go(url)
     return_code = tc.browser.code
     assert return_code in allowed_codes, "Invalid HTTP return code {}, allowed codes: {}".format(
         return_code,
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/base/twilltestcase.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/base/twilltestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import (
     Any,
     Dict,
     Iterator,
     List,
     Optional,
     Tuple,
+    Union,
 )
 from urllib.parse import (
     quote_plus,
     urlencode,
     urlparse,
 )
 
@@ -606,15 +607,17 @@
 
 
 @pytest.mark.usefixtures("shed_browser")
 class ShedTwillTestCase(ShedApiTestCase):
     """Class of FunctionalTestCase geared toward HTML interactions using the Twill library."""
 
     requires_galaxy: bool = False
-    _installation_client = None
+    _installation_client: Optional[
+        Union[StandaloneToolShedInstallationClient, GalaxyInteractorToolShedInstallationClient]
+    ] = None
     __browser: Optional[ShedBrowser] = None
 
     def setUp(self):
         super().setUp()
         # Security helper
         self.security = idencoding.IdEncodingHelper(id_secret="changethisinproductiontoo")
         self.history_id = None
@@ -1533,15 +1536,15 @@
 
     def get_repository_first_revision(self, repository: Repository) -> str:
         repo = self.get_hg_repo(self.get_repo_path(repository))
         return str(repo[0])
 
     def _get_metadata_revision_count(self, repository: Repository) -> int:
         repostiory_metadata: RepositoryMetadata = self.populator.get_metadata(repository, downloadable_only=False)
-        return len(repostiory_metadata.__root__)
+        return len(repostiory_metadata.root)
 
     def get_tools_from_repository_metadata(self, repository, include_invalid=False):
         """Get a list of valid and (optionally) invalid tool dicts from the repository metadata."""
         valid_tools = []
         invalid_tools = []
         for repository_metadata in repository.metadata_revisions:
             if "tools" in repository_metadata.metadata:
@@ -2091,15 +2094,14 @@
         timeout_counter = timeout_counter + 1
         # This timeout currently defaults to 10 minutes.
         if timeout_counter > repository_installation_timeout:
             raise AssertionError(
                 "Repository installation timed out, %d seconds elapsed, repository state is %s."
                 % (timeout_counter, repository.status)
             )
-            break
         time.sleep(1)
 
 
 def _get_tool_panel_section_from_repository_metadata(metadata):
     tool_metadata = metadata["tools"]
     tool_guid = tool_metadata[0]["guid"]
     assert "tool_panel_section" in metadata, f"Tool panel section not found in metadata: {metadata}"
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/conftest.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0000_basic_repository_features.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0000_basic_repository_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
     @skip_if_api_v2  # v2 doesn't implement repository deleting repositories
     def test_0110_delete_filtering_repository(self):
         """Delete the filtering_0000 repository and verify that it no longer has any downloadable revisions."""
         repository = self._get_repository_by_name_and_owner(repository_name, common.test_user_1_name)
         self.login(email=common.admin_email, username=common.admin_username)
         self.delete_repository(repository)
         metadata = self.populator.get_metadata(repository, downloadable_only=False)
-        for _, value in metadata.__root__.items():
+        for _, value in metadata.root.items():
             assert not value.downloadable
         # Explicitly reload all metadata revisions from the database, to ensure that we have the current status of the downloadable flag.
         # for metadata_revision in repository.metadata_revisions:
         #    self.test_db_util.refresh(metadata_revision)
         # Marking a repository as deleted should result in no metadata revisions being downloadable.
         # assert True not in [metadata.downloadable for metadata in self._db_repository(repository).metadata_revisions]
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0010_repository_with_tool_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0010_repository_with_tool_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0020_basic_repository_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0020_basic_repository_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0030_repository_dependency_revisions.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0030_repository_dependency_revisions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0040_repository_circular_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0040_repository_circular_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0050_circular_dependencies_4_levels.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0050_circular_dependencies_4_levels.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0070_invalid_tool.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0070_invalid_tool.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0080_advanced_circular_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0080_advanced_circular_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0090_tool_search.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0090_tool_search.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0100_complex_repository_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0100_complex_repository_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0110_invalid_simple_repository_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0110_invalid_simple_repository_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0120_simple_repository_dependency_multiple_owners.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0120_simple_repository_dependency_multiple_owners.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0140_tool_help_images.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0140_tool_help_images.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0150_prior_installation_required.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0150_prior_installation_required.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0160_circular_prior_installation_required.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0160_circular_prior_installation_required.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0170_complex_prior_installation_required.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0170_complex_prior_installation_required.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0300_reset_all_metadata.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0300_reset_all_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Dict
 
+import pytest
+
 from ..base import common
 from ..base.twilltestcase import ShedTwillTestCase
 
 column_maker_repository_name = "column_maker_0020"
 column_maker_repository_description = "A flexible aligner."
 column_maker_repository_long_description = "A flexible aligner and methylation caller for Bisulfite-Seq applications."
 
@@ -555,14 +557,15 @@
                 repository_tuples=[freebayes_tuple, bismark_tuple, emboss_tuple, column_tuple],
                 filepath=dependency_xml_path,
             )
             self.create_repository_dependency(
                 repository=filtering_repository, repository_tuples=[emboss_tuple], filepath=dependency_xml_path
             )
 
+    @pytest.mark.xfail
     def test_0110_reset_metadata_on_all_repositories(self):
         """Reset metadata on all repositories, then verify that it has not changed."""
         self.login(email=common.admin_email, username=common.admin_username)
         old_metadata: Dict[str, Dict] = dict()
         new_metadata: Dict[str, Dict] = dict()
         repositories = self.test_db_util.get_all_repositories()
         for repository in repositories:
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0310_hg_api_features.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0310_hg_api_features.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0420_citable_urls_for_repositories.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0420_citable_urls_for_repositories.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0430_browse_utilities.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0430_browse_utilities.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0440_deleting_dependency_definitions.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0440_deleting_dependency_definitions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0460_upload_to_repository.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0460_upload_to_repository.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0470_tool_dependency_repository_type.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0470_tool_dependency_repository_type.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0480_tool_dependency_xml_verification.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0480_tool_dependency_xml_verification.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0530_repository_admin_feature.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0530_repository_admin_feature.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_0550_metadata_updated_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_0550_metadata_updated_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1000_install_basic_repository.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1000_install_basic_repository.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1010_install_repository_with_tool_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1010_install_repository_with_tool_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1020_install_repository_with_repository_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1020_install_repository_with_repository_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1030_install_repository_with_dependency_revisions.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1030_install_repository_with_dependency_revisions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1040_install_repository_basic_circular_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1040_install_repository_basic_circular_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1050_circular_dependencies_4_levels.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1050_circular_dependencies_4_levels.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1070_invalid_tool.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1070_invalid_tool.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1080_advanced_circular_dependency_installation.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1080_advanced_circular_dependency_installation.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1090_repository_dependency_handling.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1090_repository_dependency_handling.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1100_install_updated_repository_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1100_install_updated_repository_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1120_install_repository_with_complex_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1120_install_repository_with_complex_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1130_install_repository_with_invalid_repository_dependency.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1130_install_repository_with_invalid_repository_dependency.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1140_simple_repository_dependency_multiple_owners.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1140_simple_repository_dependency_multiple_owners.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1160_tool_help_images.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1160_tool_help_images.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1170_prior_installation_required.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1170_prior_installation_required.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1180_circular_prior_installation_required.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1180_circular_prior_installation_required.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1190_complex_prior_installation_required.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1190_complex_prior_installation_required.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1200_uninstall_and_reinstall_basic_repository.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1200_uninstall_and_reinstall_basic_repository.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1210_uninstall_reinstall_repository_with_tool_dependencies.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1210_uninstall_reinstall_repository_with_tool_dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1230_uninstall_reinstall_repository_with_dependency_revisions.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1230_uninstall_reinstall_repository_with_dependency_revisions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1300_reset_all_metadata.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1300_reset_all_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1410_update_manager.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1410_update_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1430_repair_installed_repository.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1430_repair_installed_repository.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1460_data_managers.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1460_data_managers.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_1470_updating_installed_repositories.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_1470_updating_installed_repositories.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_frontend_login.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_frontend_login.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_galaxy_install.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_galaxy_install.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 class TestShedGalaxyInstallApi(ShedApiTestCase):
     def test_install_simple_tool(self):
         populator = self.populator
         repository = populator.setup_column_maker_repo(prefix="repoformetadata")
         owner = repository.owner
         name = repository.name
         installable_revisions = populator.get_ordered_installable_revisions(owner, name)
-        latest_install_revision = installable_revisions.__root__[-1]
+        latest_install_revision = installable_revisions.root[-1]
         self.install_repository(owner, name, latest_install_revision, tool_shed_url=self.url)
         response = self.galaxy_interactor._get("tools?in_panel=False")
         response.raise_for_status()
         expected_tool = populator.tool_guid(self, repository, "Add_a_column1", "1.1.0")
         tool_ids = [t["id"] for t in response.json()]
         assert expected_tool in tool_ids, f"Didn't find {expected_tool} in {tool_ids}"
 
     def test_install_simple_after_repository_metadata_reset(self):
         populator = self.populator
         repository = populator.setup_column_maker_repo(prefix="repoformetadata")
         owner = repository.owner
         name = repository.name
         installable_revisions = populator.get_ordered_installable_revisions(owner, name)
-        latest_install_revision = installable_revisions.__root__[-1]
+        latest_install_revision = installable_revisions.root[-1]
         metadata_response = populator.reset_metadata(repository)
         assert metadata_response.status == "ok"
         self.install_repository(owner, name, latest_install_revision, tool_shed_url=self.url)
         response = self.galaxy_interactor._get("tools?in_panel=False")
         response.raise_for_status()
         expected_tool = f"{self.host}:{self.port}/repos/{owner}/{name}/Add_a_column1/1.1.0"
         tool_ids = [t["id"] for t in response.json()]
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_categories.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_categories.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_graphql.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_graphql.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_repositories.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,29 +50,29 @@
         assert repository_update.is_ok
 
     # used by getRepository in TS client.
     def test_metadata_simple(self):
         populator = self.populator
         repository = populator.setup_column_maker_repo(prefix="repoformetadata")
         repository_metadata = populator.get_metadata(repository)
-        metadata_for_revisions = repository_metadata.__root__
+        metadata_for_revisions = repository_metadata.root
         assert len(metadata_for_revisions) == 1
         only_key = list(metadata_for_revisions.keys())[0]
         assert only_key.startswith("0:")
         only_revision = list(metadata_for_revisions.values())[0]
         assert only_revision
         assert only_revision.downloadable
         assert not only_revision.malicious
 
     def test_metadata_invalid_tools(self):
         populator = self.populator
         repository = populator.setup_bismark_repo()
         repository_metadata = populator.get_metadata(repository)
         assert repository_metadata
-        for _, value in repository_metadata.__root__.items():
+        for _, value in repository_metadata.root.items():
             assert value.invalid_tools
 
     def test_index_simple(self):
         # Logic and typing is pretty different if given a tool id to search for - this should
         # be tested or dropped in v2.
         populator = self.populator
         repo = populator.setup_column_maker_repo(prefix="repoforindex")
@@ -158,30 +158,30 @@
     def test_get_ordered_installable_revisions(self):
         # Used in ephemeris...
         populator = self.populator
         repository = populator.setup_column_maker_repo(prefix="repoforindex")
         assert repository.owner
         assert repository.name
         revisions = populator.get_ordered_installable_revisions(repository.owner, repository.name)
-        assert len(revisions.__root__) == 1
+        assert len(revisions.root) == 1
 
     def test_reset_on_repository(self):
         populator = self.populator
         repository = populator.setup_column_maker_repo(prefix="repoforreseta")
         assert repository.owner
         assert repository.name
         revisions = populator.get_ordered_installable_revisions(repository.owner, repository.name)
-        assert len(revisions.__root__) == 1
+        assert len(revisions.root) == 1
         metadata_response = populator.reset_metadata(repository)
         assert metadata_response.start_time
         assert metadata_response.stop_time
         assert metadata_response.status == "ok"
         assert len(metadata_response.repository_status) == 1
         revisions = populator.get_ordered_installable_revisions(repository.owner, repository.name)
-        assert len(revisions.__root__) == 1
+        assert len(revisions.root) == 1
 
     def test_repository_search(self):
         populator = self.populator
         repository = populator.setup_column_maker_repo(prefix="repoforreposearch")
         populator.reindex()
         results = populator.repo_search_query("repoforreposearch")
         assert len(results.hits) == 1
@@ -251,14 +251,14 @@
         )
         api_asserts.assert_status_code_is_ok(response)
         populator.assert_has_n_installable_revisions(repository, 3)
 
     def _get_only_revision(self, repository: HasRepositoryId) -> RepositoryRevisionMetadata:
         populator = self.populator
         repository_metadata = populator.get_metadata(repository)
-        metadata_for_revisions = repository_metadata.__root__
+        metadata_for_revisions = repository_metadata.root
         assert len(metadata_for_revisions) == 1
         only_key = list(metadata_for_revisions.keys())[0]
         assert only_key.startswith("0:")
         only_revision = list(metadata_for_revisions.values())[0]
         assert only_revision
         return only_revision
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_tools.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/test/functional/test_shed_users.py` & `galaxy-tool-shed-24.0.0/tool_shed/test/functional/test_shed_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         username = email_to_username(email)
         body = {
             "email": email,
             "password": password,
             "username": username,
         }
         request = CreateUserRequest(**body)
-        response = post(url, json=request.dict(), headers=headers)
+        response = post(url, json=request.model_dump(), headers=headers)
         api_asserts.assert_status_code_is_ok(response)
         self._verify_username_password(email, password)
         user = User(**response.json())
         assert user.id
         assert user.username == username
 
     def test_create_user_interactor(self):
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/tools/tool_validator.py` & `galaxy-tool-shed-24.0.0/tool_shed/tools/tool_validator.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/tools/tool_version_manager.py` & `galaxy-tool-shed-24.0.0/tool_shed/tools/tool_version_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/admin_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/admin_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/basic_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/basic_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/commit_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/commit_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/common_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/common_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/hg_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/hg_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,16 +147,15 @@
 
 def get_revision_label(app, repository, changeset_revision, include_date=True, include_hash=True):
     """
     Return a string consisting of the human readable changeset rev and the changeset revision string
     which includes the revision date if the receive include_date is True.
     """
     repo = repository.hg_repo
-    ctx = get_changectx_for_changeset(repo, changeset_revision)
-    if ctx:
+    if ctx := get_changectx_for_changeset(repo, changeset_revision):
         return get_revision_label_from_ctx(ctx, include_date=include_date, include_hash=include_hash)
     else:
         if include_hash:
             return f"-1:{changeset_revision}"
         else:
             return "-1"
 
@@ -164,16 +163,15 @@
 def get_rev_label_changeset_revision_from_repository_metadata(
     app, repository_metadata, repository=None, include_date=True, include_hash=True
 ):
     if repository is None:
         repository = repository_metadata.repository
     repo = repository.hg_repo
     changeset_revision = repository_metadata.changeset_revision
-    ctx = get_changectx_for_changeset(repo, changeset_revision)
-    if ctx:
+    if ctx := get_changectx_for_changeset(repo, changeset_revision):
         rev = "%04d" % ctx.rev()
         if include_date:
             changeset_revision_date = get_readable_ctx_date(ctx)
             if include_hash:
                 label = f"{ctx.rev()}:{changeset_revision} ({changeset_revision_date})"
             else:
                 label = f"{ctx.rev()} ({changeset_revision_date})"
@@ -205,16 +203,15 @@
 
 
 def get_rev_label_from_changeset_revision(repo, changeset_revision, include_date=True, include_hash=True):
     """
     Given a changeset revision hash, return two strings, the changeset rev and the changeset revision hash
     which includes the revision date if the receive include_date is True.
     """
-    ctx = get_changectx_for_changeset(repo, changeset_revision)
-    if ctx:
+    if ctx := get_changectx_for_changeset(repo, changeset_revision):
         rev = "%04d" % ctx.rev()
         label = get_revision_label_from_ctx(ctx, include_date=include_date)
     else:
         rev = "-1"
         label = f"-1:{changeset_revision}"
     return rev, label
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/hgweb_config.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/hgweb_config.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/metadata_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/metadata_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/readme_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/readme_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/repository_content_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/repository_content_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/repository_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/repository_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/search_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/search_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/shed_index.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/shed_index.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/shed_util_common.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/shed_util_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,16 +314,15 @@
 def is_path_within_dependency_dir(app: "ToolShedApp", path: str) -> bool:
     """
     Detect whether the given path is within the tool_dependency_dir folder on the disk.
     (Specified by the config option). Use to filter malicious symlinks targeting outside paths.
     """
     allowed = False
     resolved_path = os.path.realpath(path)
-    tool_dependency_dir = app.config.get("tool_dependency_dir", None)
-    if tool_dependency_dir:
+    if tool_dependency_dir := app.config.get("tool_dependency_dir", None):
         dependency_path = os.path.abspath(tool_dependency_dir)
         allowed = os.path.commonprefix([dependency_path, resolved_path]) == dependency_path
     return allowed
 
 
 def is_path_within_repo(app: "ToolShedApp", path: str, repository_id: str) -> bool:
     """
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/tool_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/tool_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/util/web_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/util/web_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/utility_containers/__init__.py` & `galaxy-tool-shed-24.0.0/tool_shed/utility_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api/authenticate.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api/authenticate.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 .. code-block:: json
 
     {
         "api_key": "<some api key>"
     }
 
 """
+
 import logging
 
 from galaxy.web import expose_api_anonymous_and_sessionless
 from galaxy.webapps.galaxy.api import depends
 from galaxy.webapps.galaxy.services.authenticate import AuthenticationService
 from . import BaseShedAPIController
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api/categories.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api/categories.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api/configuration.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 API operations allowing clients to determine Tool Shed instance's
 capabilities and configuration settings.
 """
+
 import logging
 
 from galaxy.web import expose_api_anonymous_and_sessionless
 from . import BaseShedAPIController
 
 log = logging.getLogger(__name__)
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api/groups.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,15 @@
         :param description (optional): the description of the group
 
         Example: POST /api/groups/?key=XXXYYYXXXYYY
         Content-Disposition: form-data; name="name" Group_Name
         Content-Disposition: form-data; name="description" Group_Description
         """
         group_dict = dict(message="", status="ok")
-        name = payload.get("name", "")
-        if name:
+        if name := payload.get("name", ""):
             description = payload.get("description", "")
             if not description:
                 description = ""
             else:
                 # TODO add description field to the model
                 group_dict = self.group_manager.create(trans, name=name).to_dict(
                     view="element", value_mapper=self.__get_value_mapper(trans)
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api/repositories.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api/repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,17 +98,17 @@
             log.debug(error_message)
             response_dict["status"] = "error"
             response_dict["message"] = error_message
             return response_dict
         # Update the repository registry.
         self.app.repository_registry.add_entry(repository)
         response_dict["status"] = "ok"
-        response_dict[
-            "message"
-        ] = f"Entries for repository {name} owned by {owner} have been added to the Tool Shed repository registry."
+        response_dict["message"] = (
+            f"Entries for repository {name} owned by {owner} have been added to the Tool Shed repository registry."
+        )
         return response_dict
 
     @web.legacy_expose_api_anonymous
     def get_ordered_installable_revisions(self, trans, name=None, owner=None, **kwd):
         """
         GET /api/repositories/get_ordered_installable_revisions
 
@@ -210,16 +210,15 @@
         GET /api/repositories/get_installable_revisions
 
         :param tsr_id: the encoded toolshed ID of the repository
 
         Returns a list of lists of changesets, in the format [ [ 0, fbb391dc803c ], [ 1, 9d9ec4d9c03e ], [ 2, 9b5b20673b89 ], [ 3, e8c99ce51292 ] ].
         """
         # Example URL: http://localhost:9009/api/repositories/get_installable_revisions?tsr_id=9d37e53072ff9fa4
-        tsr_id = kwd.get("tsr_id", None)
-        if tsr_id is not None:
+        if (tsr_id := kwd.get("tsr_id", None)) is not None:
             repository = repository_util.get_repository_in_tool_shed(
                 self.app, tsr_id, eagerload_columns=[model.Repository.downloadable_revisions]
             )
         else:
             error_message = "Error in the Tool Shed repositories API in get_ordered_installable_revisions: "
             error_message += "missing or invalid parameter received."
             log.debug(error_message)
@@ -267,16 +266,15 @@
 
         Examples:
             GET http://localhost:9009/api/repositories
             GET http://localhost:9009/api/repositories?q=fastq
         """
         repository_dicts = []
         deleted = util.asbool(deleted)
-        q = kwd.get("q", "")
-        if q:
+        if q := kwd.get("q", ""):
             page = kwd.get("page", 1)
             page_size = kwd.get("page_size", 10)
             try:
                 page = int(page)
                 page_size = int(page_size)
             except ValueError:
                 raise RequestParameterInvalidException('The "page" and "page_size" parameters have to be integers.')
@@ -284,16 +282,15 @@
             callback = kwd.get("callback", "callback")
             search_results = search(trans, q, page, page_size)
             if return_jsonp:
                 response = str(f"{callback}({json.dumps(search_results)});")
             else:
                 response = json.dumps(search_results)
             return response
-        tool_ids = kwd.get("tool_ids", None)
-        if tool_ids is not None:
+        if (tool_ids := kwd.get("tool_ids", None)) is not None:
             tool_ids = util.listify(tool_ids)
             response = index_tool_ids(self.app, tool_ids)
             return json.dumps(response)
         else:
             repositories = index_repositories(self.app, name, owner, deleted)
             repository_dicts = []
             for repository in repositories:
@@ -316,17 +313,17 @@
         :param tool_shed_url (required): the base URL of the Tool Shed containing the Repository
         :param name (required): the name of the Repository
         :param owner (required): the owner of the Repository
         """
         response_dict = {}
         if not trans.user_is_admin:
             response_dict["status"] = "error"
-            response_dict[
-                "message"
-            ] = "You are not authorized to remove entries from this Tool Shed's repository registry."
+            response_dict["message"] = (
+                "You are not authorized to remove entries from this Tool Shed's repository registry."
+            )
             return response_dict
         tool_shed_url = payload.get("tool_shed_url", "")
         if not tool_shed_url:
             raise HTTPBadRequest(detail="Missing required parameter 'tool_shed_url'.")
         tool_shed_url = tool_shed_url.rstrip("/")
         name = payload.get("name", "")
         if not name:
@@ -340,17 +337,17 @@
             log.debug(error_message)
             response_dict["status"] = "error"
             response_dict["message"] = error_message
             return response_dict
         # Update the repository registry.
         self.app.repository_registry.remove_entry(repository)
         response_dict["status"] = "ok"
-        response_dict[
-            "message"
-        ] = f"Entries for repository {name} owned by {owner} have been removed from the Tool Shed repository registry."
+        response_dict["message"] = (
+            f"Entries for repository {name} owned by {owner} have been removed from the Tool Shed repository registry."
+        )
         return response_dict
 
     @web.legacy_expose_api
     def reset_metadata_on_repositories(self, trans, payload, **kwd):
         """
         PUT /api/repositories/reset_metadata_on_repositories
 
@@ -462,15 +459,15 @@
 
         :param key: the API key of the Tool Shed user.
 
         The following parameters must be included in the payload.
         :param repository_id: the encoded id of the repository on which metadata is to be reset.
         """
         repository_id = payload.get("repository_id", None)
-        return reset_metadata_on_repository(trans, repository_id).dict()
+        return reset_metadata_on_repository(trans, repository_id).model_dump()
 
     @expose_api_anonymous_and_sessionless
     def show(self, trans, id, **kwd):
         """
         GET /api/repositories/{encoded_repository_id}
         Returns information about a repository in the Tool Shed.
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api/repository_revisions.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api/repository_revisions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api/tools.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api/tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api/users.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api/users.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/__init__.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,23 +287,22 @@
     """
     app = trans.app
     mapping = app.model
     session_manager = GalaxySessionManager(mapping)
     sa_session = app.model.context
     request = trans.request
     # Try to load an existing session
-    secure_id = request.get_cookie(AUTH_COOKIE_NAME)
     galaxy_session = None
     prev_galaxy_session = None
     user_for_new_session = None
     invalidate_existing_session = False
     # Track whether the session has changed so we can avoid calling flush
     # in the most common case (session exists and is valid).
     galaxy_session_requires_flush = False
-    if secure_id:
+    if secure_id := request.get_cookie(AUTH_COOKIE_NAME):
         session_key: Optional[str] = app.security.decode_guid(secure_id)
         if session_key:
             # We do NOT catch exceptions here, if the database is down the request should fail,
             # and we should not generate a new session.
             galaxy_session = session_manager.get_session_from_session_key(session_key=session_key)
         if not galaxy_session:
             session_key = None
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/authenticate.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/authenticate.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/categories.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/categories.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/configuration.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/configuration.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/repositories.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,30 +185,29 @@
         downloadable_only: bool = DownloadableQueryParam,
     ) -> dict:
         recursive = True
         as_dict = get_repository_metadata_dict(self.app, encoded_repository_id, recursive, downloadable_only)
         # fails 1020 if we try to use the model - I guess repository dependencies
         # are getting lost
         return as_dict
-        # return _hack_fastapi_4428(as_dict)
 
     @router.get(
         "/api_internal/repositories/{encoded_repository_id}/metadata",
         description="Get information about repository metadata",
         operation_id="repositories__internal_metadata",
         response_model=RepositoryMetadata,
     )
     def metadata_internal(
         self,
         encoded_repository_id: str = RepositoryIdPathParam,
         downloadable_only: bool = DownloadableQueryParam,
-    ) -> dict:
+    ) -> RepositoryMetadata:
         recursive = True
         as_dict = get_repository_metadata_dict(self.app, encoded_repository_id, recursive, downloadable_only)
-        return _hack_fastapi_4428(as_dict)
+        return RepositoryMetadata(root=as_dict)
 
     @router.get(
         "/api/repositories/get_ordered_installable_revisions",
         description="Get an ordered list of the repository changeset revisions that are installable",
         operation_id="repositories__get_ordered_installable_revisions",
     )
     def get_ordered_installable_revisions(
@@ -478,15 +477,15 @@
                 message = upload_tar_and_set_metadata(
                     trans,
                     trans.request.host,
                     repository,
                     filename,
                     commit_message or revision_request.commit_message or "Uploaded",
                 )
-                return RepositoryUpdate(__root__=ValidRepostiroyUpdateMessage(message=message))
+                return RepositoryUpdate(root=ValidRepostiroyUpdateMessage(message=message))
             finally:
                 if os.path.exists(filename):
                     os.remove(filename)
         except Exception:
             import logging
 
             log = logging.getLogger(__name__)
@@ -502,13 +501,7 @@
     def get_readmes(
         self,
         encoded_repository_id: str = RepositoryIdPathParam,
         changeset_revision: str = ChangesetRevisionPathParam,
     ) -> dict:
         repository = get_repository_in_tool_shed(self.app, encoded_repository_id)
         return readmes(self.app, repository, changeset_revision)
-
-
-def _hack_fastapi_4428(as_dict) -> dict:
-    # https://github.com/tiangolo/fastapi/pull/4428#issuecomment-1145429263
-    # after pydantic2 swap to really returning the object
-    return RepositoryMetadata(__root__=as_dict).dict()["__root__"]
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/tools.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/api2/users.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/api2/users.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/app.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/app.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/buildapp.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/buildapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provides factory methods to assemble the Galaxy web application
 """
+
 import atexit
 import logging
 import os
 from inspect import isclass
 from urllib.parse import parse_qs
 
 import routes
@@ -32,14 +33,18 @@
 
 
 class ToolShedGalaxyWebTransaction(GalaxyWebTransaction):
     @property
     def repositories_hostname(self) -> str:
         return url_for("/", qualified=True).rstrip("/")
 
+    def get_or_create_default_history(self):
+        # tool shed has no concept of histories
+        raise NotImplementedError
+
 
 class CommunityWebApplication(galaxy.webapps.base.webapp.WebApplication):
     injection_aware: bool = True
 
     def transaction_chooser(self, environ, galaxy_app: BasicSharedApp, session_cookie: str):
         return ToolShedGalaxyWebTransaction(environ, galaxy_app, self, session_cookie)
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/config.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Universe configuration builder.
 """
+
 import configparser
 import logging
 import logging.config
 import os
 from datetime import timedelta
 
 from galaxy.config import (
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/admin.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,16 +169,15 @@
         )
 
     @web.expose
     @web.require_admin
     def delete_repository(self, trans, **kwd):
         message = escape(kwd.get("message", ""))
         status = kwd.get("status", "done")
-        id = kwd.get("id", None)
-        if id:
+        if id := kwd.get("id", None):
             # Deleting multiple items is currently not allowed (allow_multiple=False), so there will only be 1 id.
             ids = util.listify(id)
             count = 0
             deleted_repositories = ""
             for repository_id in ids:
                 repository = repository_util.get_repository_in_tool_shed(trans.app, repository_id)
                 if repository:
@@ -218,16 +217,15 @@
         )
 
     @web.expose
     @web.require_admin
     def delete_repository_metadata(self, trans, **kwd):
         message = escape(kwd.get("message", ""))
         status = kwd.get("status", "done")
-        id = kwd.get("id", None)
-        if id:
+        if id := kwd.get("id", None):
             ids = util.listify(id)
             count = 0
             for repository_metadata_id in ids:
                 repository_metadata = metadata_util.get_repository_metadata_by_id(trans.app, repository_metadata_id)
                 trans.sa_session.delete(repository_metadata)
                 with transaction(trans.sa_session):
                     trans.sa_session.commit()
@@ -378,16 +376,15 @@
             status=status,
         )
 
     @web.expose
     @web.require_admin
     def undelete_repository(self, trans, **kwd):
         message = escape(kwd.get("message", ""))
-        id = kwd.get("id", None)
-        if id:
+        if id := kwd.get("id", None):
             # Undeleting multiple items is currently not allowed (allow_multiple=False), so there will only be 1 id.
             ids = util.listify(id)
             count = 0
             undeleted_repositories = ""
             for repository_id in ids:
                 repository = repository_util.get_repository_in_tool_shed(trans.app, repository_id)
                 if repository:
@@ -433,16 +430,15 @@
     @web.expose
     @web.require_admin
     def mark_category_deleted(self, trans, **kwd):
         # TODO: We should probably eliminate the Category.deleted column since it really makes no
         # sense to mark a category as deleted (category names and descriptions can be changed instead).
         # If we do this, and the following 2 methods can be eliminated.
         message = escape(kwd.get("message", ""))
-        id = kwd.get("id", None)
-        if id:
+        if id := kwd.get("id", None):
             ids = util.listify(id)
             message = "Deleted %d categories: " % len(ids)
             for category_id in ids:
                 category = suc.get_category(trans.app, category_id)
                 category.deleted = True
                 trans.sa_session.add(category)
                 with transaction(trans.sa_session):
@@ -461,16 +457,15 @@
     @web.expose
     @web.require_admin
     def purge_category(self, trans, **kwd):
         # This method should only be called for a Category that has previously been deleted.
         # Purging a deleted Category deletes all of the following from the database:
         # - RepoitoryCategoryAssociations where category_id == Category.id
         message = escape(kwd.get("message", ""))
-        id = kwd.get("id", None)
-        if id:
+        if id := kwd.get("id", None):
             ids = util.listify(id)
             count = 0
             purged_categories = ""
             message = "Purged %d categories: " % len(ids)
             for category_id in ids:
                 category = suc.get_category(trans.app, category_id)
                 if category.deleted:
@@ -489,16 +484,15 @@
             )
         )
 
     @web.expose
     @web.require_admin
     def undelete_category(self, trans, **kwd):
         message = escape(kwd.get("message", ""))
-        id = kwd.get("id", None)
-        if id:
+        if id := kwd.get("id", None):
             ids = util.listify(id)
             count = 0
             undeleted_categories = ""
             for category_id in ids:
                 category = suc.get_category(trans.app, category_id)
                 if category.deleted:
                     category.deleted = False
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/hg.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/hg.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/repository.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,16 +195,15 @@
                     changeset_revision=selected_changeset_revision,
                 )
             )
         return self.deprecated_repositories_i_own_grid(trans, **kwd)
 
     @web.expose
     def browse_my_writable_repositories(self, trans, **kwd):
-        _redir = self._redirect_if_necessary(trans, **kwd)
-        if _redir is not None:
+        if (_redir := self._redirect_if_necessary(trans, **kwd)) is not None:
             return _redir
 
         selected_changeset_revision, repository = suc.get_repository_from_refresh_on_change(trans.app, **kwd)
         if repository:
             return trans.response.send_redirect(
                 web.url_for(
                     controller="repository",
@@ -214,16 +213,15 @@
                     changeset_revision=selected_changeset_revision,
                 )
             )
         return self.my_writable_repositories_grid(trans, **kwd)
 
     @web.expose
     def browse_my_writable_repositories_missing_tool_test_components(self, trans, **kwd):
-        _redir = self._redirect_if_necessary(trans, **kwd)
-        if _redir is not None:
+        if (_redir := self._redirect_if_necessary(trans, **kwd)) is not None:
             return _redir
 
         if "message" not in kwd:
             message = "This list contains repositories that match the following criteria:<br>"
             message += "<ul>"
             message += "<li>you are authorized to update them</li>"
             message += (
@@ -233,16 +231,15 @@
             message += "</ul>"
             kwd["message"] = message
             kwd["status"] = "warning"
         return self.my_writable_repositories_missing_tool_test_components_grid(trans, **kwd)
 
     @web.expose
     def browse_my_writable_repositories_with_invalid_tools(self, trans, **kwd):
-        _redir = self._redirect_if_necessary(trans, **kwd)
-        if _redir is not None:
+        if (_redir := self._redirect_if_necessary(trans, **kwd)) is not None:
             return _redir
 
         if "message" not in kwd:
             message = "This list contains repositories that match the following criteria:<br>"
             message += "<ul>"
             message += "<li>you are authorized to update them</li>"
             message += "<li>the latest metadata revision contains at least 1 invalid tool</li>"
@@ -356,16 +353,15 @@
             trans, trailing_string=trailing_string, default=default
         )
         self.repositories_by_user_grid.title = title
         return self.repositories_by_user_grid(trans, **kwd)
 
     @web.expose
     def browse_repositories_i_can_administer(self, trans, **kwd):
-        _redir = self._redirect_if_necessary(trans, **kwd)
-        if _redir is not None:
+        if (_redir := self._redirect_if_necessary(trans, **kwd)) is not None:
             return _redir
 
         selected_changeset_revision, repository = suc.get_repository_from_refresh_on_change(trans.app, **kwd)
         if repository:
             return trans.response.send_redirect(
                 web.url_for(
                     controller="repository",
@@ -375,16 +371,15 @@
                     changeset_revision=selected_changeset_revision,
                 )
             )
         return self.repositories_i_can_administer_grid(trans, **kwd)
 
     @web.expose
     def browse_repositories_i_own(self, trans, **kwd):
-        _redir = self._redirect_if_necessary(trans, **kwd)
-        if _redir is not None:
+        if (_redir := self._redirect_if_necessary(trans, **kwd)) is not None:
             return _redir
 
         selected_changeset_revision, repository = suc.get_repository_from_refresh_on_change(trans.app, **kwd)
         if repository:
             return trans.response.send_redirect(
                 web.url_for(
                     controller="repository",
@@ -423,16 +418,15 @@
                 web.url_for(
                     controller="repository",
                     action="view_or_manage_repository",
                     id=trans.security.encode_id(repository.id),
                     changeset_revision=selected_changeset_revision,
                 )
             )
-        category_id = kwd.get("id", None)
-        if category_id:
+        if category_id := kwd.get("id", None):
             category = suc.get_category(trans.app, category_id)
             if category:
                 trailing_string = f"in Category {str(category.name)}"
             else:
                 trailing_string = "in Category"
         else:
             trailing_string = "in Category"
@@ -440,16 +434,15 @@
             trans, trailing_string=trailing_string, default="Repositories"
         )
         self.repositories_in_category_grid.title = title
         return self.repositories_in_category_grid(trans, **kwd)
 
     @web.expose
     def browse_repositories_missing_tool_test_components(self, trans, **kwd):
-        _redir = self._redirect_if_necessary(trans, **kwd)
-        if _redir is not None:
+        if (_redir := self._redirect_if_necessary(trans, **kwd)) is not None:
             return _redir
 
         if "message" not in kwd:
             message = "This list contains repositories that match the following criteria:<br>"
             message += "<ul>"
             message += (
                 "<li>the latest installable revision contains at least 1 tool with no defined tests <b>OR</b>:</li>"
@@ -458,16 +451,15 @@
             message += "</ul>"
             kwd["message"] = message
             kwd["status"] = "warning"
         return self.repositories_missing_tool_test_components_grid(trans, **kwd)
 
     @web.expose
     def browse_repositories_with_invalid_tools(self, trans, **kwd):
-        _redir = self._redirect_if_necessary(trans, **kwd)
-        if _redir is not None:
+        if (_redir := self._redirect_if_necessary(trans, **kwd)) is not None:
             return _redir
 
         if "message" not in kwd:
             message = "This list contains repositories that match the following criteria:<br>"
             message += "<ul>"
             message += "<li>the latest metadata revision contains at least 1 invalid tool</li>"
             message += "</ul>"
@@ -553,16 +545,15 @@
                 )
         return self.tool_dependencies_grid(trans, **kwd)
 
     @web.expose
     def browse_valid_categories(self, trans, **kwd):
         """Filter repositories per category by those that are valid for installing into Galaxy."""
         # The request came from Galaxy, so restrict category links to display only valid repository changeset revisions.
-        galaxy_url = common_util.handle_galaxy_url(trans, **kwd)
-        if galaxy_url:
+        if galaxy_url := common_util.handle_galaxy_url(trans, **kwd):
             kwd["galaxy_url"] = galaxy_url
         if "f-free-text-search" in kwd:
             if kwd["f-free-text-search"] == "All":
                 # The user performed a search, then clicked the "x" to eliminate the search criteria.
                 new_kwd = {}
                 return self.valid_category_grid(trans, **new_kwd)
             # Since we are searching valid repositories and not categories, redirect to browse_valid_repositories().
@@ -591,16 +582,15 @@
         )
         self.valid_category_grid.title = title
         return self.valid_category_grid(trans, **kwd)
 
     @web.expose
     def browse_valid_repositories(self, trans, **kwd):
         """Filter repositories to those that are installable into Galaxy."""
-        galaxy_url = common_util.handle_galaxy_url(trans, **kwd)
-        if galaxy_url:
+        if galaxy_url := common_util.handle_galaxy_url(trans, **kwd):
             kwd["galaxy_url"] = galaxy_url
         repository_id = kwd.get("id", None)
         if "f-free-text-search" in kwd:
             if "f-Category.name" in kwd:
                 # The user browsed to a category and then entered a search string, so get the category associated with its value.
                 category_name = kwd["f-Category.name"]
                 category = suc.get_category_by_name(trans.app, category_name)
@@ -981,21 +971,21 @@
                         grids.GridOperation(
                             "Install", url_args=install_url_args, allow_multiple=True, async_compatible=False
                         )
                     ]
                     self.install_matched_repository_grid.operations = operations
                     return self.install_matched_repository_grid(trans, **kwd)
                 else:
-                    kwd[
-                        "message"
-                    ] = "tool id: <b>{}</b><br/>tool name: <b>{}</b><br/>tool version: <b>{}</b><br/>exact matches only: <b>{}</b>".format(
-                        basic_util.stringify(tool_ids),
-                        escape(basic_util.stringify(tool_names)),
-                        escape(basic_util.stringify(tool_versions)),
-                        exact_matches_checked,
+                    kwd["message"] = (
+                        "tool id: <b>{}</b><br/>tool name: <b>{}</b><br/>tool version: <b>{}</b><br/>exact matches only: <b>{}</b>".format(
+                            basic_util.stringify(tool_ids),
+                            escape(basic_util.stringify(tool_names)),
+                            escape(basic_util.stringify(tool_versions)),
+                            exact_matches_checked,
+                        )
                     )
                     self.matched_repository_grid.title = "Repositories with matching tools"
                     return self.matched_repository_grid(trans, **kwd)
             else:
                 message = "No search performed - each field must contain the same number of comma-separated items."
                 status = "error"
         exact_matches_check_box = CheckboxField("exact_matches", value=exact_matches_checked)
@@ -1038,17 +1028,17 @@
                     repository_dependencies_dict = metadata.get("repository_dependencies", {})
                     repository_dependencies = repository_dependencies_dict.get("repository_dependencies", [])
                     (
                         has_repository_dependencies,
                         has_repository_dependencies_only_if_compiling_contained_td,
                     ) = repository_util.get_repository_dependency_types(repository_dependencies)
                     has_galaxy_utilities_dict["has_repository_dependencies"] = has_repository_dependencies
-                    has_galaxy_utilities_dict[
-                        "has_repository_dependencies_only_if_compiling_contained_td"
-                    ] = has_repository_dependencies_only_if_compiling_contained_td
+                    has_galaxy_utilities_dict["has_repository_dependencies_only_if_compiling_contained_td"] = (
+                        has_repository_dependencies_only_if_compiling_contained_td
+                    )
                     if "workflows" in metadata:
                         has_galaxy_utilities_dict["includes_workflows"] = True
             return has_galaxy_utilities_dict
 
         name = kwd.get("name", None)
         owner = kwd.get("owner", None)
         changeset_revision = kwd.get("changeset_revision", None)
@@ -1133,31 +1123,30 @@
                 update_dict["includes_data_managers"] = includes_data_managers
                 update_dict["includes_datatypes"] = includes_datatypes
                 update_dict["includes_tools"] = includes_tools
                 update_dict["includes_tools_for_display_in_tool_panel"] = includes_tools_for_display_in_tool_panel
                 update_dict["includes_tool_dependencies"] = includes_tool_dependencies
                 update_dict["includes_workflows"] = includes_workflows
                 update_dict["has_repository_dependencies"] = has_repository_dependencies
-                update_dict[
-                    "has_repository_dependencies_only_if_compiling_contained_td"
-                ] = has_repository_dependencies_only_if_compiling_contained_td
+                update_dict["has_repository_dependencies_only_if_compiling_contained_td"] = (
+                    has_repository_dependencies_only_if_compiling_contained_td
+                )
                 update_dict["changeset_revision"] = str(latest_changeset_revision)
         update_dict["ctx_rev"] = str(update_to_ctx.rev())
         return encoding_util.tool_shed_encode(update_dict)
 
     @web.expose
     def get_ctx_rev(self, trans, **kwd):
         """Given a repository and changeset_revision, return the correct ctx.rev() value."""
         repository_name = kwd["name"]
         repository_owner = kwd["owner"]
         changeset_revision = kwd["changeset_revision"]
         repository = repository_util.get_repository_by_name_and_owner(trans.app, repository_name, repository_owner)
         repo = repository.hg_repo
-        ctx = hg_util.get_changectx_for_changeset(repo, changeset_revision)
-        if ctx:
+        if ctx := hg_util.get_changectx_for_changeset(repo, changeset_revision):
             return str(ctx.rev())
         return ""
 
     @web.json
     @web.do_not_cache
     def get_file_contents(self, trans, file_path, repository_id):
         is_admin = trans.user_is_admin
@@ -1424,16 +1413,15 @@
         )
         includes_data_managers = False
         includes_datatypes = False
         includes_tools = False
         includes_tools_for_display_in_tool_panel = False
         includes_workflows = False
         readme_files_dict = None
-        metadata = repository_metadata.metadata
-        if metadata:
+        if metadata := repository_metadata.metadata:
             if "data_manager" in metadata:
                 includes_data_managers = True
             if "datatypes" in metadata:
                 includes_datatypes = True
             if "tools" in metadata:
                 includes_tools = True
                 # Handle includes_tools_for_display_in_tool_panel.
@@ -1501,20 +1489,19 @@
 
     @web.expose
     def index(self, trans, **kwd):
         message = escape(kwd.get("message", ""))
         status = kwd.get("status", "done")
         # See if there are any RepositoryMetadata records since menu items require them.
         repository_metadata = get_first_repository_metadata(trans.sa_session)
-        current_user = trans.user
         # TODO: move the following to some in-memory register so these queries can be done once
         # at startup.  The in-memory register can then be managed during the current session.
         can_administer_repositories = False
         has_deprecated_repositories = False
-        if current_user:
+        if current_user := trans.user:
             # See if the current user has any repositories that have been marked as deprecated.
             for repository in current_user.active_repositories:
                 if repository.deprecated:
                     has_deprecated_repositories = True
                     break
             # See if the current user can administer any repositories, but only if not an admin user.
             if not trans.user_is_admin:
@@ -1723,16 +1710,15 @@
                 trans.sa_session.add(repository)
                 with transaction(trans.sa_session):
                     trans.sa_session.commit()
             message = "The repository information has been updated."
         if error:
             status = "error"
         allow_push_select_field = SelectField(name="allow_push", multiple=True)
-        current_allow_push = repository.allow_push()
-        if current_allow_push:
+        if current_allow_push := repository.allow_push():
             current_allow_push_list = current_allow_push.split(",")
         else:
             current_allow_push_list = []
         options = []
         for user in trans.sa_session.scalars(select(trans.model.User)):
             if user.username not in current_allow_push_list:
                 options.append(user)
@@ -2114,16 +2100,15 @@
         # This method is called only from the ~/templates/webapps/tool_shed/repository/manage_repository.mako template.
         repository = repository_util.get_repository_in_tool_shed(trans.app, id)
         rmm = repository_metadata_manager.RepositoryMetadataManager(
             trans, repository=repository, resetting_all_metadata_on_repository=True
         )
         rmm.reset_all_metadata_on_repository_in_tool_shed()
         rmm_metadata_dict = rmm.get_metadata_dict()
-        rmm_invalid_file_tups = rmm.get_invalid_file_tups()
-        if rmm_invalid_file_tups:
+        if rmm_invalid_file_tups := rmm.get_invalid_file_tups():
             message = tool_util.generate_message_for_invalid_tools(
                 trans.app, rmm_invalid_file_tups, repository, rmm_metadata_dict
             )
             status = "error"
         else:
             message = "All repository metadata has been reset.  "
             status = "done"
@@ -2151,16 +2136,15 @@
 
     @web.expose
     @require_login("set email alerts")
     def set_email_alerts(self, trans, **kwd):
         """Set email alerts for selected repositories."""
         # This method is called from multiple grids, so the caller must be passed.
         caller = kwd["caller"]
-        user = trans.user
-        if user:
+        if user := trans.user:
             repository_ids = util.listify(kwd.get("id", ""))
             total_alerts_added = 0
             total_alerts_removed = 0
             flush_needed = False
             for repository_id in repository_ids:
                 repository = repository_util.get_repository_in_tool_shed(trans.app, repository_id)
                 if repository.email_alerts:
@@ -2446,16 +2430,15 @@
             diffs=diffs,
             message=message,
             status=status,
         )
 
     @web.expose
     def view_or_manage_repository(self, trans, **kwd):
-        repository_id = kwd.get("id", None)
-        if repository_id:
+        if repository_id := kwd.get("id", None):
             repository = repository_util.get_repository_in_tool_shed(trans.app, repository_id)
             user = trans.user
             if repository:
                 if user is not None and (
                     trans.user_is_admin or trans.app.security_agent.user_can_administer_repository(user, repository)
                 ):
                     return trans.response.send_redirect(
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/controllers/user.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/controllers/user.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/fast_app.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/fast_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,16 @@
         else:
             mount_static(find_frontend_target() / "assets")
 
     routes_package = "tool_shed.webapp.api" if SHED_API_VERSION == "v1" else "tool_shed.webapp.api2"
     include_all_package_routers(app, routes_package)
     wsgi_handler = WSGIMiddleware(gx_webapp)
     tool_shed_app.haltables.append(("WSGI Middleware threadpool", wsgi_handler.executor.shutdown))
-    app.mount("/", wsgi_handler)
+    # https://github.com/abersheeran/a2wsgi/issues/44
+    app.mount("/", wsgi_handler)  # type: ignore[arg-type]
     return app
 
 
 def get_fastapi_instance() -> FastAPI:
     return FastAPI(
         title="Galaxy Tool Shed API",
         description=("This API allows you to manage the Tool Shed repositories."),
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/fast_factory.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/fast_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/framework/decorators.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/framework/decorators.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/framework/middleware/remoteuser.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/framework/middleware/remoteuser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Middleware for handling $REMOTE_USER if use_remote_user is enabled.
 """
+
 import socket
 
 from galaxy.util import safe_str_cmp
 
 errorpage = """
 <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
 <html lang="en">
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/graphql/schema.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/graphql/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import graphene
 from graphene import relay
 from graphene_sqlalchemy import (
     SQLAlchemyConnectionField,
     SQLAlchemyObjectType,
 )
-from graphene_sqlalchemy.converter import (
-    convert_sqlalchemy_hybrid_property_type,
-    convert_sqlalchemy_type,
-)
+from graphene_sqlalchemy.converter import convert_sqlalchemy_type
+from graphene_sqlalchemy.utils import column_type_eq
 from graphql import GraphQLResolveInfo
 from sqlalchemy.orm import scoped_session
 from typing_extensions import TypedDict
 
 from galaxy.model.custom_types import TrimmedString
 from galaxy.security.idencoding import IdEncodingHelper
 from tool_shed.webapp.model import (
@@ -63,20 +61,20 @@
 
 class InfoDict(TypedDict):
     session: scoped_session
     security: IdEncodingHelper
 
 
 # Map these Galaxy-ism to Graphene for cleaner interfaces.
-@convert_sqlalchemy_type.register(TrimmedString)
+@convert_sqlalchemy_type.register(column_type_eq(TrimmedString))
 def convert_sqlalchemy_type_trimmed_string(*args, **kwd):
     return graphene.String
 
 
-@convert_sqlalchemy_hybrid_property_type.register(lambda t: t == TrimmedString)
+@convert_sqlalchemy_type.register(column_type_eq(lambda t: t == TrimmedString))
 def convert_sqlalchemy_hybrid_property_type_trimmed_string(arg):
     return graphene.String
 
 
 class HasIdMixin:
     id = graphene.NonNull(graphene.ID)
     encoded_id = graphene.NonNull(graphene.String)
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/model/__init__.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/model/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,16 +164,15 @@
 
     def set_disk_usage(self, bytes):
         pass
 
     total_disk_usage = property(get_disk_usage, set_disk_usage)
 
     def set_password_cleartext(self, cleartext):
-        message = validate_password_str(cleartext)
-        if message:
+        if message := validate_password_str(cleartext):
             raise Exception(f"Invalid password: {message}")
         # Set 'self.password' to the digest of 'cleartext'.
         self.password = new_insecure_hash(text_type=cleartext)
 
     def set_random_password(self, length=16):
         """
         Sets user password to a random string of the given length.
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/model/mapping.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/model/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Details of how the data model objects are mapped onto the relational database
 are encapsulated here.
 """
+
 import logging
 from typing import (
     Any,
     Dict,
     Optional,
 )
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/model/migrations/__init__.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/model/migrations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         msg = f"The {TOOLSHED} database has an alembic version table, but that table does not contain "
         msg += "a revision id that matches a revision in the code base."
         super().__init__(msg)
 
 
 def verify_database(url, engine_options=None) -> None:
     engine_options = engine_options or {}
-    engine = create_engine(url, **engine_options)
+    engine = create_engine(url, **engine_options, future=True)
     verifier = DatabaseStateVerifier(engine)
     verifier.run()
     engine.dispose()
 
 
 class AlembicManager(BaseAlembicManager):
     def _get_alembic_root(self) -> str:
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/model/migrations/dbscript.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/model/migrations/dbscript.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/model/migrations/scripts.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/model/migrations/scripts.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/search/repo_search.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/search/repo_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for searching the toolshed repositories"""
+
 import logging
 
 import whoosh.index
 from whoosh import scoring
 from whoosh.fields import (
     KEYWORD,
     NUMERIC,
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/search/tool_search.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/search/tool_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for searching the toolshed tools within all repositories"""
+
 import logging
 import os
 
 import whoosh.index
 from whoosh import scoring
 from whoosh.fields import (
     ID,
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/security/__init__.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/security/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tool Shed Security"""
+
 import logging
 from typing import List
 
 from sqlalchemy import (
     false,
     select,
 )
@@ -269,16 +270,15 @@
         return False
 
     def user_can_import_repository_archive(self, user, archive_owner):
         # This method should be called only if the current user is not an admin.
         if user.username == archive_owner:
             return True
         # A member of the IUC is authorized to create new repositories that are owned by another user.
-        iuc_group = get_iuc_group(self.sa_session)
-        if iuc_group is not None:
+        if (iuc_group := get_iuc_group(self.sa_session)) is not None:
             for uga in iuc_group.users:
                 if uga.user.id == user.id:
                     return True
         return False
 
 
 def get_permitted_actions(filter=None):
```

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/util/ratings_util.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/util/ratings_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-shed-23.2.1/tool_shed/webapp/util/shed_statistics.py` & `galaxy-tool-shed-24.0.0/tool_shed/webapp/util/shed_statistics.py`

 * *Files identical despite different names*

