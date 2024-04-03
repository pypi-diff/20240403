# Comparing `tmp/caplena-2.0.0.tar.gz` & `tmp/caplena-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caplena-2.0.0.tar", last modified: Thu Feb  1 13:24:53 2024, max compression
+gzip compressed data, was "caplena-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caplena-2.0.0.tar` & `caplena-2.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      123 2024-02-01 13:19:32.403742 caplena-2.0.0/.flake8
--rw-r--r--   0        0        0     1219 2023-01-27 13:58:52.681486 caplena-2.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      398 2022-06-23 21:08:21.000000 caplena-2.0.0/.gitignore
--rw-r--r--   0        0        0      133 2024-01-04 16:22:32.372796 caplena-2.0.0/.isort.cfg
--rw-r--r--   0        0        0      595 2024-02-01 13:19:32.404351 caplena-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      575 2022-02-23 16:31:29.000000 caplena-2.0.0/.vscode/settings.json
--rw-r--r--   0        0        0     1095 2022-02-23 16:31:29.000000 caplena-2.0.0/LICENSE
--rw-r--r--   0        0        0      693 2023-01-06 10:09:17.853242 caplena-2.0.0/Makefile
--rw-r--r--   0        0        0     2362 2024-01-04 16:22:32.372907 caplena-2.0.0/README.md
--rw-r--r--   0        0        0        6 2024-02-01 13:19:32.404769 caplena-2.0.0/VERSION
--rw-r--r--   0        0        0      534 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/__init__.py
--rw-r--r--   0        0        0      448 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/api/__init__.py
--rw-r--r--   0        0        0      200 2022-06-23 19:56:10.000000 caplena-2.0.0/caplena/api/api_base_uri.py
--rw-r--r--   0        0        0     3104 2024-02-01 13:19:32.405167 caplena-2.0.0/caplena/api/api_exception.py
--rw-r--r--   0        0        0     6641 2024-02-01 10:53:17.036145 caplena-2.0.0/caplena/api/api_filter.py
--rw-r--r--   0        0        0     1475 2024-01-04 16:22:32.373121 caplena-2.0.0/caplena/api/api_ordering.py
--rw-r--r--   0        0        0     9217 2024-02-01 10:53:17.036525 caplena-2.0.0/caplena/api/api_requestor.py
--rw-r--r--   0        0        0      351 2023-11-24 21:12:44.190422 caplena-2.0.0/caplena/api/api_version.py
--rw-r--r--   0        0        0     3048 2023-11-24 21:12:44.190726 caplena-2.0.0/caplena/client.py
--rw-r--r--   0        0        0     3059 2023-11-24 21:12:44.191010 caplena-2.0.0/caplena/configuration.py
--rw-r--r--   0        0        0      511 2022-06-23 21:08:21.000000 caplena-2.0.0/caplena/constants.py
--rw-r--r--   0        0        0      108 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/controllers/__init__.py
--rw-r--r--   0        0        0        0 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/endpoints/__init__.py
--rw-r--r--   0        0        0    12860 2024-02-01 10:53:17.037486 caplena-2.0.0/caplena/endpoints/base_endpoint.py
--rw-r--r--   0        0        0    31843 2024-02-01 13:19:32.405559 caplena-2.0.0/caplena/endpoints/projects_endpoint.py
--rw-r--r--   0        0        0      126 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/filters/__init__.py
--rw-r--r--   0        0        0    23852 2024-02-01 10:53:17.038581 caplena-2.0.0/caplena/filters/projects_filter.py
--rw-r--r--   0        0        0     3099 2024-02-01 10:53:17.038819 caplena-2.0.0/caplena/helpers.py
--rw-r--r--   0        0        0        0 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/http/__init__.py
--rw-r--r--   0        0        0     3815 2024-02-01 10:53:17.039704 caplena-2.0.0/caplena/http/http_client.py
--rw-r--r--   0        0        0      950 2024-02-01 10:53:17.039876 caplena-2.0.0/caplena/http/http_response.py
--rw-r--r--   0        0        0      325 2022-04-06 11:07:49.000000 caplena-2.0.0/caplena/http/json_encoder.py
--rw-r--r--   0        0        0     1693 2023-01-27 13:58:52.685112 caplena-2.0.0/caplena/http/requests_http_client.py
--rw-r--r--   0        0        0     3738 2024-02-01 10:53:17.040339 caplena-2.0.0/caplena/iterator.py
--rw-r--r--   0        0        0     3320 2024-02-01 13:19:32.406006 caplena-2.0.0/caplena/list.py
--rw-r--r--   0        0        0        0 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/logging/__init__.py
--rw-r--r--   0        0        0      478 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/logging/default_logger.py
--rw-r--r--   0        0        0     1111 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/logging/logger.py
--rw-r--r--   0        0        0        0 2022-02-23 16:31:29.000000 caplena-2.0.0/caplena/py.typed
--rw-r--r--   0        0        0      247 2024-01-04 16:22:32.373451 caplena-2.0.0/caplena/resources/__init__.py
--rw-r--r--   0        0        0       22 2024-02-01 13:19:32.406275 caplena-2.0.0/caplena/version.py
--rw-r--r--   0        0        0      638 2022-02-23 16:31:29.000000 caplena-2.0.0/docs/Makefile
--rw-r--r--   0        0        0      804 2022-02-23 16:31:29.000000 caplena-2.0.0/docs/make.bat
--rw-r--r--   0        0        0    19583 2022-02-23 16:31:29.000000 caplena-2.0.0/docs/source/_static/logo-small.svg
--rw-r--r--   0        0        0     1060 2024-01-04 16:22:32.373645 caplena-2.0.0/docs/source/api-reference.rst
--rw-r--r--   0        0        0     2316 2024-02-01 13:19:32.406562 caplena-2.0.0/docs/source/conf.py
--rw-r--r--   0        0        0     3119 2024-01-04 16:22:32.373854 caplena-2.0.0/docs/source/creating-projects.rst
--rw-r--r--   0        0        0     2481 2023-01-27 13:58:52.686374 caplena-2.0.0/docs/source/getting-started.rst
--rw-r--r--   0        0        0     1061 2024-01-04 16:22:32.373952 caplena-2.0.0/docs/source/index.rst
--rw-r--r--   0        0        0     4420 2024-01-04 16:22:32.374083 caplena-2.0.0/docs/source/retrieving-results.rst
--rw-r--r--   0        0        0       59 2023-01-27 13:58:52.686706 caplena-2.0.0/mypy.ini
--rw-r--r--   0        0        0     1946 2024-02-01 13:19:32.406906 caplena-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-02-23 16:31:29.000000 caplena-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0      441 2022-06-23 19:56:14.000000 caplena-2.0.0/tests/common.py
--rw-r--r--   0        0        0    22708 2024-02-01 10:53:17.042374 caplena-2.0.0/tests/controllers/test_projects_controller.py
--rw-r--r--   0        0        0    13260 2024-02-01 10:53:17.043352 caplena-2.0.0/tests/test_api.py
--rw-r--r--   0        0        0     3459 2024-02-01 10:53:17.043924 caplena-2.0.0/tests/test_helpers.py
--rw-r--r--   0        0        0    12167 2024-02-01 10:53:17.044170 caplena-2.0.0/tests/test_object.py
--rw-r--r--   0        0        0     4434 1970-01-01 00:00:00.000000 caplena-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-04-02 13:27:46.310056 caplena-2.0.1/.flake8
+-rw-r--r--   0        0        0     1219 2024-04-02 13:27:46.310181 caplena-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      398 2024-04-02 13:27:46.310238 caplena-2.0.1/.gitignore
+-rw-r--r--   0        0        0      133 2024-04-02 13:27:46.310299 caplena-2.0.1/.isort.cfg
+-rw-r--r--   0        0        0      595 2024-04-02 13:27:46.310373 caplena-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      575 2024-04-02 13:27:46.310458 caplena-2.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1095 2024-04-02 13:27:46.310514 caplena-2.0.1/LICENSE
+-rw-r--r--   0        0        0      693 2024-04-02 13:27:46.310576 caplena-2.0.1/Makefile
+-rw-r--r--   0        0        0     2362 2024-04-02 13:27:46.310631 caplena-2.0.1/README.md
+-rw-r--r--   0        0        0        6 2024-04-03 10:08:18.430702 caplena-2.0.1/VERSION
+-rw-r--r--   0        0        0      534 2024-04-02 13:27:46.310767 caplena-2.0.1/caplena/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-02 13:27:46.310859 caplena-2.0.1/caplena/api/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-02 13:27:46.310915 caplena-2.0.1/caplena/api/api_base_uri.py
+-rw-r--r--   0        0        0     3104 2024-04-02 13:27:46.310974 caplena-2.0.1/caplena/api/api_exception.py
+-rw-r--r--   0        0        0     6641 2024-04-02 13:27:46.311048 caplena-2.0.1/caplena/api/api_filter.py
+-rw-r--r--   0        0        0     1475 2024-04-02 13:27:46.311106 caplena-2.0.1/caplena/api/api_ordering.py
+-rw-r--r--   0        0        0     9217 2024-04-02 13:27:46.311189 caplena-2.0.1/caplena/api/api_requestor.py
+-rw-r--r--   0        0        0      351 2024-04-02 13:27:46.311243 caplena-2.0.1/caplena/api/api_version.py
+-rw-r--r--   0        0        0     3048 2024-04-02 13:27:46.311299 caplena-2.0.1/caplena/client.py
+-rw-r--r--   0        0        0     3059 2024-04-02 13:27:46.311357 caplena-2.0.1/caplena/configuration.py
+-rw-r--r--   0        0        0      511 2024-04-02 13:27:46.311416 caplena-2.0.1/caplena/constants.py
+-rw-r--r--   0        0        0      108 2024-04-02 13:27:46.311503 caplena-2.0.1/caplena/controllers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:27:46.311553 caplena-2.0.1/caplena/endpoints/__init__.py
+-rw-r--r--   0        0        0    12860 2024-04-02 13:27:46.311651 caplena-2.0.1/caplena/endpoints/base_endpoint.py
+-rw-r--r--   0        0        0    31847 2024-04-03 10:08:18.431145 caplena-2.0.1/caplena/endpoints/projects_endpoint.py
+-rw-r--r--   0        0        0      126 2024-04-02 13:27:46.311863 caplena-2.0.1/caplena/filters/__init__.py
+-rw-r--r--   0        0        0    23852 2024-04-02 13:27:46.311952 caplena-2.0.1/caplena/filters/projects_filter.py
+-rw-r--r--   0        0        0     3099 2024-04-02 13:27:46.312030 caplena-2.0.1/caplena/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:27:46.312135 caplena-2.0.1/caplena/http/__init__.py
+-rw-r--r--   0        0        0     3815 2024-04-02 13:27:46.312286 caplena-2.0.1/caplena/http/http_client.py
+-rw-r--r--   0        0        0      950 2024-04-02 13:27:46.312396 caplena-2.0.1/caplena/http/http_response.py
+-rw-r--r--   0        0        0      325 2024-04-02 13:27:46.312509 caplena-2.0.1/caplena/http/json_encoder.py
+-rw-r--r--   0        0        0     1693 2024-04-02 13:27:46.312630 caplena-2.0.1/caplena/http/requests_http_client.py
+-rw-r--r--   0        0        0     3738 2024-04-02 13:27:46.312780 caplena-2.0.1/caplena/iterator.py
+-rw-r--r--   0        0        0     3320 2024-04-02 13:27:46.312905 caplena-2.0.1/caplena/list.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:27:46.313016 caplena-2.0.1/caplena/logging/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-02 13:27:46.313152 caplena-2.0.1/caplena/logging/default_logger.py
+-rw-r--r--   0        0        0     1111 2024-04-02 13:27:46.313265 caplena-2.0.1/caplena/logging/logger.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:27:46.313313 caplena-2.0.1/caplena/py.typed
+-rw-r--r--   0        0        0      247 2024-04-02 13:27:46.313521 caplena-2.0.1/caplena/resources/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-03 10:08:18.431449 caplena-2.0.1/caplena/version.py
+-rw-r--r--   0        0        0      638 2024-04-02 13:27:46.313819 caplena-2.0.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2024-04-02 13:27:46.313941 caplena-2.0.1/docs/make.bat
+-rw-r--r--   0        0        0    19583 2024-04-02 13:27:46.314224 caplena-2.0.1/docs/source/_static/logo-small.svg
+-rw-r--r--   0        0        0     1060 2024-04-02 13:27:46.314486 caplena-2.0.1/docs/source/api-reference.rst
+-rw-r--r--   0        0        0     2316 2024-04-03 10:08:18.431845 caplena-2.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0     3119 2024-04-02 13:27:46.314617 caplena-2.0.1/docs/source/creating-projects.rst
+-rw-r--r--   0        0        0     2481 2024-04-02 13:27:46.314687 caplena-2.0.1/docs/source/getting-started.rst
+-rw-r--r--   0        0        0     1061 2024-04-02 13:27:46.314744 caplena-2.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0     4420 2024-04-02 13:27:46.314803 caplena-2.0.1/docs/source/retrieving-results.rst
+-rw-r--r--   0        0        0       59 2024-04-02 13:27:46.314849 caplena-2.0.1/mypy.ini
+-rw-r--r--   0        0        0     1946 2024-04-03 10:08:18.432077 caplena-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 13:27:46.314952 caplena-2.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      441 2024-04-03 10:08:07.034465 caplena-2.0.1/tests/common.py
+-rw-r--r--   0        0        0    22777 2024-04-03 10:08:18.432431 caplena-2.0.1/tests/controllers/test_projects_controller.py
+-rw-r--r--   0        0        0    13260 2024-04-02 13:27:46.315234 caplena-2.0.1/tests/test_api.py
+-rw-r--r--   0        0        0     3459 2024-04-02 13:27:46.315298 caplena-2.0.1/tests/test_helpers.py
+-rw-r--r--   0        0        0    12167 2024-04-02 13:27:46.315373 caplena-2.0.1/tests/test_object.py
+-rw-r--r--   0        0        0     4434 1970-01-01 00:00:00.000000 caplena-2.0.1/PKG-INFO
```

### Comparing `caplena-2.0.0/.github/workflows/build.yml` & `caplena-2.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/.pre-commit-config.yaml` & `caplena-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/.vscode/settings.json` & `caplena-2.0.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/LICENSE` & `caplena-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/Makefile` & `caplena-2.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/README.md` & `caplena-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/__init__.py` & `caplena-2.0.1/caplena/__init__.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/api/api_exception.py` & `caplena-2.0.1/caplena/api/api_exception.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/api/api_filter.py` & `caplena-2.0.1/caplena/api/api_filter.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/api/api_ordering.py` & `caplena-2.0.1/caplena/api/api_ordering.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/api/api_requestor.py` & `caplena-2.0.1/caplena/api/api_requestor.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/client.py` & `caplena-2.0.1/caplena/client.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/configuration.py` & `caplena-2.0.1/caplena/configuration.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/endpoints/base_endpoint.py` & `caplena-2.0.1/caplena/endpoints/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/endpoints/projects_endpoint.py` & `caplena-2.0.1/caplena/endpoints/projects_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
         :param r_id: The row identifier.
         :raises caplena.api.ApiException: An API exception.
         """
         response = self.get(
             path="/projects/{p_id}/rows/{r_id}",
             path_params={"p_id": p_id, "r_id": r_id},
         )
-        return self.build_response(response, resource=Row, metadata={"project": id})
+        return self.build_response(response, resource=Row, metadata={"project": p_id})
 
     def remove_row(self, *, p_id: str, r_id: str) -> None:
         """Removes a previously created row.
 
         :param p_id: The project identifier.
         :param r_id: The row identifier.
         :raises caplena.api.ApiException: An API exception.
@@ -277,15 +277,15 @@
         :raises caplena.api.ApiException: An API exception.
         """
         json = self.api.build_payload(columns=columns)
 
         response = self.patch(
             path="/projects/{p_id}/rows/{r_id}", path_params={"p_id": p_id, "r_id": r_id}, json=json
         )
-        return self.build_response(response, resource=Row, metadata={"project": id})
+        return self.build_response(response, resource=Row, metadata={"project": p_id})
 
 
 # --- Resources & Objects--- #
 
 
 class OperationsProtocol(Protocol):
     # controller: ProjectsController
```

### Comparing `caplena-2.0.0/caplena/filters/projects_filter.py` & `caplena-2.0.1/caplena/filters/projects_filter.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/helpers.py` & `caplena-2.0.1/caplena/helpers.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/http/http_client.py` & `caplena-2.0.1/caplena/http/http_client.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/http/http_response.py` & `caplena-2.0.1/caplena/http/http_response.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/http/requests_http_client.py` & `caplena-2.0.1/caplena/http/requests_http_client.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/iterator.py` & `caplena-2.0.1/caplena/iterator.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/list.py` & `caplena-2.0.1/caplena/list.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/caplena/logging/logger.py` & `caplena-2.0.1/caplena/logging/logger.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/docs/Makefile` & `caplena-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/docs/make.bat` & `caplena-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/docs/source/_static/logo-small.svg` & `caplena-2.0.1/docs/source/_static/logo-small.svg`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/docs/source/api-reference.rst` & `caplena-2.0.1/docs/source/api-reference.rst`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/docs/source/conf.py` & `caplena-2.0.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 
 # -- Project information -----------------------------------------------------
 
 project = "Caplena"
 copyright = "2024, Caplena"
 author = "Caplena"
-version = "2.0.0"
-release = "2.0.0"
+version = "2.0.1"
+release = "2.0.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `caplena-2.0.0/docs/source/creating-projects.rst` & `caplena-2.0.1/docs/source/creating-projects.rst`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/docs/source/getting-started.rst` & `caplena-2.0.1/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/docs/source/index.rst` & `caplena-2.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/docs/source/retrieving-results.rst` & `caplena-2.0.1/docs/source/retrieving-results.rst`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/pyproject.toml` & `caplena-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caplena"
-version = "2.0.0"
+version = "2.0.1"
 authors = [{name = "Caplena", email = "support@caplena.com"}]
 maintainers = [{name = "Pascal de Buren", email = "pascal@caplena.com"}]
 keywords = ["caplena", "api", "nlp", "customer feedback"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `caplena-2.0.0/tests/controllers/test_projects_controller.py` & `caplena-2.0.1/tests/controllers/test_projects_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,14 +429,15 @@
                     "value": datetime(year=2020, month=10, day=10, hour=17, tzinfo=timezone.utc),
                 },
             ],
         )
         retrieved = self.controller.retrieve_row(p_id=project.id, r_id=row.id)
 
         self.assertDictEqual(row.dict(), retrieved.dict())
+        self.assertDictEqual(row._metadata, {"project": project.id})
 
     def test_removing_a_row_succeeds(self) -> None:
         project = self.create_project()
 
         old_num_rows = self.controller.list_rows(id=project.id, limit=1).count
         row = self.controller.append_row(
             id=project.id,
```

### Comparing `caplena-2.0.0/tests/test_api.py` & `caplena-2.0.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/tests/test_helpers.py` & `caplena-2.0.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/tests/test_object.py` & `caplena-2.0.1/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `caplena-2.0.0/PKG-INFO` & `caplena-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caplena
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python Library for Caplena REST API.
 Keywords: caplena,api,nlp,customer feedback
 Author-email: Caplena <support@caplena.com>
 Maintainer-email: Pascal de Buren <pascal@caplena.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
```

