# Comparing `tmp/resilient_lib-51.0.1.0.695.tar.gz` & `tmp/resilient_lib-51.0.1.1.824.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_lib-51.0.1.0.695.tar", last modified: Wed Feb 14 14:45:57 2024, max compression
+gzip compressed data, was "resilient_lib-51.0.1.1.824.tar", last modified: Wed Apr  3 15:16:24 2024, max compression
```

## Comparing `resilient_lib-51.0.1.0.695.tar` & `resilient_lib-51.0.1.1.824.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.995633 resilient_lib-51.0.1.0.695/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7527 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2648 2024-02-14 14:45:57.995633 resilient_lib-51.0.1.0.695/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.987633 resilient_lib-51.0.1.0.695/resilient_lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      871 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.991633 resilient_lib-51.0.1.0.695/resilient_lib/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/function_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      795 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/integration_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30035 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/poller_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24854 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/requests_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24321 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/resilient_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/templates_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/components/workflow_status.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.991633 resilient_lib-51.0.1.0.695/resilient_lib/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12644 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/ui/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4491 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/ui/conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7207 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/ui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/ui/tab.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.991633 resilient_lib-51.0.1.0.695/resilient_lib/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      410 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/resilient_lib/util/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.987633 resilient_lib-51.0.1.0.695/resilient_lib.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2648 2024-02-14 14:45:57.000000 resilient_lib-51.0.1.0.695/resilient_lib.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2899 2024-02-14 14:45:57.000000 resilient_lib-51.0.1.0.695/resilient_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:57.000000 resilient_lib-51.0.1.0.695/resilient_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2024-02-14 14:45:57.000000 resilient_lib-51.0.1.0.695/resilient_lib.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2024-02-14 14:45:57.000000 resilient_lib-51.0.1.0.695/resilient_lib.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-02-14 14:45:57.000000 resilient_lib-51.0.1.0.695/resilient_lib.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1455 2024-02-14 14:45:57.995633 resilient_lib-51.0.1.0.695/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.991633 resilient_lib-51.0.1.0.695/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3114 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.991633 resilient_lib-51.0.1.0.695/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/data/default_template.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/data/override_template.jinja
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.991633 resilient_lib-51.0.1.0.695/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.991633 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_certs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_certs/cert.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_certs/key.open.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.995633 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__actions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__attachments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__const.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      798 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__functions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__incidents_.*.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9043 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__layouts.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__orgs_[0-9]+$.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1974 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__rest_session.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__task.json
--rw-rw-r--   0 travis    (2000) travis    (2000)  1618280 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types[\w]*$.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      775 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types_artifact.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types_function_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16122 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_POST__attachment.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1974 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_POST__rest_session.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      359 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_POST__table_data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9051 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_PUT__layouts_[0-9]+.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/test_function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/test_html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/test_oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/test_payload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13935 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/test_poller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38969 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/test_requests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:57.995633 resilient_lib-51.0.1.0.695/tests/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2974 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/ui/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1986 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/ui/test_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/ui/test_permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tests/ui/test_tab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      986 2024-02-14 14:45:11.000000 resilient_lib-51.0.1.0.695/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.210412 resilient_lib-51.0.1.1.824/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7635 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2648 2024-04-03 15:16:24.210412 resilient_lib-51.0.1.1.824/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.198412 resilient_lib-51.0.1.1.824/resilient_lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      871 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/resilient_lib/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/function_result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      795 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/integration_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30035 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/poller_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24854 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/requests_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24321 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/resilient_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/templates_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/workflow_status.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/resilient_lib/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      293 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12644 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4491 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7207 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/tab.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/resilient_lib/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      410 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/util/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2648 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2899 2024-04-03 15:16:24.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      188 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1455 2024-04-03 15:16:24.210412 resilient_lib-51.0.1.1.824/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3114 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/conftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      119 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/data/default_template.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/data/override_template.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.206412 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/cert.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/key.open.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.206412 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__actions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__attachments.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__const.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      798 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__functions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__incidents_.*.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9043 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__layouts.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       36 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__orgs_[0-9]+$.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1974 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__rest_session.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__task.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1618280 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types[\w]*$.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      775 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_artifact.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_function_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16122 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_POST__attachment.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1974 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_POST__rest_session.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      359 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_POST__table_data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9051 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_PUT__layouts_[0-9]+.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_payload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13935 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_poller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38969 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_requests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.210412 resilient_lib-51.0.1.1.824/tests/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2974 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1986 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/test_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/test_permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/test_tab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tox.ini
```

### Comparing `resilient_lib-51.0.1.0.695/CHANGES` & `resilient_lib-51.0.1.1.824/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2024-04: version 51.0.1.1**
+
+* No major changes. Just bumping build number to coincide with other builds
+
 **2024-02: version 51.0.1.0**
 
 * All SOAR Python libraries now officially support Python 3.11
 * Updated ``pytz`` dependency requirement to ``~= 2024.1``
 * Updated ``jinja2`` dependency requirement to ``~= 3.1`` to address CVE-2024-22195
 
 **2024-01: version 51.0.0.2**
```

### Comparing `resilient_lib-51.0.1.0.695/PKG-INFO` & `resilient_lib-51.0.1.1.824/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_lib
-Version: 51.0.1.0.695
+Version: 51.0.1.1.824
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-51.0.1.0.695/README.md` & `resilient_lib-51.0.1.1.824/README.md`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/__init__.py` & `resilient_lib-51.0.1.1.824/resilient_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/function_metrics.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/function_result.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/function_result.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/html2markdown.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/integration_errors.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/integration_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/oauth2_client_credentials_session.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/poller_common.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/poller_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/requests_common.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/requests_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/resilient_common.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/resilient_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/templates_common.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/templates_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/components/workflow_status.py` & `resilient_lib-51.0.1.1.824/resilient_lib/components/workflow_status.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/ui/common.py` & `resilient_lib-51.0.1.1.824/resilient_lib/ui/common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/ui/conditions.py` & `resilient_lib-51.0.1.1.824/resilient_lib/ui/conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/ui/elements.py` & `resilient_lib-51.0.1.1.824/resilient_lib/ui/elements.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/ui/tab.py` & `resilient_lib-51.0.1.1.824/resilient_lib/ui/tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib/util/config.py` & `resilient_lib-51.0.1.1.824/resilient_lib/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib.egg-info/PKG-INFO` & `resilient_lib-51.0.1.1.824/resilient_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-lib
-Version: 51.0.1.0.695
+Version: 51.0.1.1.824
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `resilient_lib-51.0.1.0.695/resilient_lib.egg-info/SOURCES.txt` & `resilient_lib-51.0.1.1.824/resilient_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/setup.cfg` & `resilient_lib-51.0.1.1.824/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient      >= 51.0.1.0
+	resilient      >= 51.0.1.1
 	
 	pytz           ~= 2024.1
 	deprecated     ~= 1.2
 	beautifulsoup4 ~= 4.9
 	
 	jinja2         ~= 3.1; python_version > "3.6"
```

### Comparing `resilient_lib-51.0.1.0.695/tests/conftest.py` & `resilient_lib-51.0.1.1.824/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_certs/cert.pem` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/cert.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_certs/key.open.pem` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/key.open.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__actions.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__actions.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__attachments.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__attachments.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__const.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__const.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__functions.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__functions.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__incidents_.*.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__incidents_.*.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__layouts.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__layouts.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__rest_session.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__rest_session.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__task.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__task.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types[\w]*$.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types[\w]*$.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types_artifact.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_artifact.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types_function_fields.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_function_fields.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident_fields.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident_fields.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_POST__rest_session.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_POST__rest_session.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/shared_mock_data/mock_responses/200_JSON_PUT__layouts_[0-9]+.json` & `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_PUT__layouts_[0-9]+.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/test_common.py` & `resilient_lib-51.0.1.1.824/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/test_function_metrics.py` & `resilient_lib-51.0.1.1.824/tests/test_function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/test_html2markdown.py` & `resilient_lib-51.0.1.1.824/tests/test_html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/test_oauth2_client_credentials_session.py` & `resilient_lib-51.0.1.1.824/tests/test_oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/test_payload.py` & `resilient_lib-51.0.1.1.824/tests/test_payload.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/test_poller.py` & `resilient_lib-51.0.1.1.824/tests/test_poller.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/test_requests.py` & `resilient_lib-51.0.1.1.824/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/test_templates.py` & `resilient_lib-51.0.1.1.824/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/ui/test_common.py` & `resilient_lib-51.0.1.1.824/tests/ui/test_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/ui/test_conditions.py` & `resilient_lib-51.0.1.1.824/tests/ui/test_conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/ui/test_permissions.py` & `resilient_lib-51.0.1.1.824/tests/ui/test_permissions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tests/ui/test_tab.py` & `resilient_lib-51.0.1.1.824/tests/ui/test_tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.0.695/tox.ini` & `resilient_lib-51.0.1.1.824/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 skip_missing_interpreters=true
 
 [testenv]
 passenv=TEST_RESILIENT_*
 deps =
     pytest
     pytest-cov
-    requests_mock
+    requests-mock     ~= 1.12; python_version>="3.6"
+    requests-mock      < 1.12; python_version=="2.7"
     parameterized
     mock
     setuptools-scm<6.0.0 ; python_version=="2.7"
 
 setenv =
     SETUPTOOLS_SCM_PRETEND_VERSION={env:SETUPTOOLS_SCM_PRETEND_VERSION}
```

