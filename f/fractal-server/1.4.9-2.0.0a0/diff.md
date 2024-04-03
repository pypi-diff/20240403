# Comparing `tmp/fractal_server-1.4.9.tar.gz` & `tmp/fractal_server-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.4.9.tar", max compression
+gzip compressed data, was "fractal_server-2.0.0a0.tar", max compression
```

## Comparing `fractal_server-1.4.9.tar` & `fractal_server-2.0.0a0.tar`

### file list

```diff
@@ -1,96 +1,165 @@
--rw-r--r--   0        0        0     1576 2024-02-23 13:32:12.702433 fractal_server-1.4.9/LICENSE
--rw-r--r--   0        0        0     2466 2024-02-23 13:32:12.702433 fractal_server-1.4.9/README.md
--rw-r--r--   0        0        0       22 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/__init__.py
--rw-r--r--   0        0        0     4958 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     4042 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      353 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     2000 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/models/dataset.py
--rw-r--r--   0        0        0     3287 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0      848 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     3135 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1087 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     2632 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     3933 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0        0 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/__init__.py
--rw-r--r--   0        0        0    13872 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/admin.py
--rw-r--r--   0        0        0      315 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/__init__.py
--rw-r--r--   0        0        0      944 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/v1/__init__.py
--rw-r--r--   0        0        0    11948 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/v1/_aux_functions.py
--rw-r--r--   0        0        0    16553 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/v1/dataset.py
--rw-r--r--   0        0        0     5400 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/v1/job.py
--rw-r--r--   0        0        0    15673 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/v1/project.py
--rw-r--r--   0        0        0     5745 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/v1/task.py
--rw-r--r--   0        0        0     8340 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/v1/task_collection.py
--rw-r--r--   0        0        0    10864 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/v1/workflow.py
--rw-r--r--   0        0        0     5550 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/api/v1/workflowtask.py
--rw-r--r--   0        0        0     4885 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/auth.py
--rw-r--r--   0        0        0        0 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/aux/__init__.py
--rw-r--r--   0        0        0     1246 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/aux/_job.py
--rw-r--r--   0        0        0      675 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/routes/aux/_runner.py
--rw-r--r--   0        0        0       16 2024-02-23 13:32:12.706433 fractal_server-1.4.9/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0    13812 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    24363 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     6799 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3245 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     4850 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4402 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    21010 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2930 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     5122 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    43886 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     9508 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0     4653 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/runner/handle_failed_job.py
--rw-r--r--   0        0        0     2010 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/__init__.py
--rw-r--r--   0        0        0     2549 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/_validators.py
--rw-r--r--   0        0        0     4264 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3375 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/dataset.py
--rw-r--r--   0        0        0     1258 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/dumps.py
--rw-r--r--   0        0        0     1787 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/json_schemas/manifest.json
--rw-r--r--   0        0        0     3819 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/manifest.py
--rw-r--r--   0        0        0     1196 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/project.py
--rw-r--r--   0        0        0      692 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/state.py
--rw-r--r--   0        0        0     3671 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/task.py
--rw-r--r--   0        0        0     3044 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/task_collection.py
--rw-r--r--   0        0        0     3113 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/user.py
--rw-r--r--   0        0        0     4525 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/schemas/workflow.py
--rw-r--r--   0        0        0    11203 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0    15302 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/config.py
--rw-r--r--   0        0        0      398 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/data_migrations/README.md
--rw-r--r--   0        0        0     3924 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/logger.py
--rw-r--r--   0        0        0     2706 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/main.py
--rw-r--r--   0        0        0       59 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/README
--rw-r--r--   0        0        0     2690 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      526 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     1157 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
--rw-r--r--   0        0        0     8770 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0     1632 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
--rw-r--r--   0        0        0     1353 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
--rw-r--r--   0        0        0     2684 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
--rw-r--r--   0        0        0     1115 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
--rw-r--r--   0        0        0     1057 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
--rw-r--r--   0        0        0      883 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
--rw-r--r--   0        0        0     1849 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
--rw-r--r--   0        0        0      867 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
--rw-r--r--   0        0        0      949 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
--rw-r--r--   0        0        0      963 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
--rw-r--r--   0        0        0     1221 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
--rw-r--r--   0        0        0      746 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/syringe.py
--rw-r--r--   0        0        0     3765 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/tasks/_TaskCollectPip.py
--rw-r--r--   0        0        0      176 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12744 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/tasks/background_operations.py
--rw-r--r--   0        0        0     5549 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/tasks/endpoint_operations.py
--rw-r--r--   0        0        0     2274 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/tasks/utils.py
--rw-r--r--   0        0        0     2115 2024-02-23 13:32:12.710433 fractal_server-1.4.9/fractal_server/utils.py
--rw-r--r--   0        0        0     3071 2024-02-23 13:32:12.714434 fractal_server-1.4.9/pyproject.toml
--rw-r--r--   0        0        0     4263 1970-01-01 00:00:00.000000 fractal_server-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-03 07:30:52.917648 fractal_server-2.0.0a0/LICENSE
+-rw-r--r--   0        0        0     2466 2024-04-03 07:30:52.917648 fractal_server-2.0.0a0/README.md
+-rw-r--r--   0        0        0       24 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/__init__.py
+-rw-r--r--   0        0        0     4958 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     4042 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     3378 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1090 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0      360 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v1/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v1/dataset.py
+-rw-r--r--   0        0        0     3304 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v1/job.py
+-rw-r--r--   0        0        0      859 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v1/project.py
+-rw-r--r--   0        0        0     2782 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v1/task.py
+-rw-r--r--   0        0        0     3950 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v1/workflow.py
+-rw-r--r--   0        0        0      400 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v2/__init__.py
+-rw-r--r--   0        0        0     1475 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v2/dataset.py
+-rw-r--r--   0        0        0     1535 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v2/job.py
+-rw-r--r--   0        0        0      845 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v2/project.py
+-rw-r--r--   0        0        0     3257 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v2/task.py
+-rw-r--r--   0        0        0     1256 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v2/workflow.py
+-rw-r--r--   0        0        0     2727 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/models/v2/workflowtask.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/__init__.py
+-rw-r--r--   0        0        0    13981 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/admin/v1.py
+-rw-r--r--   0        0        0     8908 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/admin/v2.py
+-rw-r--r--   0        0        0      315 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/__init__.py
+-rw-r--r--   0        0        0      958 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/__init__.py
+-rw-r--r--   0        0        0    11955 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0    16911 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/dataset.py
+-rw-r--r--   0        0        0     5427 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/job.py
+-rw-r--r--   0        0        0    15765 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/project.py
+-rw-r--r--   0        0        0     6123 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/task.py
+-rw-r--r--   0        0        0     8457 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/task_collection.py
+-rw-r--r--   0        0        0    10930 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     1212 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/__init__.py
+-rw-r--r--   0        0        0    14142 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/_aux_functions.py
+-rw-r--r--   0        0        0     7237 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/apply.py
+-rw-r--r--   0        0        0     9730 2024-04-03 07:30:52.921648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/dataset.py
+-rw-r--r--   0        0        0     5939 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/images.py
+-rw-r--r--   0        0        0     5334 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/job.py
+-rw-r--r--   0        0        0     6183 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/project.py
+-rw-r--r--   0        0        0     7130 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/task.py
+-rw-r--r--   0        0        0     8466 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/task_collection.py
+-rw-r--r--   0        0        0    12608 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/workflow.py
+-rw-r--r--   0        0        0     8895 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/workflowtask.py
+-rw-r--r--   0        0        0     4885 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/auth.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/aux/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/aux/_job.py
+-rw-r--r--   0        0        0      675 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/routes/aux/_runner.py
+-rw-r--r--   0        0        0       16 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0      829 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/async_wrap.py
+-rw-r--r--   0        0        0     4159 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/exceptions.py
+-rw-r--r--   0        0        0       89 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/local/__init__.py
+-rw-r--r--   0        0        0     3644 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/local/executor.py
+-rw-r--r--   0        0        0       65 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/__init__.py
+-rw-r--r--   0        0        0     8841 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/_batching.py
+-rw-r--r--   0        0        0     1908 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
+-rw-r--r--   0        0        0     4421 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    15552 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/_slurm_config.py
+-rw-r--r--   0        0        0     5123 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    43919 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/executor.py
+-rw-r--r--   0        0        0     5852 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/remote.py
+-rw-r--r--   0        0        0      206 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/filenames.py
+-rw-r--r--   0        0        0     1254 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/set_start_and_last_task_index.py
+-rw-r--r--   0        0        0     3264 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/task_files.py
+-rw-r--r--   0        0        0    13616 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/__init__.py
+-rw-r--r--   0        0        0    21238 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/_common.py
+-rw-r--r--   0        0        0     6937 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/_local/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/_local/_local_config.py
+-rw-r--r--   0        0        0     1493 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/_local/_submit_setup.py
+-rw-r--r--   0        0        0    10839 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/_slurm/__init__.py
+-rw-r--r--   0        0        0     2732 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     5977 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0     3294 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/common.py
+-rw-r--r--   0        0        0     4684 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v1/handle_failed_job.py
+-rw-r--r--   0        0        0    12476 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/__init__.py
+-rw-r--r--   0        0        0     6207 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/_local/__init__.py
+-rw-r--r--   0        0        0     3630 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/_local/_local_config.py
+-rw-r--r--   0        0        0     1614 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/_local/_submit_setup.py
+-rw-r--r--   0        0        0     5138 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/_slurm/__init__.py
+-rw-r--r--   0        0        0     2847 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     6621 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0      119 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/components.py
+-rw-r--r--   0        0        0      758 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/deduplicate_list.py
+-rw-r--r--   0        0        0     5149 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/handle_failed_job.py
+-rw-r--r--   0        0        0     1368 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/merge_outputs.py
+-rw-r--r--   0        0        0    10927 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/runner.py
+-rw-r--r--   0        0        0     9968 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/runner_functions.py
+-rw-r--r--   0        0        0     3844 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/runner_functions_low_level.py
+-rw-r--r--   0        0        0     1243 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/task_interface.py
+-rw-r--r--   0        0        0      495 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/runner/v2/v1_compat.py
+-rw-r--r--   0        0        0      157 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/__init__.py
+-rw-r--r--   0        0        0     2549 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/_validators.py
+-rw-r--r--   0        0        0     1787 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/json_schemas/manifest.json
+-rw-r--r--   0        0        0      692 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/state.py
+-rw-r--r--   0        0        0     3113 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/user.py
+-rw-r--r--   0        0        0     2078 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v1/__init__.py
+-rw-r--r--   0        0        0     4302 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v1/applyworkflow.py
+-rw-r--r--   0        0        0     3444 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v1/dataset.py
+-rw-r--r--   0        0        0     1274 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v1/dumps.py
+-rw-r--r--   0        0        0     3829 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v1/manifest.py
+-rw-r--r--   0        0        0     1218 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v1/project.py
+-rw-r--r--   0        0        0     3704 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v1/task.py
+-rw-r--r--   0        0        0     3057 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v1/task_collection.py
+-rw-r--r--   0        0        0     4618 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v1/workflow.py
+-rw-r--r--   0        0        0     1704 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/__init__.py
+-rw-r--r--   0        0        0     1792 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/dataset.py
+-rw-r--r--   0        0        0     2047 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/dumps.py
+-rw-r--r--   0        0        0     3203 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/job.py
+-rw-r--r--   0        0        0     4183 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/manifest.py
+-rw-r--r--   0        0        0      767 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/project.py
+-rw-r--r--   0        0        0     3603 2024-04-03 07:30:52.925648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/task.py
+-rw-r--r--   0        0        0     2993 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/task_collection.py
+-rw-r--r--   0        0        0     1784 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/workflow.py
+-rw-r--r--   0        0        0     3377 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/app/schemas/v2/workflowtask.py
+-rw-r--r--   0        0        0    11203 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0    15080 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/config.py
+-rw-r--r--   0        0        0      398 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/data_migrations/README.md
+-rw-r--r--   0        0        0     1536 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/images/__init__.py
+-rw-r--r--   0        0        0     2412 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/images/tools.py
+-rw-r--r--   0        0        0     3924 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/logger.py
+-rw-r--r--   0        0        0     3001 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2690 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      526 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      962 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/4b35c5cefbe3_tmp_is_v2_compatible.py
+-rw-r--r--   0        0        0      954 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     1157 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
+-rw-r--r--   0        0        0     8770 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0     7411 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/56af171b0159_v2.py
+-rw-r--r--   0        0        0     1632 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
+-rw-r--r--   0        0        0     1353 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
+-rw-r--r--   0        0        0     2684 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
+-rw-r--r--   0        0        0     2034 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/876f28db9d4e_tmp_split_task_and_wftask_meta.py
+-rw-r--r--   0        0        0     1115 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
+-rw-r--r--   0        0        0      933 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/974c802f0dd0_tmp_workflowtaskv2_type_in_db.py
+-rw-r--r--   0        0        0     1057 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
+-rw-r--r--   0        0        0      883 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
+-rw-r--r--   0        0        0     1168 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/9cd305cd6023_tmp_workflowtaskv2.py
+-rw-r--r--   0        0        0     1849 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
+-rw-r--r--   0        0        0     1224 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/a6231ed6273c_tmp_args_schemas_in_taskv2.py
+-rw-r--r--   0        0        0      867 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
+-rw-r--r--   0        0        0      893 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/b9e9eed9d442_tmp_taskv2_type.py
+-rw-r--r--   0        0        0      949 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
+-rw-r--r--   0        0        0     1409 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/e3e639454d4b_tmp_make_task_meta_non_optional.py
+-rw-r--r--   0        0        0      963 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
+-rw-r--r--   0        0        0     1221 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
+-rw-r--r--   0        0        0      746 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/syringe.py
+-rw-r--r--   0        0        0       23 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0     5379 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/tasks/endpoint_operations.py
+-rw-r--r--   0        0        0     3278 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/tasks/utils.py
+-rw-r--r--   0        0        0     3775 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/tasks/v1/_TaskCollectPip.py
+-rw-r--r--   0        0        0    11725 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/tasks/v1/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/tasks/v1/get_collection_data.py
+-rw-r--r--   0        0        0     3775 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/tasks/v2/_TaskCollectPip.py
+-rw-r--r--   0        0        0    12829 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/tasks/v2/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/tasks/v2/get_collection_data.py
+-rw-r--r--   0        0        0     2115 2024-04-03 07:30:52.929648 fractal_server-2.0.0a0/fractal_server/utils.py
+-rw-r--r--   0        0        0     2973 2024-04-03 07:30:52.933647 fractal_server-2.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     4205 1970-01-01 00:00:00.000000 fractal_server-2.0.0a0/PKG-INFO
```

### Comparing `fractal_server-1.4.9/LICENSE` & `fractal_server-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/README.md` & `fractal_server-2.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/__main__.py` & `fractal_server-2.0.0a0/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/alembic.ini` & `fractal_server-2.0.0a0/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/app/db/__init__.py` & `fractal_server-2.0.0a0/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/app/models/dataset.py` & `fractal_server-2.0.0a0/fractal_server/app/models/v1/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from sqlalchemy.ext.orderinglist import ordering_list
 from sqlalchemy.types import DateTime
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import Relationship
 from sqlmodel import SQLModel
 
-from ...utils import get_timestamp
-from ..schemas.dataset import _DatasetBase
-from ..schemas.dataset import _ResourceBase
+from ....utils import get_timestamp
+from ...schemas.v1.dataset import _DatasetBaseV1
+from ...schemas.v1.dataset import _ResourceBaseV1
 
 
-class Resource(_ResourceBase, SQLModel, table=True):
+class Resource(_ResourceBaseV1, SQLModel, table=True):
     id: Optional[int] = Field(default=None, primary_key=True)
     dataset_id: int = Field(foreign_key="dataset.id")
 
 
-class Dataset(_DatasetBase, SQLModel, table=True):
+class Dataset(_DatasetBaseV1, SQLModel, table=True):
     """
     Represent a dataset
 
     Attributes:
         id:
             Primary key
         project_id:
```

### Comparing `fractal_server-1.4.9/fractal_server/app/models/job.py` & `fractal_server-2.0.0a0/fractal_server/app/models/v1/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from sqlalchemy import Column
 from sqlalchemy.types import DateTime
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import SQLModel
 
-from ...utils import get_timestamp
-from ..schemas import JobStatusType
-from ..schemas.applyworkflow import _ApplyWorkflowBase
+from ....utils import get_timestamp
+from ...schemas.v1 import JobStatusTypeV1
+from ...schemas.v1.applyworkflow import _ApplyWorkflowBaseV1
 
 
-class ApplyWorkflow(_ApplyWorkflowBase, SQLModel, table=True):
+class ApplyWorkflow(_ApplyWorkflowBaseV1, SQLModel, table=True):
     """
     Represent a workflow run
 
     This table is responsible for storing the state of a workflow execution in
     the database.
 
     Attributes:
@@ -93,9 +93,9 @@
     start_timestamp: datetime = Field(
         default_factory=get_timestamp,
         sa_column=Column(DateTime(timezone=True), nullable=False),
     )
     end_timestamp: Optional[datetime] = Field(
         default=None, sa_column=Column(DateTime(timezone=True))
     )
-    status: str = JobStatusType.SUBMITTED
+    status: str = JobStatusTypeV1.SUBMITTED
     log: Optional[str] = None
```

### Comparing `fractal_server-1.4.9/fractal_server/app/models/project.py` & `fractal_server-2.0.0a0/fractal_server/app/models/v1/project.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 from sqlalchemy import Column
 from sqlalchemy.types import DateTime
 from sqlmodel import Field
 from sqlmodel import Relationship
 from sqlmodel import SQLModel
 
-from ...utils import get_timestamp
-from ..schemas.project import _ProjectBase
-from .linkuserproject import LinkUserProject
-from .security import UserOAuth
+from ....utils import get_timestamp
+from ...schemas.v1.project import _ProjectBaseV1
+from ..linkuserproject import LinkUserProject
+from ..security import UserOAuth
 
 
-class Project(_ProjectBase, SQLModel, table=True):
+class Project(_ProjectBaseV1, SQLModel, table=True):
 
     id: Optional[int] = Field(default=None, primary_key=True)
     timestamp_created: datetime = Field(
         default_factory=get_timestamp,
         sa_column=Column(DateTime(timezone=True), nullable=False),
     )
```

### Comparing `fractal_server-1.4.9/fractal_server/app/models/security.py` & `fractal_server-2.0.0a0/fractal_server/app/models/security.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from sqlalchemy import Column
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import Relationship
 from sqlmodel import SQLModel
 
 from .linkuserproject import LinkUserProject
+from .linkuserproject import LinkUserProjectV2
 
 
 class OAuthAccount(SQLModel, table=True):
     """
     OAuth account model
 
     This class is based on fastapi_users_db_sqlmodel::SQLModelBaseOAuthAccount.
@@ -103,10 +104,15 @@
         sa_relationship_kwargs={"lazy": "joined", "cascade": "all, delete"},
     )
     project_list: list["Project"] = Relationship(  # noqa
         back_populates="user_list",
         link_model=LinkUserProject,
         sa_relationship_kwargs={"lazy": "selectin"},
     )
+    project_list_v2: list["ProjectV2"] = Relationship(  # noqa
+        back_populates="user_list",
+        link_model=LinkUserProjectV2,
+        sa_relationship_kwargs={"lazy": "selectin"},
+    )
 
     class Config:
         orm_mode = True
```

### Comparing `fractal_server-1.4.9/fractal_server/app/models/state.py` & `fractal_server-2.0.0a0/fractal_server/app/models/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sqlalchemy import Column
 from sqlalchemy.types import DateTime
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import SQLModel
 
 from ...utils import get_timestamp
-from ..schemas import _StateBase
+from ..schemas.v1 import _StateBase
 
 
 class State(_StateBase, SQLModel, table=True):
     """
     Store arbitrary data in the database
 
     This table is just a state interchange that allows the system to store
```

### Comparing `fractal_server-1.4.9/fractal_server/app/models/task.py` & `fractal_server-2.0.0a0/fractal_server/app/models/v1/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 import logging
 from typing import Any
 from typing import Optional
 
 from pydantic import HttpUrl
 from sqlalchemy import Column
+from sqlalchemy import sql
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import SQLModel
 
-from ..schemas.task import _TaskBase
+from ...schemas.v1.task import _TaskBaseV1
 
 
-class Task(_TaskBase, SQLModel, table=True):
+class Task(_TaskBaseV1, SQLModel, table=True):
     """
     Task model
 
     Attributes:
         id: Primary key
         command: Executable command
         input_type: Expected type of input `Dataset`
@@ -44,14 +45,18 @@
     args_schema: Optional[dict[str, Any]] = Field(
         sa_column=Column(JSON), default=None
     )
     args_schema_version: Optional[str]
     docs_info: Optional[str] = None
     docs_link: Optional[HttpUrl] = None
 
+    is_v2_compatible: bool = Field(
+        default=False, sa_column_kwargs={"server_default": sql.false()}
+    )
+
     @property
     def parallelization_level(self) -> Optional[str]:
         try:
             return self.meta["parallelization_level"]
         except KeyError:
             return None
```

### Comparing `fractal_server-1.4.9/fractal_server/app/models/workflow.py` & `fractal_server-2.0.0a0/fractal_server/app/models/v1/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from sqlalchemy.ext.orderinglist import ordering_list
 from sqlalchemy.types import DateTime
 from sqlalchemy.types import JSON
 from sqlmodel import Field
 from sqlmodel import Relationship
 from sqlmodel import SQLModel
 
-from ...utils import get_timestamp
-from ..schemas.workflow import _WorkflowBase
-from ..schemas.workflow import _WorkflowTaskBase
+from ....utils import get_timestamp
+from ...schemas.v1.workflow import _WorkflowBaseV1
+from ...schemas.v1.workflow import _WorkflowTaskBaseV1
 from .task import Task
 
 
-class WorkflowTask(_WorkflowTaskBase, SQLModel, table=True):
+class WorkflowTask(_WorkflowTaskBaseV1, SQLModel, table=True):
     """
     A Task as part of a Workflow
 
     This is a crossing table between Task and Workflow. In addition to the
     foreign keys, it allows for parameter overriding and keeps the order
     within the list of tasks of the workflow.
 
@@ -88,15 +88,15 @@
         return self.task.is_parallel
 
     @property
     def parallelization_level(self) -> Union[str, None]:
         return self.task.parallelization_level
 
 
-class Workflow(_WorkflowBase, SQLModel, table=True):
+class Workflow(_WorkflowBaseV1, SQLModel, table=True):
     """
     Workflow
 
     Attributes:
         id:
             Primary key
         project_id:
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/admin.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/admin/v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 from fastapi.responses import StreamingResponse
 from sqlalchemy import func
 from sqlmodel import select
 
-from ...config import get_settings
-from ...syringe import Inject
-from ...utils import get_timestamp
-from ..db import AsyncSession
-from ..db import get_async_db
-from ..models import ApplyWorkflow
-from ..models import Dataset
-from ..models import JobStatusType
-from ..models import Project
-from ..models import Workflow
-from ..models.security import UserOAuth as User
-from ..runner._common import WORKFLOW_LOG_FILENAME
-from ..schemas import ApplyWorkflowRead
-from ..schemas import ApplyWorkflowUpdate
-from ..schemas import DatasetRead
-from ..schemas import ProjectRead
-from ..schemas import WorkflowRead
-from ..security import current_active_superuser
-from .aux._job import _write_shutdown_file
-from .aux._job import _zip_folder_to_byte_stream
-from .aux._runner import _check_backend_is_slurm
+from ....config import get_settings
+from ....syringe import Inject
+from ....utils import get_timestamp
+from ...db import AsyncSession
+from ...db import get_async_db
+from ...models import ApplyWorkflow
+from ...models import Dataset
+from ...models import JobStatusTypeV1
+from ...models import Project
+from ...models import Workflow
+from ...models.security import UserOAuth as User
+from ...runner.filenames import WORKFLOW_LOG_FILENAME
+from ...schemas.v1 import ApplyWorkflowReadV1
+from ...schemas.v1 import ApplyWorkflowUpdateV1
+from ...schemas.v1 import DatasetReadV1
+from ...schemas.v1 import ProjectReadV1
+from ...schemas.v1 import WorkflowReadV1
+from ...security import current_active_superuser
+from ..aux._job import _write_shutdown_file
+from ..aux._job import _zip_folder_to_byte_stream
+from ..aux._runner import _check_backend_is_slurm
 
-router_admin = APIRouter()
+router_admin_v1 = APIRouter()
 
 
 def _convert_to_db_timestamp(dt: datetime) -> datetime:
     """
     This function takes a timezone-aware datetime and converts it to UTC.
     If using SQLite, it also removes the timezone information in order to make
     the datetime comparable with datetimes in the database.
@@ -53,23 +53,23 @@
         )
     _dt = dt.astimezone(timezone.utc)
     if Inject(get_settings).DB_ENGINE == "sqlite":
         return _dt.replace(tzinfo=None)
     return _dt
 
 
-@router_admin.get("/project/", response_model=list[ProjectRead])
+@router_admin_v1.get("/project/", response_model=list[ProjectReadV1])
 async def view_project(
     id: Optional[int] = None,
     user_id: Optional[int] = None,
     timestamp_created_min: Optional[datetime] = None,
     timestamp_created_max: Optional[datetime] = None,
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_async_db),
-) -> list[ProjectRead]:
+) -> list[ProjectReadV1]:
     """
     Query `project` table.
 
     Args:
         id: If not `None`, select a given `project.id`.
         user_id: If not `None`, select a given `project.user_id`.
     """
@@ -91,25 +91,25 @@
     res = await db.execute(stm)
     project_list = res.scalars().all()
     await db.close()
 
     return project_list
 
 
-@router_admin.get("/workflow/", response_model=list[WorkflowRead])
+@router_admin_v1.get("/workflow/", response_model=list[WorkflowReadV1])
 async def view_workflow(
     id: Optional[int] = None,
     user_id: Optional[int] = None,
     project_id: Optional[int] = None,
     name_contains: Optional[str] = None,
     timestamp_created_min: Optional[datetime] = None,
     timestamp_created_max: Optional[datetime] = None,
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_async_db),
-) -> list[WorkflowRead]:
+) -> list[WorkflowReadV1]:
     """
     Query `workflow` table.
 
     Args:
         id: If not `None`, select a given `workflow.id`.
         project_id: If not `None`, select a given `workflow.project_id`.
         name_contains: If not `None`, select workflows such that their
@@ -140,26 +140,26 @@
     res = await db.execute(stm)
     workflow_list = res.scalars().all()
     await db.close()
 
     return workflow_list
 
 
-@router_admin.get("/dataset/", response_model=list[DatasetRead])
+@router_admin_v1.get("/dataset/", response_model=list[DatasetReadV1])
 async def view_dataset(
     id: Optional[int] = None,
     user_id: Optional[int] = None,
     project_id: Optional[int] = None,
     name_contains: Optional[str] = None,
     type: Optional[str] = None,
     timestamp_created_min: Optional[datetime] = None,
     timestamp_created_max: Optional[datetime] = None,
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_async_db),
-) -> list[DatasetRead]:
+) -> list[DatasetReadV1]:
     """
     Query `dataset` table.
 
     Args:
         id: If not `None`, select a given `dataset.id`.
         project_id: If not `None`, select a given `dataset.project_id`.
         name_contains: If not `None`, select datasets such that their
@@ -193,31 +193,31 @@
     res = await db.execute(stm)
     dataset_list = res.scalars().all()
     await db.close()
 
     return dataset_list
 
 
-@router_admin.get("/job/", response_model=list[ApplyWorkflowRead])
+@router_admin_v1.get("/job/", response_model=list[ApplyWorkflowReadV1])
 async def view_job(
     id: Optional[int] = None,
     user_id: Optional[int] = None,
     project_id: Optional[int] = None,
     input_dataset_id: Optional[int] = None,
     output_dataset_id: Optional[int] = None,
     workflow_id: Optional[int] = None,
-    status: Optional[JobStatusType] = None,
+    status: Optional[JobStatusTypeV1] = None,
     start_timestamp_min: Optional[datetime] = None,
     start_timestamp_max: Optional[datetime] = None,
     end_timestamp_min: Optional[datetime] = None,
     end_timestamp_max: Optional[datetime] = None,
     log: bool = True,
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_async_db),
-) -> list[ApplyWorkflowRead]:
+) -> list[ApplyWorkflowReadV1]:
     """
     Query `ApplyWorkflow` table.
 
     Args:
         id: If not `None`, select a given `applyworkflow.id`.
         project_id: If not `None`, select a given `applyworkflow.project_id`.
         input_dataset_id: If not `None`, select a given
@@ -274,78 +274,78 @@
     if not log:
         for job in job_list:
             setattr(job, "log", None)
 
     return job_list
 
 
-@router_admin.get("/job/{job_id}/", response_model=ApplyWorkflowRead)
+@router_admin_v1.get("/job/{job_id}/", response_model=ApplyWorkflowReadV1)
 async def view_single_job(
     job_id: int = None,
     show_tmp_logs: bool = False,
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_async_db),
-) -> ApplyWorkflowRead:
+) -> ApplyWorkflowReadV1:
 
     job = await db.get(ApplyWorkflow, job_id)
     if not job:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=f"Job {job_id} not found",
         )
     await db.close()
 
-    if show_tmp_logs and (job.status == JobStatusType.SUBMITTED):
+    if show_tmp_logs and (job.status == JobStatusTypeV1.SUBMITTED):
         try:
             with open(f"{job.working_dir}/{WORKFLOW_LOG_FILENAME}", "r") as f:
                 job.log = f.read()
         except FileNotFoundError:
             pass
 
     return job
 
 
-@router_admin.patch(
+@router_admin_v1.patch(
     "/job/{job_id}/",
-    response_model=ApplyWorkflowRead,
+    response_model=ApplyWorkflowReadV1,
 )
 async def update_job(
-    job_update: ApplyWorkflowUpdate,
+    job_update: ApplyWorkflowUpdateV1,
     job_id: int,
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[ApplyWorkflowRead]:
+) -> Optional[ApplyWorkflowReadV1]:
     """
     Change the status of an existing job.
 
     This endpoint is only open to superusers, and it does not apply
     project-based access-control to jobs.
     """
     job = await db.get(ApplyWorkflow, job_id)
     if job is None:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=f"Job {job_id} not found",
         )
 
-    if job_update.status != JobStatusType.FAILED:
+    if job_update.status != JobStatusTypeV1.FAILED:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=f"Cannot set job status to {job_update.status}",
         )
 
     setattr(job, "status", job_update.status)
     setattr(job, "end_timestamp", get_timestamp())
     await db.commit()
     await db.refresh(job)
     await db.close()
     return job
 
 
-@router_admin.get("/job/{job_id}/stop/", status_code=202)
+@router_admin_v1.get("/job/{job_id}/stop/", status_code=202)
 async def stop_job(
     job_id: int,
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_async_db),
 ) -> Response:
     """
     Stop execution of a workflow job.
@@ -363,15 +363,15 @@
         )
 
     _write_shutdown_file(job=job)
 
     return Response(status_code=status.HTTP_202_ACCEPTED)
 
 
-@router_admin.get(
+@router_admin_v1.get(
     "/job/{job_id}/download/",
     response_class=StreamingResponse,
 )
 async def download_job_logs(
     job_id: int,
     user: User = Depends(current_active_superuser),
     db: AsyncSession = Depends(get_async_db),
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/api/v1/_aux_functions.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/_aux_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from ....models import ApplyWorkflow
 from ....models import Dataset
 from ....models import LinkUserProject
 from ....models import Project
 from ....models import Task
 from ....models import Workflow
 from ....models import WorkflowTask
-from ....schemas import JobStatusType
+from ....schemas.v1 import JobStatusTypeV1
 from ....security import User
 
 
 async def _get_project_check_owner(
     *,
     project_id: int,
     user_id: int,
@@ -371,15 +371,15 @@
 def _get_submitted_jobs_statement() -> SelectOfScalar:
     """
     Returns:
         A sqlmodel statement that selects all `ApplyWorkflow`s with
         `ApplyWorkflow.status` equal to `submitted`.
     """
     stm = select(ApplyWorkflow).where(
-        ApplyWorkflow.status == JobStatusType.SUBMITTED
+        ApplyWorkflow.status == JobStatusTypeV1.SUBMITTED
     )
     return stm
 
 
 async def _workflow_insert_task(
     *,
     workflow_id: int,
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/api/v1/dataset.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from json.decoder import JSONDecodeError
 from pathlib import Path
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
@@ -12,46 +13,46 @@
 
 from ....db import AsyncSession
 from ....db import get_async_db
 from ....models import ApplyWorkflow
 from ....models import Dataset
 from ....models import Project
 from ....models import Resource
-from ....runner._common import HISTORY_FILENAME
-from ....schemas import DatasetCreate
-from ....schemas import DatasetRead
-from ....schemas import DatasetStatusRead
-from ....schemas import DatasetUpdate
-from ....schemas import ResourceCreate
-from ....schemas import ResourceRead
-from ....schemas import ResourceUpdate
-from ....schemas import WorkflowExport
-from ....schemas import WorkflowTaskExport
+from ....runner.filenames import HISTORY_FILENAME
+from ....schemas.v1 import DatasetCreateV1
+from ....schemas.v1 import DatasetReadV1
+from ....schemas.v1 import DatasetStatusReadV1
+from ....schemas.v1 import DatasetUpdateV1
+from ....schemas.v1 import ResourceCreateV1
+from ....schemas.v1 import ResourceReadV1
+from ....schemas.v1 import ResourceUpdateV1
+from ....schemas.v1 import WorkflowExportV1
+from ....schemas.v1 import WorkflowTaskExportV1
 from ....security import current_active_user
 from ....security import User
 from ._aux_functions import _get_dataset_check_owner
 from ._aux_functions import _get_project_check_owner
 from ._aux_functions import _get_submitted_jobs_statement
 from ._aux_functions import _get_workflow_check_owner
 
 
 router = APIRouter()
 
 
 @router.post(
     "/project/{project_id}/dataset/",
-    response_model=DatasetRead,
+    response_model=DatasetReadV1,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_dataset(
     project_id: int,
-    dataset: DatasetCreate,
+    dataset: DatasetCreateV1,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[DatasetRead]:
+) -> Optional[DatasetReadV1]:
     """
     Add new dataset to current project
     """
     await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     db_dataset = Dataset(project_id=project_id, **dataset.dict())
@@ -61,22 +62,22 @@
     await db.close()
 
     return db_dataset
 
 
 @router.get(
     "/project/{project_id}/dataset/",
-    response_model=list[DatasetRead],
+    response_model=list[DatasetReadV1],
 )
 async def read_dataset_list(
     project_id: int,
     history: bool = True,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[list[DatasetRead]]:
+) -> Optional[list[DatasetReadV1]]:
     """
     Get dataset list for given project
     """
     # Access control
     project = await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
@@ -92,22 +93,22 @@
         for ds in dataset_list:
             setattr(ds, "history", [])
     return dataset_list
 
 
 @router.get(
     "/project/{project_id}/dataset/{dataset_id}/",
-    response_model=DatasetRead,
+    response_model=DatasetReadV1,
 )
 async def read_dataset(
     project_id: int,
     dataset_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[DatasetRead]:
+) -> Optional[DatasetReadV1]:
     """
     Get info on a dataset associated to the current project
     """
     output = await _get_dataset_check_owner(
         project_id=project_id,
         dataset_id=dataset_id,
         user_id=user.id,
@@ -116,23 +117,23 @@
     dataset = output["dataset"]
     await db.close()
     return dataset
 
 
 @router.patch(
     "/project/{project_id}/dataset/{dataset_id}/",
-    response_model=DatasetRead,
+    response_model=DatasetReadV1,
 )
 async def update_dataset(
     project_id: int,
     dataset_id: int,
-    dataset_update: DatasetUpdate,
+    dataset_update: DatasetUpdateV1,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[DatasetRead]:
+) -> Optional[DatasetReadV1]:
     """
     Edit a dataset associated to the current project
     """
 
     if dataset_update.history is not None:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
@@ -225,24 +226,24 @@
     await db.commit()
 
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.post(
     "/project/{project_id}/dataset/{dataset_id}/resource/",
-    response_model=ResourceRead,
+    response_model=ResourceReadV1,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_resource(
     project_id: int,
     dataset_id: int,
-    resource: ResourceCreate,
+    resource: ResourceCreateV1,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[ResourceRead]:
+) -> Optional[ResourceReadV1]:
     """
     Add resource to an existing dataset
     """
     output = await _get_dataset_check_owner(
         project_id=project_id,
         dataset_id=dataset_id,
         user_id=user.id,
@@ -255,22 +256,22 @@
     await db.refresh(db_resource)
     await db.close()
     return db_resource
 
 
 @router.get(
     "/project/{project_id}/dataset/{dataset_id}/resource/",
-    response_model=list[ResourceRead],
+    response_model=list[ResourceReadV1],
 )
 async def get_resource_list(
     project_id: int,
     dataset_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[list[ResourceRead]]:
+) -> Optional[list[ResourceReadV1]]:
     """
     Get resources from a dataset
     """
     await _get_dataset_check_owner(
         project_id=project_id,
         dataset_id=dataset_id,
         user_id=user.id,
@@ -281,24 +282,24 @@
     resource_list = res.scalars().all()
     await db.close()
     return resource_list
 
 
 @router.patch(
     "/project/{project_id}/dataset/{dataset_id}/resource/{resource_id}/",
-    response_model=ResourceRead,
+    response_model=ResourceReadV1,
 )
 async def update_resource(
     project_id: int,
     dataset_id: int,
     resource_id: int,
-    resource_update: ResourceUpdate,
+    resource_update: ResourceUpdateV1,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[ResourceRead]:
+) -> Optional[ResourceReadV1]:
     """
     Edit a resource of a dataset
     """
     output = await _get_dataset_check_owner(
         project_id=project_id,
         dataset_id=dataset_id,
         user_id=user.id,
@@ -356,22 +357,22 @@
     await db.commit()
     await db.close()
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.get(
     "/project/{project_id}/dataset/{dataset_id}/export_history/",
-    response_model=WorkflowExport,
+    response_model=WorkflowExportV1,
 )
 async def export_history_as_workflow(
     project_id: int,
     dataset_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[WorkflowExport]:
+) -> Optional[WorkflowExportV1]:
     """
     Extract a reproducible workflow from the dataset history.
     """
     # Get the dataset DB entry
     output = await _get_dataset_check_owner(
         project_id=project_id,
         dataset_id=dataset_id,
@@ -408,38 +409,38 @@
 
     # Construct reproducible workflow
     task_list = []
     for history_item in history:
         wftask = history_item["workflowtask"]
         wftask_status = history_item["status"]
         if wftask_status == "done":
-            task_list.append(WorkflowTaskExport(**wftask))
+            task_list.append(WorkflowTaskExportV1(**wftask))
 
     def _slugify_dataset_name(_name: str) -> str:
         _new_name = _name
         for char in (" ", ".", "/", "\\"):
             _new_name = _new_name.replace(char, "_")
         return _new_name
 
     name = f"history_{_slugify_dataset_name(dataset.name)}"
 
-    workflow = WorkflowExport(name=name, task_list=task_list)
+    workflow = WorkflowExportV1(name=name, task_list=task_list)
     return workflow
 
 
 @router.get(
     "/project/{project_id}/dataset/{dataset_id}/status/",
-    response_model=DatasetStatusRead,
+    response_model=DatasetStatusReadV1,
 )
 async def get_workflowtask_status(
     project_id: int,
     dataset_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[DatasetStatusRead]:
+) -> Optional[DatasetStatusReadV1]:
     """
     Extract the status of all `WorkflowTask`s that ran on a given `Dataset`.
     """
     # Get the dataset DB entry
     output = await _get_dataset_check_owner(
         project_id=project_id,
         dataset_id=dataset_id,
@@ -507,29 +508,35 @@
         # WorkflowTask's that ran through successfully
         tmp_file = Path(running_job.working_dir) / HISTORY_FILENAME
         try:
             with tmp_file.open("r") as f:
                 history = json.load(f)
         except FileNotFoundError:
             history = []
+        except JSONDecodeError:
+            raise HTTPException(
+                status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                detail="History file does not include a valid JSON.",
+            )
+
         for history_item in history:
             wftask_id = history_item["workflowtask"]["id"]
             wftask_status = history_item["status"]
             workflow_tasks_status_dict[wftask_id] = wftask_status
 
-    response_body = DatasetStatusRead(status=workflow_tasks_status_dict)
+    response_body = DatasetStatusReadV1(status=workflow_tasks_status_dict)
     return response_body
 
 
-@router.get("/dataset/", response_model=list[DatasetRead])
+@router.get("/dataset/", response_model=list[DatasetReadV1])
 async def get_user_datasets(
     history: bool = True,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> list[DatasetRead]:
+) -> list[DatasetReadV1]:
     """
     Returns all the datasets of the current user
     """
     stm = select(Dataset)
     stm = stm.join(Project).where(Project.user_list.any(User.id == user.id))
     res = await db.execute(stm)
     dataset_list = res.scalars().all()
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/api/v1/job.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 from fastapi import status
 from fastapi.responses import StreamingResponse
 from sqlmodel import select
 
 from ....db import AsyncSession
 from ....db import get_async_db
 from ....models import ApplyWorkflow
-from ....models import JobStatusType
+from ....models import JobStatusTypeV1
 from ....models import Project
-from ....runner._common import WORKFLOW_LOG_FILENAME
-from ....schemas import ApplyWorkflowRead
+from ....runner.filenames import WORKFLOW_LOG_FILENAME
+from ....schemas.v1 import ApplyWorkflowReadV1
 from ....security import current_active_user
 from ....security import User
 from ...aux._job import _write_shutdown_file
 from ...aux._job import _zip_folder_to_byte_stream
 from ...aux._runner import _check_backend_is_slurm
 from ._aux_functions import _get_job_check_owner
 from ._aux_functions import _get_project_check_owner
 from ._aux_functions import _get_workflow_check_owner
 
 router = APIRouter()
 
 
-@router.get("/job/", response_model=list[ApplyWorkflowRead])
+@router.get("/job/", response_model=list[ApplyWorkflowReadV1])
 async def get_user_jobs(
     user: User = Depends(current_active_user),
     log: bool = True,
     db: AsyncSession = Depends(get_async_db),
-) -> list[ApplyWorkflowRead]:
+) -> list[ApplyWorkflowReadV1]:
     """
     Returns all the jobs of the current user
     """
     stm = select(ApplyWorkflow)
     stm = stm.join(Project).where(Project.user_list.any(User.id == user.id))
     res = await db.execute(stm)
     job_list = res.scalars().all()
@@ -46,59 +46,59 @@
             setattr(job, "log", None)
 
     return job_list
 
 
 @router.get(
     "/project/{project_id}/workflow/{workflow_id}/job/",
-    response_model=list[ApplyWorkflowRead],
+    response_model=list[ApplyWorkflowReadV1],
 )
 async def get_workflow_jobs(
     project_id: int,
     workflow_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[list[ApplyWorkflowRead]]:
+) -> Optional[list[ApplyWorkflowReadV1]]:
     """
     Returns all the jobs related to a specific workflow
     """
     await _get_workflow_check_owner(
         project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
     )
     stm = select(ApplyWorkflow).where(ApplyWorkflow.workflow_id == workflow_id)
     res = await db.execute(stm)
     job_list = res.scalars().all()
     return job_list
 
 
 @router.get(
     "/project/{project_id}/job/{job_id}/",
-    response_model=ApplyWorkflowRead,
+    response_model=ApplyWorkflowReadV1,
 )
 async def read_job(
     project_id: int,
     job_id: int,
     show_tmp_logs: bool = False,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[ApplyWorkflowRead]:
+) -> Optional[ApplyWorkflowReadV1]:
     """
     Return info on an existing job
     """
 
     output = await _get_job_check_owner(
         project_id=project_id,
         job_id=job_id,
         user_id=user.id,
         db=db,
     )
     job = output["job"]
     await db.close()
 
-    if show_tmp_logs and (job.status == JobStatusType.SUBMITTED):
+    if show_tmp_logs and (job.status == JobStatusTypeV1.SUBMITTED):
         try:
             with open(f"{job.working_dir}/{WORKFLOW_LOG_FILENAME}", "r") as f:
                 job.log = f.read()
         except FileNotFoundError:
             pass
 
     return job
@@ -136,22 +136,22 @@
         media_type="application/x-zip-compressed",
         headers={"Content-Disposition": f"attachment;filename={zip_filename}"},
     )
 
 
 @router.get(
     "/project/{project_id}/job/",
-    response_model=list[ApplyWorkflowRead],
+    response_model=list[ApplyWorkflowReadV1],
 )
 async def get_job_list(
     project_id: int,
     user: User = Depends(current_active_user),
     log: bool = True,
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[list[ApplyWorkflowRead]]:
+) -> Optional[list[ApplyWorkflowReadV1]]:
     """
     Get job list for given project
     """
     project = await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/api/v1/project.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 from ....db import AsyncSession
 from ....db import get_async_db
 from ....models import ApplyWorkflow
 from ....models import Dataset
 from ....models import LinkUserProject
 from ....models import Project
 from ....models import Workflow
-from ....runner import submit_workflow
-from ....runner import validate_workflow_compatibility
-from ....runner.common import set_start_and_last_task_index
-from ....schemas import ApplyWorkflowCreate
-from ....schemas import ApplyWorkflowRead
-from ....schemas import JobStatusType
-from ....schemas import ProjectCreate
-from ....schemas import ProjectRead
-from ....schemas import ProjectUpdate
+from ....runner.set_start_and_last_task_index import (
+    set_start_and_last_task_index,
+)
+from ....runner.v1 import submit_workflow
+from ....runner.v1 import validate_workflow_compatibility
+from ....schemas.v1 import ApplyWorkflowCreateV1
+from ....schemas.v1 import ApplyWorkflowReadV1
+from ....schemas.v1 import JobStatusTypeV1
+from ....schemas.v1 import ProjectCreateV1
+from ....schemas.v1 import ProjectReadV1
+from ....schemas.v1 import ProjectUpdateV1
 from ....security import current_active_user
 from ....security import current_active_verified_user
 from ....security import User
 from ._aux_functions import _check_project_exists
 from ._aux_functions import _get_dataset_check_owner
 from ._aux_functions import _get_project_check_owner
 from ._aux_functions import _get_submitted_jobs_statement
@@ -44,15 +46,15 @@
 router = APIRouter()
 
 
 def _encode_as_utc(dt: datetime):
     return dt.replace(tzinfo=timezone.utc).isoformat()
 
 
-@router.get("/", response_model=list[ProjectRead])
+@router.get("/", response_model=list[ProjectReadV1])
 async def get_list_project(
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
 ) -> list[Project]:
     """
     Return list of projects user is member of
     """
@@ -63,20 +65,20 @@
     )
     res = await db.execute(stm)
     project_list = res.scalars().all()
     await db.close()
     return project_list
 
 
-@router.post("/", response_model=ProjectRead, status_code=201)
+@router.post("/", response_model=ProjectReadV1, status_code=201)
 async def create_project(
-    project: ProjectCreate,
+    project: ProjectCreateV1,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[ProjectRead]:
+) -> Optional[ProjectReadV1]:
     """
     Create new poject
     """
 
     # Check that there is no project with the same user and name
     await _check_project_exists(
         project_name=project.name, user_id=user.id, db=db
@@ -98,34 +100,34 @@
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=str(e),
         )
 
     return db_project
 
 
-@router.get("/{project_id}/", response_model=ProjectRead)
+@router.get("/{project_id}/", response_model=ProjectReadV1)
 async def read_project(
     project_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[ProjectRead]:
+) -> Optional[ProjectReadV1]:
     """
     Return info on an existing project
     """
     project = await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     await db.close()
     return project
 
 
-@router.patch("/{project_id}/", response_model=ProjectRead)
+@router.patch("/{project_id}/", response_model=ProjectReadV1)
 async def update_project(
     project_id: int,
-    project_update: ProjectUpdate,
+    project_update: ProjectUpdateV1,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
 ):
     project = await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
 
@@ -237,26 +239,26 @@
 
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.post(
     "/{project_id}/workflow/{workflow_id}/apply/",
     status_code=status.HTTP_202_ACCEPTED,
-    response_model=ApplyWorkflowRead,
+    response_model=ApplyWorkflowReadV1,
 )
 async def apply_workflow(
     project_id: int,
     workflow_id: int,
-    apply_workflow: ApplyWorkflowCreate,
+    apply_workflow: ApplyWorkflowCreateV1,
     background_tasks: BackgroundTasks,
     input_dataset_id: int,
     output_dataset_id: int,
     user: User = Depends(current_active_verified_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[ApplyWorkflowRead]:
+) -> Optional[ApplyWorkflowReadV1]:
 
     output = await _get_dataset_check_owner(
         project_id=project_id,
         dataset_id=input_dataset_id,
         user_id=user.id,
         db=db,
     )
@@ -358,15 +360,15 @@
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e)
         )
 
     # Check that no other job with the same output_dataset_id is SUBMITTED
     stm = (
         select(ApplyWorkflow)
         .where(ApplyWorkflow.output_dataset_id == output_dataset_id)
-        .where(ApplyWorkflow.status == JobStatusType.SUBMITTED)
+        .where(ApplyWorkflow.status == JobStatusTypeV1.SUBMITTED)
     )
     res = await db.execute(stm)
     if res.scalars().all():
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=(
                 f"Output dataset {output_dataset_id} is already in use "
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/api/v1/task.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,72 +9,73 @@
 from sqlmodel import select
 
 from .....logger import set_logger
 from ....db import AsyncSession
 from ....db import get_async_db
 from ....models import Task
 from ....models import WorkflowTask
-from ....schemas import TaskCreate
-from ....schemas import TaskRead
-from ....schemas import TaskUpdate
+from ....models.v2 import TaskV2
+from ....schemas.v1 import TaskCreateV1
+from ....schemas.v1 import TaskReadV1
+from ....schemas.v1 import TaskUpdateV1
 from ....security import current_active_user
 from ....security import current_active_verified_user
 from ....security import User
 from ._aux_functions import _get_task_check_owner
 
 router = APIRouter()
 
 logger = set_logger(__name__)
 
 
-@router.get("/", response_model=list[TaskRead])
+@router.get("/", response_model=list[TaskReadV1])
 async def get_list_task(
     user: User = Depends(current_active_user),
     args_schema: bool = True,
     db: AsyncSession = Depends(get_async_db),
-) -> list[TaskRead]:
+) -> list[TaskReadV1]:
     """
     Get list of available tasks
     """
     stm = select(Task)
     res = await db.execute(stm)
     task_list = res.scalars().all()
     await db.close()
     if not args_schema:
         for task in task_list:
             setattr(task, "args_schema", None)
 
     return task_list
 
 
-@router.get("/{task_id}/", response_model=TaskRead)
+@router.get("/{task_id}/", response_model=TaskReadV1)
 async def get_task(
     task_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> TaskRead:
+) -> TaskReadV1:
     """
     Get info on a specific task
     """
     task = await db.get(Task, task_id)
     await db.close()
     if not task:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND, detail="Task not found"
         )
     return task
 
 
-@router.patch("/{task_id}/", response_model=TaskRead)
+@router.patch("/{task_id}/", response_model=TaskReadV1)
 async def patch_task(
     task_id: int,
-    task_update: TaskUpdate,
+    task_update: TaskUpdateV1,
     user: User = Depends(current_active_verified_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[TaskRead]:
+) -> Optional[TaskReadV1]:
     """
     Edit a specific task (restricted to superusers and task owner)
     """
 
     if task_update.source:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
@@ -105,20 +106,22 @@
 
     await db.commit()
     await db.refresh(db_task)
     await db.close()
     return db_task
 
 
-@router.post("/", response_model=TaskRead, status_code=status.HTTP_201_CREATED)
+@router.post(
+    "/", response_model=TaskReadV1, status_code=status.HTTP_201_CREATED
+)
 async def create_task(
-    task: TaskCreate,
+    task: TaskCreateV1,
     user: User = Depends(current_active_verified_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[TaskRead]:
+) -> Optional[TaskReadV1]:
     """
     Create a new task
     """
     # Set task.owner attribute
     if user.username:
         owner = user.username
     elif user.slurm_user:
@@ -139,15 +142,22 @@
     # to provide a user-friendly error message, but `task.source` uniqueness is
     # already guaranteed by a constraint in the table definition).
     stm = select(Task).where(Task.source == task.source)
     res = await db.execute(stm)
     if res.scalars().all():
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail=f'Task source "{task.source}" already in use',
+            detail=f"Source '{task.source}' already used by some TaskV1",
+        )
+    stm = select(TaskV2).where(TaskV2.source == task.source)
+    res = await db.execute(stm)
+    if res.scalars().all():
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=f"Source '{task.source}' already used by some TaskV2",
         )
 
     # Add task
     db_task = Task(**task.dict(), owner=owner)
     db.add(db_task)
     await db.commit()
     await db.refresh(db_task)
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/api/v1/task_collection.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/task_collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 from pydantic.error_wrappers import ValidationError
 from sqlmodel import select
 
 from .....config import get_settings
 from .....logger import close_logger
 from .....logger import set_logger
 from .....syringe import Inject
-from .....tasks._TaskCollectPip import _TaskCollectPip
-from .....tasks.background_operations import background_collect_pip
-from .....tasks.endpoint_operations import create_package_dir_pip
-from .....tasks.endpoint_operations import download_package
-from .....tasks.endpoint_operations import get_collection_data
-from .....tasks.endpoint_operations import inspect_package
-from .....tasks.utils import get_collection_log
-from .....tasks.utils import slugify_task_name
 from ....db import AsyncSession
 from ....db import get_async_db
 from ....models import State
-from ....models import Task
+from ....models.v2 import TaskV2
 from ....schemas import StateRead
-from ....schemas import TaskCollectPip
-from ....schemas import TaskCollectStatus
+from ....schemas.v2 import TaskCollectPipV2
+from ....schemas.v2 import TaskCollectStatusV2
 from ....security import current_active_user
 from ....security import current_active_verified_user
 from ....security import User
+from fractal_server.tasks.endpoint_operations import create_package_dir_pip
+from fractal_server.tasks.endpoint_operations import download_package
+from fractal_server.tasks.endpoint_operations import inspect_package
+from fractal_server.tasks.utils import get_collection_log
+from fractal_server.tasks.utils import slugify_task_name
+from fractal_server.tasks.v2._TaskCollectPip import _TaskCollectPip
+from fractal_server.tasks.v2.background_operations import (
+    background_collect_pip,
+)
+from fractal_server.tasks.v2.get_collection_data import get_collection_data
 
 router = APIRouter()
 
 logger = set_logger(__name__)
 
 
 @router.post(
@@ -53,15 +55,15 @@
                 "Package already collected. Returning info on already "
                 "available tasks"
             )
         ),
     },
 )
 async def collect_tasks_pip(
-    task_collect: TaskCollectPip,
+    task_collect: TaskCollectPipV2,
     background_tasks: BackgroundTasks,
     response: Response,
     user: User = Depends(current_active_verified_user),
     db: AsyncSession = Depends(get_async_db),
 ) -> StateRead:  # State[TaskCollectStatus]
     """
     Task collection endpoint
@@ -108,15 +110,15 @@
     try:
         venv_path = create_package_dir_pip(task_pkg=task_pkg)
     except FileExistsError:
         venv_path = create_package_dir_pip(task_pkg=task_pkg, create=False)
         try:
             task_collect_status = get_collection_data(venv_path)
             for task in task_collect_status.task_list:
-                db_task = await db.get(Task, task.id)
+                db_task = await db.get(TaskV2, task.id)
                 if (
                     (not db_task)
                     or db_task.source != task.source
                     or db_task.name != task.name
                 ):
                     await db.close()
                     raise HTTPException(
@@ -145,28 +147,28 @@
         return state
     settings = Inject(get_settings)
 
     # Check that tasks are not already in the DB
     for new_task in task_pkg.package_manifest.task_list:
         new_task_name_slug = slugify_task_name(new_task.name)
         new_task_source = f"{task_pkg.package_source}:{new_task_name_slug}"
-        stm = select(Task).where(Task.source == new_task_source)
+        stm = select(TaskV2).where(TaskV2.source == new_task_source)
         res = await db.execute(stm)
         if res.scalars().all():
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=(
                     "Cannot collect package. Task with source "
                     f'"{new_task_source}" already exists in the database.'
                 ),
             )
 
     # All checks are OK, proceed with task collection
     full_venv_path = venv_path.relative_to(settings.FRACTAL_TASKS_DIR)
-    collection_status = TaskCollectStatus(
+    collection_status = TaskCollectStatusV2(
         status="pending", venv_path=full_venv_path, package=task_pkg.package
     )
 
     # Create State object (after casting venv_path to string)
     collection_status_dict = collection_status.dict()
     collection_status_dict["venv_path"] = str(collection_status.venv_path)
     state = State(data=collection_status_dict)
@@ -188,14 +190,15 @@
     info = (
         "Collecting tasks in the background. "
         f"GET /task/collect/{state.id} to query collection status"
     )
     state.data["info"] = info
     response.status_code = status.HTTP_201_CREATED
     await db.close()
+
     return state
 
 
 @router.get("/collect/{state_id}/", response_model=StateRead)
 async def check_collection_status(
     state_id: int,
     user: User = Depends(current_active_user),
@@ -210,15 +213,15 @@
     state = await db.get(State, state_id)
     if not state:
         await db.close()
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=f"No task collection info with id={state_id}",
         )
-    data = TaskCollectStatus(**state.data)
+    data = TaskCollectStatusV2(**state.data)
 
     # In some cases (i.e. a successful or ongoing task collection), data.log is
     # not set; if so, we collect the current logs
     if verbose and not data.log:
         data.log = get_collection_log(data.venv_path)
         state.data = data.sanitised_dict()
     close_logger(logger)
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/api/v1/workflow.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/api/v2/workflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,147 +1,141 @@
-# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
-# University of Zurich
-#
-# Original author(s):
-# Jacopo Nespolo <jacopo.nespolo@exact-lab.it>
-# Marco Franzon <marco.franzon@exact-lab.it>
-# Tommaso Comparin <tommaso.comparin@exact-lab.it>
-#
-# This file is part of Fractal and was originally developed by eXact lab S.r.l.
-# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
-# Institute for Biomedical Research and Pelkmans Lab from the University of
-# Zurich.
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 from sqlmodel import select
 
 from .....logger import close_logger
 from .....logger import set_logger
 from ....db import AsyncSession
 from ....db import get_async_db
-from ....models import ApplyWorkflow
-from ....models import Project
-from ....models import Task
-from ....models import Workflow
-from ....schemas import WorkflowCreate
-from ....schemas import WorkflowExport
-from ....schemas import WorkflowImport
-from ....schemas import WorkflowRead
-from ....schemas import WorkflowTaskCreate
-from ....schemas import WorkflowUpdate
+from ....models.v1 import Task as TaskV1
+from ....models.v2 import JobV2
+from ....models.v2 import ProjectV2
+from ....models.v2 import TaskV2
+from ....models.v2 import WorkflowV2
+from ....schemas.v1 import WorkflowTaskCreateV1
+from ....schemas.v2 import WorkflowCreateV2
+from ....schemas.v2 import WorkflowExportV2
+from ....schemas.v2 import WorkflowImportV2
+from ....schemas.v2 import WorkflowReadV2
+from ....schemas.v2 import WorkflowTaskCreateV2
+from ....schemas.v2 import WorkflowUpdateV2
 from ....security import current_active_user
 from ....security import User
 from ._aux_functions import _check_workflow_exists
 from ._aux_functions import _get_project_check_owner
 from ._aux_functions import _get_submitted_jobs_statement
 from ._aux_functions import _get_workflow_check_owner
 from ._aux_functions import _workflow_insert_task
 
 
 router = APIRouter()
 
 
 @router.get(
     "/project/{project_id}/workflow/",
-    response_model=list[WorkflowRead],
+    response_model=list[WorkflowReadV2],
 )
 async def get_workflow_list(
     project_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[list[WorkflowRead]]:
+) -> Optional[list[WorkflowReadV2]]:
     """
     Get workflow list for given project
     """
     # Access control
     project = await _get_project_check_owner(
         project_id=project_id, user_id=user.id, db=db
     )
     # Find workflows of the current project. Note: this select/where approach
     # has much better scaling than refreshing all elements of
     # `project.workflow_list` - ref
     # https://github.com/fractal-analytics-platform/fractal-server/pull/1082#issuecomment-1856676097.
-    stm = select(Workflow).where(Workflow.project_id == project.id)
+    stm = select(WorkflowV2).where(WorkflowV2.project_id == project.id)
     workflow_list = (await db.execute(stm)).scalars().all()
     return workflow_list
 
 
 @router.post(
     "/project/{project_id}/workflow/",
-    response_model=WorkflowRead,
+    response_model=WorkflowReadV2,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_workflow(
     project_id: int,
-    workflow: WorkflowCreate,
+    workflow: WorkflowCreateV2,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[WorkflowRead]:
+) -> Optional[WorkflowReadV2]:
     """
     Create a workflow, associate to a project
     """
     await _get_project_check_owner(
-        project_id=project_id,
-        user_id=user.id,
-        db=db,
+        project_id=project_id, user_id=user.id, db=db
     )
     await _check_workflow_exists(
         name=workflow.name, project_id=project_id, db=db
     )
 
-    db_workflow = Workflow(project_id=project_id, **workflow.dict())
+    db_workflow = WorkflowV2(project_id=project_id, **workflow.dict())
     db.add(db_workflow)
     await db.commit()
     await db.refresh(db_workflow)
     await db.close()
     return db_workflow
 
 
 @router.get(
     "/project/{project_id}/workflow/{workflow_id}/",
-    response_model=WorkflowRead,
+    response_model=WorkflowReadV2,
 )
 async def read_workflow(
     project_id: int,
     workflow_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[WorkflowRead]:
+) -> Optional[WorkflowReadV2]:
     """
     Get info on an existing workflow
     """
 
     workflow = await _get_workflow_check_owner(
-        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
+        project_id=project_id,
+        workflow_id=workflow_id,
+        user_id=user.id,
+        db=db,
     )
 
     return workflow
 
 
 @router.patch(
     "/project/{project_id}/workflow/{workflow_id}/",
-    response_model=WorkflowRead,
+    response_model=WorkflowReadV2,
 )
 async def update_workflow(
     project_id: int,
     workflow_id: int,
-    patch: WorkflowUpdate,
+    patch: WorkflowUpdateV2,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[WorkflowRead]:
+) -> Optional[WorkflowReadV2]:
     """
     Edit a workflow
     """
     workflow = await _get_workflow_check_owner(
-        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
+        project_id=project_id,
+        workflow_id=workflow_id,
+        user_id=user.id,
+        db=db,
     )
 
     if patch.name:
         await _check_workflow_exists(
             name=patch.name, project_id=project_id, db=db
         )
 
@@ -185,21 +179,24 @@
     db: AsyncSession = Depends(get_async_db),
 ) -> Response:
     """
     Delete a workflow
     """
 
     workflow = await _get_workflow_check_owner(
-        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
+        project_id=project_id,
+        workflow_id=workflow_id,
+        user_id=user.id,
+        db=db,
     )
 
     # Fail if there exist jobs that are submitted and in relation with the
     # current workflow.
     stm = _get_submitted_jobs_statement().where(
-        ApplyWorkflow.workflow_id == workflow.id
+        JobV2.workflow_id == workflow.id
     )
     res = await db.execute(stm)
     jobs = res.scalars().all()
     if jobs:
         string_ids = str([job.id for job in jobs])[1:-1]
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
@@ -207,15 +204,15 @@
                 f"Cannot delete workflow {workflow.id} because it "
                 f"is linked to active job(s) {string_ids}."
             ),
         )
 
     # Cascade operations: set foreign-keys to null for jobs which are in
     # relationship with the current workflow
-    stm = select(ApplyWorkflow).where(ApplyWorkflow.workflow_id == workflow_id)
+    stm = select(JobV2).where(JobV2.workflow_id == workflow_id)
     res = await db.execute(stm)
     jobs = res.scalars().all()
     for job in jobs:
         job.workflow_id = None
         await db.merge(job)
     await db.commit()
 
@@ -224,55 +221,68 @@
     await db.commit()
 
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.get(
     "/project/{project_id}/workflow/{workflow_id}/export/",
-    response_model=WorkflowExport,
+    response_model=WorkflowExportV2,
 )
 async def export_worfklow(
     project_id: int,
     workflow_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[WorkflowExport]:
+) -> Optional[WorkflowExportV2]:
     """
     Export an existing workflow, after stripping all IDs
     """
     workflow = await _get_workflow_check_owner(
-        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
+        project_id=project_id,
+        workflow_id=workflow_id,
+        user_id=user.id,
+        db=db,
     )
     # Emit a warning when exporting a workflow with custom tasks
     logger = set_logger(None)
     for wftask in workflow.task_list:
-        if wftask.task.owner is not None:
-            logger.warning(
-                f"Custom tasks (like the one with id={wftask.task.id} and "
-                f'source="{wftask.task.source}") are not meant to be '
-                "portable; re-importing this workflow may not work as "
-                "expected."
-            )
+        if wftask.is_legacy_task:
+            if wftask.task_legacy.owner is not None:
+                logger.warning(
+                    f"Custom tasks (like the one with "
+                    f"id={wftask.task_legacy_id} and "
+                    f"source='{wftask.task_legacy.source}') are not meant to "
+                    "be portable; re-importing this workflow may not work as "
+                    "expected."
+                )
+        else:
+            if wftask.task.owner is not None:
+                logger.warning(
+                    f"Custom tasks (like the one with id={wftask.task_id} and "
+                    f'source="{wftask.task.source}") are not meant to be '
+                    "portable; re-importing this workflow may not work as "
+                    "expected."
+                )
     close_logger(logger)
 
     await db.close()
     return workflow
 
 
 @router.post(
     "/project/{project_id}/workflow/import/",
-    response_model=WorkflowRead,
+    response_model=WorkflowReadV2,
     status_code=status.HTTP_201_CREATED,
 )
 async def import_workflow(
     project_id: int,
-    workflow: WorkflowImport,
+    workflow: WorkflowImportV2,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[WorkflowRead]:
+) -> Optional[WorkflowReadV2]:
     """
     Import an existing workflow into a project
 
     Also create all required objects (i.e. Workflow and WorkflowTask's) along
     the way.
     """
 
@@ -284,67 +294,105 @@
     )
 
     await _check_workflow_exists(
         name=workflow.name, project_id=project_id, db=db
     )
 
     # Check that all required tasks are available
-    tasks = [wf_task.task for wf_task in workflow.task_list]
     source_to_id = {}
-    for task in tasks:
-        source = task.source
-        if source not in source_to_id.keys():
-            stm = select(Task).where(Task.source == source)
-            tasks_by_source = (await db.execute(stm)).scalars().all()
-            if len(tasks_by_source) != 1:
-                raise HTTPException(
-                    status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                    detail=(
-                        f"Found {len(tasks_by_source)} tasks with {source=}."
-                    ),
-                )
-            source_to_id[source] = tasks_by_source[0].id
+    source_to_id_legacy = {}
+
+    for wf_task in workflow.task_list:
+
+        if wf_task.is_legacy_task is True:
+            source = wf_task.task_legacy.source
+            if source not in source_to_id_legacy.keys():
+                stm = select(TaskV1).where(TaskV1.source == source)
+                tasks_by_source = (await db.execute(stm)).scalars().all()
+                if len(tasks_by_source) != 1:
+                    raise HTTPException(
+                        status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                        detail=(
+                            f"Found {len(tasks_by_source)} tasks legacy "
+                            f"with {source=}."
+                        ),
+                    )
+                source_to_id_legacy[source] = tasks_by_source[0].id
+        else:
+            source = wf_task.task.source
+            if source not in source_to_id.keys():
+                stm = select(TaskV2).where(TaskV2.source == source)
+                tasks_by_source = (await db.execute(stm)).scalars().all()
+                if len(tasks_by_source) != 1:
+                    raise HTTPException(
+                        status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                        detail=(
+                            f"Found {len(tasks_by_source)} tasks "
+                            f"with {source=}."
+                        ),
+                    )
+                source_to_id[source] = tasks_by_source[0].id
 
     # Create new Workflow (with empty task_list)
-    db_workflow = Workflow(
+    db_workflow = WorkflowV2(
         project_id=project_id,
         **workflow.dict(exclude_none=True, exclude={"task_list"}),
     )
     db.add(db_workflow)
     await db.commit()
     await db.refresh(db_workflow)
 
     # Insert tasks
-    async with db:
-        for _, wf_task in enumerate(workflow.task_list):
-            # Identify task_id
-            source = wf_task.task.source
-            task_id = source_to_id[source]
-            # Prepare new_wf_task
-            new_wf_task = WorkflowTaskCreate(
-                **wf_task.dict(exclude_none=True),
-            )
-            # Insert task
-            await _workflow_insert_task(
-                **new_wf_task.dict(),
-                workflow_id=db_workflow.id,
-                task_id=task_id,
-                db=db,
-            )
+    async with db:  # FIXME why?
+
+        for wf_task in workflow.task_list:
+            if wf_task.is_legacy_task is True:
+                # Identify task_id
+                source = wf_task.task_legacy.source
+                task_id = source_to_id_legacy[source]
+                # Prepare new_wf_task
+                new_wf_task = WorkflowTaskCreateV1(
+                    **wf_task.dict(exclude_none=True)
+                )
+                # Insert task
+                await _workflow_insert_task(
+                    **new_wf_task.dict(),
+                    is_legacy_task=True,
+                    workflow_id=db_workflow.id,
+                    task_id=task_id,
+                    db=db,
+                )
+            else:
+                # Identify task_id
+                source = wf_task.task.source
+                task_id = source_to_id[source]
+                # Prepare new_wf_task
+                new_wf_task = WorkflowTaskCreateV2(
+                    **wf_task.dict(exclude_none=True)
+                )
+                # Insert task
+                await _workflow_insert_task(
+                    **new_wf_task.dict(),
+                    workflow_id=db_workflow.id,
+                    task_id=task_id,
+                    db=db,
+                )
 
     await db.close()
     return db_workflow
 
 
-@router.get("/workflow/", response_model=list[WorkflowRead])
+@router.get("/workflow/", response_model=list[WorkflowReadV2])
 async def get_user_workflows(
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> list[WorkflowRead]:
+) -> list[WorkflowReadV2]:
     """
     Returns all the workflows of the current user
     """
-    stm = select(Workflow)
-    stm = stm.join(Project).where(Project.user_list.any(User.id == user.id))
+    stm = select(WorkflowV2)
+    stm = stm.join(ProjectV2).where(
+        ProjectV2.user_list.any(User.id == user.id)
+    )
     res = await db.execute(stm)
     workflow_list = res.scalars().all()
     return workflow_list
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/api/v1/workflowtask.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/api/v1/workflowtask.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,39 +19,39 @@
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 
 from ....db import AsyncSession
 from ....db import get_async_db
 from ....models import Task
-from ....schemas import WorkflowTaskCreate
-from ....schemas import WorkflowTaskRead
-from ....schemas import WorkflowTaskUpdate
+from ....schemas.v1 import WorkflowTaskCreateV1
+from ....schemas.v1 import WorkflowTaskReadV1
+from ....schemas.v1 import WorkflowTaskUpdateV1
 from ....security import current_active_user
 from ....security import User
 from ._aux_functions import _get_workflow_check_owner
 from ._aux_functions import _get_workflow_task_check_owner
 from ._aux_functions import _workflow_insert_task
 
 router = APIRouter()
 
 
 @router.post(
     "/project/{project_id}/workflow/{workflow_id}/wftask/",
-    response_model=WorkflowTaskRead,
+    response_model=WorkflowTaskReadV1,
     status_code=status.HTTP_201_CREATED,
 )
 async def create_workflowtask(
     project_id: int,
     workflow_id: int,
     task_id: int,
-    new_task: WorkflowTaskCreate,
+    new_task: WorkflowTaskCreateV1,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[WorkflowTaskRead]:
+) -> Optional[WorkflowTaskReadV1]:
     """
     Add a WorkflowTask to a Workflow
     """
 
     workflow = await _get_workflow_check_owner(
         project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
     )
@@ -74,15 +74,15 @@
 
     await db.close()
     return workflow_task
 
 
 @router.get(
     "/project/{project_id}/workflow/{workflow_id}/wftask/{workflow_task_id}/",
-    response_model=WorkflowTaskRead,
+    response_model=WorkflowTaskReadV1,
 )
 async def read_workflowtask(
     project_id: int,
     workflow_id: int,
     workflow_task_id: int,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
@@ -95,24 +95,24 @@
         db=db,
     )
     return workflow_task
 
 
 @router.patch(
     "/project/{project_id}/workflow/{workflow_id}/wftask/{workflow_task_id}/",
-    response_model=WorkflowTaskRead,
+    response_model=WorkflowTaskReadV1,
 )
 async def update_workflowtask(
     project_id: int,
     workflow_id: int,
     workflow_task_id: int,
-    workflow_task_update: WorkflowTaskUpdate,
+    workflow_task_update: WorkflowTaskUpdateV1,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
-) -> Optional[WorkflowTaskRead]:
+) -> Optional[WorkflowTaskReadV1]:
     """
     Edit a WorkflowTask of a Workflow
     """
 
     db_workflow_task, db_workflow = await _get_workflow_task_check_owner(
         project_id=project_id,
         workflow_task_id=workflow_task_id,
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/auth.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/auth.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/aux/_job.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/aux/_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from io import BytesIO
 from pathlib import Path
 from zipfile import ZIP_DEFLATED
 from zipfile import ZipFile
 
 from ...models import ApplyWorkflow
-from ...runner._common import SHUTDOWN_FILENAME
+from ...runner.filenames import SHUTDOWN_FILENAME
 
 
 def _write_shutdown_file(*, job: ApplyWorkflow):
     """
     Write job's shutdown file.
 
     Args:
```

### Comparing `fractal_server-1.4.9/fractal_server/app/routes/aux/_runner.py` & `fractal_server-2.0.0a0/fractal_server/app/routes/aux/_runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/__init__.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/v1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,60 +18,39 @@
 individual backends.
 """
 import os
 import traceback
 from pathlib import Path
 from typing import Optional
 
-from ... import __VERSION__
-from ...config import get_settings
-from ...logger import set_logger
-from ...syringe import Inject
-from ...utils import get_timestamp
-from ..db import DB
-from ..models import ApplyWorkflow
-from ..models import Dataset
-from ..models import Workflow
-from ..models import WorkflowTask
-from ..schemas import JobStatusType
-from ._common import WORKFLOW_LOG_FILENAME
-from ._local import process_workflow as local_process_workflow
+from ....logger import set_logger
+from ....syringe import Inject
+from ....utils import get_timestamp
+from ...db import DB
+from ...models import ApplyWorkflow
+from ...models import Dataset
+from ...models import Workflow
+from ...models import WorkflowTask
+from ...schemas.v1 import JobStatusTypeV1
+from ..exceptions import JobExecutionError
+from ..exceptions import TaskExecutionError
+from ..filenames import WORKFLOW_LOG_FILENAME
+from ..v1._local import process_workflow as local_process_workflow
+from ..v1._slurm import process_workflow as slurm_process_workflow
 from .common import close_job_logger
-from .common import JobExecutionError
-from .common import TaskExecutionError
 from .common import validate_workflow_compatibility  # noqa: F401
 from .handle_failed_job import assemble_history_failed_job
 from .handle_failed_job import assemble_meta_failed_job
+from fractal_server import __VERSION__
+from fractal_server.config import get_settings
 
 
 _backends = {}
-_backend_errors: dict[str, Exception] = {}
 _backends["local"] = local_process_workflow
-
-try:
-    from ._slurm import process_workflow as slurm_process_workflow
-
-    _backends["slurm"] = slurm_process_workflow
-except ModuleNotFoundError as e:
-    _backend_errors["slurm"] = e
-
-
-def get_process_workflow():
-    settings = Inject(get_settings)
-    try:
-        process_workflow = _backends[settings.FRACTAL_RUNNER_BACKEND]
-    except KeyError:
-        raise _backend_errors.get(
-            settings.FRACTAL_RUNNER_BACKEND,
-            RuntimeError(
-                "Unknown error during collection of backend "
-                f"`{settings.FRACTAL_RUNNER_BACKEND}`"
-            ),
-        )
-    return process_workflow
+_backends["slurm"] = slurm_process_workflow
 
 
 async def submit_workflow(
     *,
     workflow_id: int,
     input_dataset_id: int,
     output_dataset_id: int,
@@ -103,14 +82,25 @@
             Cache directory (namely a path where the user can write); for the
             slurm backend, this is used as a base directory for
             `job.working_dir_user`.
         slurm_user:
             The username to impersonate for the workflow execution, for the
             slurm backend.
     """
+
+    # Declare runner backend and set `process_workflow` function
+    settings = Inject(get_settings)
+    FRACTAL_RUNNER_BACKEND = settings.FRACTAL_RUNNER_BACKEND
+    if FRACTAL_RUNNER_BACKEND == "local":
+        process_workflow = local_process_workflow
+    elif FRACTAL_RUNNER_BACKEND == "slurm":
+        process_workflow = slurm_process_workflow
+    else:
+        raise RuntimeError(f"Invalid runner backend {FRACTAL_RUNNER_BACKEND=}")
+
     with next(DB.get_sync_db()) as db_sync:
 
         job: ApplyWorkflow = db_sync.get(ApplyWorkflow, job_id)
         if not job:
             raise ValueError(f"Cannot fetch job {job_id} from database")
 
         input_dataset: Dataset = db_sync.get(Dataset, input_dataset_id)
@@ -128,27 +118,22 @@
                     f"Cannot fetch output_dataset {output_dataset_id} "
                     "from database\n"
                 )
             if not workflow:
                 log_msg += (
                     f"Cannot fetch workflow {workflow_id} from database\n"
                 )
-            job.status = JobStatusType.FAILED
+            job.status = JobStatusTypeV1.FAILED
             job.end_timestamp = get_timestamp()
             job.log = log_msg
             db_sync.merge(job)
             db_sync.commit()
             db_sync.close()
             return
 
-        # Select backend
-        settings = Inject(get_settings)
-        FRACTAL_RUNNER_BACKEND = settings.FRACTAL_RUNNER_BACKEND
-        process_workflow = get_process_workflow()
-
         # Prepare some of process_workflow arguments
         input_paths = input_dataset.paths
         output_path = output_dataset.paths[0]
 
         # Define and create server-side working folder
         project_id = workflow.project_id
         timestamp_string = get_timestamp().strftime("%Y%m%d_%H%M%S")
@@ -169,15 +154,17 @@
         os.umask(original_umask)
 
         # Define and create user-side working folder, if needed
         if FRACTAL_RUNNER_BACKEND == "local":
             WORKFLOW_DIR_USER = WORKFLOW_DIR
         elif FRACTAL_RUNNER_BACKEND == "slurm":
 
-            from ._slurm._subprocess_run_as_user import _mkdir_as_user
+            from ..executors.slurm._subprocess_run_as_user import (
+                _mkdir_as_user,
+            )
 
             WORKFLOW_DIR_USER = (
                 Path(user_cache_dir) / f"{WORKFLOW_DIR.name}"
             ).resolve()
             _mkdir_as_user(folder=str(WORKFLOW_DIR_USER), user=slurm_user)
         else:
             raise ValueError(f"{FRACTAL_RUNNER_BACKEND=} not supported")
@@ -270,15 +257,15 @@
         # up-to-date versions, obtained within process_workflow
         output_dataset.history = output_dataset_meta_hist.pop("history")
         output_dataset.meta = output_dataset_meta_hist.pop("metadata")
 
         db_sync.merge(output_dataset)
 
         # Update job DB entry
-        job.status = JobStatusType.DONE
+        job.status = JobStatusTypeV1.DONE
         job.end_timestamp = get_timestamp()
         with log_file_path.open("r") as f:
             logs = f.read()
         job.log = logs
         db_sync.merge(job)
         close_job_logger(logger)
         db_sync.commit()
@@ -300,15 +287,15 @@
             workflow,
             logger,
             failed_wftask=failed_wftask,
         )
 
         db_sync.merge(output_dataset)
 
-        job.status = JobStatusType.FAILED
+        job.status = JobStatusTypeV1.FAILED
         job.end_timestamp = get_timestamp()
 
         exception_args_string = "\n".join(e.args)
         job.log = (
             f"TASK ERROR: "
             f"Task name: {e.task_name}, "
             f"position in Workflow: {e.workflow_task_order}\n"
@@ -333,15 +320,15 @@
             output_dataset,
             workflow,
             logger,
         )
 
         db_sync.merge(output_dataset)
 
-        job.status = JobStatusType.FAILED
+        job.status = JobStatusTypeV1.FAILED
         job.end_timestamp = get_timestamp()
         error = e.assemble_error()
         job.log = f"JOB ERROR in Fractal job {job.id}:\nTRACEBACK:\n{error}"
         db_sync.merge(job)
         close_job_logger(logger)
         db_sync.commit()
 
@@ -362,15 +349,15 @@
             output_dataset,
             workflow,
             logger,
         )
 
         db_sync.merge(output_dataset)
 
-        job.status = JobStatusType.FAILED
+        job.status = JobStatusTypeV1.FAILED
         job.end_timestamp = get_timestamp()
         job.log = (
             f"UNKNOWN ERROR in Fractal job {job.id}\n"
             f"TRACEBACK:\n{current_traceback}"
         )
         db_sync.merge(job)
         close_job_logger(logger)
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_common.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/v1/_common.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,61 +7,48 @@
 """
 import json
 import shutil
 import subprocess  # nosec
 import traceback
 from concurrent.futures import Executor
 from copy import deepcopy
-from functools import lru_cache
 from functools import partial
 from pathlib import Path
 from shlex import split as shlex_split
 from typing import Any
 from typing import Callable
 from typing import Optional
 
-from ...config import get_settings
-from ...logger import get_logger
-from ...syringe import Inject
-from ..models import Task
-from ..models import WorkflowTask
-from ..schemas import WorkflowTaskStatusType
-from .common import JobExecutionError
-from .common import TaskExecutionError
+from ....config import get_settings
+from ....logger import get_logger
+from ....syringe import Inject
+from ...models import Task
+from ...models import WorkflowTask
+from ...schemas.v1 import WorkflowTaskStatusTypeV1
+from ..exceptions import JobExecutionError
+from ..exceptions import TaskExecutionError
 from .common import TaskParameters
 from .common import write_args_file
-
-
-HISTORY_FILENAME = "history.json"
-METADATA_FILENAME = "metadata.json"
-SHUTDOWN_FILENAME = "shutdown"
-WORKFLOW_LOG_FILENAME = "workflow.log"
+from fractal_server.app.runner.filenames import HISTORY_FILENAME
+from fractal_server.app.runner.filenames import METADATA_FILENAME
+from fractal_server.app.runner.task_files import get_task_file_paths
 
 
 def no_op_submit_setup_call(
     *,
     wftask: WorkflowTask,
     workflow_dir: Path,
     workflow_dir_user: Path,
-    task_pars: TaskParameters,
 ) -> dict:
     """
     Default (no-operation) interface of submit_setup_call.
     """
     return {}
 
 
-def sanitize_component(value: str) -> str:
-    """
-    Remove {" ", "/", "."} form a string, e.g. going from
-    'plate.zarr/B/03/0' to 'plate_zarr_B_03_0'.
-    """
-    return value.replace(" ", "_").replace("/", "_").replace(".", "_")
-
-
 def _task_needs_image_list(_task: Task) -> bool:
     """
     Whether a task requires `metadata["image"]` in its `args.json` file.
 
     For details see
     https://github.com/fractal-analytics-platform/fractal-server/issues/1237
 
@@ -74,106 +61,14 @@
     )
     if _task.name in exception_task_names:
         return True
     else:
         return False
 
 
-class TaskFiles:
-    """
-    Group all file paths pertaining to a task
-
-    Attributes:
-        workflow_dir:
-            Server-owned directory to store all task-execution-related relevant
-            files (inputs, outputs, errors, and all meta files related to the
-            job execution). Note: users cannot write directly to this folder.
-        workflow_dir_user:
-            User-side directory with the same scope as `workflow_dir`, and
-            where a user can write.
-        task_order:
-            Positional order of the task within a workflow.
-        component:
-            Specific component to run the task for (relevant for tasks that
-            will be executed in parallel over many components).
-        file_prefix:
-            Prefix for all task-related files.
-        args:
-            Path for input json file.
-        metadiff:
-            Path for output json file with metadata update.
-        out:
-            Path for task-execution stdout.
-        err:
-            Path for task-execution stderr.
-    """
-
-    workflow_dir: Path
-    workflow_dir_user: Path
-    task_order: Optional[int] = None
-    component: Optional[str] = None
-
-    file_prefix: str
-    args: Path
-    out: Path
-    err: Path
-    metadiff: Path
-
-    def __init__(
-        self,
-        workflow_dir: Path,
-        workflow_dir_user: Path,
-        task_order: Optional[int] = None,
-        component: Optional[str] = None,
-    ):
-        self.workflow_dir = workflow_dir
-        self.workflow_dir_user = workflow_dir_user
-        self.task_order = task_order
-        self.component = component
-
-        if self.component is not None:
-            component_safe = sanitize_component(str(self.component))
-            component_safe = f"_par_{component_safe}"
-        else:
-            component_safe = ""
-
-        if self.task_order is not None:
-            order = str(self.task_order)
-        else:
-            order = "task"
-        self.file_prefix = f"{order}{component_safe}"
-        self.args = self.workflow_dir_user / f"{self.file_prefix}.args.json"
-        self.out = self.workflow_dir_user / f"{self.file_prefix}.out"
-        self.err = self.workflow_dir_user / f"{self.file_prefix}.err"
-        self.metadiff = (
-            self.workflow_dir_user / f"{self.file_prefix}.metadiff.json"
-        )
-
-
-@lru_cache()
-def get_task_file_paths(
-    workflow_dir: Path,
-    workflow_dir_user: Path,
-    task_order: Optional[int] = None,
-    component: Optional[str] = None,
-) -> TaskFiles:
-    """
-    Return the corrisponding TaskFiles object
-
-    This function is mainly used as a cache to avoid instantiating needless
-    objects.
-    """
-    return TaskFiles(
-        workflow_dir=workflow_dir,
-        workflow_dir_user=workflow_dir_user,
-        task_order=task_order,
-        component=component,
-    )
-
-
 def _call_command_wrapper(cmd: str, stdout: Path, stderr: Path) -> None:
     """
     Call a command and write its stdout and stderr to files
 
     Raises:
         TaskExecutionError: If the `subprocess.run` call returns a positive
                             exit code
@@ -327,15 +222,15 @@
     updated_metadata.update(diff_metadata)
     # Prepare updated_history (note: the expected type for history items is
     # defined in `_DatasetHistoryItem`)
     wftask_dump = wftask.model_dump(exclude={"task"})
     wftask_dump["task"] = wftask.task.model_dump()
     new_history_item = dict(
         workflowtask=wftask_dump,
-        status=WorkflowTaskStatusType.DONE,
+        status=WorkflowTaskStatusTypeV1.DONE,
         parallelization=None,
     )
     updated_history = task_pars.history.copy()
     updated_history.append(new_history_item)
 
     # Assemble a TaskParameter object
     out_task_parameters = TaskParameters(
@@ -525,15 +420,14 @@
             f"in metadata keys ({keys})."
         )
 
     # Backend-specific configuration
     try:
         extra_setup = submit_setup_call(
             wftask=wftask,
-            task_pars=task_pars_depend,
             workflow_dir=workflow_dir,
             workflow_dir_user=workflow_dir_user,
         )
     except Exception as e:
         tb = "".join(traceback.format_tb(e.__traceback__))
         raise RuntimeError(
             f"{type(e)} error in {submit_setup_call=}\n"
@@ -588,15 +482,15 @@
 
     # Prepare updated_history (note: the expected type for history items is
     # defined in `_DatasetHistoryItem`)
     wftask_dump = wftask.model_dump(exclude={"task"})
     wftask_dump["task"] = wftask.task.model_dump()
     new_history_item = dict(
         workflowtask=wftask_dump,
-        status=WorkflowTaskStatusType.DONE,
+        status=WorkflowTaskStatusTypeV1.DONE,
         parallelization=dict(
             parallelization_level=wftask.parallelization_level,
             component_list=component_list,
         ),
     )
     updated_history = task_pars_depend.history.copy()
     updated_history.append(new_history_item)
@@ -677,15 +571,14 @@
                 logger_name=logger_name,
             )
         else:
             # Call backend-specific submit_setup_call
             try:
                 extra_setup = submit_setup_call(
                     wftask=this_wftask,
-                    task_pars=current_task_pars,
                     workflow_dir=workflow_dir,
                     workflow_dir_user=workflow_dir_user,
                 )
             except Exception as e:
                 tb = "".join(traceback.format_tb(e.__traceback__))
                 raise RuntimeError(
                     f"{type(e)} error in {submit_setup_call=}\n"
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_local/__init__.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/v1/_local/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 to run tasks in several threads.
 Incidentally, it also represents the reference implementation for a backend.
 """
 from pathlib import Path
 from typing import Any
 from typing import Optional
 
-from ...models import Workflow
-from .._common import execute_tasks
-from ..common import async_wrap
-from ..common import set_start_and_last_task_index
-from ..common import TaskParameters
+from ....models import Workflow  # FIXME: this is v1 specific
+from ...async_wrap import async_wrap
+from ...executors.local.executor import FractalThreadPoolExecutor
+from ...set_start_and_last_task_index import set_start_and_last_task_index
+from .._common import execute_tasks  # FIXME: this is v1 specific
+from ..common import TaskParameters  # FIXME: this is v1 specific
 from ._submit_setup import _local_submit_setup
-from .executor import FractalThreadPoolExecutor
 
 
 def _process_workflow(
     *,
     workflow: Workflow,
     input_paths: list[Path],
     output_path: Path,
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/v1/_local/_local_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from pathlib import Path
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Extra
 from pydantic.error_wrappers import ValidationError
 
-from ....config import get_settings
-from ....syringe import Inject
-from ...models import WorkflowTask
+from .....config import get_settings
+from .....syringe import Inject
+from ....models.v1 import WorkflowTask
 
 
 class LocalBackendConfigError(ValueError):
     """
     Local-backend configuration error
     """
 
@@ -59,23 +59,22 @@
 ) -> LocalBackendConfig:
     """
     Prepare a `LocalBackendConfig` configuration object
 
     The sources for `parallel_tasks_per_job` attributes, starting from the
     highest-priority one, are
 
-    1. Properties in `wftask.meta` (which, for `WorkflowTask`s added through
-       `Workflow.insert_task`, also includes `wftask.task.meta`);
+    1. Properties in `wftask.meta`;
     2. The general content of the local-backend configuration file;
     3. The default value (`None`).
 
     Arguments:
         wftask:
-            WorkflowTask for which the backend configuration is is to be
-            prepared.
+            WorkflowTask (V1) for which the backend configuration should
+            be prepared.
         config_path:
             Path of local-backend configuration file; if `None`, use
             `FRACTAL_LOCAL_CONFIG_FILE` variable from settings.
 
     Returns:
         A local-backend configuration object
     """
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/v2/_local/_submit_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,45 +8,45 @@
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 """
 Submodule to define _local_submit_setup
 """
 from pathlib import Path
+from typing import Literal
 from typing import Optional
 
-from ...models import WorkflowTask
-from ..common import TaskParameters
+from ....models.v2 import WorkflowTaskV2
 from ._local_config import get_local_backend_config
 
 
 def _local_submit_setup(
     *,
-    wftask: WorkflowTask,
+    wftask: WorkflowTaskV2,
     workflow_dir: Optional[Path] = None,
     workflow_dir_user: Optional[Path] = None,
-    task_pars: Optional[TaskParameters] = None,
+    which_type: Literal["non_parallel", "parallel"],
 ) -> dict[str, object]:
     """
     Collect WorfklowTask-specific configuration parameters from different
     sources, and inject them for execution.
 
     Arguments:
         wftask:
             WorkflowTask for which the configuration is to be assembled
-        task_pars:
-            Not used in this function.
         workflow_dir:
             Not used in this function.
         workflow_dir_user:
             Not used in this function.
 
     Returns:
         submit_setup_dict:
             A dictionary that will be passed on to
             `FractalThreadPoolExecutor.submit` and
             `FractalThreadPoolExecutor.map`, so as to set extra options.
     """
 
-    local_backend_config = get_local_backend_config(wftask=wftask)
+    local_backend_config = get_local_backend_config(
+        wftask=wftask, which_type=which_type
+    )
 
     return dict(local_backend_config=local_backend_config)
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_local/executor.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/executors/local/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 """
 from concurrent.futures import ThreadPoolExecutor
 from typing import Callable
 from typing import Iterable
 from typing import Optional
 from typing import Sequence
 
-from ._local_config import get_default_local_backend_config
-from ._local_config import LocalBackendConfig
+from ...v1._local._local_config import get_default_local_backend_config
+from ...v1._local._local_config import LocalBackendConfig
 
 
 class FractalThreadPoolExecutor(ThreadPoolExecutor):
     """
     Custom version of
     [ThreadPoolExecutor](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor))
     that overrides the `submit` and `map` methods
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/v2/_slurm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,29 @@
 Executor objects.
 """
 from pathlib import Path
 from typing import Any
 from typing import Optional
 from typing import Union
 
-from ...models import Workflow
-from .._common import execute_tasks
-from ..common import async_wrap
-from ..common import set_start_and_last_task_index
-from ..common import TaskParameters
-from ._submit_setup import _slurm_submit_setup
-from .executor import FractalSlurmExecutor
+from fractal_server.app.models.v2 import WorkflowV2
+
+# from ...executors.slurm.executor import FractalSlurmExecutor
+# from ._submit_setup import _slurm_submit_setup
+# from .get_slurm_config import get_slurm_config
+
+# from .._common import execute_tasks
+# from ..common import async_wrap
+# from ..common import set_start_and_last_task_index
+# from ..common import TaskParameters
 
 
 def _process_workflow(
     *,
-    workflow: Workflow,
+    workflow: WorkflowV2,
     input_paths: list[Path],
     output_path: Path,
     input_metadata: dict[str, Any],
     input_history: list[dict[str, Any]],
     logger_name: str,
     workflow_dir: Path,
     workflow_dir_user: Path,
@@ -56,57 +59,59 @@
 
     Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
 
     Returns:
         output_dataset_metadata: Metadata of the output dataset
     """
 
-    if not slurm_user:
-        raise RuntimeError(
-            "slurm_user argument is required, for slurm backend"
-        )
-
-    if isinstance(worker_init, str):
-        worker_init = worker_init.split("\n")
-
-    with FractalSlurmExecutor(
-        debug=True,
-        keep_logs=True,
-        slurm_user=slurm_user,
-        user_cache_dir=user_cache_dir,
-        working_dir=workflow_dir,
-        working_dir_user=workflow_dir_user,
-        common_script_lines=worker_init,
-        slurm_account=slurm_account,
-    ) as executor:
-        output_task_pars = execute_tasks(
-            executor=executor,
-            task_list=workflow.task_list[
-                first_task_index : (last_task_index + 1)  # noqa
-            ],  # noqa
-            task_pars=TaskParameters(
-                input_paths=input_paths,
-                output_path=output_path,
-                metadata=input_metadata,
-                history=input_history,
-            ),
-            workflow_dir=workflow_dir,
-            workflow_dir_user=workflow_dir_user,
-            submit_setup_call=_slurm_submit_setup,
-            logger_name=logger_name,
-        )
-    output_dataset_metadata_history = dict(
-        metadata=output_task_pars.metadata, history=output_task_pars.history
-    )
-    return output_dataset_metadata_history
+    raise NotImplementedError
+
+    # if not slurm_user:
+    #     raise RuntimeError(
+    #         "slurm_user argument is required, for slurm backend"
+    #     )
+
+    # if isinstance(worker_init, str):
+    #     worker_init = worker_init.split("\n")
+
+    # with FractalSlurmExecutor(
+    #     debug=True,
+    #     keep_logs=True,
+    #     slurm_user=slurm_user,
+    #     user_cache_dir=user_cache_dir,
+    #     working_dir=workflow_dir,
+    #     working_dir_user=workflow_dir_user,
+    #     common_script_lines=worker_init,
+    #     slurm_account=slurm_account,
+    # ) as executor:
+    #     output_task_pars = execute_tasks(
+    #         executor=executor,
+    #         task_list=workflow.task_list[
+    #             first_task_index : (last_task_index + 1)  # noqa
+    #         ],  # noqa
+    #         task_pars=TaskParameters(
+    #             input_paths=input_paths,
+    #             output_path=output_path,
+    #             metadata=input_metadata,
+    #             history=input_history,
+    #         ),
+    #         workflow_dir=workflow_dir,
+    #         workflow_dir_user=workflow_dir_user,
+    #         submit_setup_call=_slurm_submit_setup,
+    #         logger_name=logger_name,
+    #     )
+    # output_dataset_metadata_history = dict(
+    #     metadata=output_task_pars.metadata, history=output_task_pars.history
+    # )
+    # return output_dataset_metadata_history
 
 
 async def process_workflow(
     *,
-    workflow: Workflow,
+    workflow: WorkflowV2,
     input_paths: list[Path],
     output_path: Path,
     input_metadata: dict[str, Any],
     input_history: list[dict[str, Any]],
     logger_name: str,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
@@ -119,32 +124,34 @@
 ) -> dict[str, Any]:
     """
     Process workflow (SLURM backend public interface)
 
     Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
     """
 
-    # Set values of first_task_index and last_task_index
-    num_tasks = len(workflow.task_list)
-    first_task_index, last_task_index = set_start_and_last_task_index(
-        num_tasks,
-        first_task_index=first_task_index,
-        last_task_index=last_task_index,
-    )
-
-    output_dataset_metadata_history = await async_wrap(_process_workflow)(
-        workflow=workflow,
-        input_paths=input_paths,
-        output_path=output_path,
-        input_metadata=input_metadata,
-        input_history=input_history,
-        logger_name=logger_name,
-        workflow_dir=workflow_dir,
-        workflow_dir_user=workflow_dir_user,
-        slurm_user=slurm_user,
-        slurm_account=slurm_account,
-        user_cache_dir=user_cache_dir,
-        worker_init=worker_init,
-        first_task_index=first_task_index,
-        last_task_index=last_task_index,
-    )
-    return output_dataset_metadata_history
+    raise NotImplementedError
+
+    # # Set values of first_task_index and last_task_index
+    # num_tasks = len(workflow.task_list)
+    # first_task_index, last_task_index = set_start_and_last_task_index(
+    #     num_tasks,
+    #     first_task_index=first_task_index,
+    #     last_task_index=last_task_index,
+    # )
+
+    # output_dataset_metadata_history = await async_wrap(_process_workflow)(
+    #     workflow=workflow,
+    #     input_paths=input_paths,
+    #     output_path=output_path,
+    #     input_metadata=input_metadata,
+    #     input_history=input_history,
+    #     logger_name=logger_name,
+    #     workflow_dir=workflow_dir,
+    #     workflow_dir_user=workflow_dir_user,
+    #     slurm_user=slurm_user,
+    #     slurm_account=slurm_account,
+    #     user_cache_dir=user_cache_dir,
+    #     worker_init=worker_init,
+    #     first_task_index=first_task_index,
+    #     last_task_index=last_task_index,
+    # )
+    # return output_dataset_metadata_history
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/_batching.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Zurich.
 """
 Submodule to determine the number of total/parallel tasks per SLURM job.
 """
 import math
 from typing import Optional
 
-from ....logger import set_logger
+from .....logger import set_logger
 
 logger = set_logger(__name__)
 
 
 class SlurmHeuristicsError(ValueError):
     pass
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import time
 import traceback
 from itertools import count
 from typing import Callable
 from typing import Optional
 
 from cfut import FileWaitThread
-from cfut import slurm
-
-from ....logger import set_logger
 
+from .....logger import set_logger
+from ._check_jobs_status import _jobs_finished
 
 logger = set_logger(__name__)
 
 
 class FractalFileWaitThread(FileWaitThread):
     """
     Overrides the original clusterfutures.FileWaitThread, so that:
@@ -117,15 +116,15 @@
 
     slurm_poll_interval = 30
 
     def check(self, i):
         super().check(i)
         if i % (self.slurm_poll_interval // self.interval) == 0:
             try:
-                finished_jobs = slurm.jobs_finished(self.waiting.values())
+                finished_jobs = _jobs_finished(self.waiting.values())
             except Exception:
                 # Don't abandon completion checking if jobs_finished errors
                 traceback.print_exc()
                 return
 
             if not finished_jobs:
                 return
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/_slurm_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,18 +18,17 @@
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Extra
 from pydantic import Field
 from pydantic.error_wrappers import ValidationError
 
-from ....config import get_settings
-from ....logger import set_logger
-from ....syringe import Inject
-from ...models import WorkflowTask
+from .....config import get_settings
+from .....logger import set_logger
+from .....syringe import Inject
 
 logger = set_logger(__name__)
 
 
 class SlurmConfigError(ValueError):
     """
     Slurm configuration error
@@ -455,155 +454,7 @@
         target_cpus_per_job=1,
         max_cpus_per_job=2,
         target_mem_per_job=100,
         max_mem_per_job=500,
         target_num_jobs=2,
         max_num_jobs=4,
     )
-
-
-def get_slurm_config(
-    wftask: WorkflowTask,
-    workflow_dir: Path,
-    workflow_dir_user: Path,
-    config_path: Optional[Path] = None,
-) -> SlurmConfig:
-    """
-    Prepare a `SlurmConfig` configuration object
-
-    The sources for `SlurmConfig` attributes, in increasing priority order, are
-
-    1. The general content of the Fractal SLURM configuration file.
-    2. The GPU-specific content of the Fractal SLURM configuration file, if
-        appropriate.
-    3. Properties in `wftask.meta` (which, for `WorkflowTask`s added through
-       `Workflow.insert_task`, also includes `wftask.task.meta`);
-
-    Note: `wftask.meta` may be `None`.
-
-    Arguments:
-        wftask:
-            WorkflowTask for which the SLURM configuration is is to be
-            prepared.
-        workflow_dir:
-            Server-owned directory to store all task-execution-related relevant
-            files (inputs, outputs, errors, and all meta files related to the
-            job execution). Note: users cannot write directly to this folder.
-        workflow_dir_user:
-            User-side directory with the same scope as `workflow_dir`, and
-            where a user can write.
-        config_path:
-            Path of aFractal  SLURM configuration file; if `None`, use
-            `FRACTAL_SLURM_CONFIG_FILE` variable from settings.
-
-    Returns:
-        slurm_config:
-            The SlurmConfig object
-    """
-
-    logger.debug(
-        "[get_slurm_config] WorkflowTask meta attribute: {wftask.meta=}"
-    )
-
-    # Incorporate slurm_env.default_slurm_config
-    slurm_env = load_slurm_config_file(config_path=config_path)
-    slurm_dict = slurm_env.default_slurm_config.dict(
-        exclude_unset=True, exclude={"mem"}
-    )
-    if slurm_env.default_slurm_config.mem:
-        slurm_dict["mem_per_task_MB"] = slurm_env.default_slurm_config.mem
-
-    # Incorporate slurm_env.batching_config
-    for key, value in slurm_env.batching_config.dict().items():
-        slurm_dict[key] = value
-
-    # Incorporate slurm_env.user_local_exports
-    slurm_dict["user_local_exports"] = slurm_env.user_local_exports
-
-    logger.debug(
-        "[get_slurm_config] Fractal SLURM configuration file: "
-        f"{slurm_env.dict()=}"
-    )
-
-    # GPU-related options
-    # Notes about priority:
-    # 1. This block of definitions takes priority over other definitions from
-    #    slurm_env which are not under the `needs_gpu` subgroup
-    # 2. This block of definitions has lower priority than whatever comes next
-    #    (i.e. from WorkflowTask.meta).
-    if wftask.meta is not None:
-        needs_gpu = wftask.meta.get("needs_gpu", False)
-    else:
-        needs_gpu = False
-    logger.debug(f"[get_slurm_config] {needs_gpu=}")
-    if needs_gpu:
-        for key, value in slurm_env.gpu_slurm_config.dict(
-            exclude_unset=True, exclude={"mem"}
-        ).items():
-            slurm_dict[key] = value
-        if slurm_env.gpu_slurm_config.mem:
-            slurm_dict["mem_per_task_MB"] = slurm_env.gpu_slurm_config.mem
-
-    # Number of CPUs per task, for multithreading
-    if wftask.meta is not None and "cpus_per_task" in wftask.meta:
-        cpus_per_task = int(wftask.meta["cpus_per_task"])
-        slurm_dict["cpus_per_task"] = cpus_per_task
-
-    # Required memory per task, in MB
-    if wftask.meta is not None and "mem" in wftask.meta:
-        raw_mem = wftask.meta["mem"]
-        mem_per_task_MB = _parse_mem_value(raw_mem)
-        slurm_dict["mem_per_task_MB"] = mem_per_task_MB
-
-    # Job name
-    job_name = wftask.task.name.replace(" ", "_")
-    slurm_dict["job_name"] = job_name
-
-    # Optional SLURM arguments and extra lines
-    if wftask.meta is not None:
-        account = wftask.meta.get("account", None)
-        if account is not None:
-            error_msg = (
-                f"Invalid {account=} property in WorkflowTask `meta` "
-                "attribute.\n"
-                "SLURM account must be set in the request body of the "
-                "apply-workflow endpoint, or by modifying the user properties."
-            )
-            logger.error(error_msg)
-            raise SlurmConfigError(error_msg)
-        for key in ["time", "gres", "constraint"]:
-            value = wftask.meta.get(key, None)
-            if value:
-                slurm_dict[key] = value
-    if wftask.meta is not None:
-        extra_lines = wftask.meta.get("extra_lines", [])
-    else:
-        extra_lines = []
-    extra_lines = slurm_dict.get("extra_lines", []) + extra_lines
-    if len(set(extra_lines)) != len(extra_lines):
-        logger.debug(
-            "[get_slurm_config] Removing repeated elements "
-            f"from {extra_lines=}."
-        )
-        extra_lines = list(set(extra_lines))
-    slurm_dict["extra_lines"] = extra_lines
-
-    # Job-batching parameters (if None, they will be determined heuristically)
-    if wftask.meta is not None:
-        tasks_per_job = wftask.meta.get("tasks_per_job", None)
-        parallel_tasks_per_job = wftask.meta.get(
-            "parallel_tasks_per_job", None
-        )
-    else:
-        tasks_per_job = None
-        parallel_tasks_per_job = None
-    slurm_dict["tasks_per_job"] = tasks_per_job
-    slurm_dict["parallel_tasks_per_job"] = parallel_tasks_per_job
-
-    # Put everything together
-    logger.debug(
-        "[get_slurm_config] Now create a SlurmConfig object based "
-        f"on {slurm_dict=}"
-    )
-    slurm_config = SlurmConfig(**slurm_dict)
-
-    return slurm_config
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/v2/_slurm/_submit_setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,28 +11,27 @@
 # Zurich.
 """
 Submodule to define _slurm_submit_setup, which is also the reference
 implementation of `submit_setup_call` in
 [fractal_server.app.runner._common][]).
 """
 from pathlib import Path
-from typing import Optional
+from typing import Literal
 
-from ...models import WorkflowTask
-from .._common import get_task_file_paths
-from ..common import TaskParameters
-from ._slurm_config import get_slurm_config
+from ...task_files import get_task_file_paths
+from .get_slurm_config import get_slurm_config
+from fractal_server.app.models.v2 import WorkflowTaskV2
 
 
 def _slurm_submit_setup(
     *,
-    wftask: WorkflowTask,
+    wftask: WorkflowTaskV2,
     workflow_dir: Path,
     workflow_dir_user: Path,
-    task_pars: Optional[TaskParameters] = None,
+    which_type: Literal["non_parallel", "parallel"],
 ) -> dict[str, object]:
     """
     Collect WorfklowTask-specific configuration parameters from different
     sources, and inject them for execution.
 
     Here goes all the logic for reading attributes from the appropriate sources
     and transforming them into an appropriate `SlurmConfig` object (encoding
@@ -42,17 +41,14 @@
     For now, this is the reference implementation for the argument
     `submit_setup_call` of
     [fractal_server.app.runner._common.execute_tasks][].
 
     Arguments:
         wftask:
             WorkflowTask for which the configuration is to be assembled
-        task_pars:
-            Task parameters to be passed to the task
-            (not used in this function)
         workflow_dir:
             Server-owned directory to store all task-execution-related relevant
             files (inputs, outputs, errors, and all meta files related to the
             job execution). Note: users cannot write directly to this folder.
         workflow_dir_user:
             User-side directory with the same scope as `workflow_dir`, and
             where a user can write.
@@ -65,14 +61,15 @@
     """
 
     # Get SlurmConfig object
     slurm_config = get_slurm_config(
         wftask=wftask,
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
+        which_type=which_type,
     )
 
     # Get TaskFiles object
     task_files = get_task_file_paths(
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
         task_order=wftask.order,
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 `os.path.exists`, but extended so that they can be executed on behalf of
 another user. Note that this requires appropriate sudo permissions.
 """
 import shlex
 import subprocess  # nosec
 from typing import Optional
 
-from ....logger import set_logger
+from .....logger import set_logger
 
 logger = set_logger(__name__)
 
 
 def _run_command_as_user(
     *,
     cmd: str,
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 from typing import Optional
 from typing import Sequence
 
 import cloudpickle
 from cfut import SlurmExecutor
 from cfut.util import random_string
 
-from ....config import get_settings
-from ....logger import set_logger
-from ....syringe import Inject
-from .._common import get_task_file_paths
-from .._common import SHUTDOWN_FILENAME
-from .._common import TaskFiles
-from ..common import JobExecutionError
-from ..common import TaskExecutionError
+from .....config import get_settings
+from .....logger import set_logger
+from .....syringe import Inject
+from ...exceptions import JobExecutionError
+from ...exceptions import TaskExecutionError
+from ...filenames import SHUTDOWN_FILENAME
+from ...task_files import get_task_file_paths
+from ...task_files import TaskFiles
 from ._batching import heuristics
 from ._executor_wait_thread import FractalSlurmWaitThread
 from ._slurm_config import get_default_slurm_config
 from ._slurm_config import SlurmConfig
 from ._subprocess_run_as_user import _glob_as_user
 from ._subprocess_run_as_user import _glob_as_user_strict
 from ._subprocess_run_as_user import _path_exists_as_user
@@ -997,15 +997,15 @@
         cmdlines = []
         for ind_task in range(job.num_tasks_tot):
             input_pickle_file = job.input_pickle_files[ind_task]
             output_pickle_file = job.output_pickle_files[ind_task]
             cmdlines.append(
                 (
                     f"{python_worker_interpreter}"
-                    " -m fractal_server.app.runner._slurm.remote "
+                    " -m fractal_server.app.runner.executors.slurm.remote "
                     f"--input-file {input_pickle_file} "
                     f"--output-file {output_pickle_file}"
                 )
             )
 
         # ...
         sbatch_script = self._prepare_sbatch_script(
```

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/executors/slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/app/runner/handle_failed_job.py` & `fractal_server-2.0.0a0/fractal_server/app/runner/v1/handle_failed_job.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 import json
 import logging
 from copy import deepcopy
 from pathlib import Path
 from typing import Any
 from typing import Optional
 
-from ..models import ApplyWorkflow
-from ..models import Dataset
-from ..models import Workflow
-from ..models import WorkflowTask
-from ..models import WorkflowTaskStatusType
-from ._common import HISTORY_FILENAME
-from ._common import METADATA_FILENAME
+from ...models.v1 import ApplyWorkflow
+from ...models.v1 import Dataset
+from ...models.v1 import Workflow
+from ...models.v1 import WorkflowTask
+from ...schemas.v1 import WorkflowTaskStatusTypeV1
+from ..filenames import HISTORY_FILENAME
+from ..filenames import METADATA_FILENAME
 
 
 def assemble_history_failed_job(
     job: ApplyWorkflow,
     output_dataset: Dataset,
     workflow: Workflow,
     logger: logging.Logger,
@@ -94,15 +94,15 @@
 
     # Part 3/B: Append failed task to history
     if failed_wftask is not None:
         failed_wftask_dump = failed_wftask.model_dump(exclude={"task"})
         failed_wftask_dump["task"] = failed_wftask.task.model_dump()
         new_history_item = dict(
             workflowtask=failed_wftask_dump,
-            status=WorkflowTaskStatusType.FAILED,
+            status=WorkflowTaskStatusTypeV1.FAILED,
             parallelization=dict(
                 parallelization_level=failed_wftask.parallelization_level,
             ),
         )
         new_history.append(new_history_item)
 
     return new_history
```

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/__init__.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/v1/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
 Schemas for API request/response bodies
 """
-from .applyworkflow import ApplyWorkflowCreate  # noqa: F401
-from .applyworkflow import ApplyWorkflowRead  # noqa: F401
-from .applyworkflow import ApplyWorkflowUpdate  # noqa: F401
-from .applyworkflow import JobStatusType  # noqa: F401
-from .dataset import DatasetCreate  # noqa: F401
-from .dataset import DatasetRead  # noqa: F401
-from .dataset import DatasetStatusRead  # noqa: F401
-from .dataset import DatasetUpdate  # noqa: F401
-from .dataset import ResourceCreate  # noqa: F401
-from .dataset import ResourceRead  # noqa: F401
-from .dataset import ResourceUpdate  # noqa: F401
+from ..state import _StateBase  # noqa: F401
+from ..state import StateRead  # noqa: F401
+from ..user import UserCreate  # noqa: F401
+from ..user import UserRead  # noqa: F401
+from ..user import UserUpdate  # noqa: F401
+from ..user import UserUpdateStrict  # noqa: F401
+from .applyworkflow import ApplyWorkflowCreateV1  # noqa: F401
+from .applyworkflow import ApplyWorkflowReadV1  # noqa: F401
+from .applyworkflow import ApplyWorkflowUpdateV1  # noqa: F401
+from .applyworkflow import JobStatusTypeV1  # noqa: F401
+from .dataset import DatasetCreateV1  # noqa: F401
+from .dataset import DatasetReadV1  # noqa: F401
+from .dataset import DatasetStatusReadV1  # noqa: F401
+from .dataset import DatasetUpdateV1  # noqa: F401
+from .dataset import ResourceCreateV1  # noqa: F401
+from .dataset import ResourceReadV1  # noqa: F401
+from .dataset import ResourceUpdateV1  # noqa: F401
 from .manifest import ManifestV1  # noqa: F401
 from .manifest import TaskManifestV1  # noqa: F401
-from .project import ProjectCreate  # noqa: F401
-from .project import ProjectRead  # noqa: F401
-from .project import ProjectUpdate  # noqa: F401
-from .state import _StateBase  # noqa: F401
-from .state import StateRead  # noqa: F401
-from .task import TaskCreate  # noqa: F401
-from .task import TaskImport  # noqa: F401
-from .task import TaskRead  # noqa: F401
-from .task import TaskUpdate  # noqa: F401
-from .task_collection import TaskCollectPip  # noqa: F401
-from .task_collection import TaskCollectStatus  # noqa: F401
-from .user import UserCreate  # noqa: F401
-from .user import UserRead  # noqa: F401
-from .user import UserUpdate  # noqa: F401
-from .user import UserUpdateStrict  # noqa: F401
-from .workflow import WorkflowCreate  # noqa: F401
-from .workflow import WorkflowExport  # noqa: F401
-from .workflow import WorkflowImport  # noqa: F401
-from .workflow import WorkflowRead  # noqa: F401
-from .workflow import WorkflowTaskCreate  # noqa: F401
-from .workflow import WorkflowTaskExport  # noqa: F401
-from .workflow import WorkflowTaskImport  # noqa: F401
-from .workflow import WorkflowTaskRead  # noqa: F401
-from .workflow import WorkflowTaskStatusType  # noqa: F401
-from .workflow import WorkflowTaskUpdate  # noqa: F401
-from .workflow import WorkflowUpdate  # noqa: F401
+from .project import ProjectCreateV1  # noqa: F401
+from .project import ProjectReadV1  # noqa: F401
+from .project import ProjectUpdateV1  # noqa: F401
+from .task import TaskCreateV1  # noqa: F401
+from .task import TaskImportV1  # noqa: F401
+from .task import TaskReadV1  # noqa: F401
+from .task import TaskUpdateV1  # noqa: F401
+from .task_collection import TaskCollectPipV1  # noqa: F401
+from .task_collection import TaskCollectStatusV1  # noqa: F401
+from .workflow import WorkflowCreateV1  # noqa: F401
+from .workflow import WorkflowExportV1  # noqa: F401
+from .workflow import WorkflowImportV1  # noqa: F401
+from .workflow import WorkflowReadV1  # noqa: F401
+from .workflow import WorkflowTaskCreateV1  # noqa: F401
+from .workflow import WorkflowTaskExportV1  # noqa: F401
+from .workflow import WorkflowTaskImportV1  # noqa: F401
+from .workflow import WorkflowTaskReadV1  # noqa: F401
+from .workflow import WorkflowTaskStatusTypeV1  # noqa: F401
+from .workflow import WorkflowTaskUpdateV1  # noqa: F401
+from .workflow import WorkflowUpdateV1  # noqa: F401
```

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/_validators.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/applyworkflow.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/v1/applyworkflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import validator
 from pydantic.types import StrictStr
 
-from ._validators import valstr
-from ._validators import valutc
-from .dumps import DatasetDump
-from .dumps import ProjectDump
-from .dumps import WorkflowDump
+from .._validators import valstr
+from .._validators import valutc
+from .dumps import DatasetDumpV1
+from .dumps import ProjectDumpV1
+from .dumps import WorkflowDumpV1
 
 
 __all__ = (
-    "_ApplyWorkflowBase",
-    "ApplyWorkflowCreate",
-    "ApplyWorkflowRead",
+    "_ApplyWorkflowBaseV1",
+    "ApplyWorkflowCreateV1",
+    "ApplyWorkflowReadV1",
 )
 
 
-class JobStatusType(str, Enum):
+class JobStatusTypeV1(str, Enum):
     """
     Define the available job statuses
 
     Attributes:
         SUBMITTED:
             The job was created. This does not guarantee that it was also
             submitted to an executor (e.g. other errors could have prevented
@@ -37,26 +37,26 @@
     """
 
     SUBMITTED = "submitted"
     DONE = "done"
     FAILED = "failed"
 
 
-class _ApplyWorkflowBase(BaseModel):
+class _ApplyWorkflowBaseV1(BaseModel):
     """
     Base class for `ApplyWorkflow`.
 
     Attributes:
         worker_init:
     """
 
     worker_init: Optional[str]
 
 
-class ApplyWorkflowCreate(_ApplyWorkflowBase):
+class ApplyWorkflowCreateV1(_ApplyWorkflowBaseV1):
     """
     Class for `ApplyWorkflow` creation.
 
     Attributes:
         first_task_index:
         last_task_index:
         slurm_account:
@@ -100,15 +100,15 @@
                 raise ValueError(
                     f"{first_task_index=} cannot be larger than "
                     f"{last_task_index=}"
                 )
         return v
 
 
-class ApplyWorkflowRead(_ApplyWorkflowBase):
+class ApplyWorkflowReadV1(_ApplyWorkflowBaseV1):
     """
     Class for `ApplyWorkflow` read from database.
 
     Attributes:
         id:
         project_id:
         project_dump:
@@ -128,23 +128,23 @@
         working_dir_user:
         first_task_index:
         last_task_index:
     """
 
     id: int
     project_id: Optional[int]
-    project_dump: ProjectDump
+    project_dump: ProjectDumpV1
     user_email: str
     slurm_account: Optional[str]
     workflow_id: Optional[int]
-    workflow_dump: WorkflowDump
+    workflow_dump: WorkflowDumpV1
     input_dataset_id: Optional[int]
-    input_dataset_dump: DatasetDump
+    input_dataset_dump: DatasetDumpV1
     output_dataset_id: Optional[int]
-    output_dataset_dump: DatasetDump
+    output_dataset_dump: DatasetDumpV1
     start_timestamp: datetime
     end_timestamp: Optional[datetime]
     status: str
     log: Optional[str]
     working_dir: Optional[str]
     working_dir_user: Optional[str]
     first_task_index: Optional[int]
@@ -154,16 +154,16 @@
         valutc("start_timestamp")
     )
     _end_timestamp = validator("end_timestamp", allow_reuse=True)(
         valutc("end_timestamp")
     )
 
 
-class ApplyWorkflowUpdate(BaseModel):
+class ApplyWorkflowUpdateV1(BaseModel):
     """
     Class for updating a job status.
 
     Attributes:
         status: New job status.
     """
 
-    status: JobStatusType
+    status: JobStatusTypeV1
```

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/dataset.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/v1/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,169 +2,169 @@
 from typing import Any
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from ._validators import val_absolute_path
-from ._validators import valstr
-from ._validators import valutc
-from .dumps import WorkflowTaskDump
-from .project import ProjectRead
-from .workflow import WorkflowTaskStatusType
+from .._validators import val_absolute_path
+from .._validators import valstr
+from .._validators import valutc
+from .dumps import WorkflowTaskDumpV1
+from .project import ProjectReadV1
+from .workflow import WorkflowTaskStatusTypeV1
 
 __all__ = (
-    "DatasetUpdate",
-    "DatasetCreate",
-    "DatasetRead",
-    "ResourceCreate",
-    "ResourceRead",
-    "ResourceUpdate",
-    "DatasetStatusRead",
+    "DatasetUpdateV1",
+    "DatasetCreateV1",
+    "DatasetReadV1",
+    "ResourceCreateV1",
+    "ResourceReadV1",
+    "ResourceUpdateV1",
+    "DatasetStatusReadV1",
 )
 
 
-class _ResourceBase(BaseModel):
+class _ResourceBaseV1(BaseModel):
     """
     Base class for `Resource`.
 
     Attributes:
         path:
     """
 
     path: str
 
 
-class ResourceCreate(_ResourceBase):
+class ResourceCreateV1(_ResourceBaseV1):
     """
     Class for `Resource` creation.
     """
 
     # Validators
     _path = validator("path", allow_reuse=True)(val_absolute_path("path"))
 
 
-class ResourceUpdate(_ResourceBase):
+class ResourceUpdateV1(_ResourceBaseV1):
     """
     Class for `Resource` update.
     """
 
     # Validators
     _path = validator("path", allow_reuse=True)(val_absolute_path("path"))
 
 
-class ResourceRead(_ResourceBase):
+class ResourceReadV1(_ResourceBaseV1):
     """
     Class for `Resource` read from database.
 
     Attributes:
         id:
         dataset_id:
     """
 
     id: int
     dataset_id: int
 
 
-class _DatasetHistoryItem(BaseModel):
+class _DatasetHistoryItemV1(BaseModel):
     """
     Class for an item of `Dataset.history`.
 
     Attributes:
         workflowtask:
         status:
         parallelization: If provided, it includes keys `parallelization_level`
             and `component_list`.
     """
 
-    workflowtask: WorkflowTaskDump
-    status: WorkflowTaskStatusType
+    workflowtask: WorkflowTaskDumpV1
+    status: WorkflowTaskStatusTypeV1
     parallelization: Optional[dict]
 
 
-class _DatasetBase(BaseModel):
+class _DatasetBaseV1(BaseModel):
     """
     Base class for `Dataset`.
 
     Attributes:
         name:
         type:
         meta:
         history:
         read_only:
     """
 
     name: str
     type: Optional[str]
     meta: dict[str, Any] = Field(default={})
-    history: list[_DatasetHistoryItem] = Field(default=[])
+    history: list[_DatasetHistoryItemV1] = Field(default=[])
     read_only: bool = False
 
 
-class DatasetUpdate(_DatasetBase):
+class DatasetUpdateV1(_DatasetBaseV1):
     """
     Class for `Dataset` update.
 
     Attributes:
         name:
         meta:
         history:
         read_only:
     """
 
     name: Optional[str]
     meta: Optional[dict[str, Any]] = None
-    history: Optional[list[_DatasetHistoryItem]] = None
+    history: Optional[list[_DatasetHistoryItemV1]] = None
     read_only: Optional[bool]
 
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
     _type = validator("type", allow_reuse=True)(valstr("type"))
 
 
-class DatasetCreate(_DatasetBase):
+class DatasetCreateV1(_DatasetBaseV1):
     """
     Class for `Dataset` creation.
     """
 
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
     _type = validator("type", allow_reuse=True)(valstr("type"))
 
 
-class DatasetRead(_DatasetBase):
+class DatasetReadV1(_DatasetBaseV1):
     """
     Class for `Dataset` read from database.
 
     Attributes:
         id:
         read_only:
         resource_list:
         project_id:
         project:
     """
 
     id: int
-    resource_list: list[ResourceRead]
+    resource_list: list[ResourceReadV1]
     project_id: int
     read_only: bool
-    project: ProjectRead
+    project: ProjectReadV1
     timestamp_created: datetime
 
     _timestamp_created = validator("timestamp_created", allow_reuse=True)(
         valutc("timestamp_created")
     )
 
 
-class DatasetStatusRead(BaseModel):
+class DatasetStatusReadV1(BaseModel):
     """
     Response type for the
     `/project/{project_id}/dataset/{dataset_id}/status/` endpoint
     """
 
     status: Optional[
         dict[
             int,
-            WorkflowTaskStatusType,
+            WorkflowTaskStatusTypeV1,
         ]
     ] = None
```

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/dumps.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/v1/dumps.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,55 +10,55 @@
 """
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Extra
 
 
-class ProjectDump(BaseModel, extra=Extra.forbid):
+class ProjectDumpV1(BaseModel, extra=Extra.forbid):
 
     id: int
     name: str
     read_only: bool
     timestamp_created: str
 
 
-class TaskDump(BaseModel):
+class TaskDumpV1(BaseModel):
     id: int
     source: str
     name: str
     command: str
     input_type: str
     output_type: str
     owner: Optional[str]
     version: Optional[str]
 
 
-class WorkflowTaskDump(BaseModel):
+class WorkflowTaskDumpV1(BaseModel):
     id: int
     order: Optional[int]
     workflow_id: int
     task_id: int
-    task: TaskDump
+    task: TaskDumpV1
 
 
-class WorkflowDump(BaseModel):
+class WorkflowDumpV1(BaseModel):
     id: int
     name: str
     project_id: int
     timestamp_created: str
 
 
-class ResourceDump(BaseModel):
+class ResourceDumpV1(BaseModel):
     id: int
     path: str
     dataset_id: int
 
 
-class DatasetDump(BaseModel):
+class DatasetDumpV1(BaseModel):
     id: int
     name: str
     type: Optional[str]
     read_only: bool
-    resource_list: list[ResourceDump]
+    resource_list: list[ResourceDumpV1]
     project_id: int
     timestamp_created: str
```

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/json_schemas/manifest.json` & `fractal_server-2.0.0a0/fractal_server/app/schemas/json_schemas/manifest.json`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/manifest.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/v1/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydantic import root_validator
 from pydantic import validator
 
 
 __all__ = ("TaskManifestV1", "ManifestV1")
 
 
-class _TaskManifestBase(BaseModel):
+class _TaskManifestBaseV1(BaseModel):
     """
     Base class for `TaskManifestV1`.
 
     Represents a task within a manfest
 
     Attributes:
         name:
@@ -50,18 +50,18 @@
     output_type: str
     meta: Optional[dict[str, Any]] = Field(default_factory=dict)
     args_schema: Optional[dict[str, Any]]
     docs_info: Optional[str]
     docs_link: Optional[HttpUrl]
 
 
-TaskManifestType = TypeVar("TaskManifestType", bound=_TaskManifestBase)
+TaskManifestType = TypeVar("TaskManifestType", bound=_TaskManifestBaseV1)
 
 
-class _ManifestBase(BaseModel):
+class _ManifestBaseV1(BaseModel):
     """
     Base class for `ManifestV1`.
 
     Packages containing tasks are required to include a special file
     `__FRACTAL_MANIFEST__.json` in order to be discovered and used by Fractal.
 
     This model class and the model classes it depends on provide the base
@@ -98,23 +98,23 @@
                     raise ValueError(
                         f'has_args_schemas={has_args_schemas} but task "'
                         f'{task.name}" has args_schema={task.args_schema}.'
                     )
         return values
 
 
-class TaskManifestV1(_TaskManifestBase):
+class TaskManifestV1(_TaskManifestBaseV1):
     """
     Task manifest schema version 1.
     """
 
     pass
 
 
-class ManifestV1(_ManifestBase):
+class ManifestV1(_ManifestBaseV1):
     """
     Manifest schema version 1.
 
     Attributes:
         task_list:
     """
```

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/project.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/v1/project.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from datetime import datetime
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import validator
 
-from ._validators import valstr
-from ._validators import valutc
+from .._validators import valstr
+from .._validators import valutc
 
 
 __all__ = (
-    "ProjectCreate",
-    "ProjectRead",
-    "ProjectUpdate",
+    "ProjectCreateV1",
+    "ProjectReadV1",
+    "ProjectUpdateV1",
 )
 
 
-class _ProjectBase(BaseModel):
+class _ProjectBaseV1(BaseModel):
     """
     Base class for `Project`.
 
     Attributes:
         name:
         read_only:
     """
 
     name: str
     read_only: bool = False
 
 
-class ProjectCreate(_ProjectBase):
+class ProjectCreateV1(_ProjectBaseV1):
     """
     Class for `Project` creation.
     """
 
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
 
 
-class ProjectRead(_ProjectBase):
+class ProjectReadV1(_ProjectBaseV1):
     """
     Class for `Project` read from database.
 
     Attributes:
         id:
         name:
         read_only:
@@ -51,15 +51,15 @@
     timestamp_created: datetime
 
     _timestamp_created = validator("timestamp_created", allow_reuse=True)(
         valutc("timestamp_created")
     )
 
 
-class ProjectUpdate(_ProjectBase):
+class ProjectUpdateV1(_ProjectBaseV1):
     """
     Class for `Project` update.
 
     Attributes:
         name:
         read_only:
     """
```

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/state.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/task.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/v1/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import HttpUrl
 from pydantic import validator
 
-from ._validators import valstr
+from .._validators import valstr
 
 __all__ = (
-    "TaskCreate",
-    "TaskUpdate",
-    "TaskRead",
-    "TaskImport",
-    "TaskExport",
+    "TaskCreateV1",
+    "TaskUpdateV1",
+    "TaskReadV1",
+    "TaskImportV1",
+    "TaskExportV1",
 )
 
 
-class _TaskBase(BaseModel):
+class _TaskBaseV1(BaseModel):
     """
 
     Base class for `Task`.
 
     Attributes:
         source:
             This is the information is used to match tasks across fractal
             installations when a workflow is imported.
     """
 
     source: str
     _source = validator("source", allow_reuse=True)(valstr("source"))
 
 
-class TaskUpdate(_TaskBase):
+class TaskUpdateV1(_TaskBaseV1):
     """
     Class for `Task` update.
 
     Attributes:
         name:
         input_type:
         output_type:
@@ -72,31 +72,31 @@
     )
     _command = validator("command", allow_reuse=True)(valstr("command"))
     _version = validator("version", allow_reuse=True)(
         valstr("version", accept_none=True)
     )
 
 
-class TaskImport(_TaskBase):
+class TaskImportV1(_TaskBaseV1):
     """
     Class for `Task` import.
     """
 
     pass
 
 
-class TaskExport(_TaskBase):
+class TaskExportV1(_TaskBaseV1):
     """
     Class for `Task` export.
     """
 
     pass
 
 
-class TaskRead(_TaskBase):
+class TaskReadV1(_TaskBaseV1):
     """
     Class for `Task` read from database.
 
     Attributes:
         id:
         name:
         command:
@@ -120,15 +120,15 @@
     version: Optional[str]
     args_schema: Optional[dict[str, Any]]
     args_schema_version: Optional[str]
     docs_info: Optional[str]
     docs_link: Optional[HttpUrl]
 
 
-class TaskCreate(_TaskBase):
+class TaskCreateV1(_TaskBaseV1):
     """
     Class for `Task` creation.
 
     Attributes:
         name:
         command:
         input_type:
```

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/task_collection.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/v1/task_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from typing import Literal
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from ._validators import valstr
-from .task import TaskRead
+from .._validators import valstr
+from .task import TaskReadV1
 
 __all__ = (
-    "TaskCollectPip",
-    "TaskCollectStatus",
+    "TaskCollectPipV1",
+    "TaskCollectStatusV1",
 )
 
 
-class TaskCollectPip(BaseModel):
+class TaskCollectPipV1(BaseModel):
     """
     TaskCollectPip class
 
     This class only encodes the attributes required to trigger a
     task-collection operation. Other attributes (that are assigned *during*
     task collection) are defined as part of fractal-server.
 
@@ -77,15 +77,15 @@
         if values["package"].endswith(".whl"):
             raise ValueError(
                 "Cannot provide version when package is a Wheel file."
             )
         return v
 
 
-class TaskCollectStatus(BaseModel):
+class TaskCollectStatusV1(BaseModel):
     """
     TaskCollectStatus class
 
     Attributes:
         status:
         package:
         venv_path:
@@ -93,15 +93,15 @@
         log:
         info:
     """
 
     status: Literal["pending", "installing", "collecting", "fail", "OK"]
     package: str
     venv_path: Path
-    task_list: Optional[list[TaskRead]] = Field(default=[])
+    task_list: Optional[list[TaskReadV1]] = Field(default=[])
     log: Optional[str]
     info: Optional[str]
 
     def sanitised_dict(self):
         """
         Return `self.dict()` after casting `self.venv_path` to a string
         """
```

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/user.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/app/schemas/workflow.py` & `fractal_server-2.0.0a0/fractal_server/app/schemas/v1/workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,60 +2,60 @@
 from enum import Enum
 from typing import Any
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import validator
 
-from ._validators import valint
-from ._validators import valstr
-from ._validators import valutc
-from .project import ProjectRead
-from .task import TaskExport
-from .task import TaskImport
-from .task import TaskRead
+from .._validators import valint
+from .._validators import valstr
+from .._validators import valutc
+from .project import ProjectReadV1
+from .task import TaskExportV1
+from .task import TaskImportV1
+from .task import TaskReadV1
 
 __all__ = (
-    "WorkflowCreate",
-    "WorkflowRead",
-    "WorkflowUpdate",
-    "WorkflowImport",
-    "WorkflowExport",
-    "WorkflowTaskCreate",
-    "WorkflowTaskImport",
-    "WorkflowTaskExport",
-    "WorkflowTaskRead",
-    "WorkflowTaskUpdate",
-    "WorkflowTaskStatusType",
+    "WorkflowCreateV1",
+    "WorkflowReadV1",
+    "WorkflowUpdateV1",
+    "WorkflowImportV1",
+    "WorkflowExportV1",
+    "WorkflowTaskCreateV1",
+    "WorkflowTaskImportV1",
+    "WorkflowTaskExportV1",
+    "WorkflowTaskReadV1",
+    "WorkflowTaskUpdateV1",
+    "WorkflowTaskStatusTypeV1",
 )
 
 
-class _WorkflowTaskBase(BaseModel):
+class _WorkflowTaskBaseV1(BaseModel):
     """
     Base class for `WorkflowTask`.
     """
 
     meta: Optional[dict[str, Any]] = None
     args: Optional[dict[str, Any]] = None
 
 
-class WorkflowTaskCreate(_WorkflowTaskBase):
+class WorkflowTaskCreateV1(_WorkflowTaskBaseV1):
     """
     Class for `WorkflowTask` creation.
 
     Attributes:
         order:
     """
 
     order: Optional[int]
     # Validators
     _order = validator("order", allow_reuse=True)(valint("order", min_val=0))
 
 
-class WorkflowTaskRead(_WorkflowTaskBase):
+class WorkflowTaskReadV1(_WorkflowTaskBaseV1):
     """
     Class for `WorkflowTask` read from database.
 
     Attributes:
         id:
         order:
         workflow_id:
@@ -63,97 +63,97 @@
         task:
     """
 
     id: int
     order: Optional[int]
     workflow_id: int
     task_id: int
-    task: TaskRead
+    task: TaskReadV1
 
 
-class WorkflowTaskImport(_WorkflowTaskBase):
+class WorkflowTaskImportV1(_WorkflowTaskBaseV1):
     """
     Class for `WorkflowTask` import.
 
     Attributes:
         task:
     """
 
-    task: TaskImport
+    task: TaskImportV1
 
 
-class WorkflowTaskExport(_WorkflowTaskBase):
+class WorkflowTaskExportV1(_WorkflowTaskBaseV1):
     """
     Class for `WorkflowTask` export.
 
     Attributes:
         task:
     """
 
-    task: TaskExport
+    task: TaskExportV1
 
 
-class WorkflowTaskUpdate(_WorkflowTaskBase):
+class WorkflowTaskUpdateV1(_WorkflowTaskBaseV1):
     """
     Class for `WorkflowTask` update.
     """
 
     # Validators
     @validator("meta")
     def check_no_parallelisation_level(cls, m):
         if "parallelization_level" in m:
             raise ValueError(
                 "Overriding task parallelization level currently not allowed"
             )
         return m
 
 
-class _WorkflowBase(BaseModel):
+class _WorkflowBaseV1(BaseModel):
     """
     Base class for `Workflow`.
 
     Attributes:
         name: Workflow name.
     """
 
     name: str
 
 
-class WorkflowRead(_WorkflowBase):
+class WorkflowReadV1(_WorkflowBaseV1):
     """
     Task for `Workflow` read from database.
 
     Attributes:
         id:
         project_id:
         task_list:
         project:
     """
 
     id: int
     project_id: int
-    task_list: list[WorkflowTaskRead]
-    project: ProjectRead
+    task_list: list[WorkflowTaskReadV1]
+    project: ProjectReadV1
     timestamp_created: datetime
 
     _timestamp_created = validator("timestamp_created", allow_reuse=True)(
         valutc("timestamp_created")
     )
 
 
-class WorkflowCreate(_WorkflowBase):
+class WorkflowCreateV1(_WorkflowBaseV1):
     """
     Task for `Workflow` creation.
     """
 
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
 
 
-class WorkflowUpdate(_WorkflowBase):
+class WorkflowUpdateV1(_WorkflowBaseV1):
     """
     Task for `Workflow` update.
 
     Attributes:
         name:
         reordered_workflowtask_ids:
     """
@@ -169,40 +169,40 @@
         if any(i < 0 for i in value):
             raise ValueError("Negative `id` in `reordered_workflowtask_ids`")
         if len(value) != len(set(value)):
             raise ValueError("`reordered_workflowtask_ids` has repetitions")
         return value
 
 
-class WorkflowImport(_WorkflowBase):
+class WorkflowImportV1(_WorkflowBaseV1):
     """
     Class for `Workflow` import.
 
     Attributes:
         task_list:
     """
 
-    task_list: list[WorkflowTaskImport]
+    task_list: list[WorkflowTaskImportV1]
 
     # Validators
     _name = validator("name", allow_reuse=True)(valstr("name"))
 
 
-class WorkflowExport(_WorkflowBase):
+class WorkflowExportV1(_WorkflowBaseV1):
     """
     Class for `Workflow` export.
 
     Attributes:
         task_list:
     """
 
-    task_list: list[WorkflowTaskExport]
+    task_list: list[WorkflowTaskExportV1]
 
 
-class WorkflowTaskStatusType(str, Enum):
+class WorkflowTaskStatusTypeV1(str, Enum):
     """
     Define the available values for the status of a `WorkflowTask`.
 
     This model is used within the `Dataset.history` attribute, which is
     constructed in the runner and then used in the API (e.g. in the
     `api/v1/project/{project_id}/dataset/{dataset_id}/status` endpoint).
```

### Comparing `fractal_server-1.4.9/fractal_server/app/security/__init__.py` & `fractal_server-2.0.0a0/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/config.py` & `fractal_server-2.0.0a0/fractal_server/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,35 +386,30 @@
         if not self.FRACTAL_RUNNER_WORKING_BASE_DIR:
             raise FractalConfigurationError(
                 "FRACTAL_RUNNER_WORKING_BASE_DIR cannot be None."
             )
 
         info = f"FRACTAL_RUNNER_BACKEND={self.FRACTAL_RUNNER_BACKEND}"
         if self.FRACTAL_RUNNER_BACKEND == "slurm":
-            try:
-                import cfut  # noqa: F401
-            except ModuleNotFoundError:
-                raise FractalConfigurationError(
-                    f"{info} but `clusterfutures` is not available"
-                )
+
+            from fractal_server.app.runner.executors.slurm._slurm_config import (  # noqa: E501
+                load_slurm_config_file,
+            )
+
             if not self.FRACTAL_SLURM_CONFIG_FILE:
                 raise FractalConfigurationError(
                     f"Must set FRACTAL_SLURM_CONFIG_FILE when {info}"
                 )
             else:
                 if not self.FRACTAL_SLURM_CONFIG_FILE.exists():
                     raise FractalConfigurationError(
                         f"{info} but FRACTAL_SLURM_CONFIG_FILE="
                         f"{self.FRACTAL_SLURM_CONFIG_FILE} not found."
                     )
 
-                from fractal_server.app.runner._slurm._slurm_config import (
-                    load_slurm_config_file,
-                )
-
                 load_slurm_config_file(self.FRACTAL_SLURM_CONFIG_FILE)
                 if not shutil.which("sbatch"):
                     raise FractalConfigurationError(
                         f"{info} but `sbatch` command not found."
                     )
                 if not shutil.which("squeue"):
                     raise FractalConfigurationError(
```

### Comparing `fractal_server-1.4.9/fractal_server/logger.py` & `fractal_server-2.0.0a0/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/main.py` & `fractal_server-2.0.0a0/fractal_server/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,21 +28,29 @@
 
     Args:
         app:
             The application to register the routers to.
     """
     from .app.routes.api import router_api
     from .app.routes.api.v1 import router_api_v1
-    from .app.routes.admin import router_admin
+    from .app.routes.api.v2 import router_api_v2
+    from .app.routes.admin.v1 import router_admin_v1
+    from .app.routes.admin.v2 import router_admin_v2
     from .app.routes.auth import router_auth
 
     app.include_router(router_api, prefix="/api")
     app.include_router(router_api_v1, prefix="/api/v1")
-    app.include_router(router_admin, prefix="/admin", tags=["Admin area"])
-    app.include_router(router_auth, prefix="/auth", tags=["auth"])
+    app.include_router(router_api_v2, prefix="/api/v2")
+    app.include_router(
+        router_admin_v1, prefix="/admin/v1", tags=["V1 Admin area"]
+    )
+    app.include_router(
+        router_admin_v2, prefix="/admin/v2", tags=["V2 Admin area"]
+    )
+    app.include_router(router_auth, prefix="/auth", tags=["Authentication"])
 
 
 def check_settings() -> None:
     """
     Check and register the settings
 
     Verify the consistency of the settings, in particular that required
```

### Comparing `fractal_server-1.4.9/fractal_server/migrations/env.py` & `fractal_server-2.0.0a0/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/script.py.mako` & `fractal_server-2.0.0a0/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-2.0.0a0/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/syringe.py` & `fractal_server-2.0.0a0/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/fractal_server/tasks/_TaskCollectPip.py` & `fractal_server-2.0.0a0/fractal_server/tasks/v1/_TaskCollectPip.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 from typing import Optional
 
 from pydantic import root_validator
 
-from fractal_server.app.schemas import ManifestV1
-from fractal_server.app.schemas import TaskCollectPip
+from fractal_server.app.schemas.v1 import ManifestV1
+from fractal_server.app.schemas.v1 import TaskCollectPipV1
 
 
-class _TaskCollectPip(TaskCollectPip):
+class _TaskCollectPip(TaskCollectPipV1):
     """
     Internal TaskCollectPip schema
 
     Differences with its parent class (`TaskCollectPip`):
 
         1. We check if the package corresponds to a path in the filesystem, and
            whether it exists (via new validator `check_local_package`, new
```

### Comparing `fractal_server-1.4.9/fractal_server/tasks/background_operations.py` & `fractal_server-2.0.0a0/fractal_server/tasks/v1/background_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,35 @@
 """
 The main function exported from this module is `background_collect_pip`, which
 is used as a background task for the task-collection endpoint.
 """
 import json
 from pathlib import Path
 from shutil import rmtree as shell_rmtree
-from typing import Optional
 
+from ..utils import _init_venv
+from ..utils import _normalize_package_name
+from ..utils import get_collection_log
+from ..utils import get_collection_path
+from ..utils import get_log_path
+from ..utils import slugify_task_name
+from ._TaskCollectPip import _TaskCollectPip
 from fractal_server.app.db import DBSyncSession
 from fractal_server.app.db import get_sync_db
 from fractal_server.app.models import State
 from fractal_server.app.models import Task
-from fractal_server.app.schemas import TaskCollectStatus
-from fractal_server.app.schemas import TaskCreate
-from fractal_server.app.schemas import TaskRead
+from fractal_server.app.schemas.v1 import TaskCollectStatusV1
+from fractal_server.app.schemas.v1 import TaskCreateV1
+from fractal_server.app.schemas.v1 import TaskReadV1
 from fractal_server.logger import close_logger
 from fractal_server.logger import get_logger
 from fractal_server.logger import set_logger
-from fractal_server.tasks._TaskCollectPip import _TaskCollectPip
-from fractal_server.tasks.utils import _normalize_package_name
-from fractal_server.tasks.utils import get_collection_log
-from fractal_server.tasks.utils import get_collection_path
-from fractal_server.tasks.utils import get_log_path
-from fractal_server.tasks.utils import get_python_interpreter
-from fractal_server.tasks.utils import slugify_task_name
 from fractal_server.utils import execute_command
 
 
-async def _init_venv(
-    *,
-    path: Path,
-    python_version: Optional[str] = None,
-    logger_name: str,
-) -> Path:
-    """
-    Set a virtual environment at `path/venv`
-
-    Args:
-        path : Path
-            path to directory in which to set up the virtual environment
-        python_version : default=None
-            Python version the virtual environment will be based upon
-
-    Returns:
-        python_bin : Path
-            path to python interpreter
-    """
-    logger = get_logger(logger_name)
-    logger.debug(f"[_init_venv] {path=}")
-    interpreter = get_python_interpreter(version=python_version)
-    logger.debug(f"[_init_venv] {interpreter=}")
-    await execute_command(
-        cwd=path,
-        command=f"{interpreter} -m venv venv",
-        logger_name=logger_name,
-    )
-    python_bin = path / "venv/bin/python"
-    logger.debug(f"[_init_venv] {python_bin=}")
-    return python_bin
-
-
 async def _pip_install(
     venv_path: Path,
     task_pkg: _TaskCollectPip,
     logger_name: str,
 ) -> Path:
     """
     Install package in venv
@@ -214,15 +180,15 @@
 
 
 async def create_package_environment_pip(
     *,
     task_pkg: _TaskCollectPip,
     venv_path: Path,
     logger_name: str,
-) -> list[TaskCreate]:
+) -> list[TaskCreateV1]:
     """
     Create environment, install package, and prepare task list
     """
 
     logger = get_logger(logger_name)
 
     # Normalize package name
@@ -259,15 +225,15 @@
             manifest = task_pkg.package_manifest
             if manifest.has_args_schemas:
                 additional_attrs = dict(
                     args_schema_version=manifest.args_schema_version
                 )
             else:
                 additional_attrs = {}
-            this_task = TaskCreate(
+            this_task = TaskCreateV1(
                 **t.dict(),
                 command=cmd,
                 version=task_pkg.package_version,
                 **additional_attrs,
                 source=task_source,
             )
             task_list.append(this_task)
@@ -275,15 +241,15 @@
     except Exception as e:
         logger.error("Task manifest loading failed")
         raise e
     return task_list
 
 
 async def _insert_tasks(
-    task_list: list[TaskCreate],
+    task_list: list[TaskCreateV1],
     db: DBSyncSession,
 ) -> list[Task]:
     """
     Insert tasks into database
     """
     task_db_list = [Task(**t.dict()) for t in task_list]
     db.add_all(task_db_list)
@@ -315,15 +281,15 @@
     )
     logger.debug("Start background task collection")
     for key, value in task_pkg.dict(exclude={"package_manifest"}).items():
         logger.debug(f"{key}: {value}")
 
     with next(get_sync_db()) as db:
         state: State = db.get(State, state_id)
-        data = TaskCollectStatus(**state.data)
+        data = TaskCollectStatusV1(**state.data)
         data.info = None
 
         try:
             # install
             logger.debug("Task-collection status: installing")
             data.status = "installing"
 
@@ -343,17 +309,19 @@
             db.merge(state)
             db.commit()
             tasks = await _insert_tasks(task_list=task_list, db=db)
 
             # finalise
             logger.debug("Task-collection status: finalising")
             collection_path = get_collection_path(venv_path)
-            data.task_list = [TaskRead(**task.model_dump()) for task in tasks]
+            data.task_list = [
+                TaskReadV1(**task.model_dump()) for task in tasks
+            ]
             with collection_path.open("w") as f:
-                json.dump(data.sanitised_dict(), f)
+                json.dump(data.sanitised_dict(), f, indent=2)
 
             # Update DB
             data.status = "OK"
             data.log = get_collection_log(venv_path)
             state.data = data.sanitised_dict()
             db.add(state)
             db.merge(state)
```

### Comparing `fractal_server-1.4.9/fractal_server/tasks/endpoint_operations.py` & `fractal_server-2.0.0a0/fractal_server/tasks/endpoint_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 import json
 from pathlib import Path
 from typing import Optional
 from typing import Union
 from zipfile import ZipFile
 
-from fractal_server.app.schemas import ManifestV1
-from fractal_server.app.schemas import TaskCollectStatus
+from .utils import _normalize_package_name
+from .utils import get_python_interpreter
+from .v1._TaskCollectPip import _TaskCollectPip as _TaskCollectPipV1
+from .v2._TaskCollectPip import _TaskCollectPip as _TaskCollectPipV2
+from fractal_server.app.schemas.v1 import ManifestV1
+from fractal_server.app.schemas.v2 import ManifestV2
 from fractal_server.config import get_settings
 from fractal_server.logger import get_logger
 from fractal_server.syringe import Inject
-from fractal_server.tasks._TaskCollectPip import _TaskCollectPip
-from fractal_server.tasks.utils import _normalize_package_name
-from fractal_server.tasks.utils import get_absolute_venv_path
-from fractal_server.tasks.utils import get_collection_path
-from fractal_server.tasks.utils import get_python_interpreter
 from fractal_server.utils import execute_command
 
 
 FRACTAL_PUBLIC_TASK_SUBDIR = ".fractal"
 
 
-def get_collection_data(venv_path: Path) -> TaskCollectStatus:
-    package_path = get_absolute_venv_path(venv_path)
-    collection_path = get_collection_path(package_path)
-    with collection_path.open() as f:
-        data = json.load(f)
-    return TaskCollectStatus(**data)
-
-
 async def download_package(
     *,
-    task_pkg: _TaskCollectPip,
+    task_pkg: Union[_TaskCollectPipV1, _TaskCollectPipV2],
     dest: Union[str, Path],
-):
+) -> Path:
     """
     Download package to destination
     """
     interpreter = get_python_interpreter(version=task_pkg.python_version)
     pip = f"{interpreter} -m pip"
     version = (
         f"=={task_pkg.package_version}" if task_pkg.package_version else ""
@@ -48,15 +39,15 @@
         line.split()[-1] for line in stdout.split("\n") if "Saved" in line
     )
     return Path(pkg_file)
 
 
 def _load_manifest_from_wheel(
     path: Path, wheel: ZipFile, logger_name: Optional[str] = None
-) -> ManifestV1:
+) -> Union[ManifestV1, ManifestV2]:
     logger = get_logger(logger_name)
     namelist = wheel.namelist()
     try:
         manifest = next(
             name for name in namelist if "__FRACTAL_MANIFEST__.json" in name
         )
     except StopIteration:
@@ -65,14 +56,17 @@
         raise ValueError(msg)
     with wheel.open(manifest) as manifest_fd:
         manifest_dict = json.load(manifest_fd)
     manifest_version = str(manifest_dict["manifest_version"])
     if manifest_version == "1":
         pkg_manifest = ManifestV1(**manifest_dict)
         return pkg_manifest
+    elif manifest_version == "2":
+        pkg_manifest = ManifestV2(**manifest_dict)
+        return pkg_manifest
     else:
         msg = f"Manifest version {manifest_version=} not supported"
         logger.error(msg)
         raise ValueError(msg)
 
 
 def inspect_package(path: Path, logger_name: Optional[str] = None) -> dict:
@@ -142,15 +136,15 @@
         pkg_manifest=pkg_manifest,
     )
     return info
 
 
 def create_package_dir_pip(
     *,
-    task_pkg: _TaskCollectPip,
+    task_pkg: Union[_TaskCollectPipV1, _TaskCollectPipV2],
     create: bool = True,
 ) -> Path:
     """
     Create venv folder for a task package and return corresponding Path object
     """
     settings = Inject(get_settings)
     user = FRACTAL_PUBLIC_TASK_SUBDIR
```

### Comparing `fractal_server-1.4.9/fractal_server/utils.py` & `fractal_server-2.0.0a0/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.4.9/pyproject.toml` & `fractal_server-2.0.0a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.4.9"
+version = "2.0.0a0"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -30,24 +30,22 @@
 aiosqlite = "^0.19.0"
 fastapi-users = {extras = ["oauth"], version = "^12.1.0"}
 alembic = "^1.9.1"
 uvicorn = "^0.27.0"
 pydantic = ">=1.10.8,<2"
 bcrypt = "4.0.1"
 packaging = "^23.2"
-
-clusterfutures = { version = "^0.5", optional = true}
-cloudpickle = {version = ">=2.2.1,<2.3.0", optional = true}
+clusterfutures = "^0.5"
+cloudpickle = ">=2.2.1,<2.3.0"
 
 asyncpg = { version = "^0.29.0", optional = true }
 psycopg2 = { version = "^2.9.5", optional = true }
 gunicorn = { version = "^21.2.0", optional = true }
 
 [tool.poetry.extras]
-slurm = ["clusterfutures", "cloudpickle"]
 postgres = ["asyncpg", "psycopg2"]
 gunicorn = ["gunicorn"]
 
 [tool.poetry.group.dev.dependencies]
 asgi-lifespan = "^2"
 pytest = "^7.2"
 httpx = "^0.23"
@@ -83,15 +81,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.4.9"
+current_version = "2.0.0a0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.4.9/PKG-INFO` & `fractal_server-2.0.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.4.9
+Version: 2.0.0a0
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: gunicorn
 Provides-Extra: postgres
-Provides-Extra: slurm
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: alembic (>=1.9.1,<2.0.0)
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0) ; extra == "postgres"
 Requires-Dist: bcrypt (==4.0.1)
-Requires-Dist: cloudpickle (>=2.2.1,<2.3.0) ; extra == "slurm"
-Requires-Dist: clusterfutures (>=0.5,<0.6) ; extra == "slurm"
+Requires-Dist: cloudpickle (>=2.2.1,<2.3.0)
+Requires-Dist: clusterfutures (>=0.5,<0.6)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: fastapi-users[oauth] (>=12.1.0,<13.0.0)
 Requires-Dist: gunicorn (>=21.2.0,<22.0.0) ; extra == "gunicorn"
 Requires-Dist: packaging (>=23.2,<24.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "postgres"
 Requires-Dist: pydantic (>=1.10.8,<2)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
```

