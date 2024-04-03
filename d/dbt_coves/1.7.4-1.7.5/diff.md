# Comparing `tmp/dbt_coves-1.7.4.tar.gz` & `tmp/dbt_coves-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coves-1.7.4.tar", max compression
+gzip compressed data, was "dbt_coves-1.7.5.tar", max compression
```

## Comparing `dbt_coves-1.7.4.tar` & `dbt_coves-1.7.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    11357 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/LICENSE
--rw-r--r--   0        0        0    28693 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/README.md
--rw-r--r--   0        0        0       22 2024-03-28 19:02:14.968508 dbt_coves-1.7.4/dbt_coves/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/config/__init__.py
--rw-r--r--   0        0        0    12670 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/config/config.py
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/core/__init__.py
--rw-r--r--   0        0        0     1364 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/core/exceptions.py
--rw-r--r--   0        0        0     8982 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/core/main.py
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/__init__.py
--rw-r--r--   0        0        0     3008 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/data_sync/__init__.py
--rw-r--r--   0        0        0      864 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/data_sync/main.py
--rw-r--r--   0        0        0     3369 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/data_sync/snowflake.py
--rw-r--r--   0        0        0     2833 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/data_sync/sql_database/README.md
--rw-r--r--   0        0        0     7165 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/data_sync/sql_database/__init__.py
--rw-r--r--   0        0        0     5174 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/data_sync/sql_database/helpers.py
--rw-r--r--   0        0        0     2459 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/data_sync/sql_database/schema_types.py
--rw-r--r--   0        0        0     5397 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/dbt/main.py
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/extract/__init__.py
--rw-r--r--   0        0        0    12275 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/extract/airbyte.py
--rw-r--r--   0        0        0      475 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/extract/base.py
--rw-r--r--   0        0        0     4555 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/extract/fivetran.py
--rw-r--r--   0        0        0      963 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/extract/main.py
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/__init__.py
--rw-r--r--   0        0        0    16975 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/airflow_dags.py
--rw-r--r--   0        0        0      226 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/airflow_generators/__init__.py
--rw-r--r--   0        0        0     6997 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/airflow_generators/airbyte.py
--rw-r--r--   0        0        0     6320 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/airflow_generators/base.py
--rw-r--r--   0        0        0     6593 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/airflow_generators/fivetran.py
--rw-r--r--   0        0        0    18628 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/base.py
--rw-r--r--   0        0        0     5897 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/docs.py
--rw-r--r--   0        0        0     1473 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/main.py
--rw-r--r--   0        0        0    10624 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/metadata.py
--rw-r--r--   0        0        0     8736 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/properties.py
--rw-r--r--   0        0        0    15161 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/sources.py
--rw-r--r--   0        0        0     2682 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/generate/templates.py
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/load/__init__.py
--rw-r--r--   0        0        0    25832 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/load/airbyte.py
--rw-r--r--   0        0        0      640 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/load/base.py
--rw-r--r--   0        0        0    18462 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/load/fivetran.py
--rw-r--r--   0        0        0      946 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/load/main.py
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/setup/__init__.py
--rw-r--r--   0        0        0      494 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/setup/base.py
--rw-r--r--   0        0        0     4287 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/setup/dbt.py
--rw-r--r--   0        0        0     6751 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/setup/git.py
--rw-r--r--   0        0        0     1214 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/setup/main.py
--rw-r--r--   0        0        0     1667 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/setup/pre_commit.py
--rw-r--r--   0        0        0    10262 2024-03-28 19:01:44.024989 dbt_coves-1.7.4/dbt_coves/tasks/setup/ssh.py
--rw-r--r--   0        0        0      845 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
--rw-r--r--   0        0        0     2110 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
--rw-r--r--   0        0        0       75 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
--rw-r--r--   0        0        0     2743 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
--rw-r--r--   0        0        0      668 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
--rw-r--r--   0        0        0      102 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
--rw-r--r--   0        0        0     1371 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/tasks/setup/utils.py
--rw-r--r--   0        0        0      255 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/templates/model_props.yml
--rw-r--r--   0        0        0      214 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/templates/source_props.yml
--rw-r--r--   0        0        0     1201 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/templates/staging_model.sql
--rw-r--r--   0        0        0      495 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/templates/staging_model_props.yml
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/ui/__init__.py
--rw-r--r--   0        0        0     1202 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/ui/traceback.py
--rw-r--r--   0        0        0        0 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/utils/__init__.py
--rw-r--r--   0        0        0    11451 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/utils/api_caller.py
--rw-r--r--   0        0        0    18547 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/utils/flags.py
--rw-r--r--   0        0        0     1131 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/utils/jinja.py
--rw-r--r--   0        0        0      785 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/utils/log.py
--rw-r--r--   0        0        0     1749 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/utils/secrets.py
--rw-r--r--   0        0        0     1342 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/utils/shell.py
--rw-r--r--   0        0        0     2205 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/utils/tracking.py
--rw-r--r--   0        0        0     1575 2024-03-28 19:01:44.028988 dbt_coves-1.7.4/dbt_coves/utils/yaml.py
--rw-r--r--   0        0        0     3828 2024-03-28 19:02:14.968508 dbt_coves-1.7.4/pyproject.toml
--rw-r--r--   0        0        0    30875 1970-01-01 00:00:00.000000 dbt_coves-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/LICENSE
+-rw-r--r--   0        0        0    28693 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/README.md
+-rw-r--r--   0        0        0       22 2024-04-03 19:39:59.713091 dbt_coves-1.7.5/dbt_coves/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/config/__init__.py
+-rw-r--r--   0        0        0    12670 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/config/config.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/core/__init__.py
+-rw-r--r--   0        0        0     1364 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/core/exceptions.py
+-rw-r--r--   0        0        0     8982 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/core/main.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/__init__.py
+-rw-r--r--   0        0        0     3008 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/data_sync/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/data_sync/main.py
+-rw-r--r--   0        0        0     3369 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/data_sync/snowflake.py
+-rw-r--r--   0        0        0     2833 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/data_sync/sql_database/README.md
+-rw-r--r--   0        0        0     7165 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/data_sync/sql_database/__init__.py
+-rw-r--r--   0        0        0     5174 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/data_sync/sql_database/helpers.py
+-rw-r--r--   0        0        0     2459 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/data_sync/sql_database/schema_types.py
+-rw-r--r--   0        0        0     5397 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/dbt/main.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/extract/__init__.py
+-rw-r--r--   0        0        0    12275 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/extract/airbyte.py
+-rw-r--r--   0        0        0      475 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/extract/base.py
+-rw-r--r--   0        0        0     4555 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/extract/fivetran.py
+-rw-r--r--   0        0        0      963 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/extract/main.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/__init__.py
+-rw-r--r--   0        0        0    16975 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/airflow_dags.py
+-rw-r--r--   0        0        0      226 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/airflow_generators/__init__.py
+-rw-r--r--   0        0        0     6997 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/airflow_generators/airbyte.py
+-rw-r--r--   0        0        0     6320 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/airflow_generators/base.py
+-rw-r--r--   0        0        0     6593 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/airflow_generators/fivetran.py
+-rw-r--r--   0        0        0    18628 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/base.py
+-rw-r--r--   0        0        0     5897 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/docs.py
+-rw-r--r--   0        0        0     1473 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/main.py
+-rw-r--r--   0        0        0    10624 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/metadata.py
+-rw-r--r--   0        0        0     8736 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/properties.py
+-rw-r--r--   0        0        0    15161 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/sources.py
+-rw-r--r--   0        0        0     2682 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/generate/templates.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/load/__init__.py
+-rw-r--r--   0        0        0    25832 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/load/airbyte.py
+-rw-r--r--   0        0        0      640 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/load/base.py
+-rw-r--r--   0        0        0    18462 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/load/fivetran.py
+-rw-r--r--   0        0        0      946 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/load/main.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/base.py
+-rw-r--r--   0        0        0     4287 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/dbt.py
+-rw-r--r--   0        0        0     6751 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/git.py
+-rw-r--r--   0        0        0     1214 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/main.py
+-rw-r--r--   0        0        0     1667 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/pre_commit.py
+-rw-r--r--   0        0        0    10262 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/ssh.py
+-rw-r--r--   0        0        0      845 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
+-rw-r--r--   0        0        0     2110 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
+-rw-r--r--   0        0        0       75 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
+-rw-r--r--   0        0        0     2743 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
+-rw-r--r--   0        0        0      668 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
+-rw-r--r--   0        0        0      102 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
+-rw-r--r--   0        0        0     1371 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/tasks/setup/utils.py
+-rw-r--r--   0        0        0      255 2024-04-03 19:39:31.280741 dbt_coves-1.7.5/dbt_coves/templates/model_props.yml
+-rw-r--r--   0        0        0      214 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/templates/source_props.yml
+-rw-r--r--   0        0        0     1201 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/templates/staging_model.sql
+-rw-r--r--   0        0        0      495 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/templates/staging_model_props.yml
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/ui/__init__.py
+-rw-r--r--   0        0        0     1202 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/ui/traceback.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/utils/__init__.py
+-rw-r--r--   0        0        0    11451 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/utils/api_caller.py
+-rw-r--r--   0        0        0    18547 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/utils/flags.py
+-rw-r--r--   0        0        0     1131 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/utils/jinja.py
+-rw-r--r--   0        0        0      785 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/utils/log.py
+-rw-r--r--   0        0        0     1749 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/utils/secrets.py
+-rw-r--r--   0        0        0     1342 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/utils/shell.py
+-rw-r--r--   0        0        0     2205 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/utils/tracking.py
+-rw-r--r--   0        0        0     1575 2024-04-03 19:39:31.284741 dbt_coves-1.7.5/dbt_coves/utils/yaml.py
+-rw-r--r--   0        0        0     3880 2024-04-03 19:39:59.713091 dbt_coves-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0    30963 1970-01-01 00:00:00.000000 dbt_coves-1.7.5/PKG-INFO
```

### Comparing `dbt_coves-1.7.4/LICENSE` & `dbt_coves-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/README.md` & `dbt_coves-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/config/config.py` & `dbt_coves-1.7.5/dbt_coves/config/config.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/core/exceptions.py` & `dbt_coves-1.7.5/dbt_coves/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/core/main.py` & `dbt_coves-1.7.5/dbt_coves/core/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/base.py` & `dbt_coves-1.7.5/dbt_coves/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/data_sync/main.py` & `dbt_coves-1.7.5/dbt_coves/tasks/data_sync/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/data_sync/snowflake.py` & `dbt_coves-1.7.5/dbt_coves/tasks/data_sync/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/data_sync/sql_database/README.md` & `dbt_coves-1.7.5/dbt_coves/tasks/data_sync/sql_database/README.md`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/data_sync/sql_database/__init__.py` & `dbt_coves-1.7.5/dbt_coves/tasks/data_sync/sql_database/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/data_sync/sql_database/helpers.py` & `dbt_coves-1.7.5/dbt_coves/tasks/data_sync/sql_database/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/data_sync/sql_database/schema_types.py` & `dbt_coves-1.7.5/dbt_coves/tasks/data_sync/sql_database/schema_types.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/dbt/main.py` & `dbt_coves-1.7.5/dbt_coves/tasks/dbt/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/extract/airbyte.py` & `dbt_coves-1.7.5/dbt_coves/tasks/extract/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/extract/fivetran.py` & `dbt_coves-1.7.5/dbt_coves/tasks/extract/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/extract/main.py` & `dbt_coves-1.7.5/dbt_coves/tasks/extract/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/airflow_dags.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/airflow_dags.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/airflow_generators/airbyte.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/airflow_generators/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/airflow_generators/base.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/airflow_generators/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/airflow_generators/fivetran.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/airflow_generators/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/base.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/docs.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/docs.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/main.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/metadata.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/properties.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/sources.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/sources.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/generate/templates.py` & `dbt_coves-1.7.5/dbt_coves/tasks/generate/templates.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/load/airbyte.py` & `dbt_coves-1.7.5/dbt_coves/tasks/load/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/load/base.py` & `dbt_coves-1.7.5/dbt_coves/tasks/load/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/load/fivetran.py` & `dbt_coves-1.7.5/dbt_coves/tasks/load/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/load/main.py` & `dbt_coves-1.7.5/dbt_coves/tasks/load/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/dbt.py` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/git.py` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/git.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/main.py` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/pre_commit.py` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/pre_commit.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/ssh.py` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/ssh.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/copier.yml` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/copier.yml`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/tasks/setup/utils.py` & `dbt_coves-1.7.5/dbt_coves/tasks/setup/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/templates/staging_model.sql` & `dbt_coves-1.7.5/dbt_coves/templates/staging_model.sql`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/ui/traceback.py` & `dbt_coves-1.7.5/dbt_coves/ui/traceback.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/utils/api_caller.py` & `dbt_coves-1.7.5/dbt_coves/utils/api_caller.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/utils/flags.py` & `dbt_coves-1.7.5/dbt_coves/utils/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/utils/jinja.py` & `dbt_coves-1.7.5/dbt_coves/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/utils/log.py` & `dbt_coves-1.7.5/dbt_coves/utils/log.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/utils/secrets.py` & `dbt_coves-1.7.5/dbt_coves/utils/secrets.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/utils/shell.py` & `dbt_coves-1.7.5/dbt_coves/utils/shell.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/utils/tracking.py` & `dbt_coves-1.7.5/dbt_coves/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/dbt_coves/utils/yaml.py` & `dbt_coves-1.7.5/dbt_coves/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.4/pyproject.toml` & `dbt_coves-1.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt_coves"
-version = "1.7.4"
+version = "1.7.5"
 description = "CLI tool for dbt users adopting analytics engineering best practices."
 authors = ["Datacoves <hello@datacoves.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Information Technology",
@@ -45,14 +45,16 @@
 copier = "6.0.0"
 gitpython = "^3.1.31"
 mixpanel = "^4.10.0"
 black = "^23.11.0"
 isort = "^5.12.0"
 dlt = "^0.4.7"
 psycopg2 = "^2.9.9"
+pyyaml-include = "1.3.2"
+psycopg2-binary = "^2.9.9"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 mypy = "^0.991"
 towncrier = "^22.12.0"
 pytest-mock = "^3.6.1"
```

### Comparing `dbt_coves-1.7.4/PKG-INFO` & `dbt_coves-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_coves
-Version: 1.7.4
+Version: 1.7.5
 Summary: CLI tool for dbt users adopting analytics engineering best practices.
 Home-page: https://datacoves.com
 License: Apache 2.0
 Keywords: data engineering,analytics engineering,dbt,ETL,data modelling
 Author: Datacoves
 Author-email: hello@datacoves.com
 Requires-Python: >=3.8.1,<3.12
@@ -32,17 +32,19 @@
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: luddite (>=1.0.1,<2.0.0)
 Requires-Dist: mixpanel (>=4.10.0,<5.0.0)
 Requires-Dist: packaging (>=20.8)
 Requires-Dist: pretty-errors (>=1.2.19,<2.0.0)
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
 Requires-Dist: python-slugify (<9.0.0)
+Requires-Dist: pyyaml-include (==1.3.2)
 Requires-Dist: questionary (>=1.9.0,<2.0.0)
 Requires-Dist: rich (>=10.4,<14.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: typing_extensions (>=4.0,<5.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: yamlloader (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://github.com/datacoves/dbt-coves/blob/main/README.md
 Project-URL: Repository, https://github.com/datacoves/dbt-coves
```

