# Comparing `tmp/astro_provider_databricks-0.2.0.tar.gz` & `tmp/astro_provider_databricks-0.2.1.tar.gz`

## Comparing `astro_provider_databricks-0.2.0.tar` & `astro_provider_databricks-0.2.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/.deepsource.toml
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/Tiltfile
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/codecov.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/mlc-config.json
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/noxfile.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/yamllint-config.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/.github/ci-test-connections.yaml
--rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/.github/scripts/verify_tag_and_version.py
--rw-r--r--   0        0        0     7342 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/.github/workflows/mlc_config.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/dev/.dockerignore
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/dev/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/dev/Dockerfile
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/dev/docker-compose.yaml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/dev/packages.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/dev/requirements.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/dev/.astro/config.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/Makefile
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/conf.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/contributing.rst
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/make.bat
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/requirements.txt
--rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/_static/banner.png
--rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/_static/dbt_dag.png
--rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/_static/dbt_task_group.png
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/_static/logo-dark.png
--rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/_static/logo-light.png
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0   212922 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/_static/screenshots/workflow_1_airflow.png
--rw-r--r--   0        0        0   763410 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/_static/screenshots/workflow_1_databricks.png
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/assets/images/dbutils-notebook-success.png
--rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/assets/images/repair-all-failed.png
--rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/docs/assets/images/repair-single-failed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/example_dags/.airflowignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/example_dags/__init__.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/example_dags/example_databricks_notebook.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/example_dags/example_databricks_workflow.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/example_dags/example_task_group.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/quickstart/astro-cli.md
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/quickstart/without-astro-cli.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/astro_databricks/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/astro_databricks/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/astro_databricks/operators/__init__.py
--rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/astro_databricks/operators/common.py
--rw-r--r--   0        0        0    14887 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/astro_databricks/operators/notebook.py
--rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/astro_databricks/operators/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/astro_databricks/plugins/__init__.py
--rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/astro_databricks/plugins/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/pytest.ini
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/test_example_dags.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/databricks/__init__.py
--rw-r--r--   0        0        0    14764 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/databricks/test_common.py
--rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/databricks/test_notebook.py
--rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/databricks/test_plugin.py
--rw-r--r--   0        0        0    14204 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/tests/databricks/test_workflow.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/LICENSE
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/README.md
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.deepsource.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/Tiltfile
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/codecov.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/mlc-config.json
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/noxfile.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/yamllint-config.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/ci-test-connections.yaml
+-rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/scripts/verify_tag_and_version.py
+-rw-r--r--   0        0        0     7342 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/workflows/mlc_config.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/.dockerignore
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/Dockerfile
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/docker-compose.yaml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/packages.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/requirements.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/.astro/config.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/conf.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/contributing.rst
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/requirements.txt
+-rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/banner.png
+-rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/dbt_dag.png
+-rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/dbt_task_group.png
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/logo-dark.png
+-rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/logo-light.png
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0   212922 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/screenshots/workflow_1_airflow.png
+-rw-r--r--   0        0        0   763410 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/screenshots/workflow_1_databricks.png
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/assets/images/dbutils-notebook-success.png
+-rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/assets/images/repair-all-failed.png
+-rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/assets/images/repair-single-failed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/.airflowignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/__init__.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/example_databricks_notebook.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/example_databricks_workflow.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/example_task_group.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/quickstart/astro-cli.md
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/quickstart/without-astro-cli.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/operators/__init__.py
+-rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/operators/common.py
+-rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/operators/notebook.py
+-rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/operators/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/plugins/__init__.py
+-rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/plugins/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/pytest.ini
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/test_example_dags.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/__init__.py
+-rw-r--r--   0        0        0    14764 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/test_common.py
+-rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/test_notebook.py
+-rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/test_plugin.py
+-rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/test_workflow.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/README.md
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/PKG-INFO
```

### Comparing `astro_provider_databricks-0.2.0/.pre-commit-config.yaml` & `astro_provider_databricks-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/CHANGELOG.rst` & `astro_provider_databricks-0.2.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.2.1 (03-04-24)
+----------------
+
+Bug fixes
+
+* Support ``existing_cluster_id`` for ``DatabricksNotebookOperator`` when used from within ``DatabricksWorkflowTaskGroup`` (PR `#73 <https://github.com/astronomer/astro-provider-databricks/pull/73>`_ by @Hang1225)
+
+
 0.2.0 (20-03-24)
 ----------------
 
 Feature
 
 * Allow users to specify Databricks API version via an environment variable (PR `#66 <https://github.com/astronomer/astro-provider-databricks/pull/66>`_ by @pankajkoti)
```

### Comparing `astro_provider_databricks-0.2.0/CODE_OF_CONDUCT.md` & `astro_provider_databricks-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/Tiltfile` & `astro_provider_databricks-0.2.1/Tiltfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/noxfile.py` & `astro_provider_databricks-0.2.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/.github/scripts/verify_tag_and_version.py` & `astro_provider_databricks-0.2.1/.github/scripts/verify_tag_and_version.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/.github/workflows/ci.yml` & `astro_provider_databricks-0.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/.github/workflows/docs.yml` & `astro_provider_databricks-0.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/dev/Dockerfile` & `astro_provider_databricks-0.2.1/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/dev/docker-compose.yaml` & `astro_provider_databricks-0.2.1/dev/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/Makefile` & `astro_provider_databricks-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/conf.py` & `astro_provider_databricks-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/contributing.rst` & `astro_provider_databricks-0.2.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/index.rst` & `astro_provider_databricks-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/make.bat` & `astro_provider_databricks-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/_static/banner.png` & `astro_provider_databricks-0.2.1/docs/_static/banner.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/_static/dbt_dag.png` & `astro_provider_databricks-0.2.1/docs/_static/dbt_dag.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/_static/dbt_task_group.png` & `astro_provider_databricks-0.2.1/docs/_static/dbt_task_group.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/_static/logo-dark.png` & `astro_provider_databricks-0.2.1/docs/_static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/_static/logo-light.png` & `astro_provider_databricks-0.2.1/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/_static/screenshots/workflow_1_airflow.png` & `astro_provider_databricks-0.2.1/docs/_static/screenshots/workflow_1_airflow.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/_static/screenshots/workflow_1_databricks.png` & `astro_provider_databricks-0.2.1/docs/_static/screenshots/workflow_1_databricks.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/assets/images/dbutils-notebook-success.png` & `astro_provider_databricks-0.2.1/docs/assets/images/dbutils-notebook-success.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/assets/images/repair-all-failed.png` & `astro_provider_databricks-0.2.1/docs/assets/images/repair-all-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/docs/assets/images/repair-single-failed.png` & `astro_provider_databricks-0.2.1/docs/assets/images/repair-single-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/example_dags/example_databricks_notebook.py` & `astro_provider_databricks-0.2.1/example_dags/example_databricks_notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/example_dags/example_databricks_workflow.py` & `astro_provider_databricks-0.2.1/example_dags/example_databricks_workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/example_dags/example_task_group.py` & `astro_provider_databricks-0.2.1/example_dags/example_task_group.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/quickstart/astro-cli.md` & `astro_provider_databricks-0.2.1/quickstart/astro-cli.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/quickstart/without-astro-cli.md` & `astro_provider_databricks-0.2.1/quickstart/without-astro-cli.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/astro_databricks/operators/common.py` & `astro_provider_databricks-0.2.1/astro_databricks/operators/common.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/astro_databricks/operators/notebook.py` & `astro_provider_databricks-0.2.1/astro_databricks/operators/notebook.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,17 +203,25 @@
         result = {
             "task_key": self._get_databricks_task_id(self.task_id),
             "depends_on": [
                 {"task_key": self._get_databricks_task_id(t)}
                 for t in self.upstream_task_ids
                 if t in relevant_upstreams
             ],
-            "job_cluster_key": self.job_cluster_key,
             **base_task_json,
         }
+
+        if self.existing_cluster_id and self.job_cluster_key:
+            raise ValueError ("Both existing_cluster_id and job_cluster_key are set. Only one cluster can be set per task.")
+        
+        if self.existing_cluster_id:
+            result['existing_cluster_id'] = self.existing_cluster_id
+        elif self.job_cluster_key:
+            result['job_cluster_key'] = self.job_cluster_key
+
         return result
 
     def _get_databricks_task_id(self, task_id: str):
         """Get the databricks task ID using dag_id and task_id. removes illegal characters."""
         return self.dag_id + "__" + task_id.replace(".", "__")
 
     def monitor_databricks_job(self):
```

### Comparing `astro_provider_databricks-0.2.0/astro_databricks/operators/workflow.py` & `astro_provider_databricks-0.2.1/astro_databricks/operators/workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/astro_databricks/plugins/plugin.py` & `astro_provider_databricks-0.2.1/astro_databricks/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/tests/conftest.py` & `astro_provider_databricks-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/tests/test_example_dags.py` & `astro_provider_databricks-0.2.1/tests/test_example_dags.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/tests/utils.py` & `astro_provider_databricks-0.2.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/tests/databricks/test_common.py` & `astro_provider_databricks-0.2.1/tests/databricks/test_common.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/tests/databricks/test_notebook.py` & `astro_provider_databricks-0.2.1/tests/databricks/test_notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/tests/databricks/test_plugin.py` & `astro_provider_databricks-0.2.1/tests/databricks/test_plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/tests/databricks/test_workflow.py` & `astro_provider_databricks-0.2.1/tests/databricks/test_workflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import logging
 from unittest import mock
 
 import pytest
+import copy
 from airflow.exceptions import AirflowException
 from airflow.utils.task_group import TaskGroup
 from astro_databricks.operators.notebook import DatabricksNotebookOperator
 from astro_databricks.operators.workflow import DatabricksWorkflowTaskGroup
 from astro_databricks.settings import DATABRICKS_JOBS_API_VERSION
 
 expected_workflow_json = {
@@ -46,14 +47,18 @@
             "task_key": "unit_test_dag__test_workflow__notebook_2",
             "timeout_seconds": 0,
         },
     ],
     "timeout_seconds": 0,
 }
 
+expected_workflow_json_existing_cluster_id = copy.deepcopy(expected_workflow_json)
+# remove job_cluster_key and add existing_cluster_id
+expected_workflow_json_existing_cluster_id['tasks'][1].pop('job_cluster_key')
+expected_workflow_json_existing_cluster_id['tasks'][1]['existing_cluster_id'] = 'foo'
 
 @mock.patch("astro_databricks.operators.workflow.DatabricksHook")
 @mock.patch("astro_databricks.operators.workflow.ApiClient")
 @mock.patch("astro_databricks.operators.workflow.JobsApi")
 @mock.patch(
     "astro_databricks.operators.workflow.RunsApi.get_run",
     return_value={"state": {"life_cycle_state": "SKIPPED"}},
@@ -370,7 +375,62 @@
     assert inner_notebook_json["libraries"] == [{"pypi": {"package": "mlflow==2.4.0"}}]
 
     assert (
         outer_notebook_json["task_key"]
         == "unit_test_dag__test_workflow__middle_task_group__inner_task_group__inner_notebook"
     )
     assert outer_notebook_json["libraries"] == [{"pypi": {"package": "mlflow==2.4.0"}}]
+
+@mock.patch("astro_databricks.operators.workflow.DatabricksHook")
+@mock.patch("astro_databricks.operators.workflow.ApiClient")
+@mock.patch("astro_databricks.operators.workflow.JobsApi")
+@mock.patch(
+    "astro_databricks.operators.workflow.RunsApi.get_run",
+    return_value={"state": {"life_cycle_state": "RUNNING"}},
+)
+def test_create_workflow_from_notebooks_with_different_clusters(
+    mock_run_api, mock_jobs_api, mock_api, mock_hook, dag
+):
+    mock_jobs_api.return_value.create_job.return_value = {"job_id": 1}
+    with dag:
+        task_group = DatabricksWorkflowTaskGroup(
+            group_id="test_workflow",
+            databricks_conn_id="foo",
+            job_clusters=[{"job_cluster_key": "foo"}],
+            notebook_params={"notebook_path": "/foo/bar"},
+            notebook_packages=[{"tg_index": {"package": "tg_package"}}],
+        )
+        with task_group:
+            notebook_1 = DatabricksNotebookOperator(
+                task_id="notebook_1",
+                databricks_conn_id="foo",
+                notebook_path="/foo/bar",
+                notebook_packages=[{"nb_index": {"package": "nb_package"}}],
+                source="WORKSPACE",
+                job_cluster_key="foo",
+            )
+            notebook_2 = DatabricksNotebookOperator(
+                task_id="notebook_2",
+                databricks_conn_id="foo",
+                notebook_path="/foo/bar",
+                source="WORKSPACE",
+                existing_cluster_id="foo",
+                notebook_params={
+                    "foo": "bar",
+                },
+            )
+            notebook_1 >> notebook_2
+
+    assert len(task_group.children) == 3
+    task_group.children["test_workflow.launch"].execute(context={})
+    mock_jobs_api.return_value.create_job.assert_called_once_with(
+        json=expected_workflow_json_existing_cluster_id,
+        version=DATABRICKS_JOBS_API_VERSION,
+    )
+    mock_jobs_api.return_value.run_now.assert_called_once_with(
+        job_id=1,
+        jar_params=[],
+        notebook_params={"notebook_path": "/foo/bar"},
+        python_params=[],
+        spark_submit_params=[],
+        version=DATABRICKS_JOBS_API_VERSION,
+    )
```

### Comparing `astro_provider_databricks-0.2.0/.gitignore` & `astro_provider_databricks-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/LICENSE` & `astro_provider_databricks-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/README.md` & `astro_provider_databricks-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/pyproject.toml` & `astro_provider_databricks-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.0/PKG-INFO` & `astro_provider_databricks-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astro-provider-databricks
-Version: 0.2.0
+Version: 0.2.1
 Summary: Affordable Databricks Workflows in Apache Airflow
 Project-URL: Homepage, https://github.com/astronomer/astro-provider-databricks/
 Project-URL: Documentation, https://github.com/astronomer/astro-provider-databricks/
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags
```

