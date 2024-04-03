# Comparing `tmp/pytest_resilient_circuits-51.0.1.0.695.tar.gz` & `tmp/pytest_resilient_circuits-51.0.1.1.824.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_resilient_circuits-51.0.1.0.695.tar", last modified: Wed Feb 14 14:46:30 2024, max compression
+gzip compressed data, was "pytest_resilient_circuits-51.0.1.1.824.tar", last modified: Wed Apr  3 15:17:01 2024, max compression
```

## Comparing `pytest_resilient_circuits-51.0.1.0.695.tar` & `pytest_resilient_circuits-51.0.1.1.824.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:30.099633 pytest_resilient_circuits-51.0.1.0.695/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11492 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2024-02-14 14:46:30.103633 pytest_resilient_circuits-51.0.1.0.695/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:30.095633 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      403 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4267 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/circuits_fixtures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:30.099633 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__actions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__attachments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__const.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      798 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__functions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9043 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__layouts.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__message_destinations.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__task.json
--rw-rw-r--   0 travis    (2000) travis    (2000)  1618280 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      775 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   254353 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types_incident.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      580 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      501 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__wikis.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_POST__attachment.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      359 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_POST__table_data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9051 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_PUT__layouts.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      542 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19050 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/mocks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1954 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/plugin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22326 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/resilient_circuits_fixtures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:30.099633 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/shared_mock_data/mock_constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-14 14:46:30.095633 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2024-02-14 14:46:29.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1933 2024-02-14 14:46:30.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-14 14:46:29.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2024-02-14 14:46:29.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      164 2024-02-14 14:46:29.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2024-02-14 14:46:29.000000 pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1401 2024-02-14 14:46:30.103633 pytest_resilient_circuits-51.0.1.0.695/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2024-02-14 14:45:11.000000 pytest_resilient_circuits-51.0.1.0.695/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:01.834412 pytest_resilient_circuits-51.0.1.1.824/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11492 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2024-04-03 15:17:01.838412 pytest_resilient_circuits-51.0.1.1.824/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:01.830412 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      403 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4267 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/circuits_fixtures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:01.834412 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__actions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__attachments.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__const.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      798 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__functions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9043 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__layouts.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__message_destinations.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__task.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1618280 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      775 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   254353 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types_incident.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      580 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      501 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__wikis.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_POST__attachment.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      359 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_POST__table_data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9051 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_PUT__layouts.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      542 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19050 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/mocks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1954 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/plugin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22326 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/resilient_circuits_fixtures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:01.834412 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/shared_mock_data/mock_constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:17:01.830412 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2024-04-03 15:17:01.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1933 2024-04-03 15:17:01.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:17:01.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       72 2024-04-03 15:17:01.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2024-04-03 15:17:01.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2024-04-03 15:17:01.000000 pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2024-04-03 15:17:01.838412 pytest_resilient_circuits-51.0.1.1.824/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      196 2024-04-03 15:15:23.000000 pytest_resilient_circuits-51.0.1.1.824/setup.py
```

### Comparing `pytest_resilient_circuits-51.0.1.0.695/CHANGES` & `pytest_resilient_circuits-51.0.1.1.824/CHANGES`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/PKG-INFO` & `pytest_resilient_circuits-51.0.1.1.824/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_resilient_circuits
-Version: 51.0.1.0.695
+Version: 51.0.1.1.824
 Summary: Resilient Circuits fixtures for PyTest
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `pytest_resilient_circuits-51.0.1.0.695/README.md` & `pytest_resilient_circuits-51.0.1.1.824/README.md`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/LICENSE` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/circuits_fixtures.py` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/circuits_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__actions.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__actions.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__attachments.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__attachments.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__const.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__const.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__functions.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__functions.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__incidents_2314.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__layouts.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__layouts.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__task.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__task.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types_artifact.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types_function_fields.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types_incident.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types_incident.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__types_incident_fields.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__wiki100.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_GET__wiki3.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/data/200_JSON_PUT__layouts.json` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/data/200_JSON_PUT__layouts.json`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/misc.py` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/misc.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/mocks.py` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/mocks.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/plugin.py` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits/resilient_circuits_fixtures.py` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits/resilient_circuits_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits.egg-info/PKG-INFO` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-resilient-circuits
-Version: 51.0.1.0.695
+Version: 51.0.1.1.824
 Summary: Resilient Circuits fixtures for PyTest
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-resilient-circuits
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
```

### Comparing `pytest_resilient_circuits-51.0.1.0.695/pytest_resilient_circuits.egg-info/SOURCES.txt` & `pytest_resilient_circuits-51.0.1.1.824/pytest_resilient_circuits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_resilient_circuits-51.0.1.0.695/setup.cfg` & `pytest_resilient_circuits-51.0.1.1.824/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient-circuits >= 51.0.1.0
+	resilient-circuits >= 51.0.1.1
 	
-	requests-mock      ~= 1.9
+	requests-mock     ~= 1.12; python_version>="3.6"
+	requests-mock      < 1.12; python_version=="2.7"
 	
 	ConfigParser       ~= 5.2; python_version >= "3.6"
 	pytest             ~= 7.0; python_version >= "3.6"
 	
 	ConfigParser       ~= 4.0; python_version == "2.7"
 	pytest             ~= 4.6; python_version == "2.7"
```

