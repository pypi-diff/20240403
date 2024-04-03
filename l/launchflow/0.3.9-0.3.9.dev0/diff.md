# Comparing `tmp/launchflow-0.3.9.tar.gz` & `tmp/launchflow-0.3.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchflow-0.3.9.tar", last modified: Fri Mar 29 17:29:10 2024, max compression
+gzip compressed data, was "launchflow-0.3.9.dev0.tar", last modified: Wed Apr  3 21:45:37 2024, max compression
```

## Comparing `launchflow-0.3.9.tar` & `launchflow-0.3.9.dev0.tar`

### file list

```diff
@@ -1,119 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.962141 launchflow-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-29 17:29:02.000000 launchflow-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-29 17:29:10.962141 launchflow-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-29 17:29:02.000000 launchflow-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.946141 launchflow-0.3.9/launchflow/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.946141 launchflow-0.3.9/launchflow/aws/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/aws/rds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/aws/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.946141 launchflow-0.3.9/launchflow/cache/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cache/launchflow_tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.946141 launchflow-0.3.9/launchflow/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.946141 launchflow-0.3.9/launchflow/cli/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/accounts/account_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.950141 launchflow-0.3.9/launchflow/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/config/config_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.950141 launchflow-0.3.9/launchflow/cli/environments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/environments/environment_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.950141 launchflow-0.3.9/launchflow/cli/gen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.950141 launchflow-0.3.9/launchflow/cli/gen/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.950141 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.950141 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.950141 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/app/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/app/infra.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/app/models.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/launchflow.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/requirements.txt.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.950141 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.954141 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/app/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/app/infra.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/launchflow.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/requirements.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/fastapi_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.954141 launchflow-0.3.9/launchflow/cli/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/project/project_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/project_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.954141 launchflow-0.3.9/launchflow/cli/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/resources/resource_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/resources_ast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.954141 launchflow-0.3.9/launchflow/cli/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/services/service_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.954141 launchflow-0.3.9/launchflow/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/templates/dockerfile_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/templates/infra_dot_py_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/templates/main_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/cli/utyper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.954141 launchflow-0.3.9/launchflow/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/accounts_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/connect_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/environments_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/operations_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/projects_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/resources_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/response_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/clients/services_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.958141 launchflow-0.3.9/launchflow/config/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/config/launchflow_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/config/launchflow_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/config/launchflow_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.958141 launchflow-0.3.9/launchflow/context/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14064 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/context/launchflow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.958141 launchflow-0.3.9/launchflow/flows/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/flows/account_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/flows/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    17746 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/flows/cloud_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/flows/environments_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/flows/project_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/flows/resource_flows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.958141 launchflow-0.3.9/launchflow/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/gcp/cloudsql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/gcp/compute_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/gcp/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/gcp/memorystore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-29 17:29:02.000000 launchflow-0.3.9/launchflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:29:10.958141 launchflow-0.3.9/launchflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-29 17:29:10.000000 launchflow-0.3.9/launchflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-29 17:29:10.000000 launchflow-0.3.9/launchflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:29:10.000000 launchflow-0.3.9/launchflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-29 17:29:10.000000 launchflow-0.3.9/launchflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-29 17:29:10.000000 launchflow-0.3.9/launchflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 17:29:10.000000 launchflow-0.3.9/launchflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-29 17:29:02.000000 launchflow-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 17:29:10.962141 launchflow-0.3.9/setup.cfg
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.690895 launchflow-0.3.9.dev0/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      118 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/MANIFEST.in
+-rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-03 21:45:37.690895 launchflow-0.3.9.dev0/PKG-INFO
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1996 2024-03-13 23:12:43.000000 launchflow-0.3.9.dev0/README.md
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.662894 launchflow-0.3.9.dev0/launchflow/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      528 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.662894 launchflow-0.3.9.dev0/launchflow/aws/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       67 2024-03-20 15:00:34.000000 launchflow-0.3.9.dev0/launchflow/aws/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4534 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/aws/rds.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3512 2024-04-02 20:56:37.000000 launchflow-0.3.9.dev0/launchflow/aws/s3.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cache/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       95 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev0/launchflow/cache/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4980 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cache/launchflow_tmp.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cli/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-25 20:38:50.000000 launchflow-0.3.9.dev0/launchflow/cli/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cli/accounts/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev0/launchflow/cli/accounts/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1250 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/accounts/account_commands.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cli/config/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev0/launchflow/cli/config/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1026 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/config/config_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      566 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/constants.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cli/environments/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev0/launchflow/cli/environments/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2535 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/environments/environment_commands.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cli/gen/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2692 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/template.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      209 2024-04-02 23:44:00.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/__pycache__/__init__.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.666894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      216 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    15518 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.670894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:53:05.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      162 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/Makefile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2552 2024-04-03 19:45:42.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.670894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      100 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/admin.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/apps.py.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.670894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      748 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      151 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/models.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      487 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/serializers.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      264 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2021 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.670894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/asgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/wsgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/requirements.txt.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.674894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:52:02.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/Makefile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2552 2024-04-03 19:45:52.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.674894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/app/apps.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      164 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      326 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/app/views.py.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.674894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/asgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/wsgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_simple_template/requirements.txt.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    14570 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/django_template.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.674894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.674894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      217 2024-04-02 23:47:30.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17805 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.674894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2000 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.678894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      576 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/models.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/requirements.txt.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.678894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2000 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.678894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      573 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/requirements.txt.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    18560 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/fastapi_template.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.678894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.678894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      215 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17114 2024-04-03 20:00:39.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.678894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2086 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.678894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      297 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/models.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_postgres_template/requirements.txt.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.678894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_simple_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2086 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.678894 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_simple_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_simple_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_simple_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      324 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_simple_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_simple_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/_simple_template/requirements.txt.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17509 2024-04-03 19:59:50.000000 launchflow-0.3.9.dev0/launchflow/cli/gen/templates/flask/flask_template.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    19278 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/main.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.682895 launchflow-0.3.9.dev0/launchflow/cli/project/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-30 20:01:40.000000 launchflow-0.3.9.dev0/launchflow/cli/project/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1702 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev0/launchflow/cli/project/project_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3067 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/project_gen.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.682895 launchflow-0.3.9.dev0/launchflow/cli/resources/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev0/launchflow/cli/resources/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4436 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/resources/resource_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5382 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/cli/resources_ast.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.682895 launchflow-0.3.9.dev0/launchflow/cli/services/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev0/launchflow/cli/services/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4413 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/cli/services/service_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3501 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev0/launchflow/cli/utils.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      482 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev0/launchflow/cli/utyper.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.682895 launchflow-0.3.9.dev0/launchflow/clients/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      296 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev0/launchflow/clients/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1155 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev0/launchflow/clients/accounts_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1137 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev0/launchflow/clients/client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1832 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev0/launchflow/clients/connect_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4806 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/clients/environments_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1911 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev0/launchflow/clients/operations_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1820 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev0/launchflow/clients/projects_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5117 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev0/launchflow/clients/resources_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3767 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev0/launchflow/clients/response_schemas.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3477 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev0/launchflow/clients/services_client.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.682895 launchflow-0.3.9.dev0/launchflow/config/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev0/launchflow/config/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4412 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev0/launchflow/config/launchflow_config.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1361 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev0/launchflow/config/launchflow_env.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5144 2024-03-14 16:50:08.000000 launchflow-0.3.9.dev0/launchflow/config/launchflow_yaml.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.682895 launchflow-0.3.9.dev0/launchflow/context/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-03-13 17:41:44.000000 launchflow-0.3.9.dev0/launchflow/context/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    16515 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/context/launchflow_ctx.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/exceptions.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5180 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev0/launchflow/fastapi.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       52 2024-03-27 23:08:23.000000 launchflow-0.3.9.dev0/launchflow/flask.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.686895 launchflow-0.3.9.dev0/launchflow/flows/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      129 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev0/launchflow/flows/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1236 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev0/launchflow/flows/account_id.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3746 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev0/launchflow/flows/auth.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17746 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/flows/cloud_provider.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     7171 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev0/launchflow/flows/environments_flows.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev0/launchflow/flows/project_flows.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    18602 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev0/launchflow/flows/resource_flows.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.686895 launchflow-0.3.9.dev0/launchflow/gcp/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      219 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/gcp/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     7762 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/gcp/cloudsql.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2978 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/gcp/compute_engine.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3523 2024-04-02 20:56:22.000000 launchflow-0.3.9.dev0/launchflow/gcp/gcs.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2755 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/gcp/memorystore.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      982 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev0/launchflow/gcp/utils.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2059 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev0/launchflow/operations.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2288 2024-04-02 21:12:53.000000 launchflow-0.3.9.dev0/launchflow/resource.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       50 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev0/launchflow/service.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      789 2024-03-28 23:07:50.000000 launchflow-0.3.9.dev0/launchflow/utils.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-03 21:45:37.686895 launchflow-0.3.9.dev0/launchflow.egg-info/
+-rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-03 21:45:37.000000 launchflow-0.3.9.dev0/launchflow.egg-info/PKG-INFO
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     8331 2024-04-03 21:45:37.000000 launchflow-0.3.9.dev0/launchflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        1 2024-04-03 21:45:37.000000 launchflow-0.3.9.dev0/launchflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       84 2024-04-03 21:45:37.000000 launchflow-0.3.9.dev0/launchflow.egg-info/entry_points.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      309 2024-04-03 21:45:37.000000 launchflow-0.3.9.dev0/launchflow.egg-info/requires.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       11 2024-04-03 21:45:37.000000 launchflow-0.3.9.dev0/launchflow.egg-info/top_level.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1421 2024-04-03 21:45:30.000000 launchflow-0.3.9.dev0/pyproject.toml
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       38 2024-04-03 21:45:37.690895 launchflow-0.3.9.dev0/setup.cfg
```

### Comparing `launchflow-0.3.9/PKG-INFO` & `launchflow-0.3.9.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchflow
-Version: 0.3.9
+Version: 0.3.9.dev0
 Summary: Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic.
 Author-email: CalebTVanDyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: beaupy
 Requires-Dist: rich
```

### Comparing `launchflow-0.3.9/README.md` & `launchflow-0.3.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/aws/rds.py` & `launchflow-0.3.9.dev0/launchflow/aws/rds.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     ) -> None:
         super().__init__(
             name=name,
             product_name="aws_rds_postgres",
             create_args={},
         )
 
-    def django_options(self):
+    def django_settings(self):
         if psycopg2 is None:
             raise ImportError(
                 "psycopg2 is not installed. Please install it with `pip install psycopg2`."
             )
 
         connection_info = self.connect()
         return {
```

### Comparing `launchflow-0.3.9/launchflow/aws/s3.py` & `launchflow-0.3.9.dev0/launchflow/aws/s3.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cache/launchflow_tmp.py` & `launchflow-0.3.9.dev0/launchflow/cache/launchflow_tmp.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     return f"{project}:{environment}:{product}:{resource}"
 
 
 @dataclass
 class LaunchFlowCache:
     resource_connection_bucket_paths: Dict[str, str] = field(default_factory=dict)
     resource_connection_info: Dict[str, Dict[str, str]] = field(default_factory=dict)
+    gcp_service_account_emails: Dict[str, str] = field(default_factory=dict)
 
     def get_resource_connection_bucket_path(
         self, project: str, environment: str, product: str, resource: str
     ) -> Optional[str]:
         key = _build_key(project, environment, product, resource)
         return self.resource_connection_bucket_paths.get(key)
 
@@ -61,37 +62,56 @@
     def delete_resource_connection_info(
         self, project: str, environment: str, product: str, resource: str
     ):
         key = _build_key(project, environment, product, resource)
         self.resource_connection_info.pop(key, None)
         self.save_to_file(find_launchflow_tmp())
 
+    def get_gcp_service_account_email(
+        self, project: str, environment: str
+    ) -> Optional[str]:
+        key = f"{project}:{environment}"
+        return self.gcp_service_account_emails.get(key)
+
+    def set_gcp_service_account_email(self, project: str, environment: str, email: str):
+        key = f"{project}:{environment}"
+        self.gcp_service_account_emails[key] = email
+        self.save_to_file(find_launchflow_tmp())
+
+    def delete_gcp_service_account_email(self, project: str, environment: str):
+        key = f"{project}:{environment}"
+        self.gcp_service_account_emails.pop(key, None)
+        self.save_to_file(find_launchflow_tmp())
+
     @classmethod
     def load_from_file(cls, file_path: str):
         if not os.path.exists(file_path):
             logging.debug(
                 f"The file '{file_path}' does not exist. Creating with default values."
             )
             return cls()
 
         with open(file_path, "r") as file:
             data = toml.load(file)
             resource_connection_bucket_paths = data.get(
                 "resource_connection_bucket_paths", {}
             )
             resource_connection_info = data.get("resource_connection_info", {})
+            gcp_service_account_emails = data.get("gcp_service_account_emails", {})
         return cls(
             resource_connection_bucket_paths=resource_connection_bucket_paths,
             resource_connection_info=resource_connection_info,
+            gcp_service_account_emails=gcp_service_account_emails,
         )
 
     def save_to_file(self, file_path: str):
         data = {
             "resource_connection_bucket_paths": self.resource_connection_bucket_paths,
             "resource_connection_info": self.resource_connection_info,
+            "gcp_service_account_emails": self.gcp_service_account_emails,
         }
         os.makedirs(os.path.dirname(file_path), exist_ok=True)
         with open(file_path, "w") as file:
             toml.dump(data, file)
         logging.debug(f"Saved to {file_path}")
```

### Comparing `launchflow-0.3.9/launchflow/cli/accounts/account_commands.py` & `launchflow-0.3.9.dev0/launchflow/cli/accounts/account_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/config/config_commands.py` & `launchflow-0.3.9.dev0/launchflow/cli/config/config_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/constants.py` & `launchflow-0.3.9.dev0/launchflow/cli/constants.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/environments/environment_commands.py` & `launchflow-0.3.9.dev0/launchflow/cli/environments/environment_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/gen/template.py` & `launchflow-0.3.9.dev0/launchflow/cli/gen/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,24 +41,28 @@
                 # Create directories in the destination path
                 os.makedirs(destination_dir, exist_ok=True)
 
                 for file in files:
                     source_path = Path(root, file)
                     destination_file_path = destination_dir / file
 
+                    if file == "__pycache__":
+                        continue
+
                     if file.endswith(".jinja"):
                         # Render Jinja template
                         if relative_root.name:
                             template_content = resources.read_text(
-                                f"{template_dir}.{relative_root.name}", file
+                                f"{template_dir}.{'.'.join(relative_root.parts)}",
+                                file,
                             )
                         else:
                             template_content = resources.read_text(template_dir, file)
                         template = Template(template_content)
-                        output_content = template.render(render_context)
+                        output_content = template.render(render_context) + "\n"
 
                         # Save the rendered file, removing the '.jinja' extension
                         destination_file_path = destination_file_path.with_suffix("")
 
                         with open(destination_file_path, "w") as f:
                             f.write(output_content)
                     else:
```

### Comparing `launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja` & `launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja` & `launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja` & `launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja` & `launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja` & `launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/gen/templates/fastapi/fastapi_template.py` & `launchflow-0.3.9.dev0/launchflow/cli/gen/templates/fastapi/fastapi_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,15 +407,15 @@
             resource_info = get_resource_info(resource)
             infra_names.append(resource_info.infra_name)
             if resource_info.fastapi_setup is not None:
                 infra_steps.append(resource_info.fastapi_setup)
         return "\n".join(
             [
                 "# Connects to all resources on startup",
-                f"    await launchflow.connect_all_async({', '.join(infra_names)})",
+                f"    await launchflow.connect_all({', '.join(infra_names)})",
             ]
             + infra_steps
         )
 
     # Used by app/main.py
     @property
     def app_infra_endpoints(self) -> List[str]:
@@ -478,22 +478,23 @@
             "app_infra_imports": self.app_infra_imports,
             "app_global_setup": self.app_global_setup,
             "app_infra_setup": self.app_infra_setup,
             "app_infra_endpoints": self.app_infra_endpoints,
         }
 
 
-# if __name__ == "__main__":
-#     generator = FastAPIProjectGenerator(
-#         resources=[
-#             # ComputeEngineRedis,
-#             # GCSBucket,
-#             # CloudSQLPostgres,
-#             S3Bucket,
-#             RDSPostgres,
-#         ],
-#         cloud_provider="aws",
-#         launchflow_project_name="my-project",
-#         launchflow_environment_name="dev",
-#         launchflow_service_name="my-service",
-#     )
-#     generator.generate_project(destination_path="/tmp/launchflow")
+if __name__ == "__main__":
+    cloud_provider = "gcp"
+    generator = FastAPIProjectGenerator(
+        resources=[
+            ComputeEngineRedis,
+            GCSBucket,
+            CloudSQLPostgres,
+            # S3Bucket,
+            # RDSPostgres,
+        ],
+        cloud_provider=cloud_provider,
+        launchflow_project_name=f"{cloud_provider}-examples",
+        launchflow_environment_name="dev",
+        launchflow_service_name="fastapi-service",
+    )
+    generator.generate_project(destination_path="/tmp/launchflow")
```

### Comparing `launchflow-0.3.9/launchflow/cli/main.py` & `launchflow-0.3.9.dev0/launchflow/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 from launchflow.cli.constants import (
     ENVIRONMENT_HELP,
     PROJECT_HELP,
     SCAN_DIRECTORY_HELP,
     SERVICE_HELP,
 )
 from launchflow.cli.environments import environment_commands
+from launchflow.cli.gen.templates.django.django_template import DjangoProjectGenerator
 from launchflow.cli.gen.templates.fastapi.fastapi_template import (
     FastAPIProjectGenerator,
 )
+from launchflow.cli.gen.templates.flask.flask_template import FlaskProjectGenerator
 from launchflow.cli.project import project_commands
 from launchflow.cli.resources import resource_commands
 from launchflow.cli.resources_ast import find_launchflow_resources
 from launchflow.cli.services import service_commands
 from launchflow.cli.utils import print_response, tar_source_in_memory
 from launchflow.cli.utyper import UTyper
 from launchflow.clients.client import LaunchFlowAsyncClient
@@ -153,29 +155,44 @@
             generator = FastAPIProjectGenerator(
                 resources=resources,
                 cloud_provider=cloud_provider,
                 launchflow_project_name=project.name,
                 launchflow_environment_name=environment.name,
             )
             generator.generate_project(full_directory_path)
+        elif framework == project_gen.Framework.FLASK:
+            generator = FlaskProjectGenerator(
+                resources=resources,
+                cloud_provider=cloud_provider,
+                launchflow_project_name=project.name,
+                launchflow_environment_name=environment.name,
+            )
+            generator.generate_project(full_directory_path)
+        elif framework == project_gen.Framework.DJANGO:
+            generator = DjangoProjectGenerator(
+                resources=resources,
+                cloud_provider=cloud_provider,
+                launchflow_project_name=project.name,
+                launchflow_environment_name=environment.name,
+            )
+            generator.generate_project(full_directory_path)
+        else:
+            raise NotImplementedError(f"Framework {framework} is not supported yet.")
 
         print()
         print("Done!")
         print()
         print("Navigate to your project directory:")
         rich.print(f"  $ [green]cd {relative_path}")
         print()
         print("To create your resources run:")
         rich.print("  $ [green]launchflow create")
         print()
         print("To build and deploy your app remotely run:")
         rich.print("  $ [green]launchflow deploy")
-        print()
-        print("To run all of the above in one command run:")
-        rich.print("  $ [green]launchflow launch")
 
 
 @app.command()
 async def create(
     resource: str = typer.Argument(
         None,
         help="Resource to create. If none we will scan the directory for resources.",
```

### Comparing `launchflow-0.3.9/launchflow/cli/project/project_commands.py` & `launchflow-0.3.9.dev0/launchflow/cli/project/project_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/resources/resource_commands.py` & `launchflow-0.3.9.dev0/launchflow/cli/resources/resource_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/resources_ast.py` & `launchflow-0.3.9.dev0/launchflow/cli/resources_ast.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,21 @@
             break
     if not maybe_resource:
         return False
     split_path = import_path.split(".")
     resource_name = split_path[-1]
     module = ".".join(split_path[:-1])
     module_type = importlib.import_module(module)
+
+    # This checks if the resource_name starts with a lowercase character to act as a
+    # proxy check for the resource being a class. This is not foolproof but should
+    # filter out most utility functions.
+    if resource_name[0].islower():
+        return False
+
     if hasattr(module_type, resource_name) and issubclass(
         getattr(module_type, resource_name), Resource
     ):
         return True
     return False
```

### Comparing `launchflow-0.3.9/launchflow/cli/services/service_commands.py` & `launchflow-0.3.9.dev0/launchflow/cli/services/service_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/cli/templates/dockerfile_template.py` & `launchflow-0.3.9.dev0/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,48 @@
-import sys
-from typing import Literal
-
-from launchflow.cli.project_gen import Framework
-
-DOCKERFILE_SERVICE_TEMPLATE = """\
 # NOTE: This Dockerfile uses multi-stage builds for efficient caching and smaller image sizes
 # Learn more at https://docs.docker.com/build/building/multi-stage/
 
 # Build Stage 1: Build stage for installing dependencies
-FROM {docker_repo_prefix}python:{python_major_version}.{python_minor_version}-slim as builder
+FROM {{ docker_repository_prefix }}python:{{ python_major_version }}.{{ python_minor_version }}-slim as builder
 
 # Set a working directory for the build stage
 WORKDIR /build
 
 # Install system dependencies required for Python packages to build
-RUN apt-get update \\
-    && apt-get install -y --no-install-recommends gcc libpq-dev \\
-    && apt-get clean \\
+RUN apt-get update \
+    && apt-get install -y --no-install-recommends gcc libpq-dev \
+    && apt-get clean \
     && rm -rf /var/lib/apt/lists/*
 
 # Upgrade pip and install dependencies
 COPY requirements.txt .
-RUN pip install --no-cache-dir -U pip setuptools wheel \\
+RUN pip install --no-cache-dir -U pip setuptools wheel \
     && pip install --no-cache-dir --target=/install -r requirements.txt
 
 # Build Stage 2: Build a final slim image for running the application
-FROM {docker_repo_prefix}python:{python_major_version}.{python_minor_version}-slim
+FROM {{ docker_repository_prefix }}python:{{ python_major_version }}.{{ python_minor_version }}-slim
 
 # Create a non-root user for security purposes
 RUN useradd --create-home appuser
 USER appuser
 
 # Set environment variables for Python to run in unbuffered mode and not write .pyc files
-ENV PYTHONDONTWRITEBYTECODE=1
-ENV PYTHONUNBUFFERED=1
-ENV PORT={port}
+ENV PYTHONDONTWRITEBYTECODE=1 \
+    PYTHONUNBUFFERED=1 \
+    PORT={{ port }}
 
 # Copy installed dependencies from the builder stage
-COPY --from=builder /install /usr/local/lib/python{python_major_version}.{python_minor_version}/site-packages
-ENV PATH="${{PATH}}:/usr/local/lib/python{python_major_version}.{python_minor_version}/site-packages/bin"
+COPY --from=builder /install /usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages
+ENV PATH="${PATH}:/usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages/bin"
 
 # Set the working directory and copy only the necessary application files
 WORKDIR /code
-COPY --chown=appuser:appuser ./{app_dir} /code/{app_dir}
+COPY --chown=appuser:appuser ./app /code/app
+COPY --chown=appuser:appuser ./django_app /code/django_app
 COPY --chown=appuser:appuser ./launchflow.yaml /code/launchflow.yaml
+COPY --chown=appuser:appuser ./manage.py /code/manage.py
 
 # Expose the port the app runs on
-EXPOSE {port}
+EXPOSE $PORT
 
 # Start the application
-CMD {startup_cmd}
-"""
-
-
-def template(framework: Framework, cloud_provider: Literal["aws", "gcp"]):
-    docker_repo_prefix = ""
-    if cloud_provider == "aws":
-        docker_repo_prefix = "public.ecr.aws/docker/library/"
-    # Dynamically get the current Python major and minor versions
-    python_major_version = sys.version_info.major
-    python_minor_version = sys.version_info.minor
-
-    if framework == Framework.FASTAPI:
-        startup_cmd = "uvicorn app.main:app --host 0.0.0.0 --port $PORT"
-        # TODO: app_dir should be a parameter / inferred somehow
-        app_dir = "app"
-    else:
-        raise NotImplementedError(f"{framework} is not supported yet.")
-
-    return DOCKERFILE_SERVICE_TEMPLATE.format(
-        docker_repo_prefix=docker_repo_prefix,
-        python_major_version=python_major_version,
-        python_minor_version=python_minor_version,
-        port=8000,
-        app_dir=app_dir,
-        startup_cmd=startup_cmd,
-    )
-
-
-if __name__ == "__main__":
-    print(template(Framework.FASTAPI))
+CMD exec gunicorn --bind 0.0.0.0:$PORT --workers 1 --threads 8 --timeout 0 django_app.wsgi:application
```

### Comparing `launchflow-0.3.9/launchflow/cli/utils.py` & `launchflow-0.3.9.dev0/launchflow/cli/utils.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/clients/accounts_client.py` & `launchflow-0.3.9.dev0/launchflow/clients/accounts_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/clients/client.py` & `launchflow-0.3.9.dev0/launchflow/clients/client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/clients/connect_client.py` & `launchflow-0.3.9.dev0/launchflow/clients/connect_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/clients/environments_client.py` & `launchflow-0.3.9.dev0/launchflow/clients/environments_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,74 @@
 
 
 class _CloudProvider(enum.Enum):
     AWS = "aws"
     GCP = "gcp"
 
 
+class EnvironmentsSyncClient:
+    def __init__(self, http_client: httpx.Client):
+        self.http_client = http_client
+
+    def base_url(self, project_name: str) -> str:
+        return f"{config.settings.launch_service_address}/projects/{project_name}/environments"
+
+    def _create(
+        self,
+        project_name: str,
+        env_name: str,
+        env_type: EnvironmentType,
+        cloud_provider: _CloudProvider,
+    ) -> OperationResponse:
+        body = {
+            "name": env_name,
+            "environment_type": env_type.value,
+        }
+        response = self.http_client.post(
+            f"{self.base_url(project_name)}/{cloud_provider.value}",
+            json=body,
+            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+        )
+        if response.status_code not in [200, 201, 202]:
+            raise LaunchFlowRequestFailure(response)
+        return OperationResponse.model_validate(response.json())
+
+    def create_aws(
+        self, project_name: str, env_name: str, env_type: EnvironmentType
+    ) -> OperationResponse:
+        return self._create(project_name, env_name, env_type, _CloudProvider.AWS)
+
+    def create_gcp(
+        self, project_name: str, env_name: str, env_type: EnvironmentType
+    ) -> OperationResponse:
+        return self._create(project_name, env_name, env_type, _CloudProvider.GCP)
+
+    def get(self, project_name: str, env_name: str):
+        url = f"{self.base_url(project_name)}/{env_name}"
+        response = self.http_client.get(
+            url,
+            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+        )
+        if response.status_code != 200:
+            raise LaunchFlowRequestFailure(response)
+        return EnvironmentResponse.model_validate(response.json())
+
+    def list(self, project_name):
+        response = self.http_client.get(
+            self.base_url(project_name),
+            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+        )
+        if response.status_code != 200:
+            raise LaunchFlowRequestFailure(response)
+        return [
+            EnvironmentResponse.model_validate(env)
+            for env in response.json()["environments"]
+        ]
+
+
 class EnvironmentsAsyncClient:
     def __init__(self, http_client: httpx.AsyncClient):
         self.http_client = http_client
 
     def base_url(self, project_name: str) -> str:
         return f"{config.settings.launch_service_address}/projects/{project_name}/environments"
```

### Comparing `launchflow-0.3.9/launchflow/clients/operations_client.py` & `launchflow-0.3.9.dev0/launchflow/clients/operations_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/clients/projects_client.py` & `launchflow-0.3.9.dev0/launchflow/clients/projects_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/clients/resources_client.py` & `launchflow-0.3.9.dev0/launchflow/clients/resources_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/clients/response_schemas.py` & `launchflow-0.3.9.dev0/launchflow/clients/response_schemas.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/clients/services_client.py` & `launchflow-0.3.9.dev0/launchflow/clients/services_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/config/launchflow_config.py` & `launchflow-0.3.9.dev0/launchflow/config/launchflow_config.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/config/launchflow_env.py` & `launchflow-0.3.9.dev0/launchflow/config/launchflow_env.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/config/launchflow_yaml.py` & `launchflow-0.3.9.dev0/launchflow/config/launchflow_yaml.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/context/launchflow_ctx.py` & `launchflow-0.3.9.dev0/launchflow/context/launchflow_ctx.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from typing import Dict, Optional
 
 import fsspec
 import httpx
 import yaml
 from launchflow.cache import cache
 from launchflow.clients.client import LaunchFlowAsyncClient
+from launchflow.clients.environments_client import (
+    EnvironmentsAsyncClient,
+    EnvironmentsSyncClient,
+)
 from launchflow.clients.resources_client import (
     ResourcesAsyncClient,
     ResourcesSyncClient,
 )
 from launchflow.config import config
 from launchflow.operations import AsyncResourceNoOp, AsyncResourceOp
 
@@ -161,18 +165,33 @@
             bucket_name = connection_bucket_path.removeprefix("s3://").split("/")[0]
             bucket_url = f"https://s3.console.aws.amazon.com/s3/buckets/{bucket_name}"
         raise exceptions.ForbiddenConnectionInfo(bucket_url) from e
 
     return resource_connection_info
 
 
+def _load_gcp_service_account_email_from_cache(
+    project_name: str, environment_name: str
+):
+    gcp_service_account_email = cache.get_gcp_service_account_email(
+        project_name, environment_name
+    )
+    if gcp_service_account_email is not None:
+        logging.debug(
+            f"Using cached GCP service account email for {project_name}/{environment_name}"
+        )
+        return gcp_service_account_email
+
+
 @dataclass
 class LaunchFlowContext:
     _resource_async_client: Optional[ResourcesAsyncClient] = None
     _resource_sync_client: Optional[ResourcesSyncClient] = None
+    _environment_async_client: Optional[EnvironmentsAsyncClient] = None
+    _environment_sync_client: Optional[EnvironmentsSyncClient] = None
     _lf_client: Optional[LaunchFlowAsyncClient] = None
 
     @property
     def lf_client(self):
         if self._lf_client is None:
             self._lf_client = LaunchFlowAsyncClient()
         return self._lf_client
@@ -187,14 +206,30 @@
 
     @property
     def resource_sync_client(self):
         if self._resource_sync_client is None:
             self._resource_sync_client = ResourcesSyncClient(httpx.Client(timeout=60))
         return self._resource_sync_client
 
+    @property
+    def environment_async_client(self):
+        if self._environment_async_client is None:
+            self._environment_async_client = EnvironmentsAsyncClient(
+                httpx.AsyncClient(timeout=60)
+            )
+        return self._environment_async_client
+
+    @property
+    def environment_sync_client(self):
+        if self._environment_sync_client is None:
+            self._environment_sync_client = EnvironmentsSyncClient(
+                httpx.Client(timeout=60)
+            )
+        return self._environment_sync_client
+
     def get_resource_connection_info_sync(
         self,
         product_name: str,
         resource_name: str,
         project_name: Optional[str] = None,
         environment_name: Optional[str] = None,
     ) -> Dict:
@@ -269,14 +304,15 @@
 
         # Load connection info from remote bucket
         connection_bucket_path = _get_connection_bucket_path_from_local(resource_uri)
         if connection_bucket_path is None:
             connection_bucket_path = await _get_connection_bucket_from_remote_async(
                 self.resource_async_client, resource_uri
             )
+            print(connection_bucket_path)
 
         resource_connection_info = _load_connection_info_from_remote_bucket(
             connection_bucket_path, resource_uri.resource_name
         )
         cache.set_resource_connection_info(
             resource_uri.project_name,
             resource_uri.environment_name,
@@ -375,7 +411,36 @@
             return AsyncResourceOp(
                 resource_ref=f"{resource_type}(name={resource_name})",
                 operation_id=None,
                 client=self.lf_client,
                 _op=create_operation,
                 _type="create",
             )
+
+    def get_gcp_service_account_email(
+        self,
+        project_name: Optional[str] = None,
+        environment_name: Optional[str] = None,
+    ):
+        project_name = project_name or config.project
+        environment_name = environment_name or config.environment
+        if project_name is None or environment_name is None:
+            raise exceptions.ProjectOrEnvironmentNotSet(project_name, environment_name)
+
+        gcp_service_account_email = _load_gcp_service_account_email_from_cache(
+            project_name, environment_name
+        )
+
+        if gcp_service_account_email is None:
+            environment_info = self.environment_sync_client.get(
+                project_name=project_name, env_name=environment_name
+            )
+            if environment_info.gcp_config is None:
+                raise exceptions.GCPConfigNotFound(environment_name)
+            gcp_service_account_email = (
+                environment_info.gcp_config.gcp_service_account_email
+            )
+            cache.set_gcp_service_account_email(
+                project_name, environment_name, gcp_service_account_email
+            )
+
+        return gcp_service_account_email
```

### Comparing `launchflow-0.3.9/launchflow/exceptions.py` & `launchflow-0.3.9.dev0/launchflow/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,7 +96,15 @@
 
 
 class ServiceProductMismatch(Exception):
     def __init__(self, product: str, service: str) -> None:
         super().__init(
             f"Product '{product}' does not match the product of service '{service}'."
         )
+
+
+class GCPConfigNotFound(Exception):
+    def __init__(self, environment_name: str) -> None:
+        super().__init(
+            f"GCP configuration not found for environment '{environment_name}'. "
+            "This environment is most likely an AWS environment."
+        )
```

### Comparing `launchflow-0.3.9/launchflow/fastapi.py` & `launchflow-0.3.9.dev0/launchflow/fastapi.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/flows/account_id.py` & `launchflow-0.3.9.dev0/launchflow/flows/account_id.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/flows/auth.py` & `launchflow-0.3.9.dev0/launchflow/flows/auth.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/flows/cloud_provider.py` & `launchflow-0.3.9.dev0/launchflow/flows/cloud_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.prompt import Prompt
 
 from launchflow.clients import LaunchFlowAsyncClient
 
 
 class CloudProvider(Enum):
-    GCP = "GCP"
-    AWS = "AWS"
-    AZURE = "Azure"
+    GCP = "gcp"
+    AWS = "aws"
+    AZURE = "azure"
 
 
 CLOUD_PROVIDER_CHOICES = [
     (CloudProvider.GCP, "Google Cloud Platform"),
     (CloudProvider.AWS, "Amazon Web Services"),
     # (CloudProvider.AZURE, "Microsoft Azure"),
 ]
```

### Comparing `launchflow-0.3.9/launchflow/flows/environments_flows.py` & `launchflow-0.3.9.dev0/launchflow/flows/environments_flows.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/flows/project_flows.py` & `launchflow-0.3.9.dev0/launchflow/flows/project_flows.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/flows/resource_flows.py` & `launchflow-0.3.9.dev0/launchflow/flows/resource_flows.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/gcp/cloudsql.py` & `launchflow-0.3.9.dev0/launchflow/gcp/cloudsql.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             name=name,
             product_name="gcp_sql_postgres",
             create_args={
                 "postgres_version": postgres_version.value,
             },
         )
 
-    def django_options(self):
+    def django_settings(self):
         if psycopg2 is None:
             raise ImportError(
                 "psycopg2 is not installed. Please install it with `pip install psycopg2`."
             )
 
         connection_info = self.connect()
```

### Comparing `launchflow-0.3.9/launchflow/gcp/compute_engine.py` & `launchflow-0.3.9.dev0/launchflow/gcp/compute_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -49,39 +49,46 @@
             product_name="gcp_compute_engine_redis",
             create_args={},
         )
 
         self._async_pool = None
         self._sync_client = None
 
-    def redis(self):
+    def django_settings(self):
+        connection_info = self.connect()
+        return {
+            "BACKEND": "django.core.cache.backends.redis.RedisCache",
+            "LOCATION": f"redis://default:{connection_info.password}@{connection_info.host}:{connection_info.port}",
+        }
+
+    def redis(self, *, decode_responses: bool = True):
         """Get a Generic Redis Client object from the redis-py library.
 
         **Returns**:
         - The [Generic Redis Client](https://redis-py.readthedocs.io/en/stable/connections.html#generic-client) from the redis-py library.
         """
         _check_installs()
         connection_info = self.connect()
         if self._sync_client is None:
             self._sync_client = redis.Redis(
                 host=connection_info.host,
                 port=connection_info.port,
                 password=connection_info.password,
-                decode_responses=True,
+                decode_responses=decode_responses,
             )
         return self._sync_client
 
-    async def redis_async(self):
+    async def redis_async(self, *, decode_responses: bool = True):
         """Get an Async Redis Client object from the redis-py library.
 
         **Returns**:
         - The [Async Redis Client object](https://redis-py.readthedocs.io/en/stable/connections.html#async-client) from the redis-py library.
         """
         _check_installs()
         connection_info = await self.connect_async()
         if self._async_pool is None:
             self._async_pool = await redis.asyncio.from_url(
                 f"redis://{connection_info.host}:{connection_info.port}",
                 password=connection_info.password,
-                decode_responses=True,
+                decode_responses=decode_responses,
             )
         return self._async_pool
```

### Comparing `launchflow-0.3.9/launchflow/gcp/gcs.py` & `launchflow-0.3.9.dev0/launchflow/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/gcp/memorystore.py` & `launchflow-0.3.9.dev0/launchflow/gcp/memorystore.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,14 +47,21 @@
     def __init__(self, name: str, *, memory_size_gb: int = 1) -> None:
         super().__init__(
             name=name,
             product_name="gcp_memorystore_redis",
             create_args={"memory_size_gb": memory_size_gb},
         )
 
+    def django_settings(self):
+        connection_info = self.connect()
+        return {
+            "BACKEND": "django.core.cache.backends.redis.RedisCache",
+            "LOCATION": f"redis://default:{connection_info.password}@{connection_info.host}:{connection_info.port}",
+        }
+
     def redis(self):
         """Get a Generic Redis Client object from the redis-py library.
 
         **Returns**:
         - The [Generic Redis Client](https://redis-py.readthedocs.io/en/stable/connections.html#generic-client) from the redis-py library.
         """
         _check_installs()
```

### Comparing `launchflow-0.3.9/launchflow/operations.py` & `launchflow-0.3.9.dev0/launchflow/operations.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/resource.py` & `launchflow-0.3.9.dev0/launchflow/resource.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow/utils.py` & `launchflow-0.3.9.dev0/launchflow/utils.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9/launchflow.egg-info/PKG-INFO` & `launchflow-0.3.9.dev0/launchflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchflow
-Version: 0.3.9
+Version: 0.3.9.dev0
 Summary: Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic.
 Author-email: CalebTVanDyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: beaupy
 Requires-Dist: rich
```

### Comparing `launchflow-0.3.9/pyproject.toml` & `launchflow-0.3.9.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "launchflow"
-version = "0.3.9"
+version = "0.3.9.dev0"
 description = "Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic."
 authors = [
     { name = "CalebTVanDyke", email = "caleb@launchflow.com" },
     { name = "Josh Tanke", email = "josh@launchflow.com" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
```

