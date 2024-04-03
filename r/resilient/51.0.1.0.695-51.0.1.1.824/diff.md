# Comparing `tmp/resilient-51.0.1.0.695.tar.gz` & `tmp/resilient-51.0.1.1.824.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient-51.0.1.0.695.tar", last modified: Wed Feb 14 14:45:42 2024, max compression
+gzip compressed data, was "resilient-51.0.1.1.824.tar", last modified: Wed Apr  3 15:16:05 2024, max compression
```

## Comparing `resilient-51.0.1.0.695.tar` & `resilient-51.0.1.1.824.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10829 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.967633 resilient-51.0.1.0.695/co3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      377 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/co3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.967633 resilient-51.0.1.0.695/resilient/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11944 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/app_config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.967633 resilient-51.0.1.0.695/resilient/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/bin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/bin/finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/bin/gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/bin/res_keyring.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37206 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12801 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/co3argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40264 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1966 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      854 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/definitions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17651 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2607 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/resilient/resilient_rest_mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.967633 resilient-51.0.1.0.695/resilient.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2024-02-14 14:45:42.000000 resilient-51.0.1.0.695/resilient.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2024-02-14 14:45:42.000000 resilient-51.0.1.0.695/resilient.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:42.000000 resilient-51.0.1.0.695/resilient.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2024-02-14 14:45:42.000000 resilient-51.0.1.0.695/resilient.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      367 2024-02-14 14:45:42.000000 resilient-51.0.1.0.695/resilient.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-02-14 14:45:42.000000 resilient-51.0.1.0.695/resilient.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2037 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/tests/shared_mock_data/mock_plugins/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_plugins/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_plugins/mock_plugins.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/tests/shared_mock_data/mock_responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_responses/session.JSON
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/.jwk/
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/API_KEY
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/EMAIL
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/EMPTY
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/PASSWORD
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/shared_mock_data/mock_secrets/URL
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/template_test.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9531 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/test_app_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9693 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/test_co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/test_co3_ii.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21843 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/test_co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/test_co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/test_finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11152 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/xtest_gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/xtest_patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tests/xtest_res_keyring.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:42.971633 resilient-51.0.1.0.695/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tools/res_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1048 2024-02-14 14:45:11.000000 resilient-51.0.1.0.695/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11169 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.098412 resilient-51.0.1.1.824/co3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      377 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/co3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.102412 resilient-51.0.1.1.824/resilient/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11944 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/app_config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.102412 resilient-51.0.1.1.824/resilient/bin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/bin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/bin/finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/bin/gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/bin/res_keyring.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37206 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12447 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/co3argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40264 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1966 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      854 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/definitions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17651 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2607 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/resilient_rest_mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.102412 resilient-51.0.1.1.824/resilient.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2024-04-03 15:16:05.000000 resilient-51.0.1.1.824/resilient.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      367 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2037 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/mock_plugins/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_plugins/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_plugins/mock_plugins.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/mock_responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_responses/session.JSON
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/.jwk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/API_KEY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/EMAIL
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/EMPTY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/PASSWORD
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/URL
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/template_test.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9531 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_app_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9693 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_co3_ii.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21843 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11152 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/xtest_gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/xtest_patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/xtest_res_keyring.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tools/res_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1129 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tox.ini
```

### Comparing `resilient-51.0.1.0.695/CHANGES` & `resilient-51.0.1.1.824/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+**2024-04: version 51.0.1.1**
+
+* Updated ``jwcrypto`` dependency requirement to ``~= 1.5.6`` (for Python 3.9 and 3.11) to address CVE-2024-28102
+  Note that Python 3.6 and Python 2.7 are no longer receiving security updates and should be moved away from immediately.
+  See previous release below for details on our support for Python 3.11
+
 **2024-02: version 51.0.1.0**
 
 * All SOAR Python libraries now officially support Python 3.11
 * All SOAR Python libraries are now published in a docker container format on Quay.io.
   This is to better support our apps build process to include the latest SOAR libraries
   in the base image. This also allows us to better control the OS and Python dependencies
   that appear in the eventual app container. To take advantage of this new image in your app
```

### Comparing `resilient-51.0.1.0.695/PKG-INFO` & `resilient-51.0.1.1.824/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 51.0.1.0.695
+Version: 51.0.1.1.824
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-51.0.1.0.695/README.md` & `resilient-51.0.1.1.824/README.md`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/LICENSE` & `resilient-51.0.1.1.824/resilient/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/__init__.py` & `resilient-51.0.1.1.824/resilient/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/app_config.py` & `resilient-51.0.1.1.824/resilient/app_config.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/bin/finfo.py` & `resilient-51.0.1.1.824/resilient/bin/finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/bin/gadget.py` & `resilient-51.0.1.1.824/resilient/bin/gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/bin/res_keyring.py` & `resilient-51.0.1.1.824/resilient/bin/res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/co3.py` & `resilient-51.0.1.1.824/resilient/co3.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/co3argparse.py` & `resilient-51.0.1.1.824/resilient/co3argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         default_org = self.getopt("resilient", "org")
         default_cafile = self.getopt("resilient", "cafile")
         default_cache_ttl = int(self.getopt("resilient", "cache_ttl") or 0)
         default_proxy_host = self.getopt("resilient", "proxy_host")
         default_proxy_port = self.getopt("resilient", "proxy_port") or 0
         default_proxy_user = self.getopt("resilient", "proxy_user")
         default_proxy_password = self.getopt("resilient", "proxy_password")
-        default_stomp_prefetch_limit = int(self.getopt("resilient", "stomp_prefetch_limit") or 20)
         default_resilient_mock = self.getopt("resilient", "resilient_mock")
 
         default_max_request_retries = self.getopt(constants.PACKAGE_NAME, constants.APP_CONFIG_REQUEST_MAX_RETRIES) or constants.APP_CONFIG_REQUEST_MAX_RETRIES_DEFAULT
         default_request_retry_delay = self.getopt(constants.PACKAGE_NAME, constants.APP_CONFIG_REQUEST_RETRY_DELAY) or constants.APP_CONFIG_REQUEST_RETRY_DELAY_DEFAULT
         default_request_retry_backoff = self.getopt(constants.PACKAGE_NAME, constants.APP_CONFIG_REQUEST_RETRY_BACKOFF) or constants.APP_CONFIG_REQUEST_RETRY_BACKOFF_DEFAULT
 
         # PAM plugin configurations
@@ -184,19 +183,14 @@
                           default=default_proxy_user,
                           help="HTTP Proxy username for Resilient connection authentication.")
 
         self.add_argument("--proxy_password",
                           default=default_proxy_password,
                           help="HTTP Proxy password for Resilient connection authentication.")
 
-        self.add_argument("--stomp-prefetch-limit",
-                          default=default_stomp_prefetch_limit,
-                          type=int,
-                          help="MAX number of Action Module messages to send before ACK is required")
-
         self.add_argument("--{0}".format(constants.APP_CONFIG_REQUEST_MAX_RETRIES),
                           type=int,
                           default=default_max_request_retries,
                           help="Max number of times to retry a request to SOAR before exiting. Defaults to 5")
 
         self.add_argument("--{0}".format(constants.APP_CONFIG_REQUEST_RETRY_DELAY),
                           type=int,
```

### Comparing `resilient-51.0.1.0.695/resilient/co3base.py` & `resilient-51.0.1.1.824/resilient/co3base.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/co3sslutil.py` & `resilient-51.0.1.1.824/resilient/co3sslutil.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/constants.py` & `resilient-51.0.1.1.824/resilient/constants.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/definitions.py` & `resilient-51.0.1.1.824/resilient/definitions.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/helpers.py` & `resilient-51.0.1.1.824/resilient/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/patch.py` & `resilient-51.0.1.1.824/resilient/patch.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient/resilient_rest_mock.py` & `resilient-51.0.1.1.824/resilient/resilient_rest_mock.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/resilient.egg-info/PKG-INFO` & `resilient-51.0.1.1.824/resilient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient
-Version: 51.0.1.0.695
+Version: 51.0.1.1.824
 Summary: Python client module for the IBM SOAR REST API
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient-51.0.1.0.695/resilient.egg-info/SOURCES.txt` & `resilient-51.0.1.1.824/resilient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/setup.cfg` & `resilient-51.0.1.1.824/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 	requests          ~= 2.27
 	requests-toolbelt ~= 1.0
 	six               ~= 1.16
 	
 	keyring           ~= 23.5;   python_version  > "3.6"
 	cachetools        ~= 5.0;    python_version  > "3.6"
 	setuptools        ~= 65.5.1; python_version  > "3.6"
-	jwcrypto          ~= 1.5.3;  python_version  > "3.6"
+	jwcrypto          ~= 1.5.6;  python_version  > "3.6"
 	
 	keyring           ~= 23.4;   python_version == "3.6"
 	cachetools        ~= 2.1;    python_version == "3.6"
 	setuptools        ~= 59.6;   python_version == "3.6"
 	jwcrypto          == 1.5.1;  python_version == "3.6" # see https://github.com/latchset/jwcrypto/pull/340
 	
 	configparser      ~= 4.0;    python_version == "2.7"
```

### Comparing `resilient-51.0.1.0.695/tests/conftest.py` & `resilient-51.0.1.1.824/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/helpers.py` & `resilient-51.0.1.1.824/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/shared_mock_data/mock_paths.py` & `resilient-51.0.1.1.824/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/shared_mock_data/mock_plugins/mock_plugins.py` & `resilient-51.0.1.1.824/tests/shared_mock_data/mock_plugins/mock_plugins.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/shared_mock_data/mock_responses/session.JSON` & `resilient-51.0.1.1.824/tests/shared_mock_data/mock_responses/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/test_app_config.py` & `resilient-51.0.1.1.824/tests/test_app_config.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/test_co3.py` & `resilient-51.0.1.1.824/tests/test_co3.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/test_co3_ii.py` & `resilient-51.0.1.1.824/tests/test_co3_ii.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/test_co3base.py` & `resilient-51.0.1.1.824/tests/test_co3base.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/test_finfo.py` & `resilient-51.0.1.1.824/tests/test_finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/test_helpers.py` & `resilient-51.0.1.1.824/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/xtest_gadget.py` & `resilient-51.0.1.1.824/tests/xtest_gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/xtest_patch.py` & `resilient-51.0.1.1.824/tests/xtest_patch.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tests/xtest_res_keyring.py` & `resilient-51.0.1.1.824/tests/xtest_res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tools/res_utils.py` & `resilient-51.0.1.1.824/tools/res_utils.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.0.695/tox.ini` & `resilient-51.0.1.1.824/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 [testenv]
 passenv=TEST_RESILIENT_*
 deps =
     pytest
     pytest-cov
     mock
-    requests-mock ~= 1.9
+    requests-mock     ~= 1.12; python_version>="3.6"
+    requests-mock      < 1.12; python_version=="2.7"
     jinja2 ~= 3.0; python_version >= "3.6" # only needed for tests
     jinja2 ~= 2.0; python_version == "2.7"
     setuptools-scm<6.0.0 ; python_version=="2.7"
 
 setenv =
     SETUPTOOLS_SCM_PRETEND_VERSION={env:SETUPTOOLS_SCM_PRETEND_VERSION}
```

