# Comparing `tmp/resilient_circuits-51.0.1.0.695.tar.gz` & `tmp/resilient_circuits-51.0.1.1.824.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_circuits-51.0.1.0.695.tar", last modified: Wed Feb 14 14:46:15 2024, max compression
+gzip compressed data, was "resilient_circuits-51.0.1.1.824.tar", last modified: Wed Apr  3 15:16:46 2024, max compression
```

## Comparing `resilient_circuits-51.0.1.0.695.tar` & `resilient_circuits-51.0.1.1.824.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.139633 resilient_circuits-51.0.1.0.695/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14992 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3001 2024-02-14 14:46:15.139633 resilient_circuits-51.0.1.0.695/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.123633 resilient_circuits-51.0.1.0.695/resilient_circuits/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/README
--rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    15525 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/action_message.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    60018 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/actions_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/actions_test_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11645 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12400 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/app_argument_parser.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6658 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/app_function_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7793 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/app_restartable.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.127633 resilient_circuits-51.0.1.0.695/resilient_circuits/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/bin/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/bin/res_action_test.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    17093 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/bin/resilient_circuits_cmd.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3091 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/bin/service_wrapper.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.127633 resilient_circuits-51.0.1.0.695/resilient_circuits/cmds/
--rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16061 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/cmds/selftest.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2919 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.127633 resilient_circuits-51.0.1.0.695/resilient_circuits/data/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3063 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/data/app.config.base
--rwxrwxr-x   0 travis    (2000) travis    (2000)    20589 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15462 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/helpers.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/keyring_arguments.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5100 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/rest_helper.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    14444 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/stomp_component.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/stomp_events.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/stomp_transport.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/template_functions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.131633 resilient_circuits-51.0.1.0.695/resilient_circuits/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/util/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/util/resilient_config.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/util/resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1128 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/resilient_circuits/validate_configs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.127633 resilient_circuits-51.0.1.0.695/resilient_circuits.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3001 2024-02-14 14:46:14.000000 resilient_circuits-51.0.1.0.695/resilient_circuits.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2616 2024-02-14 14:46:15.000000 resilient_circuits-51.0.1.0.695/resilient_circuits.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:46:14.000000 resilient_circuits-51.0.1.0.695/resilient_circuits.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2024-02-14 14:46:14.000000 resilient_circuits-51.0.1.0.695/resilient_circuits.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2024-02-14 14:46:14.000000 resilient_circuits-51.0.1.0.695/resilient_circuits.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2024-02-14 14:46:14.000000 resilient_circuits-51.0.1.0.695/resilient_circuits.egg-info/top_level.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1565 2024-02-14 14:46:15.139633 resilient_circuits-51.0.1.0.695/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.135633 resilient_circuits-51.0.1.0.695/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      287 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.135633 resilient_circuits-51.0.1.0.695/tests/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5845 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/cmds/test_selftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4173 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.135633 resilient_circuits-51.0.1.0.695/tests/selftest_tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/selftest_tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/selftest_tests/mocked_fail_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/selftest_tests/mocked_success_script.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      282 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/selftest_tests/mocked_unimplemented_script.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.135633 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_commented_app_config
--rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1750 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_import_definition.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      545 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_action_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_actions_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4280 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_app_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2675 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_app_function_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2003 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_app_redacting_filter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_app_restartable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_component_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8403 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10922 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_resilient_circuits_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7419 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_rest_helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_stomp_component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:15.139633 resilient_circuits-51.0.1.0.695/tests/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tests/util/test_resilient_customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1054 2024-02-14 14:45:11.000000 resilient_circuits-51.0.1.0.695/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.098412 resilient_circuits-51.0.1.1.824/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15605 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3001 2024-04-03 15:16:46.098412 resilient_circuits-51.0.1.1.824/PKG-INFO
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2095 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.090412 resilient_circuits-51.0.1.1.824/resilient_circuits/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1057 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/LICENSE
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      129 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/README
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      742 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    15556 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/action_message.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    60098 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/actions_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11127 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/actions_test_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    11645 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13207 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/app_argument_parser.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6658 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/app_function_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7793 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/app_restartable.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.090412 resilient_circuits-51.0.1.1.824/resilient_circuits/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/bin/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9741 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/bin/res_action_test.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    17093 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/bin/resilient_circuits_cmd.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3091 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/bin/service_wrapper.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.090412 resilient_circuits-51.0.1.1.824/resilient_circuits/cmds/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       59 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16074 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/cmds/selftest.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6750 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2920 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.090412 resilient_circuits-51.0.1.1.824/resilient_circuits/data/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3064 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/data/app.config.base
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    21563 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16094 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/helpers.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      313 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/keyring_arguments.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5100 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/rest_helper.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    14516 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/stomp_component.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3606 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/stomp_events.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3991 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/stomp_transport.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      760 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/template_functions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.090412 resilient_circuits-51.0.1.1.824/resilient_circuits/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      559 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/util/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/util/resilient_config.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    16321 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/util/resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1412 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/resilient_circuits/validate_configs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.090412 resilient_circuits-51.0.1.1.824/resilient_circuits.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3001 2024-04-03 15:16:45.000000 resilient_circuits-51.0.1.1.824/resilient_circuits.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2616 2024-04-03 15:16:46.000000 resilient_circuits-51.0.1.1.824/resilient_circuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:16:45.000000 resilient_circuits-51.0.1.1.824/resilient_circuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2024-04-03 15:16:45.000000 resilient_circuits-51.0.1.1.824/resilient_circuits.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2024-04-03 15:16:45.000000 resilient_circuits-51.0.1.1.824/resilient_circuits.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2024-04-03 15:16:45.000000 resilient_circuits-51.0.1.1.824/resilient_circuits.egg-info/top_level.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1565 2024-04-03 15:16:46.098412 resilient_circuits-51.0.1.1.824/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      199 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.094412 resilient_circuits-51.0.1.1.824/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      287 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.094412 resilient_circuits-51.0.1.1.824/tests/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5845 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/cmds/test_selftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4173 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2045 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.094412 resilient_circuits-51.0.1.1.824/tests/selftest_tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/selftest_tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/selftest_tests/mocked_fail_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/selftest_tests/mocked_success_script.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      282 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/selftest_tests/mocked_unimplemented_script.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.098412 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_commented_app_config
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2615 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1750 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55022 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_import_definition.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      545 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_action_message.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3049 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_actions_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4280 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_app_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2675 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_app_function_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2003 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_app_redacting_filter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_app_restartable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2311 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_component_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8412 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3486 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12122 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_resilient_circuits_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7419 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_rest_helper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5818 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_stomp_component.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:46.098412 resilient_circuits-51.0.1.1.824/tests/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1744 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tests/util/test_resilient_customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1054 2024-04-03 15:15:23.000000 resilient_circuits-51.0.1.1.824/tox.ini
```

### Comparing `resilient_circuits-51.0.1.0.695/CHANGES` & `resilient_circuits-51.0.1.1.824/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+**2024-04: version 51.0.1.1**
+
+* Updated selftest to better handle connection issues when running in App Host
+* Modified ``stomp_prefetch_limit`` configuration option to default to the same value as ``num_workers``.
+  The prefetch limit can still be manually adjusted by changing ``stomp_prefetch_limit`` in the ``[resilient]``
+  section of app.config if you desire the prefetch and workers to have different values
+* Inbound app decorator now expects headers as the second parameter for the decorated function. This is intended
+  for better debugging with more inbound message information passed to the handler
+
 **2024-02: version 51.0.1.0**
 
 * All SOAR Python libraries now officially support Python 3.11
 * Selftest now outputs ``pip`` environment details to better debug failing tests by quickly seeing the dependency versions
 * ``resilient_circuits.rest_helper.get_resilient_client`` now uses a cache rather than a global variable to store
   previously fetched clients. This is an improvement for threaded applications using this logic to store multiple
   client objects for different instances
```

### Comparing `resilient_circuits-51.0.1.0.695/PKG-INFO` & `resilient_circuits-51.0.1.1.824/resilient_circuits.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resilient_circuits
-Version: 51.0.1.0.695
+Name: resilient-circuits
+Version: 51.0.1.1.824
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-51.0.1.0.695/README.md` & `resilient_circuits-51.0.1.1.824/README.md`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/LICENSE` & `resilient_circuits-51.0.1.1.824/resilient_circuits/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/__init__.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/action_message.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/action_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             message = {}
         LOG.debug("Source: %s", source)
         LOG.debug("Headers: %s", json.dumps(headers, indent=2))
         LOG.debug("Message: %s", json.dumps(message, indent=2))
 
         self.deferred = False
         self.message = message
+        self.headers = headers
         self.frame = frame
         self.context = headers.get("Co3ContextToken")
         self.action_id = message.get("action_id")
         self.object_type = message.get("object_type")
         self.test = test
         self.test_msg_id = test_msg_id
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/actions_component.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/actions_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,17 +385,17 @@
 
         timer_internal = int(opts['resilient'].get("stomp_timer_interval", RETRY_TIMER_INTERVAL))
 
         _retry_timer = Timer(timer_internal, Event.create("retry_failed_deliveries"), persist=True)
         _retry_timer.register(self)
 
         # Make a worker thread-pool that will run functions
-        LOG.debug("num_workers set to %s", opts.get("num_workers"))
         self._num_workers = opts.get("num_workers")
         self._functionworker = FunctionWorker(process=False, channel="functionworker", workers=opts.get("num_workers"))
+        LOG.info("num_workers set to %s", opts.get("num_workers"))
         self._functionworker.register(self.root)
 
         if opts.get("test_actions", False):
             # Let user submit test actions from the command line for testing
             LOG.info("Action Tests enabled. Run 'resilient-circuits test' for the interactive action test tool.")
             test_options = {}
             if opts.get("test_port", None):
@@ -420,14 +420,15 @@
         rest_client = self.rest_client()
         self.org_id = rest_client.org_id
 
         list_action_defs = rest_client.get("/actions")["entities"]
         self.action_defs = dict((int(action["id"]), action) for action in list_action_defs)
 
         self.subscribe_headers = {"activemq.prefetchSize": opts["stomp_prefetch_limit"]}
+        LOG.info("stomp_prefetch_limit set to %s", opts["stomp_prefetch_limit"])
 
     # Public Utility methods
 
     def action_name(self, action_id):
         """Get the name of an action, from its id"""
         if action_id is None:
             # Unnamed action, probably triggered from a v28 workflow
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/actions_test_component.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/actions_test_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/app.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/app.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/app_argument_parser.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/app_argument_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,20 +66,23 @@
                                                          "test_actions")) or False
         default_test_host = self.getopt(self.DEFAULT_APP_SECTION, "test_host") or None
         default_test_port = self.getopt(self.DEFAULT_APP_SECTION, "test_port") or None
         default_log_responses = self.getopt(self.DEFAULT_APP_SECTION,
                                             "log_http_responses") or ""
         default_resource_prefix = self.getopt(self.DEFAULT_APP_SECTION, "resource_prefix") or None
         default_num_workers = self.getopt(self.DEFAULT_APP_SECTION, "num_workers") or self.DEFAULT_NUM_WORKERS
+        default_stomp_prefetch_limit = int(self.getopt("resilient", "stomp_prefetch_limit") or default_num_workers)
         default_trap_exception = self.getopt(self.DEFAULT_APP_SECTION, constants.APP_CONFIG_TRAP_EXCEPTION) or self.DEFAULT_APP_EXCEPTION
         default_trap_exception = self._is_true(default_trap_exception)
 
         default_heartbeat_timeout_threshold = self.getopt(self.DEFAULT_APP_SECTION, constants.APP_CONFIG_HEARTBEAT_TIMEOUT_THRESHOLD) or self.DEFAULT_HEARTBEAT_TIMEOUT_THRESHOLD
         default_rc_use_persistent_sessions = self.getopt(self.DEFAULT_APP_SECTION, constants.APP_CONFIG_RC_USE_PERSISTENT_SESSIONS) or self.DEFAULT_RC_USE_PERSISTENT_SESSIONS
 
+        default_selftest_timeout = self.getopt(self.DEFAULT_APP_SECTION, constants.APP_CONFIG_SELFTEST_TIMEOUT) or constants.DEFAULT_SELFTEST_TIMEOUT_VALUE
+
         self._unset_temp_logger()
 
         self.add_argument("--stomp-host",
                           type=str,
                           default=default_stomp_url,
                           help="Resilient server STOMP host url")
         self.add_argument("--stomp-port",
@@ -165,26 +168,34 @@
                           help=("Log all responses from Resilient "
                                 "REST API to this directory"))
         self.add_argument("--num-workers",
                           type=int,
                           default=default_num_workers,
                           help=("Number of FunctionWorkers to use. "
                                 "Number of Functions that can run in parallel"))
+        self.add_argument("--stomp-prefetch-limit",
+                          default=default_stomp_prefetch_limit,
+                          type=int,
+                          help="MAX number of Action Module messages to send before ACK is required")
         self.add_argument("--trap-exception",
                           type=bool,
                           default=default_trap_exception,
                           help=("If set to 'True' a Function's exception will be ignored"))
         self.add_argument("--{0}".format(constants.APP_CONFIG_HEARTBEAT_TIMEOUT_THRESHOLD),
                           type=int,
                           default=default_heartbeat_timeout_threshold,
                           help=("The amount of time in seconds that can occur between HeartbeatTimeouts before exiting"))
         self.add_argument("--{0}".format(constants.APP_CONFIG_RC_USE_PERSISTENT_SESSIONS),
                           type=str,
                           default=default_rc_use_persistent_sessions,
                           help=("Set to False to disable the use of persistent sessions with RequestsCommon in app functions"))
+        self.add_argument("--{0}".format(constants.APP_CONFIG_SELFTEST_TIMEOUT),
+                          type=int,
+                          default=default_selftest_timeout,
+                          help=("Selftest timeout. Defaults to {0}".format(default_selftest_timeout)))
 
     def parse_args(self, args=None, namespace=None, ALLOW_UNRECOGNIZED=False):
         """Parse commandline arguments and construct an opts dictionary"""
         self._setup_temp_logger()
         opts = super(AppArgumentParser, self).parse_args(args, namespace, ALLOW_UNRECOGNIZED)
         if self.config:
             for section in self.config.sections():
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/app_function_component.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/app_restartable.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/app_restartable.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/bin/res_action_test.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/bin/res_action_test.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/bin/resilient_circuits_cmd.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/bin/resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/bin/service_wrapper.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/bin/service_wrapper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/cmds/selftest.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/cmds/selftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
         if not proxy_details:
             proxy_details = get_and_parse_proxy_env_var(res_constants.ENV_HTTP_PROXY)
 
         LOG.info("- Using a '{0}' Proxy with Host '{1}' and Port '{2}'".format(proxy_details.get("scheme"), proxy_details.get("hostname"), proxy_details.get("port")))
 
     try:
-        res_client = helpers.get_resilient_client(ALLOW_UNRECOGNIZED=True)
+        res_client = helpers.get_resilient_client_for_selftest(ALLOW_UNRECOGNIZED=True)
 
     except BasicHTTPException as e:
         # Connection unauthorized
         error_connecting_to_soar(host, e.response.reason, e.response.status_code)
 
     except SimpleHTTPException as e:
         # Incorrect User/Password
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/component_loader.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/constants.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 PASSWORD_PATTERNS = ['token', 'pass', 'secret', 'pin', 'key', 'session', 'connection', 'jwt']
 
 INBOUND_MSG_DEST_PREFIX = "inbound_destinations"
 
 APP_FUNCTION_PAYLOAD_VERSION = 2.0
 
 MIN_NUM_WORKERS = 1
-MAX_NUM_WORKERS = 500
+MAX_NUM_WORKERS = 2000
 MIN_LOG_BYTES = 100000
 MIN_BACKUP_COUNT = 0
 DEFAULT_SELFTEST_TIMEOUT_VALUE = 10
 
 APP_LOG_DIR = os.environ.get("APP_LOG_DIR", "logs")
 CMDS_LOGGER_NAME = "resilient_circuits_cmd_logger"
 LOG_DIVIDER = "\n------------------------\n"
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/data/app.config.base` & `resilient_circuits-51.0.1.1.824/resilient_circuits/data/app.config.base`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 # Setting log_max_bytes to 0 is unlimited.
 # Setting log_backup_count to 0 means no backups will be used.
 # NOTE: if either log_max_bytes or log_backup_count are zero,
 # the log file will never roll over and will continue to grow
 #log_max_bytes=10000000
 #log_backup_count=10
 
-# The number of Functions to run concurrently (within the range: 1 <= 500)
+# The number of Functions to run concurrently (within the range: 1 <= 2000)
 num_workers=50
 
 # Timeout value in seconds for selftest to wait for a response from SOAR
 selftest_timeout=10
 
 # If set to True a Function's exception will be ignored with the error sent as a Status Message
 # and a default payload returned with 'success=False', allowing the Workflow or Playbook to continue
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/decorators.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,16 +49,16 @@
         func.function = True
 
         # Circuits properties
         func.names = self.names
         func.priority = self.kwargs.get("priority", 0)
         func.channel = self.kwargs.get("channel", ",".join(["functions.{}".format(name) for name in self.names]))
         func.override = self.kwargs.get("override", False)
-        
-        # If getfullargspec if available to us 
+
+        # If getfullargspec if available to us
         if hasattr(_inspect, 'getfullargspec'):
             args = _inspect.getfullargspec(func)[0]
         else:  # fall back to deprecated getargspec
             args = _inspect.getargspec(func)[0]
 
         if args and args[0] == "self":
             del args[0]
@@ -158,22 +158,45 @@
                 Returns result_list when method with the decorator `@inbound_app(<inbound_destination_api_name>)` is
                 finished processing.
 
                 A method that has this handler should yield a str when done
                     -  E.g:
                         `yield "Processing Complete!"`
 
+                The method that is wrapped with this handler should will receive three items:
+                    - message
+                    - headers
+                    - inbound action
+
+                The subclass of ``ResilientComponent`` is also required to set the
+                ``app_configs`` attribute.
+
+                Example:
+
+                .. code-block:: python
+
+                    class SoarInboundConsumer(ResilientComponent):
+                        def __init__(self, opts):
+                            super(SoarInboundConsumer, self).__init__(opts)
+                            self.opts = opts
+                            self.app_configs = opts.get(PACKAGE_NAME, {})
+
+                        @inbound_app(QUEUE_NAME)
+                        def _inbound_soar_escalator(self, message, headers, inbound_action):
+                            pass
+
                 :param evt: The Event with the StompFrame and the Message read off the Message Destination
                 :type ia: resilient_circuits.action_message.FunctionMessage
                 """
                 result_list = []
                 LOG.debug("Running _invoke_inbound_app in Thread: %s", threading.currentThread().name)
 
                 # Invoke the actual Function
-                ia_results = ia(itself, evt.message, evt.message.get("action", "Unknown"))
+                # Pass along the message, the headers, and the action if present in the message
+                ia_results = ia(itself, evt.message, evt.headers, evt.message.get("action", "Unknown"))
 
                 for r in ia_results:
                     LOG.debug(r)
                     result_list.append(r)
 
                 return result_list
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/helpers.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,27 +128,40 @@
     if not path_config_file:
         path_config_file = get_config_file()
 
     configs = AppArgumentParser(config_file=path_config_file).parse_args(ALLOW_UNRECOGNIZED=ALLOW_UNRECOGNIZED)
     return configs
 
 
-def get_resilient_client(path_config_file=None, ALLOW_UNRECOGNIZED=False):
+def get_resilient_client_for_selftest(path_config_file=None, ALLOW_UNRECOGNIZED=False, default_connection_retries=3):
     """
     Return a SimpleClient for Resilient REST API using configurations
-    options from provided path_config_file or from ~/.resilient/app.config
+    options from provided path_config_file or from ~/.resilient/app.config.
+
+    This method is only intended for use in selftest. For other use cases, use
+    ``from resilient_circuits.rest_helper import get_resilient_client``
 
     :param path_config_file: path to the app.config to parse
     :type path_config_file: str
     :param ALLOW_UNRECOGNIZED: bool to specify if AppArgumentParser will allow unknown comandline args or not. Default is False
     :type ALLOW_UNRECOGNIZED: bool
+    :param default_connection_retries: used for selftest limiting the number of retries when connecting. Default is 3 tries
+    :type default_connection_retries: int
     :return: SimpleClient for Resilient REST API
     :rtype: SimpleClient
     """
-    client = get_client(get_configs(path_config_file=path_config_file, ALLOW_UNRECOGNIZED=ALLOW_UNRECOGNIZED))
+
+    # if default_connection_retries is provided or default
+    if default_connection_retries is not None:
+        # add retry configs
+        kwargs = {res_constants.APP_CONFIG_MAX_CONNECTION_RETRIES: default_connection_retries}
+    else:
+        kwargs = {}
+
+    client = get_client(get_configs(path_config_file=path_config_file, ALLOW_UNRECOGNIZED=ALLOW_UNRECOGNIZED), **kwargs)
     return client
 
 
 def validate_configs(configs, validate_dict):
     """
     Checks if the configs are valid and raise a ValueError if they are not.
     Check if the config is required, has a value and meets its 'condition'
@@ -359,15 +372,15 @@
 
     return heartbeat_timeouts
 
 def sub_fn_inputs_from_protected_secrets(fn_inputs, opts):
     """
     Substitute any protected secret *or regular secret
     into a function input. Requires the ``opts`` dictionary
-    (usually actually a AppConfigManager object) to be 
+    (usually actually a AppConfigManager object) to be
     given to properly create a temporary AppConfigManager
     that will have access to the pam plugin if relevant.
 
     This supports the same syntax as secrets in app.config:
       - if $ or ^ starts a string, if the following string
         is found in secrets, it will be replaced
       - if ${} or ^{} is found within a string, the value
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/rest_helper.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/stomp_component.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/stomp_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,44 +219,45 @@
             LOG.error("Exiting due to unrecoverable error")
             sys.exit(1) # this will exit resilient-circuits
         return "fail"
 
     @handler("ServerHeartbeat")
     def check_server_heartbeat(self, event):
         """ Confirm that heartbeat from server hasn't timed out """
+        LOG.debug("Checking server heartbeat")
         now = time.time()
         self.last_heartbeat = self._client.lastReceived or self.last_heartbeat
         if self.last_heartbeat:
             elapsed = now-self.last_heartbeat
         else:
             elapsed = -1
         if ((self._client.serverHeartBeat / 1000.0) * self.ALLOWANCE + self.last_heartbeat) < now:
             LOG.error("Server heartbeat timeout. %d seconds since last heartbeat.", elapsed)
             event.success = False
             self.fire(HeartbeatTimeout(now))
 
     @handler("ClientHeartbeat")
     def send_heartbeat(self, event):
         if self.connected:
-            LOG.debug("Sending heartbeat")
+            LOG.debug("Sending client heartbeat")
             try:
                 self._client.beat()
             except (StompConnectionError, StompError) as err:
                 event.success = False
                 self.fire(OnStompError(None, err))
 
     @handler("generate_events")
     def generate_events(self, event):
         event.reduce_time_left(0.1)
         if not self.connected:
             return
         try:
             if self._client.canRead(0):
                 frame = self._client.receiveFrame()
-                LOG.debug("Recieved frame %s", frame)
+                LOG.debug("Received frame %s", frame)
                 if frame.command == StompSpec.ERROR:
                     self.fire(OnStompError(frame, None))
                 else:
                     self.fire(Message(frame))
         except (StompConnectionError, StompError) as err:
             LOG.error("Failed attempt to generate events.")
             self.fire(OnStompError(None, err))
@@ -264,15 +265,15 @@
     @handler("Send")
     def send(self, event, destination, body, headers=None, receipt=None):
         LOG.debug("send()")
         try:
             self._client.send(destination, body=body.encode('utf-8'), headers=headers, receipt=receipt)
             LOG.debug("Message sent")
         except (StompConnectionError, StompError) as err:
-            LOG.error("Error sending frame")
+            LOG.error("Error sending frame. %s", err)
             event.success = False
             self.fire(OnStompError(None, err))
             raise  # To fire Send_failure event
 
     @handler("Subscribe")
     def _subscribe(self, event, destination, additional_headers=None, ack=ACK_CLIENT_INDIVIDUAL):
         if ack not in ACK_MODES:
@@ -324,15 +325,15 @@
     @handler("Ack")
     def ack_frame(self, event, frame):
         LOG.debug("ack_frame()")
         try:
             self._client.ack(frame)
             LOG.debug("Ack Sent")
         except (StompConnectionError, StompError) as err:
-            LOG.error("Error sending ack")
+            LOG.error("Error sending ack. %s", err)
             event.success = False
             self.fire(OnStompError(frame, err))
             raise  # To fire Ack_failure event
 
     def get_subscription(self, frame):
         """ Get subscription from frame """
         _, token = self._client.message(frame)
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/stomp_events.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/stomp_events.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/stomp_transport.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/stomp_transport.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/template_functions.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/template_functions.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/util/__init__.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/util/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/util/resilient_config.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/util/resilient_config.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/util/resilient_customize.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/util/resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits/validate_configs.py` & `resilient_circuits-51.0.1.1.824/resilient_circuits/validate_configs.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 
 VALIDATE_DICT = {
     "num_workers": {
         "required": False,
         "valid_condition": lambda c: True if c >= MIN_NUM_WORKERS and c <= MAX_NUM_WORKERS else False,
         "invalid_msg": "num_workers must be in the range {} <= {}".format(MIN_NUM_WORKERS, MAX_NUM_WORKERS)
     },
+    "stomp_prefetch_limit": {
+        "required": False,
+        "valid_condition": lambda c: True if c >= MIN_NUM_WORKERS and c <= MAX_NUM_WORKERS else False,
+        "invalid_msg": "stomp_prefetch_limit must be in the range {} <= {}".format(MIN_NUM_WORKERS, MAX_NUM_WORKERS)
+    },
     APP_CONFIG_LOG_MAX_BYTES: {
         "required": False,
         "valid_condition": lambda c: True if c == 0 or c >= MIN_LOG_BYTES else False,
         "invalid_msg": "{} must be either 0 or >= {}".format(APP_CONFIG_LOG_MAX_BYTES, MIN_LOG_BYTES)
     },
     APP_CONFIG_LOG_BACKUP_COUNT: {
         "required": False,
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits.egg-info/PKG-INFO` & `resilient_circuits-51.0.1.1.824/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: resilient-circuits
-Version: 51.0.1.0.695
+Name: resilient_circuits
+Version: 51.0.1.1.824
 Summary: Framework used to run IBM SOAR Apps and Integrations
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_circuits-51.0.1.0.695/resilient_circuits.egg-info/SOURCES.txt` & `resilient_circuits-51.0.1.1.824/resilient_circuits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/setup.cfg` & `resilient_circuits-51.0.1.1.824/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient     >= 51.0.1.0
-	resilient-lib >= 51.0.1.0
+	resilient     >= 51.0.1.1
+	resilient-lib >= 51.0.1.1
 	
 	stompest      ~= 2.3
 	circuits      ~= 3.2
 	pysocks       ~= 1.6
 	filelock      ~= 3.2
 	
 	watchdog      ~= 2.1;  python_version >= "3.6"
```

### Comparing `resilient_circuits-51.0.1.0.695/tests/cmds/test_selftest.py` & `resilient_circuits-51.0.1.1.824/tests/cmds/test_selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/conftest.py` & `resilient_circuits-51.0.1.1.824/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/helpers.py` & `resilient_circuits-51.0.1.1.824/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_app_config` & `resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_app_config`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_app_function_component.py` & `resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_commented_app_config` & `resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_commented_app_config`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_component.py` & `resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_component.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     @handler("reload")
     def _reload(self, event, opts):
         """Configuration options have changed, save new values"""
         self.app_configs = opts.get(PACKAGE_NAME, {})
 
     @inbound_app(QUEUE_NAME)
-    def _inbound_app_mock_one(self, message, inbound_action):
+    def _inbound_app_mock_one(self, message, headers, inbound_action):
 
         if inbound_action == "create":
             msg_content = message.get("content", {})
             LOG.info(u"Creating incident\nIncident Description: %s", msg_content.get("description", "None"))
 
         elif inbound_action == "close":
             LOG.info(u"Closing incident")
@@ -44,20 +44,24 @@
 
         else:
             LOG.error(u"Unsupported functionality. Message: %s", message)
 
         yield "Done!"
 
     @inbound_app(mock_constants.MOCK_INBOUND_Q_NAME)
-    def inbound_app_mock(self, message, inbound_action):
+    def inbound_app_mock(self, message, headers, inbound_action):
         assert isinstance(message, dict)
+        assert isinstance(headers, dict)
+        assert headers["destination"] == "/queue/inbound_destinations.201.{0}".format(mock_constants.MOCK_INBOUND_Q_NAME)
         yield inbound_action
 
     @inbound_app(mock_constants.MOCK_INBOUND_Q_NAME_CREATE)
-    def inbound_app_mock_create(self, message, inbound_action):
+    def inbound_app_mock_create(self, message, headers, inbound_action):
         assert inbound_action == "create"
         assert isinstance(message, dict)
+        assert isinstance(headers, dict)
+        assert headers["destination"] == "/queue/inbound_destinations.201.{0}".format(mock_constants.MOCK_INBOUND_Q_NAME_CREATE)
         yield u"Mock incident created with unicode զ է ը թ"
 
     @inbound_app(mock_constants.MOCK_INBOUND_Q_NAME_EX)
-    def inbound_app_mock_raise_exception(self, message, inbound_action):
+    def inbound_app_mock_raise_exception(self, message, headers, inbound_action):
         raise IntegrationError(u"mock error message with unicode զ է ը թ ժ ի լ խ")
```

### Comparing `resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_constants.py` & `resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_constants.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_function_component.py` & `resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_import_definition.txt` & `resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_import_definition.txt`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/shared_mock_data/mock_paths.py` & `resilient_circuits-51.0.1.1.824/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_action_message.py` & `resilient_circuits-51.0.1.1.824/tests/test_action_message.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_actions_component.py` & `resilient_circuits-51.0.1.1.824/tests/test_actions_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_app_config.py` & `resilient_circuits-51.0.1.1.824/tests/test_app_config.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_app_function_component.py` & `resilient_circuits-51.0.1.1.824/tests/test_app_function_component.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_app_redacting_filter.py` & `resilient_circuits-51.0.1.1.824/tests/test_app_redacting_filter.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_app_restartable.py` & `resilient_circuits-51.0.1.1.824/tests/test_app_restartable.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_component_loader.py` & `resilient_circuits-51.0.1.1.824/tests/test_component_loader.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_decorators.py` & `resilient_circuits-51.0.1.1.824/tests/test_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         with pytest.raises(IntegrationError, match=r"mock error message with unicode"):
             helpers.call_inbound_app(circuits_app, mock_constants.MOCK_INBOUND_Q_NAME_EX)
 
     def test_too_many_q_names(self):
         with pytest.raises(ValueError, match=r"Usage: @inbound_app\(<inbound_destination_api_name>\)"):
             class MockInboundAppComponent2(ResilientComponent):
                 @inbound_app("mock_q_2", "mock_q_3")
-                def inbound_app_mock_2(self, message, *args, **kwargs):
+                def inbound_app_mock_2(self, message, headers, *args, **kwargs):
                     return
 
 
 class TestAppFunctionDecorator:
 
     def test_basic_decoration(self):
         assert AppFunctionMockComponent._app_function_mock_one.handler is True
```

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_errors.py` & `resilient_circuits-51.0.1.1.824/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_helpers.py` & `resilient_circuits-51.0.1.1.824/tests/test_helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # (c) Copyright IBM Corp. 2010, 2022. All Rights Reserved.
 
 import os
 import time
 
+from mock import patch
 import pkg_resources
 import pytest
 from resilient_app_config_plugins.plugin_base import PAMPluginInterface
 from resilient_circuits import ResilientComponent, constants, function, helpers
 from resilient_circuits.stomp_events import HeartbeatTimeout
 from tests import (AppFunctionMockComponent, MockInboundAppComponent,
                    mock_constants)
@@ -232,14 +233,38 @@
     assert filtered_hbs[1].ts == 20
     assert filtered_hbs[-1].ts == 30
 
 
 def test_filter_heartbeat_timeout_events_empty():
     assert helpers.filter_heartbeat_timeout_events([]) == []
 
+@patch("resilient_circuits.helpers.get_client")
+@patch("resilient_circuits.helpers.get_configs")
+def test_get_resilient_client_for_selftest(patch_get_configs, patch_co3_get_client):
+    patch_get_configs.return_value = {}
+
+    helpers.get_resilient_client_for_selftest(ALLOW_UNRECOGNIZED=True)
+    patch_co3_get_client.assert_called_with({}, max_connection_retries=3)
+
+@patch("resilient_circuits.helpers.get_client")
+@patch("resilient_circuits.helpers.get_configs")
+def test_get_resilient_client_for_selftest_overwrite_retries(patch_get_configs, patch_co3_get_client):
+    patch_get_configs.return_value = {}
+
+    helpers.get_resilient_client_for_selftest(ALLOW_UNRECOGNIZED=True, default_connection_retries=5)
+    patch_co3_get_client.assert_called_with({}, max_connection_retries=5)
+
+@patch("resilient_circuits.helpers.get_client")
+@patch("resilient_circuits.helpers.get_configs")
+def test_get_resilient_client_for_selftest_set_no_retries(patch_get_configs, patch_co3_get_client):
+    patch_get_configs.return_value = {}
+
+    helpers.get_resilient_client_for_selftest(ALLOW_UNRECOGNIZED=True, default_connection_retries=None)
+    patch_co3_get_client.assert_called_with({})
+
 def test_sub_fn_inputs_from_protected_secrets(fx_reset_environmental_variables):
     class MyMockPlugin(PAMPluginInterface):
         def __init__(self, *args, **kwargs):
             pass
         def get(self, key, default=None):
             return "PAM secret found"
         def selftest(self):
```

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_resilient_circuits_cmd.py` & `resilient_circuits-51.0.1.1.824/tests/test_resilient_circuits_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_rest_helper.py` & `resilient_circuits-51.0.1.1.824/tests/test_rest_helper.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/test_templates.py` & `resilient_circuits-51.0.1.1.824/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tests/util/test_resilient_customize.py` & `resilient_circuits-51.0.1.1.824/tests/util/test_resilient_customize.py`

 * *Files identical despite different names*

### Comparing `resilient_circuits-51.0.1.0.695/tox.ini` & `resilient_circuits-51.0.1.1.824/tox.ini`

 * *Files identical despite different names*

