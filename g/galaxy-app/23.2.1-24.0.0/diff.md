# Comparing `tmp/galaxy-app-23.2.1.tar.gz` & `tmp/galaxy-app-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/app/dist/.tmp-bf699zda/galaxy-app-23.2.1.tar", last modified: Thu Feb 22 03:56:47 2024, max compression
+gzip compressed data, was "galaxy-app-24.0.0.tar", last modified: Wed Apr  3 02:46:37 2024, max compression
```

## Comparing `galaxy-app-23.2.1.tar` & `galaxy-app-24.0.0.tar`

### file list

```diff
@@ -1,700 +1,707 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    45288 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    46626 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17546 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/actions/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    39152 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/app_unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/app_unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/app_unittest_utils/galaxy_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/app_unittest_utils/toolbox_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/app_unittest_utils/tools_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/authnz/
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/authnz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26328 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/authnz/custos_authnz.py
--rw-r--r--   0 runner    (1001) docker     (127)    25176 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/authnz/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/authnz/psa_authnz.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/authnz/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/carbon_emissions/
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/carbon_emissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/celery/
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/celery/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/celery/base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/celery/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/config_watchers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/dependencies/conditional-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/dependencies/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/dependencies/lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/dependencies/pinned-lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16176 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/dependencies/pinned-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/dependencies/pinned-typecheck-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3365 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/dependencies/update.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      820 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/dependencies/update_lint_requirements.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/di.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/forms/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)   121427 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/command_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73557 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/dynamic_tool_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    59025 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/rule_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/runners/
--rw-r--r--   0 runner    (1001) docker     (127)    39944 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23005 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/chronos.py
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/condor.py
--rw-r--r--   0 runner    (1001) docker     (127)    21004 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/drmaa.py
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/godocker.py
--rw-r--r--   0 runner    (1001) docker     (127)    46391 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    23569 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55198 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/pulsar.py
--rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/state_handler_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/runners/state_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/state_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/state_handlers/_safe_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/state_handlers/resubmit.py
--rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    31766 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/univa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/slurm_torque.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/torque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/shell/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/shell/rsh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/condor/
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/fork_safe_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/job_script/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/job_script/CLUSTER_SLOTS_STATEMENT.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/job_script/MEMORY_STATEMENT_TEMPLATE.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/job_script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/kill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/process_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/pykube_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/runners/util/sudo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/jobs/splitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/splitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/splitters/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/splitters/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/jobs/stock_rules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9033 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/main_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/annotatable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    53424 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/citations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18890 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/cloudauthzs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38451 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/collections_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    38376 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/dbkeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/deletable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/display_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/export_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/folders.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/genomes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    28098 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/hdas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/hdcas.py
--rw-r--r--   0 runner    (1001) docker     (127)    36600 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    26904 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/history_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/interactivetool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/job_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    45014 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/lddas.py
--rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    12155 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/library_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)   185469 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/markdown_export_base.css
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/markdown_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    40402 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/markdown_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/model_stores.py
--rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    24240 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/quotas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/ratable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/rbac_secured.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/remote_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/secured.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    22208 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/sharable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/taggable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/tool_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    37516 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    97381 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/managers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/structured_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tool_shed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    46846 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/install_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    51727 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/installed_repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/metadata/installed_repository_metadata_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/repository_dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/repository_dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36467 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/repository_dependencies/repository_dependency_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/tools/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    27642 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/tools/tool_panel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/update_repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tool_shed/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55928 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/metadata/metadata_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/repository_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tool_shed/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/tools/data_table_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/tools/tool_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tool_shed/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/unittest_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/basic_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/container_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17652 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/dependency_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/hg_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/metadata_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    35443 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/repository_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/shed_util_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/tool_dependency_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/tool_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    38543 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tool_shed/util/utility_container_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/
--rw-r--r--   0 runner    (1001) docker     (127)   169861 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/actions/
--rw-r--r--   0 runner    (1001) docker     (127)    60863 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/actions/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/actions/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/actions/history_imp_exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/actions/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/actions/model_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/actions/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    19147 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/actions/upload_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/apply_rules.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/biotools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/build_list.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/build_list_1.2.0.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_export/
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_export/export_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_export/export_remote.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_export/send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_export/send.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/access_libraries.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/biomart.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/biomart_test.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/cbi_rice_mart.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ebi_sra.xml
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/eupathdb.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/fly_modencode.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/flymine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/flymine_test.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/genbank.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/genbank.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/gramene_mart.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/hapmapmart.xml
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/hbvar.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/import.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/intermine.xml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/metabolicmine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/microbial_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/microbial_import.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/microbial_import_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/modmine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/mousemine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ncbi_datasets.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ratmine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/sra.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/upload.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/worm_modencode.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/wormbase.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/wormbase_test.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/yeastmine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/data_source/zebrafishmine.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/expression_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/expression_tools/expression_macros.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/expression_tools/parse_values_from_file.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16734 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/expression_tools/pick_value.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/extract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/extract/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12747 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/extract/extract_genomic_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/extract/extract_genomic_dna.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/extract/liftOver_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/extract/liftOver_wrapper.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/CreateInterval.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/CreateInterval.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_concat_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_concat_fasta.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_fasta.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_lav.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_lav.xml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_lav_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/bed2gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/bed_to_bigbed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/bed_to_gff_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/catWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/catWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/changeCase.pl
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/changeCase.xml
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/commWrapper.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/commWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/compare.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/condense_characters.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/condense_characters.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/convert_characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/convert_characters.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/cutWrapper.pl
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/cutWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/fileGrep.xml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/fixedValueColumn.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/fixedValueColumn.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/extract_GFF_Features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/extract_GFF_Features.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff2bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff_to_bed_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/grep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/grep.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/grep_1.0.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gtf2bedgraph.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/gtf_to_bedgraph_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/headWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/joinWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/joiner.xml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/joiner2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/lav_to_bed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/lav_to_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/lav_to_bed_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/mergeCols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/mergeCols.xml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/pasteWrapper.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/pasteWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/random_lines_two_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/randomlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/randomlines.xml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/remove_beginning.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/remove_beginning.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/secure_hash_message_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/secure_hash_message_digest.xml
--rw-r--r--   0 runner    (1001) docker     (127)    46787 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/sff_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/sff_extractor.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/sorter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/tailWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/trimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/trimmer.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2707 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     4410 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/uniq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/uniq.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/wc_gnu.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/wig_to_bigwig.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)      919 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/wiggle_to_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/filters/wiggle_to_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/default_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_askomics.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_bam_iobio.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_cellxgene_0.16.2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_cellxgene_1.1.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_climate_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_ethercalc.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_geoexplorer.xml
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_guacamole_desktop.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_hicbrowser.xml
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_higlass.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_isee.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16488 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook_1.0.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_metashark.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_mgnify_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15412 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_ml_jupyter_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_neo4j.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_openrefine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_pangeo_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_panoply.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_paraview.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_pavian.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_phinch.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_pyiron.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_radiant.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_simtext_app.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_vcf_iobio.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_vrm_editor.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_wallace.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_wilson.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28382 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/interactive/simtext_app.R
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/genebed_maf_to_fasta.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6278 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval2maf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19538 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval2maf.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval2maf_pairwise.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.xml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/macros.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_by_block_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_by_block_number.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_filter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_limit_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_limit_size.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_limit_to_species.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_limit_to_species.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_reverse_complement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_reverse_complement.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_split_by_species.py
--rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_split_by_species.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_stats.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_thread_for_species.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_thread_for_species.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_bed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_bed_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_fasta.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2018 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_fasta_concat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2116 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_fasta_multiple_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_interval.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/meme/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/meme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/meme/fimo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/meme/fimo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16909 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/meme/meme.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/blat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/blat_wrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/shrimp_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/shrimp_wrapper.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2627 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/bwa_solid2fastq_modified.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/solid2fastq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/solid2fastq.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/ngs_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/ngs_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/ngs_simulation/ngs_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/ngs_simulation/ngs_simulation.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1331 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/BEAM2_wrapper.sh
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/beam.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2033 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/gpass.pl
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/gpass.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/ldtools.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1000 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/ldtools_wrapper.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/linkToDavid.pl
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/linkToDavid.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2713 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/linkToGProfile.pl
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/linkToGProfile.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     3346 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/lped_to_geno.pl
--rw-r--r--   0 runner    (1001) docker     (127)    15041 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/lps.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/lps_tool_wrapper.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     7394 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/master2gd_snp.pl
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/master2gd_snp.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     4319 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/master2pg.pl
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/master2pg.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1389 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/mergeSnps.pl
--rwxr-xr-x   0 runner    (1001) docker     (127)     9287 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/pagetag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/pass.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/pass_wrapper.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     7131 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/senatag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/sift.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     5328 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/sift_variants_wrapper.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/plotting/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/plotting/bar_chart.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/plotting/boxplot.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper_code.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3011 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/qualsolid_boxplot_graph.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/solid_qual_boxplot.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/solid_qual_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/solid_qual_stats.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17496 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/velvetg.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/velvetg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/velveth.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/velveth_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)    19821 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/PerM.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/bfast_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/bfast_wrapper.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     4977 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/fastq_statistics.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/mosaik.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/srma_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/srma_wrapper.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/aggregate_binned_scores_in_intervals.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     8793 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/aggregate_scores_in_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/filtering.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/filtering_1_1_0.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/grouping.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     5492 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/gsummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/gsummary.xml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/bundled/stats/r_wrapper.sh
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/data/
--rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/data_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/data_fetch.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/data_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/data_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/data_manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/duplicate_file_to_collection.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/base_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/github.py
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    38985 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    28105 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/expressions/cwlNodeEngine.js
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/expressions/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/expressions/script.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/expressions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/extract_dataset.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/filter_empty_collection.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/filter_failed_collection.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/filter_from_file.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/flatten_collection.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/imp_exp/
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/imp_exp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/imp_exp/exp_history_to_archive.xml
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/imp_exp/exp_history_to_uri.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/imp_exp/export_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/imp_exp/imp_history_from_archive.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/imp_exp/unpack_tar_gz_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/merge_collection.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)    26963 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   118925 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/dataset_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    32051 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/dynamic_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    35768 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/history_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/input_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)    24116 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/parameters/wrapped_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/relabel_from_file.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/remote_tool_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/search/
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/sort_collection_list.xml
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/special_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/tag_collection_from_file.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17910 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/unzip_collection.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/tools/util/galaxyops/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/util/galaxyops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30760 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/util/maf_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    30195 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/tools/zip_collection.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/cigar.py
--rw-r--r--   0 runner    (1001) docker     (127)    62312 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/genome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/baseparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/newickparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/nexusparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/phyloxmlparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/data_providers/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/visualization/genome/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/genome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14825 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/genomes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/visualization/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21974 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/plugins/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12820 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/plugins/resource_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/visualization/tracks/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/visualization/tracks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/webhooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/work/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/work/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/work/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18691 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)   114853 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/workflow/refactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/refactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28877 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/refactor/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/refactor/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/workflow/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/workflow/reports/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/reports/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/reports/generators/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/workflow/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/resources/example.py.sample
--rw-r--r--   0 runner    (1001) docker     (127)    31649 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    30497 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/run_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy/workflow/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/schedulers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17008 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/scheduling_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy/workflow/trs_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46626 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26166 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_app.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_ext/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy_ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_ext/container_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy_ext/container_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy_ext/container_monitor/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_ext/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy_ext/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy_ext/expressions/handle_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/galaxy_ext/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy_ext/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy_ext/metadata/set_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/galaxy_ext/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/tool_shed_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/tool_shed_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/tool_shed_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:56:47.000000 galaxy-app-23.2.1/tool_shed_client/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/tool_shed_client/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/tool_shed_client/schema/trs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/tool_shed_client/schema/trs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-22 03:50:43.000000 galaxy-app-23.2.1/tool_shed_client/trs_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    58057 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    60604 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.432251 galaxy-app-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.432251 galaxy-app-24.0.0/galaxy/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17523 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/actions/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38970 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.432251 galaxy-app-24.0.0/galaxy/app_unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app_unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app_unittest_utils/galaxy_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app_unittest_utils/toolbox_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app_unittest_utils/tools_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/authnz/
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29236 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/custos_authnz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27994 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/psa_authnz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/carbon_emissions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/carbon_emissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/celery/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/celery/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17119 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/celery/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/config_watchers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/conditional-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/pinned-lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16149 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/pinned-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/pinned-typecheck-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3373 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/update.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      721 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/update_lint_requirements.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/di.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12593 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/forms/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.440251 galaxy-app-24.0.0/galaxy/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)   121947 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/command_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73578 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/dynamic_tool_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59027 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/rule_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.440251 galaxy-app-24.0.0/galaxy/jobs/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)    40111 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22955 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/chronos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20985 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/drmaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/godocker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56110 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23554 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55187 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/state_handler_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/_safe_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31764 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/univa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/slurm_torque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/torque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.448252 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/rsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.448252 galaxy-app-24.0.0/galaxy/jobs/runners/util/condor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/fork_safe_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.448252 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/CLUSTER_SLOTS_STATEMENT.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/MEMORY_STATEMENT_TEMPLATE.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/process_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/pykube_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/sudo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.448252 galaxy-app-24.0.0/galaxy/jobs/splitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/splitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/splitters/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/splitters/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/stock_rules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9033 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/main_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/annotatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53644 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18890 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/cloudauthzs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38419 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/collections_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11780 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40089 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/dbkeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/deletable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/display_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/export_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/genomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28314 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/hdas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/hdcas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42387 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28357 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/interactivetool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/job_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45695 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/lddas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16788 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/library_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)   185469 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/markdown_export_base.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/markdown_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41485 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/markdown_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/model_stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24542 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/ratable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/rbac_secured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/remote_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/secured.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22209 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/sharable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/taggable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/tool_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38938 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98587 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/queues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/short_term_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/short_term_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/structured_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46846 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/install_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51730 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/installed_repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/metadata/installed_repository_metadata_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/repository_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/repository_dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36468 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/repository_dependencies/repository_dependency_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27537 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/tool_panel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/update_repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.464252 galaxy-app-24.0.0/galaxy/tool_shed/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55922 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/metadata/metadata_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/repository_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.464252 galaxy-app-24.0.0/galaxy/tool_shed/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/tools/data_table_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/tools/tool_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.464252 galaxy-app-24.0.0/galaxy/tool_shed/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/unittest_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.464252 galaxy-app-24.0.0/galaxy/tool_shed/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/basic_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/container_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17636 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/dependency_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/hg_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/metadata_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35443 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/repository_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/shed_util_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/tool_dependency_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/tool_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38555 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/utility_container_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.472252 galaxy-app-24.0.0/galaxy/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)   173796 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.472252 galaxy-app-24.0.0/galaxy/tools/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)    61141 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/history_imp_exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/model_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/upload_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/apply_rules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/biotools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/build_list.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/build_list_1.2.0.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.472252 galaxy-app-24.0.0/galaxy/tools/bundled/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.472252 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/export_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/export_remote.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/send.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.480252 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/access_libraries.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart_test.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/cbi_rice_mart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ebi_sra.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/eupathdb.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/fly_modencode.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine_test.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/genbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/genbank.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/gramene_mart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hapmapmart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hbvar.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/import.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/intermine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/metabolicmine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/modmine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/mousemine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ncbi_datasets.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ratmine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/sra.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/upload.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/worm_modencode.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase_test.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/yeastmine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/zebrafishmine.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.480252 galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/expression_macros.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/parse_values_from_file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16734 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/pick_value.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.480252 galaxy-app-24.0.0/galaxy/tools/bundled/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12747 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/extract_genomic_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/extract_genomic_dna.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/liftOver_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/liftOver_wrapper.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.496252 galaxy-app-24.0.0/galaxy/tools/bundled/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/CreateInterval.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/CreateInterval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_concat_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_concat_fasta.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_fasta.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed2gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed_to_bigbed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed_to_gff_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/catWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/catWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/changeCase.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/changeCase.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/commWrapper.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/commWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/compare.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/condense_characters.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/condense_characters.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/convert_characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/convert_characters.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/cutWrapper.pl
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/cutWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/fileGrep.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/fixedValueColumn.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/fixedValueColumn.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.496252 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/extract_GFF_Features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/extract_GFF_Features.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff2bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff_to_bed_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep_1.0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gtf2bedgraph.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gtf_to_bedgraph_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/headWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/joinWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/joiner.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/joiner2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/mergeCols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/mergeCols.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/pasteWrapper.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/pasteWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/random_lines_two_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/randomlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/randomlines.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/remove_beginning.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/remove_beginning.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/secure_hash_message_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/secure_hash_message_digest.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    46787 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/sff_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/sff_extractor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/sorter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/tailWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/trimmer.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2707 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4410 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/uniq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/uniq.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/wc_gnu.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/wig_to_bigwig.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      919 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/wiggle_to_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/wiggle_to_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.504252 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/default_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_askomics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_bam_iobio.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_cellxgene_0.16.2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_cellxgene_1.1.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_climate_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_ethercalc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_geoexplorer.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_guacamole_desktop.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_hicbrowser.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_higlass.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_isee.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16488 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook_1.0.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_metashark.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_mgnify_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15412 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_ml_jupyter_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_neo4j.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_openrefine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pangeo_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_panoply.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_paraview.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pavian.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_phinch.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pyiron.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_qiskit_jupyter_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_radiant.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_simtext_app.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_vcf_iobio.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_vrm_editor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_wallace.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_wilson.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28382 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/simtext_app.R
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.512252 galaxy-app-24.0.0/galaxy/tools/bundled/maf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/genebed_maf_to_fasta.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6278 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19538 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf_pairwise.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/macros.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_by_block_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_by_block_number.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_filter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_size.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_to_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_to_species.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_reverse_complement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_reverse_complement.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_split_by_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_split_by_species.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_stats.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_thread_for_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_thread_for_species.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2018 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta_concat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2116 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta_multiple_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_interval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.512252 galaxy-app-24.0.0/galaxy/tools/bundled/meme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/meme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/meme/fimo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/meme/fimo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16909 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/meme/meme.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.512252 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/blat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/blat_wrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_wrapper.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.516252 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2627 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/bwa_solid2fastq_modified.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid2fastq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid2fastq.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.516252 galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/ngs_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/ngs_simulation.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.520253 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1331 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/BEAM2_wrapper.sh
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/beam.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2033 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/gpass.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/gpass.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/ldtools.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1000 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/ldtools_wrapper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToDavid.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToDavid.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2713 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToGProfile.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToGProfile.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3346 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lped_to_geno.pl
+-rw-r--r--   0 runner    (1001) docker     (127)    15041 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lps.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lps_tool_wrapper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7394 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2gd_snp.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2gd_snp.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4319 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2pg.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2pg.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1389 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/mergeSnps.pl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9287 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pagetag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pass.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pass_wrapper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7131 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/senatag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/sift.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5328 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/sift_variants_wrapper.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.520253 galaxy-app-24.0.0/galaxy/tools/bundled/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/plotting/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/plotting/bar_chart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/plotting/boxplot.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.520253 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper_code.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3011 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/qualsolid_boxplot_graph.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_boxplot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_stats.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.524253 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17496 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velvetg.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velvetg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velveth.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velveth_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.524253 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)    19821 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/PerM.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/bfast_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/bfast_wrapper.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4977 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/fastq_statistics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/mosaik.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/srma_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/srma_wrapper.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/bundled/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/aggregate_binned_scores_in_intervals.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8793 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/aggregate_scores_in_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering_1_1_0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/grouping.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5492 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/gsummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/gsummary.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/r_wrapper.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24682 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data_fetch.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/data_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11221 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data_manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/duplicate_file_to_collection.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/error_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/base_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14012 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38958 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/cwlNodeEngine.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/extract_dataset.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/filter_empty_collection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/filter_failed_collection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/filter_from_file.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/flatten_collection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/harmonize_two_collections_list.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/imp_exp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/exp_history_to_archive.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/exp_history_to_uri.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/export_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/imp_history_from_archive.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/unpack_tar_gz_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/keep_success_collection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/merge_collection.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)    26963 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119986 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/cancelable_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/dataset_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38238 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/dynamic_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35745 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/history_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/input_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24117 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/workflow_building_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/wrapped_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16840 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/relabel_from_file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/remote_tool_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/search/
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/sort_collection_list.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/special_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/tag_collection_from_file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17886 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/unzip_collection.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/util/galaxyops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/util/galaxyops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30671 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/util/maf_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30444 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/zip_collection.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/data_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/cigar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62285 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/genome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/baseparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/newickparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/nexusparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/phyloxmlparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/genome/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/genomes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/resource_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/tracks/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/tracks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/webhooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/work/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/work/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/work/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18797 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114980 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/refactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/refactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28870 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/refactor/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/refactor/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/reports/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/reports/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/reports/generators/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/resources/example.py.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    31810 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30630 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/run_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/schedulers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17008 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/scheduling_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/trs_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    60604 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26467 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_ext/container_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/container_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/container_monitor/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_ext/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/expressions/handle_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_ext/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/metadata/set_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 02:46:37.548253 galaxy-app-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/tool_shed_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/tool_shed_client/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/schema/trs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/schema/trs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/trs_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-app-23.2.1/HISTORY.rst` & `galaxy-app-24.0.0/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,113 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Reload built-in converters on toolbox reload by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17209 <https://github.com/galaxyproject/galaxy/pull/17209>`_
+* Optional Reply-to SMTP header in tool error reports by `@neoformit <https://github.com/neoformit>`_ in `#17243 <https://github.com/galaxyproject/galaxy/pull/17243>`_
+* Package tests fixes by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17301 <https://github.com/galaxyproject/galaxy/pull/17301>`_
+* Follow-up on #17274 and #17262 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17302 <https://github.com/galaxyproject/galaxy/pull/17302>`_
+* Rollback invalidated transaction: catch them earlier by `@jdavcs <https://github.com/jdavcs>`_ in `#17312 <https://github.com/galaxyproject/galaxy/pull/17312>`_
+* Fixes for flake8-bugbear 24.1.17 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17340 <https://github.com/galaxyproject/galaxy/pull/17340>`_
+* Fix data_source and data_source_async bugs by `@wm75 <https://github.com/wm75>`_ in `#17422 <https://github.com/galaxyproject/galaxy/pull/17422>`_
+* More efficient change_state queries, maybe fix deadlock by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17632 <https://github.com/galaxyproject/galaxy/pull/17632>`_
+* Don't index tasks without task_uuid by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17646 <https://github.com/galaxyproject/galaxy/pull/17646>`_
+* Separate `ConnectedValue` from `RuntimeValue` by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17678 <https://github.com/galaxyproject/galaxy/pull/17678>`_
+* Fix step type serialization for StoredWorkflowDetailed models by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17716 <https://github.com/galaxyproject/galaxy/pull/17716>`_
+* Fix usage of DISTINCT by `@jdavcs <https://github.com/jdavcs>`_ in `#17759 <https://github.com/galaxyproject/galaxy/pull/17759>`_
+* Also set extension and metadata on copies of job outputs when finishing job by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17777 <https://github.com/galaxyproject/galaxy/pull/17777>`_
+* Use ``hg clone --stream`` to clone repos by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17786 <https://github.com/galaxyproject/galaxy/pull/17786>`_
+* Defer job attributes that are usually not needed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17795 <https://github.com/galaxyproject/galaxy/pull/17795>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+* Fix archived histories mixing with active in histories list by `@davelopez <https://github.com/davelopez>`_ in `#17856 <https://github.com/galaxyproject/galaxy/pull/17856>`_
+* Normalize extensions when loading tool by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17868 <https://github.com/galaxyproject/galaxy/pull/17868>`_
+* Ignore user data table errors for now by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17880 <https://github.com/galaxyproject/galaxy/pull/17880>`_
+
+============
+Enhancements
+============
+
+* Add harmonize collections tool (or whatever other name) by `@lldelisle <https://github.com/lldelisle>`_ in `#16662 <https://github.com/galaxyproject/galaxy/pull/16662>`_
+* Add support for Python 3.12 by `@tuncK <https://github.com/tuncK>`_ in `#16796 <https://github.com/galaxyproject/galaxy/pull/16796>`_
+* SQLAlchemy 2.0 upgrades (part 5) by `@jdavcs <https://github.com/jdavcs>`_ in `#16932 <https://github.com/galaxyproject/galaxy/pull/16932>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
+* Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
+* Add select parameter with options from remote resources by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17087 <https://github.com/galaxyproject/galaxy/pull/17087>`_
+*  Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
+* Vueify Admin Roles Grid by `@guerler <https://github.com/guerler>`_ in `#17118 <https://github.com/galaxyproject/galaxy/pull/17118>`_
+* SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17123 <https://github.com/galaxyproject/galaxy/pull/17123>`_
+* Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
+* Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
+* Vueify Admin Forms and Quota grids by `@guerler <https://github.com/guerler>`_ in `#17141 <https://github.com/galaxyproject/galaxy/pull/17141>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17157 <https://github.com/galaxyproject/galaxy/pull/17157>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17201 <https://github.com/galaxyproject/galaxy/pull/17201>`_
+* Vendorize fastapi-utls.cbv by `@jdavcs <https://github.com/jdavcs>`_ in `#17205 <https://github.com/galaxyproject/galaxy/pull/17205>`_
+* Fix usage of graphene-sqlalchemy, bump to 3.0.0rc1 by `@jdavcs <https://github.com/jdavcs>`_ in `#17216 <https://github.com/galaxyproject/galaxy/pull/17216>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17230 <https://github.com/galaxyproject/galaxy/pull/17230>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17235 <https://github.com/galaxyproject/galaxy/pull/17235>`_
+* Allow job files to consume TUS uploads by `@jmchilton <https://github.com/jmchilton>`_ in `#17242 <https://github.com/galaxyproject/galaxy/pull/17242>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17247 <https://github.com/galaxyproject/galaxy/pull/17247>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Consider Null inputs by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17271 <https://github.com/galaxyproject/galaxy/pull/17271>`_
+* Add OIDC backend configuration schema and validation by `@uwwint <https://github.com/uwwint>`_ in `#17274 <https://github.com/galaxyproject/galaxy/pull/17274>`_
+* Adds delete, purge and undelete batch operations to History Grid by `@guerler <https://github.com/guerler>`_ in `#17282 <https://github.com/galaxyproject/galaxy/pull/17282>`_
+* Add ``__KEEP_SUCCESS_DATASETS__`` by `@lldelisle <https://github.com/lldelisle>`_ in `#17294 <https://github.com/galaxyproject/galaxy/pull/17294>`_
+* Improve ModelManager type hints by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17299 <https://github.com/galaxyproject/galaxy/pull/17299>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17333 <https://github.com/galaxyproject/galaxy/pull/17333>`_
+* Add element_identifier and ext to inputs config file export by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17357 <https://github.com/galaxyproject/galaxy/pull/17357>`_
+* Remove unused statements in job search function by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17361 <https://github.com/galaxyproject/galaxy/pull/17361>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Fix type annotation of code using XML etree by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17367 <https://github.com/galaxyproject/galaxy/pull/17367>`_
+* More specific type annotation for ``BaseJobExec.parse_status()`` by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17381 <https://github.com/galaxyproject/galaxy/pull/17381>`_
+* Cancel all active jobs when the user is deleted by `@davelopez <https://github.com/davelopez>`_ in `#17390 <https://github.com/galaxyproject/galaxy/pull/17390>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Purge `groups` and `roles` from DB (for real) by `@davelopez <https://github.com/davelopez>`_ in `#17411 <https://github.com/galaxyproject/galaxy/pull/17411>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17420 <https://github.com/galaxyproject/galaxy/pull/17420>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* Adds published histories to grid list by `@guerler <https://github.com/guerler>`_ in `#17449 <https://github.com/galaxyproject/galaxy/pull/17449>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* `data_column` parameter: use `column_names` metadata if present by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17478 <https://github.com/galaxyproject/galaxy/pull/17478>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17486 <https://github.com/galaxyproject/galaxy/pull/17486>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+* Update k8s docker python to 3.12 by `@nuwang <https://github.com/nuwang>`_ in `#17494 <https://github.com/galaxyproject/galaxy/pull/17494>`_
+* add encode ID API endpoint by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#17510 <https://github.com/galaxyproject/galaxy/pull/17510>`_
+* Fixing data_source tools and incrementing tool profile by `@wm75 <https://github.com/wm75>`_ in `#17515 <https://github.com/galaxyproject/galaxy/pull/17515>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17541 <https://github.com/galaxyproject/galaxy/pull/17541>`_
+* Add `image_diff` comparison method for test output verification using images by `@kostrykin <https://github.com/kostrykin>`_ in `#17556 <https://github.com/galaxyproject/galaxy/pull/17556>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17580 <https://github.com/galaxyproject/galaxy/pull/17580>`_
+* Restore histories API behavior for `keys` query parameter by `@davelopez <https://github.com/davelopez>`_ in `#17779 <https://github.com/galaxyproject/galaxy/pull/17779>`_
+* Fix datasets API custom keys encoding by `@davelopez <https://github.com/davelopez>`_ in `#17793 <https://github.com/galaxyproject/galaxy/pull/17793>`_
+* Improved error messages for runtime sharing problems. by `@jmchilton <https://github.com/jmchilton>`_ in `#17794 <https://github.com/galaxyproject/galaxy/pull/17794>`_
+* Allow admin to sharpen language about selected object stores. by `@jmchilton <https://github.com/jmchilton>`_ in `#17806 <https://github.com/galaxyproject/galaxy/pull/17806>`_
+
+=============
+Other changes
+=============
+
+* consistently compare profile versions by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16492 <https://github.com/galaxyproject/galaxy/pull/16492>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -77,15 +177,15 @@
 * Workflow Comments 💬 by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#16612 <https://github.com/galaxyproject/galaxy/pull/16612>`_
 * Switch out conditional requirement parser by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16636 <https://github.com/galaxyproject/galaxy/pull/16636>`_
 * Add scroll pagination and username filter to `HistoryPublishedList` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#16642 <https://github.com/galaxyproject/galaxy/pull/16642>`_
 * Bump samtools converters by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16668 <https://github.com/galaxyproject/galaxy/pull/16668>`_
 * Galaxy Markdown - add workflow image and license to Galaxy markdown. by `@jmchilton <https://github.com/jmchilton>`_ in `#16672 <https://github.com/galaxyproject/galaxy/pull/16672>`_
 * Implement instance URLs in Galaxy markdown. by `@jmchilton <https://github.com/jmchilton>`_ in `#16675 <https://github.com/galaxyproject/galaxy/pull/16675>`_
 * Change Sentry error reporting plug-in by `@kysrpex <https://github.com/kysrpex>`_ in `#16686 <https://github.com/galaxyproject/galaxy/pull/16686>`_
-*  Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
+* Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
 * Enhance task monitor composable by `@davelopez <https://github.com/davelopez>`_ in `#16695 <https://github.com/galaxyproject/galaxy/pull/16695>`_
 * Misc. edits/refactorings to session handling  by `@jdavcs <https://github.com/jdavcs>`_ in `#16712 <https://github.com/galaxyproject/galaxy/pull/16712>`_
 * SQLAlchemy 2.0 upgrades (part 2) by `@jdavcs <https://github.com/jdavcs>`_ in `#16724 <https://github.com/galaxyproject/galaxy/pull/16724>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16735 <https://github.com/galaxyproject/galaxy/pull/16735>`_
 * Convert ISO to UTC for Date/Time in workflow reports by `@assuntad23 <https://github.com/assuntad23>`_ in `#16758 <https://github.com/galaxyproject/galaxy/pull/16758>`_
 * Replace ELIXIR AAI button with Life Science login by `@sebastian-schaaf <https://github.com/sebastian-schaaf>`_ in `#16762 <https://github.com/galaxyproject/galaxy/pull/16762>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16770 <https://github.com/galaxyproject/galaxy/pull/16770>`_
```

### Comparing `galaxy-app-23.2.1/LICENSE` & `galaxy-app-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/PKG-INFO` & `galaxy-app-24.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,77 @@
 Metadata-Version: 2.1
 Name: galaxy-app
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy application (backend)
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-auth
+Requires-Dist: galaxy-config
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-files
+Requires-Dist: galaxy-job-execution
+Requires-Dist: galaxy-job-metrics
+Requires-Dist: galaxy-objectstore
+Requires-Dist: galaxy-tool-util[cwl,edam]
+Requires-Dist: galaxy-tours
+Requires-Dist: galaxy-util
+Requires-Dist: galaxy-web-framework
+Requires-Dist: galaxy-web-stack
+Requires-Dist: Beaker
+Requires-Dist: boltons
+Requires-Dist: bx-python
+Requires-Dist: celery
+Requires-Dist: cloudauthz==0.6.0
+Requires-Dist: dparse
+Requires-Dist: gxformat2
+Requires-Dist: kombu>=5.3
+Requires-Dist: lagom
+Requires-Dist: lxml!=4.2.2
+Requires-Dist: Mako
+Requires-Dist: Markdown
+Requires-Dist: MarkupSafe
+Requires-Dist: packaging
+Requires-Dist: paramiko!=2.9.0,!=2.9.1
+Requires-Dist: pebble
+Requires-Dist: pulsar-galaxy-lib>=0.15.0.dev0
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: pysam>=0.21
+Requires-Dist: PyJWT
+Requires-Dist: PyYAML
+Requires-Dist: refgenconf>=0.12.0
+Requires-Dist: regex
+Requires-Dist: requests
+Requires-Dist: SQLAlchemy<2,>=1.4.25
+Requires-Dist: sqlitedict
+Requires-Dist: starlette
+Requires-Dist: svgwrite
+Requires-Dist: typing-extensions
+Requires-Dist: WebOb
+Requires-Dist: Whoosh
 
 
 .. image:: https://badge.fury.io/py/galaxy-app.svg
    :target: https://pypi.org/project/galaxy-app/
 
 
 Overview
@@ -42,14 +85,114 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Reload built-in converters on toolbox reload by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17209 <https://github.com/galaxyproject/galaxy/pull/17209>`_
+* Optional Reply-to SMTP header in tool error reports by `@neoformit <https://github.com/neoformit>`_ in `#17243 <https://github.com/galaxyproject/galaxy/pull/17243>`_
+* Package tests fixes by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17301 <https://github.com/galaxyproject/galaxy/pull/17301>`_
+* Follow-up on #17274 and #17262 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17302 <https://github.com/galaxyproject/galaxy/pull/17302>`_
+* Rollback invalidated transaction: catch them earlier by `@jdavcs <https://github.com/jdavcs>`_ in `#17312 <https://github.com/galaxyproject/galaxy/pull/17312>`_
+* Fixes for flake8-bugbear 24.1.17 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17340 <https://github.com/galaxyproject/galaxy/pull/17340>`_
+* Fix data_source and data_source_async bugs by `@wm75 <https://github.com/wm75>`_ in `#17422 <https://github.com/galaxyproject/galaxy/pull/17422>`_
+* More efficient change_state queries, maybe fix deadlock by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17632 <https://github.com/galaxyproject/galaxy/pull/17632>`_
+* Don't index tasks without task_uuid by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17646 <https://github.com/galaxyproject/galaxy/pull/17646>`_
+* Separate `ConnectedValue` from `RuntimeValue` by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17678 <https://github.com/galaxyproject/galaxy/pull/17678>`_
+* Fix step type serialization for StoredWorkflowDetailed models by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17716 <https://github.com/galaxyproject/galaxy/pull/17716>`_
+* Fix usage of DISTINCT by `@jdavcs <https://github.com/jdavcs>`_ in `#17759 <https://github.com/galaxyproject/galaxy/pull/17759>`_
+* Also set extension and metadata on copies of job outputs when finishing job by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17777 <https://github.com/galaxyproject/galaxy/pull/17777>`_
+* Use ``hg clone --stream`` to clone repos by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17786 <https://github.com/galaxyproject/galaxy/pull/17786>`_
+* Defer job attributes that are usually not needed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17795 <https://github.com/galaxyproject/galaxy/pull/17795>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+* Fix archived histories mixing with active in histories list by `@davelopez <https://github.com/davelopez>`_ in `#17856 <https://github.com/galaxyproject/galaxy/pull/17856>`_
+* Normalize extensions when loading tool by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17868 <https://github.com/galaxyproject/galaxy/pull/17868>`_
+* Ignore user data table errors for now by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17880 <https://github.com/galaxyproject/galaxy/pull/17880>`_
+
+============
+Enhancements
+============
+
+* Add harmonize collections tool (or whatever other name) by `@lldelisle <https://github.com/lldelisle>`_ in `#16662 <https://github.com/galaxyproject/galaxy/pull/16662>`_
+* Add support for Python 3.12 by `@tuncK <https://github.com/tuncK>`_ in `#16796 <https://github.com/galaxyproject/galaxy/pull/16796>`_
+* SQLAlchemy 2.0 upgrades (part 5) by `@jdavcs <https://github.com/jdavcs>`_ in `#16932 <https://github.com/galaxyproject/galaxy/pull/16932>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
+* Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
+* Add select parameter with options from remote resources by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17087 <https://github.com/galaxyproject/galaxy/pull/17087>`_
+*  Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
+* Vueify Admin Roles Grid by `@guerler <https://github.com/guerler>`_ in `#17118 <https://github.com/galaxyproject/galaxy/pull/17118>`_
+* SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17123 <https://github.com/galaxyproject/galaxy/pull/17123>`_
+* Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
+* Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
+* Vueify Admin Forms and Quota grids by `@guerler <https://github.com/guerler>`_ in `#17141 <https://github.com/galaxyproject/galaxy/pull/17141>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17157 <https://github.com/galaxyproject/galaxy/pull/17157>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17201 <https://github.com/galaxyproject/galaxy/pull/17201>`_
+* Vendorize fastapi-utls.cbv by `@jdavcs <https://github.com/jdavcs>`_ in `#17205 <https://github.com/galaxyproject/galaxy/pull/17205>`_
+* Fix usage of graphene-sqlalchemy, bump to 3.0.0rc1 by `@jdavcs <https://github.com/jdavcs>`_ in `#17216 <https://github.com/galaxyproject/galaxy/pull/17216>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17230 <https://github.com/galaxyproject/galaxy/pull/17230>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17235 <https://github.com/galaxyproject/galaxy/pull/17235>`_
+* Allow job files to consume TUS uploads by `@jmchilton <https://github.com/jmchilton>`_ in `#17242 <https://github.com/galaxyproject/galaxy/pull/17242>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17247 <https://github.com/galaxyproject/galaxy/pull/17247>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Consider Null inputs by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17271 <https://github.com/galaxyproject/galaxy/pull/17271>`_
+* Add OIDC backend configuration schema and validation by `@uwwint <https://github.com/uwwint>`_ in `#17274 <https://github.com/galaxyproject/galaxy/pull/17274>`_
+* Adds delete, purge and undelete batch operations to History Grid by `@guerler <https://github.com/guerler>`_ in `#17282 <https://github.com/galaxyproject/galaxy/pull/17282>`_
+* Add ``__KEEP_SUCCESS_DATASETS__`` by `@lldelisle <https://github.com/lldelisle>`_ in `#17294 <https://github.com/galaxyproject/galaxy/pull/17294>`_
+* Improve ModelManager type hints by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17299 <https://github.com/galaxyproject/galaxy/pull/17299>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17333 <https://github.com/galaxyproject/galaxy/pull/17333>`_
+* Add element_identifier and ext to inputs config file export by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17357 <https://github.com/galaxyproject/galaxy/pull/17357>`_
+* Remove unused statements in job search function by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17361 <https://github.com/galaxyproject/galaxy/pull/17361>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Fix type annotation of code using XML etree by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17367 <https://github.com/galaxyproject/galaxy/pull/17367>`_
+* More specific type annotation for ``BaseJobExec.parse_status()`` by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17381 <https://github.com/galaxyproject/galaxy/pull/17381>`_
+* Cancel all active jobs when the user is deleted by `@davelopez <https://github.com/davelopez>`_ in `#17390 <https://github.com/galaxyproject/galaxy/pull/17390>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Purge `groups` and `roles` from DB (for real) by `@davelopez <https://github.com/davelopez>`_ in `#17411 <https://github.com/galaxyproject/galaxy/pull/17411>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17420 <https://github.com/galaxyproject/galaxy/pull/17420>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* Adds published histories to grid list by `@guerler <https://github.com/guerler>`_ in `#17449 <https://github.com/galaxyproject/galaxy/pull/17449>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* `data_column` parameter: use `column_names` metadata if present by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17478 <https://github.com/galaxyproject/galaxy/pull/17478>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17486 <https://github.com/galaxyproject/galaxy/pull/17486>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+* Update k8s docker python to 3.12 by `@nuwang <https://github.com/nuwang>`_ in `#17494 <https://github.com/galaxyproject/galaxy/pull/17494>`_
+* add encode ID API endpoint by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#17510 <https://github.com/galaxyproject/galaxy/pull/17510>`_
+* Fixing data_source tools and incrementing tool profile by `@wm75 <https://github.com/wm75>`_ in `#17515 <https://github.com/galaxyproject/galaxy/pull/17515>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17541 <https://github.com/galaxyproject/galaxy/pull/17541>`_
+* Add `image_diff` comparison method for test output verification using images by `@kostrykin <https://github.com/kostrykin>`_ in `#17556 <https://github.com/galaxyproject/galaxy/pull/17556>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17580 <https://github.com/galaxyproject/galaxy/pull/17580>`_
+* Restore histories API behavior for `keys` query parameter by `@davelopez <https://github.com/davelopez>`_ in `#17779 <https://github.com/galaxyproject/galaxy/pull/17779>`_
+* Fix datasets API custom keys encoding by `@davelopez <https://github.com/davelopez>`_ in `#17793 <https://github.com/galaxyproject/galaxy/pull/17793>`_
+* Improved error messages for runtime sharing problems. by `@jmchilton <https://github.com/jmchilton>`_ in `#17794 <https://github.com/galaxyproject/galaxy/pull/17794>`_
+* Allow admin to sharpen language about selected object stores. by `@jmchilton <https://github.com/jmchilton>`_ in `#17806 <https://github.com/galaxyproject/galaxy/pull/17806>`_
+
+=============
+Other changes
+=============
+
+* consistently compare profile versions by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16492 <https://github.com/galaxyproject/galaxy/pull/16492>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -119,15 +262,15 @@
 * Workflow Comments 💬 by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#16612 <https://github.com/galaxyproject/galaxy/pull/16612>`_
 * Switch out conditional requirement parser by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16636 <https://github.com/galaxyproject/galaxy/pull/16636>`_
 * Add scroll pagination and username filter to `HistoryPublishedList` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#16642 <https://github.com/galaxyproject/galaxy/pull/16642>`_
 * Bump samtools converters by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16668 <https://github.com/galaxyproject/galaxy/pull/16668>`_
 * Galaxy Markdown - add workflow image and license to Galaxy markdown. by `@jmchilton <https://github.com/jmchilton>`_ in `#16672 <https://github.com/galaxyproject/galaxy/pull/16672>`_
 * Implement instance URLs in Galaxy markdown. by `@jmchilton <https://github.com/jmchilton>`_ in `#16675 <https://github.com/galaxyproject/galaxy/pull/16675>`_
 * Change Sentry error reporting plug-in by `@kysrpex <https://github.com/kysrpex>`_ in `#16686 <https://github.com/galaxyproject/galaxy/pull/16686>`_
-*  Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
+* Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
 * Enhance task monitor composable by `@davelopez <https://github.com/davelopez>`_ in `#16695 <https://github.com/galaxyproject/galaxy/pull/16695>`_
 * Misc. edits/refactorings to session handling  by `@jdavcs <https://github.com/jdavcs>`_ in `#16712 <https://github.com/galaxyproject/galaxy/pull/16712>`_
 * SQLAlchemy 2.0 upgrades (part 2) by `@jdavcs <https://github.com/jdavcs>`_ in `#16724 <https://github.com/galaxyproject/galaxy/pull/16724>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16735 <https://github.com/galaxyproject/galaxy/pull/16735>`_
 * Convert ISO to UTC for Date/Time in workflow reports by `@assuntad23 <https://github.com/assuntad23>`_ in `#16758 <https://github.com/galaxyproject/galaxy/pull/16758>`_
 * Replace ELIXIR AAI button with Life Science login by `@sebastian-schaaf <https://github.com/sebastian-schaaf>`_ in `#16762 <https://github.com/galaxyproject/galaxy/pull/16762>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16770 <https://github.com/galaxyproject/galaxy/pull/16770>`_
```

### Comparing `galaxy-app-23.2.1/galaxy/actions/library.py` & `galaxy-app-24.0.0/galaxy/actions/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains library functions
 """
+
 import json
 import logging
 import os.path
 from typing import Optional
 
 from markupsafe import escape
 
@@ -220,16 +221,15 @@
         for path, name, folder in files_and_folders:
             uploaded_datasets.append(
                 self._make_library_uploaded_dataset(trans, params, name, path, "path_paste", library_bunch, folder)
             )
         return uploaded_datasets, 200, None
 
     def _get_path_files_and_folders(self, params, preserve_dirs):
-        problem_response = self._check_path_paste_params(params)
-        if problem_response:
+        if problem_response := self._check_path_paste_params(params):
             return problem_response
         files_and_folders = []
         for line, path in self._paths_list(params):
             line_files_and_folders = self._get_single_path_files_and_folders(line, path, preserve_dirs)
             files_and_folders.extend(line_files_and_folders)
         return files_and_folders, None, None
```

### Comparing `galaxy-app-23.2.1/galaxy/app.py` & `galaxy-app-24.0.0/galaxy/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,20 +97,26 @@
     reload_toolbox,
     send_local_control_task,
 )
 from galaxy.quota import (
     get_quota_agent,
     QuotaAgent,
 )
-from galaxy.schema.fields import BaseDatabaseIdField
+from galaxy.schema.fields import Security
 from galaxy.security.idencoding import IdEncodingHelper
 from galaxy.security.vault import (
     Vault,
     VaultFactory,
 )
+from galaxy.short_term_storage import (
+    ShortTermStorageAllocator,
+    ShortTermStorageConfiguration,
+    ShortTermStorageManager,
+    ShortTermStorageMonitor,
+)
 from galaxy.tool_shed.cache import ToolShedRepositoryCache
 from galaxy.tool_shed.galaxy_install.client import InstallationTarget
 from galaxy.tool_shed.galaxy_install.installed_repository_manager import InstalledRepositoryManager
 from galaxy.tool_shed.galaxy_install.update_repository_manager import UpdateRepositoryManager
 from galaxy.tool_util.data import ToolDataTableManager as BaseToolDataTableManager
 from galaxy.tool_util.deps import containers
 from galaxy.tool_util.deps.dependencies import AppInfo
@@ -137,20 +143,14 @@
 from galaxy.util.tool_shed import tool_shed_registry
 from galaxy.visualization.data_providers.registry import DataProviderRegistry
 from galaxy.visualization.genomes import Genomes
 from galaxy.visualization.plugins.registry import VisualizationsRegistry
 from galaxy.web import url_for
 from galaxy.web.framework.base import server_starttime
 from galaxy.web.proxy import ProxyManager
-from galaxy.web.short_term_storage import (
-    ShortTermStorageAllocator,
-    ShortTermStorageConfiguration,
-    ShortTermStorageManager,
-    ShortTermStorageMonitor,
-)
 from galaxy.web_stack import (
     application_stack_instance,
     ApplicationStack,
 )
 from galaxy.webhooks import WebhooksRegistry
 from galaxy.workflow import scheduling_manager
 from galaxy.workflow.trs_proxy import TrsProxy
@@ -255,14 +255,16 @@
         # Security helper
         self._configure_security()
         self._register_singleton(IdEncodingHelper, self.security)
         self._register_singleton(SharedModelMapping, self.model)
         self._register_singleton(GalaxyModelMapping, self.model)
         self._register_singleton(galaxy_scoped_session, self.model.context)
         self._register_singleton(install_model_scoped_session, self.install_model.context)
+        # Load quota management.
+        self.quota_agent = self._register_singleton(QuotaAgent, get_quota_agent(self.config, self.model))
 
     def configure_fluent_log(self):
         if self.config.fluent_log:
             from galaxy.util.custom_logging.fluent_log import FluentTraceLogger
 
             self.trace_logger: Optional[FluentTraceLogger] = FluentTraceLogger(
                 "galaxy", self.config.fluent_host, self.config.fluent_port
@@ -403,15 +405,15 @@
             )
 
     def _configure_object_store(self, **kwds):
         self.object_store = build_object_store_from_config(self.config, **kwds)
 
     def _configure_security(self):
         self.security = IdEncodingHelper(id_secret=self.config.id_secret)
-        BaseDatabaseIdField.security = self.security
+        Security.security = self.security
 
     def _configure_engines(self, db_url, install_db_url, combined_install_database):
         trace_logger = getattr(self, "trace_logger", None)
         engine = build_engine(
             db_url,
             self.config.database_engine_options,
             self.config.database_query_profiling_proxy,
@@ -566,16 +568,14 @@
 
         self.vault = self._register_singleton(Vault, VaultFactory.from_app(self))  # type: ignore[type-abstract]
         # Load security policy.
         self.security_agent = self.model.security_agent
         self.host_security_agent = galaxy.model.security.HostAgent(
             model=self.security_agent.model, permitted_actions=self.security_agent.permitted_actions
         )
-        # Load quota management.
-        self.quota_agent = self._register_singleton(QuotaAgent, get_quota_agent(self.config, self.model))
 
         # We need the datatype registry for running certain tasks that modify HDAs, and to build the registry we need
         # to setup the installed repositories ... this is not ideal
         self._configure_tool_config_files()
         self.installed_repository_manager = self._register_singleton(
             InstalledRepositoryManager, InstalledRepositoryManager(self)
         )
@@ -696,17 +696,14 @@
         self.datatypes_registry.load_display_applications(self)
         # Load datatype converters defined in local datatypes_conf.xml
         self.datatypes_registry.load_datatype_converters(self.toolbox)
         # Load external metadata tool
         self.datatypes_registry.load_external_metadata_tool(self.toolbox)
         # Load history import/export tools.
         load_lib_tools(self.toolbox)
-        # Load built-in converters
-        if self.config.display_builtin_converters:
-            self.toolbox.load_builtin_converters()
         self.toolbox.persist_cache(register_postfork=True)
         # visualizations registry: associates resources with visualizations, controls how to render
         self.visualizations_registry = self._register_singleton(
             VisualizationsRegistry,
             VisualizationsRegistry(
                 self,
                 directories_setting=self.config.visualization_plugins_directory,
@@ -838,16 +835,15 @@
     def to_str(self, **kwd):
         self.galaxy_statsd_client.timing(self.timer_id, self.elapsed * 1000.0, kwd)
         return super().to_str(**kwd)
 
 
 class ExecutionTimerFactory:
     def __init__(self, config):
-        statsd_host = getattr(config, "statsd_host", None)
-        if statsd_host:
+        if statsd_host := getattr(config, "statsd_host", None):
             from galaxy.web.statsd_client import GalaxyStatsdClient
 
             self.galaxy_statsd_client: Optional[GalaxyStatsdClient] = GalaxyStatsdClient(
                 statsd_host,
                 getattr(config, "statsd_port", 8125),
                 getattr(config, "statsd_prefix", "galaxy"),
                 getattr(config, "statsd_influxdb", False),
```

### Comparing `galaxy-app-23.2.1/galaxy/app_unittest_utils/galaxy_mock.py` & `galaxy-app-24.0.0/galaxy/app_unittest_utils/galaxy_mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Mock infrastructure for testing ModelManagers.
 """
+
 import os
 import shutil
 import tempfile
 from typing import (
     Any,
     cast,
     Optional,
@@ -37,31 +38,31 @@
 from galaxy.model.mapping import GalaxyModelMapping
 from galaxy.model.scoped_session import galaxy_scoped_session
 from galaxy.model.unittest_utils import (
     GalaxyDataTestApp,
     GalaxyDataTestConfig,
 )
 from galaxy.security import idencoding
+from galaxy.short_term_storage import (
+    ShortTermStorageAllocator,
+    ShortTermStorageConfiguration,
+    ShortTermStorageManager,
+    ShortTermStorageMonitor,
+)
 from galaxy.structured_app import (
     BasicSharedApp,
     MinimalManagerApp,
     StructuredApp,
 )
 from galaxy.tool_util.deps.containers import NullContainerFinder
 from galaxy.tools import ToolBox
 from galaxy.tools.cache import ToolCache
 from galaxy.tools.data import ToolDataTableManager
 from galaxy.util import StructuredExecutionTimer
 from galaxy.util.bunch import Bunch
-from galaxy.web.short_term_storage import (
-    ShortTermStorageAllocator,
-    ShortTermStorageConfiguration,
-    ShortTermStorageManager,
-    ShortTermStorageMonitor,
-)
 from galaxy.web_stack import ApplicationStack
 
 
 # =============================================================================
 def buildMockEnviron(**kwargs):
     environ = {
         "CONTENT_LENGTH": "0",
@@ -154,14 +155,18 @@
 
         self.url_for = url_for
 
     @property
     def toolbox(self) -> ToolBox:
         return self._toolbox
 
+    @toolbox.setter
+    def toolbox(self, toolbox: ToolBox):
+        self._toolbox = toolbox
+
     def wait_for_toolbox_reload(self, toolbox):
         # TODO: If the tpm test case passes, does the operation really
         # need to wait.
         return True
 
     def reindex_tool_search(self) -> None:
         raise NotImplementedError
@@ -254,14 +259,15 @@
         self.tool_configs = []
         self.manage_dependency_relationships = False
         self.enable_tool_shed_check = False
         self.monitor_thread_join_timeout = 1
         self.integrated_tool_panel_config = None
         self.vault_config_file = kwargs.get("vault_config_file")
         self.max_discovered_files = 10000
+        self.display_builtin_converters = True
         self.enable_notification_system = True
 
     @property
     def config_dict(self):
         return self.dict()
 
     def __getattr__(self, name):
@@ -276,26 +282,30 @@
 
 class MockWebapp:
     def __init__(self, security: idencoding.IdEncodingHelper, **kwargs):
         self.name = kwargs.get("name", "galaxy")
         self.security = security
 
 
+def mock_url_builder(*a, **k):
+    return f"(fake url): {a}, {k}"
+
+
 class MockTrans:
     def __init__(self, app=None, user=None, history=None, **kwargs):
         self.app = cast(UniverseApplication, app or MockApp(**kwargs))
         self.model = self.app.model
         self.webapp = MockWebapp(self.app.security, **kwargs)
         self.sa_session = self.app.model.session
         self.workflow_building_mode = False
         self.error_message = None
         self.anonymous = False
         self.debug = True
         self.user_is_admin = True
-        self.url_builder = None
+        self.url_builder = mock_url_builder
 
         self.galaxy_session = None
         self.__user = user
         self.security = self.app.security
         self.history = history
 
         self.request: Any = Bunch(headers={}, is_body_readable=False, host="request.host")
```

### Comparing `galaxy-app-23.2.1/galaxy/app_unittest_utils/toolbox_support.py` & `galaxy-app-24.0.0/galaxy/app_unittest_utils/toolbox_support.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/app_unittest_utils/tools_support.py` & `galaxy-app-24.0.0/galaxy/app_unittest_utils/tools_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Module contains test fixtures meant to aide in the testing of jobs and
 tool evaluation. Such extensive "fixtures" are something of an anti-pattern
-so use of this should be limitted to tests of very 'extensive' classes.
+so use of this should be limited to tests of very 'extensive' classes.
 """
 
 import os.path
 import shutil
 import string
 import tempfile
 from collections import defaultdict
@@ -119,15 +119,15 @@
             out.write(contents)
 
 
 class MockContext:
     def __init__(self, model_objects=None):
         self.expunged_all = False
         self.flushed = False
-        self.model_objects = model_objects or defaultdict(lambda: {})
+        self.model_objects = model_objects or defaultdict(dict)
         self.created_objects = []
         self.current = self
 
     def expunge_all(self):
         self.expunged_all = True
 
     def query(self, clazz):
```

### Comparing `galaxy-app-23.2.1/galaxy/authnz/custos_authnz.py` & `galaxy-app-24.0.0/galaxy/authnz/custos_authnz.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,46 +56,61 @@
     label: str
     client_id: str
     client_secret: str
     require_create_confirmation: bool
     redirect_uri: str
     ca_bundle: Optional[str]
     pkce_support: bool
+    accepted_audiences: List[str]
     extra_params: Optional[dict]
     authorization_endpoint: Optional[str]
     token_endpoint: Optional[str]
     end_session_endpoint: Optional[str]
     well_known_oidc_config_uri: Optional[str]
     iam_client_secret: Optional[str]
     userinfo_endpoint: Optional[str]
     credential_url: Optional[str]
+    issuer: Optional[str]
+    jwks_uri: Optional[str]
 
 
 class OIDCAuthnzBase(IdentityProvider):
     def __init__(self, provider, oidc_config, oidc_backend_config, idphint=None):
         provider = provider.lower()
+        self.jwks_client: Optional[jwt.PyJWKClient]
         self.config = CustosAuthnzConfiguration(
             provider=provider,
             verify_ssl=oidc_config["VERIFY_SSL"],
             url=oidc_backend_config["url"],
             label=oidc_backend_config.get("label", provider.capitalize()),
             client_id=oidc_backend_config["client_id"],
             client_secret=oidc_backend_config["client_secret"],
             require_create_confirmation=oidc_backend_config.get("require_create_confirmation", provider == "custos"),
             redirect_uri=oidc_backend_config["redirect_uri"],
             ca_bundle=oidc_backend_config.get("ca_bundle", None),
             pkce_support=oidc_backend_config.get("pkce_support", False),
+            accepted_audiences=list(
+                filter(
+                    None,
+                    map(
+                        str.strip,
+                        oidc_backend_config.get("accepted_audiences", oidc_backend_config["client_id"]).split(","),
+                    ),
+                )
+            ),
             extra_params={},
             authorization_endpoint=None,
             token_endpoint=None,
             end_session_endpoint=None,
             well_known_oidc_config_uri=None,
             iam_client_secret=None,
             userinfo_endpoint=None,
             credential_url=None,
+            issuer=None,
+            jwks_uri=None,
         )
 
     def _decode_token_no_signature(self, token):
         return jwt.decode(token, audience=self.config.client_id, options={"verify_signature": False})
 
     def refresh(self, trans, custos_authnz_token):
         if custos_authnz_token is None:
@@ -217,15 +232,15 @@
             user = trans.user
             existing_user = trans.sa_session.query(User).filter_by(email=email).first()
             if not user:
                 if existing_user:
                     if trans.app.config.fixed_delegated_auth:
                         user = existing_user
                     else:
-                        message = f"There already exists a user with email {email}.  To associate this external login, you must first be logged in as that existing account."
+                        message = f"There already exists a user with email {email}. To associate this external login, you must first be logged in as that existing account."
                         log.info(message)
                         login_redirect_url = (
                             f"{login_redirect_url}login/start"
                             f"?connect_external_provider={self.config.provider}"
                             f"&connect_external_email={email}"
                             f"&connect_external_label={self.config.label}"
                         )
@@ -445,14 +460,20 @@
         return f"{base_url}/.well-known/openid-configuration"
 
     def _load_well_known_oidc_config(self, well_known_oidc_config):
         self.config.authorization_endpoint = well_known_oidc_config["authorization_endpoint"]
         self.config.token_endpoint = well_known_oidc_config["token_endpoint"]
         self.config.userinfo_endpoint = well_known_oidc_config["userinfo_endpoint"]
         self.config.end_session_endpoint = well_known_oidc_config.get("end_session_endpoint")
+        self.config.issuer = well_known_oidc_config.get("issuer")
+        self.config.jwks_uri = well_known_oidc_config.get("jwks_uri")
+        if self.config.jwks_uri:
+            self.jwks_client = jwt.PyJWKClient(self.config.jwks_uri, cache_jwk_set=True, lifespan=360)
+        else:
+            self.jwks_client = None
 
     def _get_verify_param(self):
         """Return 'ca_bundle' if 'verify_ssl' is true and 'ca_bundle' is configured."""
         # in requests_oauthlib, the verify param can either be a boolean or a CA bundle path
         if self.config.ca_bundle is not None and self.config.verify_ssl:
             return self.config.ca_bundle
         else:
@@ -469,14 +490,60 @@
             count = 0
             while trans.sa_session.query(trans.app.model.User).filter_by(username=(f"{username}{count}")).first():
                 count += 1
             return f"{username}{count}"
         else:
             return username
 
+    def decode_user_access_token(self, sa_session, access_token):
+        """Verifies and decodes an access token against this provider, returning the user and
+        a dict containing the decoded token data.
+
+        :type  sa_session:      sqlalchemy.orm.scoping.scoped_session
+        :param sa_session:      SQLAlchemy database handle.
+
+        :type  access_token: string
+        :param access_token: An OIDC access token
+
+        :return: A tuple containing the user and decoded jwt data or [None, None]
+                 if the access token does not belong to this provider.
+        :rtype: Tuple[User, dict]
+        """
+        if not self.jwks_client:
+            return None
+        try:
+            signing_key = self.jwks_client.get_signing_key_from_jwt(access_token)
+            decoded_jwt = jwt.decode(
+                access_token,
+                signing_key.key,
+                algorithms=["RS256"],
+                issuer=self.config.issuer,
+                audience=self.config.accepted_audiences,
+                options={
+                    "verify_signature": True,
+                    "verify_exp": True,
+                    "verify_nbf": True,
+                    "verify_iat": True,
+                    "verify_aud": bool(self.config.accepted_audiences),
+                    "verify_iss": True,
+                },
+            )
+        except jwt.exceptions.PyJWKClientError:
+            log.debug(f"Could not get signing keys for access token with provider: {self.config.provider}. Ignoring...")
+            return None, None
+        except jwt.exceptions.InvalidIssuerError:
+            # An Invalid issuer means that the access token is not relevant to this provider.
+            # All other exceptions are bubbled up
+            return None, None
+        # jwt verified, we can now fetch the user
+        user_id = decoded_jwt["sub"]
+        custos_authnz_token = self._get_custos_authnz_token(sa_session, user_id, self.config.provider)
+        user = custos_authnz_token.user if custos_authnz_token else None
+        return user, decoded_jwt
+
 
 class OIDCAuthnzBaseKeycloak(OIDCAuthnzBase):
     def __init__(self, provider, oidc_config, oidc_backend_config, idphint=None):
         super().__init__(provider, oidc_config, oidc_backend_config, idphint)
         self.config.extra_params = {"kc_idp_hint": oidc_backend_config.get("idphint", "oidc")}
         self._load_config()
```

### Comparing `galaxy-app-23.2.1/galaxy/authnz/managers.py` & `galaxy-app-24.0.0/galaxy/authnz/managers.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,29 @@
     asbool,
     etree,
     listify,
     parse_xml,
     string_as_bool,
     unicodify,
 )
+from galaxy.util.resources import files
 from .custos_authnz import (
     CustosAuthFactory,
     KEYCLOAK_BACKENDS,
 )
 from .psa_authnz import (
     BACKENDS_NAME,
     on_the_fly_config,
     PSAAuthnz,
     Storage,
     Strategy,
 )
 
+OIDC_BACKEND_SCHEMA = files("galaxy.authnz.xsd") / "oidc_backends_config.xsd"
+
 log = logging.getLogger(__name__)
 
 # Note: This if for backward compatibility. Icons can be specified in oidc_backends_config.xml.
 DEFAULT_OIDC_IDP_ICONS = {
     "google": "https://developers.google.com/identity/images/btn_google_signin_light_normal_web.png",
     "elixir": "https://lifescience-ri.eu/fileadmin/lifescience-ri/media/Images/button-login-small.png",
     "okta": "https://www.okta.com/sites/all/themes/Okta/images/blog/Logos/Okta_Logo_BrightBlue_Medium.png",
@@ -101,15 +104,15 @@
     def _get_idp_icon(self, idp):
         return self.oidc_backends_config[idp].get("icon") or DEFAULT_OIDC_IDP_ICONS.get(idp)
 
     def _parse_oidc_backends_config(self, config_file):
         self.oidc_backends_config = {}
         self.oidc_backends_implementation = {}
         try:
-            tree = parse_xml(config_file)
+            tree = parse_xml(config_file, schemafname=OIDC_BACKEND_SCHEMA)
             root = tree.getroot()
             if root.tag != "OIDC":
                 raise etree.ParseError(
                     "The root element in OIDC config xml file is expected to be `OIDC`, "
                     f"found `{root.tag}` instead -- unable to continue."
                 )
             for child in root:
@@ -161,14 +164,16 @@
             rtv["icon"] = config_xml.find("icon").text
         if config_xml.find("extra_scopes") is not None:
             rtv["extra_scopes"] = listify(config_xml.find("extra_scopes").text)
         if config_xml.find("tenant_id") is not None:
             rtv["tenant_id"] = config_xml.find("tenant_id").text
         if config_xml.find("pkce_support") is not None:
             rtv["pkce_support"] = asbool(config_xml.find("pkce_support").text)
+        if config_xml.find("accepted_audiences") is not None:
+            rtv["accepted_audiences"] = config_xml.find("accepted_audiences").text
         # this is a EGI Check-in specific config
         if config_xml.find("checkin_env") is not None:
             rtv["checkin_env"] = config_xml.find("checkin_env").text
 
         return rtv
 
     def _parse_custos_config(self, config_xml):
@@ -191,14 +196,16 @@
             self.allowed_idps = list(map(lambda idp: idp.text, config_xml.findall("allowed_idp")))
         if config_xml.find("ca_bundle") is not None:
             rtv["ca_bundle"] = config_xml.find("ca_bundle").text
         if config_xml.find("icon") is not None:
             rtv["icon"] = config_xml.find("icon").text
         if config_xml.find("pkce_support") is not None:
             rtv["pkce_support"] = asbool(config_xml.find("pkce_support").text)
+        if config_xml.find("accepted_audiences") is not None:
+            rtv["accepted_audiences"] = config_xml.find("accepted_audiences").text
         return rtv
 
     def get_allowed_idps(self):
         # None, if no allowed idp list is set, and a list of EntityIDs if configured (in oidc_backend)
         return self.allowed_idps
 
     def _unify_provider_name(self, provider):
@@ -403,14 +410,62 @@
             log.exception("Error creating user")
             raise
         except Exception:
             msg = f"An error occurred when creating a user with `{provider}` identity provider.  Please contact an administrator for assistance."
             log.exception(msg)
             return False, msg, (None, None)
 
+    def _assert_jwt_contains_scopes(self, user, jwt, required_scopes):
+        if not jwt:
+            raise exceptions.AuthenticationFailed(
+                err_msg=f"User: {user.username} does not have the required scopes: [{required_scopes}]"
+            )
+        scopes = jwt.get("scope") or ""
+        if not set(required_scopes).issubset(scopes.split(" ")):
+            raise exceptions.AuthenticationFailed(
+                err_msg=f"User: {user.username} has JWT with scopes: [{scopes}] but not required scopes: [{required_scopes}]"
+            )
+
+    def _validate_permissions(self, user, jwt):
+        required_scopes = [f"{self.app.config.oidc_scope_prefix}:*"]
+        self._assert_jwt_contains_scopes(user, jwt, required_scopes)
+
+    def _match_access_token_to_user_in_provider(self, sa_session, provider, access_token):
+        try:
+            success, message, backend = self._get_authnz_backend(provider)
+            if success is False:
+                msg = f"An error occurred when obtaining user by token with provider `{provider}`: {message}"
+                log.error(msg)
+                return None
+            user, jwt = None, None
+            try:
+                user, jwt = backend.decode_user_access_token(sa_session, access_token)
+            except Exception:
+                log.exception("Could not decode access token")
+                raise exceptions.AuthenticationFailed(err_msg="Invalid access token or an unexpected error occurred.")
+            if user and jwt:
+                self._validate_permissions(user, jwt)
+                return user
+            elif not user and jwt:
+                # jwt was decoded, but no user could be matched
+                raise exceptions.AuthenticationFailed(
+                    err_msg="Cannot locate user by access token. The user should log into Galaxy at least once with this OIDC provider."
+                )
+            # Both jwt and user are empty, which means that this provider can't process this access token
+            return None
+        except NotImplementedError:
+            return None
+
+    def match_access_token_to_user(self, sa_session, access_token):
+        for provider in self.oidc_backends_config:
+            user = self._match_access_token_to_user_in_provider(sa_session, provider, access_token)
+            if user:
+                return user
+        return None
+
     def logout(self, provider, trans, post_user_logout_href=None):
         """
         Log the user out of the identity provider.
 
         :type provider: string
         :param provider: set the name of the identity provider.
         :type trans: GalaxyWebTransaction
```

### Comparing `galaxy-app-23.2.1/galaxy/authnz/psa_authnz.py` & `galaxy-app-24.0.0/galaxy/authnz/psa_authnz.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/carbon_emissions/__init__.py` & `galaxy-app-24.0.0/galaxy/carbon_emissions/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/celery/__init__.py` & `galaxy-app-24.0.0/galaxy/celery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,15 @@
         if galaxy.app.app:
             return galaxy.app.app
     return build_app()
 
 
 @lru_cache(maxsize=1)
 def build_app():
-    kwargs = get_app_properties()
-    if kwargs:
+    if kwargs := get_app_properties():
         kwargs["check_migrate_databases"] = False
         kwargs["use_display_applications"] = False
         kwargs["use_converters"] = False
         import galaxy.app
 
         galaxy_app = galaxy.app.GalaxyManagerApplication(configure_logging=False, **kwargs)
         return galaxy_app
```

### Comparing `galaxy-app-23.2.1/galaxy/celery/_serialization.py` & `galaxy-app-24.0.0/galaxy/celery/_serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class SchemaEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, BaseModel):
             return {
                 "__type__": "__pydantic_object__",
                 "__class__": fullname(obj),
-                "__object__": obj.dict(),
+                "__object__": obj.model_dump(mode="json"),
             }
         if isinstance(obj, UUID):
             return str(obj)
         else:
             return json.JSONEncoder.default(self, obj)
```

### Comparing `galaxy-app-23.2.1/galaxy/celery/base_task.py` & `galaxy-app-24.0.0/galaxy/celery/base_task.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/celery/tasks.py` & `galaxy-app-24.0.0/galaxy/celery/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,30 +54,30 @@
     PrepareDatasetCollectionDownload,
     PurgeDatasetsTaskRequest,
     SetupHistoryExportJob,
     WriteHistoryContentTo,
     WriteHistoryTo,
     WriteInvocationTo,
 )
+from galaxy.short_term_storage import ShortTermStorageMonitor
 from galaxy.structured_app import MinimalManagerApp
 from galaxy.tools import create_tool_from_representation
 from galaxy.tools.data_fetch import do_fetch
 from galaxy.util import galaxy_directory
 from galaxy.util.custom_logging import get_logger
-from galaxy.web.short_term_storage import ShortTermStorageMonitor
 
 log = get_logger(__name__)
 
 
-@lru_cache()
+@lru_cache
 def setup_data_table_manager(app):
     app._configure_tool_data_tables(from_shed_config=False)
 
 
-@lru_cache()
+@lru_cache
 def cached_create_tool_from_representation(app, raw_tool_source):
     return create_tool_from_representation(
         app=app, raw_tool_source=raw_tool_source, tool_dir="", tool_source_class="XmlToolSource"
     )
 
 
 @galaxy_task(action="recalculate a user's disk usage")
```

### Comparing `galaxy-app-23.2.1/galaxy/config_watchers.py` & `galaxy-app-24.0.0/galaxy/config_watchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,21 @@
         # and will be blind to further changes in these tools.
 
         def reload_toolbox():
             save_integrated_tool_panel = False
             try:
                 # Run and wait for toolbox reload on the process that watches the config files.
                 # The toolbox reload will update the integrated_tool_panel_file
-                self.app.queue_worker.send_local_control_task("reload_toolbox", get_response=True),
+                self.app.queue_worker.send_local_control_task("reload_toolbox", get_response=True)
             except Exception:
                 save_integrated_tool_panel = True
                 log.exception("Exception occured while reloading toolbox")
             self.app.queue_worker.send_control_task(
                 "reload_toolbox", noop_self=True, kwargs={"save_integrated_tool_panel": save_integrated_tool_panel}
-            ),
+            )
 
         self.tool_config_watcher = get_tool_conf_watcher(
             reload_callback=reload_toolbox,
             tool_cache=self.app.tool_cache,
         )
         self.data_manager_config_watcher = get_tool_conf_watcher(
             reload_callback=lambda: self.app.queue_worker.send_control_task("reload_data_managers"),
```

### Comparing `galaxy-app-23.2.1/galaxy/dependencies/__init__.py` & `galaxy-app-24.0.0/galaxy/dependencies/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,26 +63,23 @@
                 job_conf_path = join(dirname(self.config_file), "job_conf.yml")
                 if not exists(job_conf_path):
                     job_conf_path = join(dirname(self.config_file), "job_conf.xml")
             else:
                 job_conf_path = join(dirname(self.config_file), job_conf_path)
             if ".xml" in job_conf_path:
                 try:
-                    try:
-                        for plugin in parse_xml(job_conf_path).find("plugins").findall("plugin"):
+                    job_conf_tree = parse_xml(job_conf_path)
+                    plugins_elem = job_conf_tree.find("plugins")
+                    if plugins_elem:
+                        for plugin in plugins_elem.findall("plugin"):
                             if "load" in plugin.attrib:
                                 self.job_runners.append(plugin.attrib["load"])
-                    except OSError:
-                        pass
-                    try:
-                        for plugin in parse_xml(job_conf_path).findall('.//destination/param[@id="rules_module"]'):
-                            self.job_rule_modules.append(plugin.text)
-                    except OSError:
-                        pass
-                except etree.ParseError:
+                    for plugin in job_conf_tree.findall('.//destination/param[@id="rules_module"]'):
+                        self.job_rule_modules.append(plugin.text)
+                except (OSError, etree.ParseError):
                     pass
             else:
                 try:
                     with open(job_conf_path) as f:
                         job_conf_dict = yaml.safe_load(f)
                     load_job_config_dict(job_conf_dict)
                 except OSError:
@@ -203,15 +200,15 @@
 
     def check_total_perspective_vortex(self):
         return "tpv.rules" in self.job_rule_modules
 
     def check_pbs_python(self):
         return "galaxy.jobs.runners.pbs:PBSJobRunner" in self.job_runners
 
-    def check_pykube(self):
+    def check_pykube_ng(self):
         return "galaxy.jobs.runners.kubernetes:KubernetesJobRunner" in self.job_runners or which("kubectl")
 
     def check_chronos_python(self):
         return "galaxy.jobs.runners.chronos:ChronosJobRunner" in self.job_runners
 
     def check_boto3_python(self):
         return "galaxy.jobs.runners.aws:AWSBatchJobRunner" in self.job_runners
```

### Comparing `galaxy-app-23.2.1/galaxy/dependencies/conditional-requirements.txt` & `galaxy-app-24.0.0/galaxy/dependencies/conditional-requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # These dependencies are only required when certain config options are set
-psycopg2-binary==2.9.5
+psycopg2-binary==2.9.9
 mysqlclient
 fluent-logger
 sentry-sdk[fastapi]
 pbs_python
 drmaa
 statsd
 azure-storage==0.32.0
@@ -31,15 +31,15 @@
 hvac
 custos-sdk
 
 # Chronos client
 chronos-python==1.2.1
 
 # Kubernetes job runner
-pykube==0.15.0
+pykube-ng==21.3.0
 
 # Synnefo / Pithos+ object store client
 kamaki
 
 watchdog
 
 # Error reporters optional modules
```

### Comparing `galaxy-app-23.2.1/galaxy/dependencies/dev-requirements.txt` & `galaxy-app-24.0.0/galaxy/dependencies/dev-requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,179 +1,171 @@
-aiohttp==3.8.6 ; python_version >= "3.7" and python_version < "3.12"
-aiosignal==1.3.1 ; python_version >= "3.7" and python_version < "3.12"
-alabaster==0.7.13 ; python_version >= "3.7" and python_version < "3.12"
-amqp==5.2.0 ; python_version >= "3.7" and python_version < "3.12"
-anyio==3.7.1 ; python_version >= "3.7" and python_version < "3.12"
-ase==3.22.1 ; python_version >= "3.7" and python_version < "3.12"
-async-timeout==4.0.3 ; python_version >= "3.7" and python_version < "3.12"
-asynctest==0.13.0 ; python_version >= "3.7" and python_version < "3.8"
-attrs==23.1.0 ; python_version >= "3.7" and python_version < "3.12"
-axe-selenium-python==2.1.6 ; python_version >= "3.7" and python_version < "3.12"
-babel==2.13.1 ; python_version >= "3.7" and python_version < "3.12"
-billiard==3.6.4.0 ; python_version >= "3.7" and python_version < "3.8"
-billiard==4.2.0 ; python_version >= "3.8" and python_version < "3.12"
-black==23.3.0 ; python_version >= "3.7" and python_version < "3.12"
-bleach==6.0.0 ; python_version >= "3.7" and python_version < "3.12"
-build==1.0.3 ; python_version >= "3.7" and python_version < "3.12"
-cachecontrol[filecache]==0.13.1 ; python_version >= "3.7" and python_version < "3.12"
-cached-property==1.5.2 ; python_version >= "3.7" and python_version < "3.8"
-celery==5.2.7 ; python_version >= "3.7" and python_version < "3.8"
-celery==5.3.6 ; python_version >= "3.8" and python_version < "3.12"
-certifi==2023.11.17 ; python_version >= "3.7" and python_version < "3.12"
-cffi==1.15.1 ; python_version >= "3.7" and python_version < "3.12"
-charset-normalizer==3.3.2 ; python_version >= "3.7" and python_version < "3.12"
-click-didyoumean==0.3.0 ; python_version >= "3.7" and python_version < "3.12"
-click-plugins==1.1.1 ; python_version >= "3.7" and python_version < "3.12"
-click-repl==0.3.0 ; python_version >= "3.7" and python_version < "3.12"
-click==8.1.7 ; python_version >= "3.7" and python_version < "3.12"
-codespell==2.2.5 ; python_version >= "3.7" and python_version < "3.12"
-colorama==0.4.6 ; python_version >= "3.7" and python_version < "3.12" and (sys_platform == "win32" or platform_system == "Windows" or os_name == "nt")
-coverage[toml]==7.2.7 ; python_version >= "3.7" and python_version < "3.12"
-cryptography==41.0.5 ; python_version >= "3.7" and python_version < "3.12"
-cwltest==2.3.20230825125225 ; python_version >= "3.7" and python_version < "3.12"
-cycler==0.11.0 ; python_version >= "3.7" and python_version < "3.12"
-darker==1.7.2 ; python_version >= "3.7" and python_version < "3.12"
-defusedxml==0.7.1 ; python_version >= "3.7" and python_version < "3.12"
-deprecated==1.2.14 ; python_version >= "3.7" and python_version < "3.12"
-docutils==0.18.1 ; python_version >= "3.7" and python_version < "3.12"
-exceptiongroup==1.2.0 ; python_version >= "3.7" and python_version < "3.11"
-filelock==3.12.2 ; python_version >= "3.7" and python_version < "3.12"
-fluent-logger==0.10.0 ; python_version >= "3.7" and python_version < "3.12"
-fonttools==4.38.0 ; python_version >= "3.7" and python_version < "3.12"
-frozenlist==1.3.3 ; python_version >= "3.7" and python_version < "3.12"
-future==0.18.3 ; python_version >= "3.7" and python_version < "3.12"
-galaxy-release-util==0.1.5 ; python_version >= "3.7" and python_version < "3.12"
-greenlet==2.0.2 ; python_version >= "3.7" and python_version < "3.12"
-h11==0.14.0 ; python_version >= "3.7" and python_version < "3.12"
-httpcore==0.17.3 ; python_version >= "3.7" and python_version < "3.12"
-httpx==0.24.1 ; python_version >= "3.7" and python_version < "3.12"
-idna==3.5 ; python_version >= "3.7" and python_version < "3.12"
-imagesize==1.4.1 ; python_version >= "3.7" and python_version < "3.12"
-importlib-metadata==4.13.0 ; python_version >= "3.7" and python_version < "3.12"
-importlib-resources==5.12.0 ; python_version >= "3.7" and python_version < "3.12"
-iniconfig==2.0.0 ; python_version >= "3.7" and python_version < "3.12"
-isodate==0.6.1 ; python_version >= "3.7" and python_version < "3.12"
-isort==5.11.5 ; python_version >= "3.7" and python_version < "3.12"
-jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "3.12"
-jeepney==0.8.0 ; python_version >= "3.7" and python_version < "3.12" and sys_platform == "linux"
-jinja2==3.1.2 ; python_version >= "3.7" and python_version < "3.12"
-junit-xml==1.9 ; python_version >= "3.7" and python_version < "3.12"
-keyring==24.1.1 ; python_version >= "3.7" and python_version < "3.12"
-kiwisolver==1.4.5 ; python_version >= "3.7" and python_version < "3.12"
-kombu==5.2.4 ; python_version >= "3.7" and python_version < "3.8"
-kombu==5.3.5 ; python_version >= "3.8" and python_version < "3.12"
-lxml==4.9.3 ; python_version >= "3.7" and python_version < "3.12"
-markdown-it-py==2.2.0 ; python_version >= "3.7" and python_version < "3.12"
-markdown-it-reporter==0.0.2 ; python_version >= "3.7" and python_version < "3.12"
-markupsafe==2.1.3 ; python_version >= "3.7" and python_version < "3.12"
-matplotlib==3.5.3 ; python_version >= "3.7" and python_version < "3.8"
-matplotlib==3.7.4 ; python_version >= "3.8" and python_version < "3.9"
-matplotlib==3.8.2 ; python_version >= "3.9" and python_version < "3.12"
-mdit-py-plugins==0.3.5 ; python_version >= "3.7" and python_version < "3.12"
-mdurl==0.1.2 ; python_version >= "3.7" and python_version < "3.12"
-mirakuru==2.5.1 ; python_version >= "3.7" and python_version < "3.12"
-mistune==2.0.5 ; python_version >= "3.7" and python_version < "3.12"
-more-itertools==9.1.0 ; python_version >= "3.7" and python_version < "3.12"
-msgpack==1.0.5 ; python_version >= "3.7" and python_version < "3.12"
-multidict==6.0.4 ; python_version >= "3.7" and python_version < "3.12"
-mypy-extensions==1.0.0 ; python_version >= "3.7" and python_version < "3.12"
-myst-parser==1.0.0 ; python_version >= "3.7" and python_version < "3.12"
-numpy==1.21.6 ; python_version >= "3.7" and python_version < "3.8"
+aiohttp==3.9.3 ; python_version >= "3.8" and python_version < "3.13"
+aiosignal==1.3.1 ; python_version >= "3.8" and python_version < "3.13"
+alabaster==0.7.13 ; python_version >= "3.8" and python_version < "3.13"
+amqp==5.2.0 ; python_version >= "3.8" and python_version < "3.13"
+anyio==4.3.0 ; python_version >= "3.8" and python_version < "3.13"
+ase==3.22.1 ; python_version >= "3.8" and python_version < "3.13"
+async-timeout==4.0.3 ; python_version >= "3.8" and python_version < "3.11"
+attrs==23.2.0 ; python_version >= "3.8" and python_version < "3.13"
+axe-selenium-python==2.1.6 ; python_version >= "3.8" and python_version < "3.13"
+babel==2.14.0 ; python_version >= "3.8" and python_version < "3.13"
+backports-zoneinfo==0.2.1 ; python_version >= "3.8" and python_version < "3.9"
+backports-zoneinfo[tzdata]==0.2.1 ; python_version >= "3.8" and python_version < "3.9"
+billiard==4.2.0 ; python_version >= "3.8" and python_version < "3.13"
+black==24.1.1 ; python_version >= "3.8" and python_version < "3.13"
+build==1.1.1 ; python_version >= "3.8" and python_version < "3.13"
+cachecontrol[filecache]==0.13.1 ; python_version >= "3.8" and python_version < "3.13"
+celery==5.3.6 ; python_version >= "3.8" and python_version < "3.13"
+certifi==2024.2.2 ; python_version >= "3.8" and python_version < "3.13"
+cffi==1.16.0 ; python_version >= "3.8" and python_version < "3.13"
+charset-normalizer==3.3.2 ; python_version >= "3.8" and python_version < "3.13"
+click-didyoumean==0.3.0 ; python_version >= "3.8" and python_version < "3.13"
+click-plugins==1.1.1 ; python_version >= "3.8" and python_version < "3.13"
+click-repl==0.3.0 ; python_version >= "3.8" and python_version < "3.13"
+click==8.1.7 ; python_version >= "3.8" and python_version < "3.13"
+codespell==2.2.6 ; python_version >= "3.8" and python_version < "3.13"
+colorama==0.4.6 ; python_version >= "3.8" and python_version < "3.13" and (sys_platform == "win32" or platform_system == "Windows" or os_name == "nt")
+contourpy==1.1.1 ; python_version >= "3.8" and python_version < "3.13"
+coverage[toml]==7.4.3 ; python_version >= "3.8" and python_version < "3.13"
+cryptography==42.0.5 ; python_version >= "3.8" and python_version < "3.13"
+cwltest==2.5.20240304113812 ; python_version >= "3.8" and python_version < "3.13"
+cycler==0.12.1 ; python_version >= "3.8" and python_version < "3.13"
+darker==1.7.3 ; python_version >= "3.8" and python_version < "3.13"
+defusedxml==0.7.1 ; python_version >= "3.8" and python_version < "3.13"
+deprecated==1.2.14 ; python_version >= "3.8" and python_version < "3.13"
+docutils==0.18.1 ; python_version >= "3.8" and python_version < "3.13"
+exceptiongroup==1.2.0 ; python_version >= "3.8" and python_version < "3.11"
+filelock==3.13.1 ; python_version >= "3.8" and python_version < "3.13"
+fluent-logger==0.11.0 ; python_version >= "3.8" and python_version < "3.13"
+fonttools==4.49.0 ; python_version >= "3.8" and python_version < "3.13"
+frozenlist==1.4.1 ; python_version >= "3.8" and python_version < "3.13"
+galaxy-release-util==0.1.7 ; python_version >= "3.8" and python_version < "3.13"
+greenlet==3.0.3 ; python_version >= "3.8" and python_version < "3.13"
+h11==0.14.0 ; python_version >= "3.8" and python_version < "3.13"
+httpcore==1.0.4 ; python_version >= "3.8" and python_version < "3.13"
+httpx==0.27.0 ; python_version >= "3.8" and python_version < "3.13"
+idna==3.6 ; python_version >= "3.8" and python_version < "3.13"
+imagesize==1.4.1 ; python_version >= "3.8" and python_version < "3.13"
+importlib-metadata==7.0.1 ; python_version >= "3.8" and python_version < "3.13"
+importlib-resources==6.1.2 ; python_version >= "3.8" and python_version < "3.10"
+iniconfig==2.0.0 ; python_version >= "3.8" and python_version < "3.13"
+isodate==0.6.1 ; python_version >= "3.8" and python_version < "3.13"
+isort==5.13.2 ; python_version >= "3.8" and python_version < "3.13"
+jaraco-classes==3.3.1 ; python_version >= "3.8" and python_version < "3.13"
+jeepney==0.8.0 ; python_version >= "3.8" and python_version < "3.13" and sys_platform == "linux"
+jinja2==3.1.3 ; python_version >= "3.8" and python_version < "3.13"
+junit-xml==1.9 ; python_version >= "3.8" and python_version < "3.13"
+keyring==24.3.1 ; python_version >= "3.8" and python_version < "3.13"
+kiwisolver==1.4.5 ; python_version >= "3.8" and python_version < "3.13"
+kombu==5.3.5 ; python_version >= "3.8" and python_version < "3.13"
+lxml==4.9.4 ; python_version >= "3.8" and python_version < "3.13"
+markdown-it-py==3.0.0 ; python_version >= "3.8" and python_version < "3.13"
+markdown-it-reporter==0.0.2 ; python_version >= "3.8" and python_version < "3.13"
+markupsafe==2.1.5 ; python_version >= "3.8" and python_version < "3.13"
+matplotlib==3.7.5 ; python_version >= "3.8" and python_version < "3.9"
+matplotlib==3.8.3 ; python_version >= "3.9" and python_version < "3.13"
+mdit-py-plugins==0.4.0 ; python_version >= "3.8" and python_version < "3.13"
+mdurl==0.1.2 ; python_version >= "3.8" and python_version < "3.13"
+mirakuru==2.5.2 ; python_version >= "3.8" and python_version < "3.13"
+mistune==2.0.5 ; python_version >= "3.8" and python_version < "3.13"
+more-itertools==10.2.0 ; python_version >= "3.8" and python_version < "3.13"
+msgpack==1.0.8 ; python_version >= "3.8" and python_version < "3.13"
+multidict==6.0.5 ; python_version >= "3.8" and python_version < "3.13"
+mypy-extensions==1.0.0 ; python_version >= "3.8" and python_version < "3.13"
+myst-parser==2.0.0 ; python_version >= "3.8" and python_version < "3.13"
+nh3==0.2.15 ; python_version >= "3.8" and python_version < "3.13"
 numpy==1.24.4 ; python_version >= "3.8" and python_version < "3.9"
-numpy==1.26.2 ; python_version >= "3.9" and python_version < "3.12"
-outcome==1.3.0.post0 ; python_version >= "3.7" and python_version < "3.12"
-packaging==23.2 ; python_version >= "3.7" and python_version < "3.12"
-pathspec==0.11.2 ; python_version >= "3.7" and python_version < "3.12"
-pillow==9.5.0 ; python_version >= "3.7" and python_version < "3.12"
-pkce==1.0.3 ; python_version >= "3.7" and python_version < "3.12"
-pkginfo==1.9.6 ; python_version >= "3.7" and python_version < "3.12"
-platformdirs==4.0.0 ; python_version >= "3.7" and python_version < "3.12"
-playwright==1.35.0 ; python_version >= "3.7" and python_version < "3.12"
-pluggy==1.2.0 ; python_version >= "3.7" and python_version < "3.12"
-port-for==0.7.1 ; python_version >= "3.7" and python_version < "3.12"
-prettytable==3.7.0 ; python_version >= "3.7" and python_version < "3.12"
-prompt-toolkit==3.0.41 ; python_version >= "3.7" and python_version < "3.12"
-psutil==5.9.6 ; python_version >= "3.7" and python_version < "3.12" and sys_platform != "cygwin"
-py==1.11.0 ; python_version >= "3.7" and python_version < "3.12"
-pycparser==2.21 ; python_version >= "3.7" and python_version < "3.12"
-pyee==9.0.4 ; python_version >= "3.7" and python_version < "3.12"
-pygithub==2.1.1 ; python_version >= "3.7" and python_version < "3.12"
-pygments==2.17.2 ; python_version >= "3.7" and python_version < "3.12"
-pyjwt[crypto]==2.8.0 ; python_version >= "3.7" and python_version < "3.12"
-pynacl==1.5.0 ; python_version >= "3.7" and python_version < "3.12"
-pyparsing==3.0.9 ; python_version >= "3.7" and python_version < "3.12"
-pyproject-hooks==1.0.0 ; python_version >= "3.7" and python_version < "3.12"
-pysocks==1.7.1 ; python_version >= "3.7" and python_version < "3.12"
-pytest-asyncio==0.21.1 ; python_version >= "3.7" and python_version < "3.12"
-pytest-base-url==2.0.0 ; python_version >= "3.7" and python_version < "3.12"
-pytest-celery==0.0.0 ; python_version >= "3.7" and python_version < "3.12"
-pytest-cov==4.1.0 ; python_version >= "3.7" and python_version < "3.12"
-pytest-html==3.2.0 ; python_version >= "3.7" and python_version < "3.12"
-pytest-httpserver==1.0.6 ; python_version >= "3.7" and python_version < "3.12"
-pytest-json-report==1.5.0 ; python_version >= "3.7" and python_version < "3.12"
-pytest-metadata==3.0.0 ; python_version >= "3.7" and python_version < "3.12"
-pytest-mock==3.11.1 ; python_version >= "3.7" and python_version < "3.12"
-pytest-playwright==0.3.3 ; python_version >= "3.7" and python_version < "3.12"
-pytest-postgresql==4.1.1 ; python_version >= "3.7" and python_version < "3.12"
-pytest-shard==0.1.2 ; python_version >= "3.7" and python_version < "3.12"
-pytest==7.4.3 ; python_version >= "3.7" and python_version < "3.12"
-python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "3.12"
-python-irodsclient==1.1.9 ; python_version >= "3.7" and python_version < "3.12"
-python-slugify==8.0.1 ; python_version >= "3.7" and python_version < "3.12"
-pytz==2023.3.post1 ; python_version >= "3.7" and python_version < "3.12"
-pywin32-ctypes==0.2.2 ; python_version >= "3.7" and python_version < "3.12" and sys_platform == "win32"
-pyyaml==6.0.1 ; python_version >= "3.7" and python_version < "3.12"
-rdflib==6.2.0 ; python_version >= "3.7" and python_version < "3.12"
-readme-renderer==37.3 ; python_version >= "3.7" and python_version < "3.12"
-requests-toolbelt==1.0.0 ; python_version >= "3.7" and python_version < "3.12"
-requests==2.31.0 ; python_version >= "3.7" and python_version < "3.12"
-responses==0.23.3 ; python_version >= "3.7" and python_version < "3.12"
-rfc3986==2.0.0 ; python_version >= "3.7" and python_version < "3.12"
-rich==13.7.0 ; python_version >= "3.7" and python_version < "3.12"
-ruamel-yaml-clib==0.2.8 ; platform_python_implementation == "CPython" and python_version < "3.11" and python_version >= "3.7"
-ruamel-yaml==0.17.21 ; python_version >= "3.7" and python_version < "3.12"
-schema-salad==8.4.20230808163024 ; python_version >= "3.7" and python_version < "3.12"
-scipy==1.7.3 ; python_version >= "3.7" and python_version < "3.8"
+numpy==1.26.4 ; python_version >= "3.9" and python_version < "3.13"
+outcome==1.3.0.post0 ; python_version >= "3.8" and python_version < "3.13"
+packaging==23.2 ; python_version >= "3.8" and python_version < "3.13"
+pathspec==0.12.1 ; python_version >= "3.8" and python_version < "3.13"
+pillow==10.2.0 ; python_version >= "3.8" and python_version < "3.13"
+pkce==1.0.3 ; python_version >= "3.8" and python_version < "3.13"
+pkginfo==1.10.0 ; python_version >= "3.8" and python_version < "3.13"
+platformdirs==4.2.0 ; python_version >= "3.8" and python_version < "3.13"
+playwright==1.41.2 ; python_version >= "3.8" and python_version < "3.13"
+pluggy==1.4.0 ; python_version >= "3.8" and python_version < "3.13"
+port-for==0.7.2 ; python_version >= "3.8" and python_version < "3.13"
+prettytable==3.10.0 ; python_version >= "3.8" and python_version < "3.13"
+prompt-toolkit==3.0.43 ; python_version >= "3.8" and python_version < "3.13"
+psutil==5.9.8 ; python_version >= "3.8" and python_version < "3.13" and sys_platform != "cygwin"
+psycopg==3.1.18 ; python_version >= "3.8" and python_version < "3.13"
+pycparser==2.21 ; python_version >= "3.8" and python_version < "3.13"
+pyee==11.0.1 ; python_version >= "3.8" and python_version < "3.13"
+pygithub==2.2.0 ; python_version >= "3.8" and python_version < "3.13"
+pygments==2.17.2 ; python_version >= "3.8" and python_version < "3.13"
+pyjwt[crypto]==2.8.0 ; python_version >= "3.8" and python_version < "3.13"
+pynacl==1.5.0 ; python_version >= "3.8" and python_version < "3.13"
+pyparsing==3.1.1 ; python_version >= "3.8" and python_version < "3.13"
+pyproject-hooks==1.0.0 ; python_version >= "3.8" and python_version < "3.13"
+pysocks==1.7.1 ; python_version >= "3.8" and python_version < "3.13"
+pytest-asyncio==0.23.5 ; python_version >= "3.8" and python_version < "3.13"
+pytest-base-url==2.1.0 ; python_version >= "3.8" and python_version < "3.13"
+pytest-celery==0.0.0 ; python_version >= "3.8" and python_version < "3.13"
+pytest-cov==4.1.0 ; python_version >= "3.8" and python_version < "3.13"
+pytest-html==4.1.1 ; python_version >= "3.8" and python_version < "3.13"
+pytest-httpserver==1.0.10 ; python_version >= "3.8" and python_version < "3.13"
+pytest-json-report==1.5.0 ; python_version >= "3.8" and python_version < "3.13"
+pytest-metadata==3.1.1 ; python_version >= "3.8" and python_version < "3.13"
+pytest-mock==3.12.0 ; python_version >= "3.8" and python_version < "3.13"
+pytest-playwright==0.4.4 ; python_version >= "3.8" and python_version < "3.13"
+pytest-postgresql==5.1.0 ; python_version >= "3.8" and python_version < "3.13"
+pytest-shard==0.1.2 ; python_version >= "3.8" and python_version < "3.13"
+pytest==7.4.4 ; python_version >= "3.8" and python_version < "3.13"
+python-dateutil==2.9.0.post0 ; python_version >= "3.8" and python_version < "3.13"
+python-irodsclient==2.0.0 ; python_version >= "3.8" and python_version < "3.13"
+python-slugify==8.0.4 ; python_version >= "3.8" and python_version < "3.13"
+pytz==2024.1 ; python_version >= "3.8" and python_version < "3.9"
+pywin32-ctypes==0.2.2 ; python_version >= "3.8" and python_version < "3.13" and sys_platform == "win32"
+pyyaml==6.0.1 ; python_version >= "3.8" and python_version < "3.13"
+rdflib==6.3.2 ; python_version >= "3.8" and python_version < "3.13"
+readme-renderer==43.0 ; python_version >= "3.8" and python_version < "3.13"
+requests-toolbelt==1.0.0 ; python_version >= "3.8" and python_version < "3.13"
+requests==2.31.0 ; python_version >= "3.8" and python_version < "3.13"
+responses==0.25.0 ; python_version >= "3.8" and python_version < "3.13"
+rfc3986==2.0.0 ; python_version >= "3.8" and python_version < "3.13"
+rich==13.7.1 ; python_version >= "3.8" and python_version < "3.13"
+ruamel-yaml-clib==0.2.8 ; platform_python_implementation == "CPython" and python_version < "3.13" and python_version >= "3.8"
+ruamel-yaml==0.18.6 ; python_version >= "3.8" and python_version < "3.13"
+schema-salad==8.5.20240102191335 ; python_version >= "3.8" and python_version < "3.13"
 scipy==1.10.1 ; python_version >= "3.8" and python_version < "3.9"
-scipy==1.11.4 ; python_version >= "3.9" and python_version < "3.12"
-secretstorage==3.3.3 ; python_version >= "3.7" and python_version < "3.12" and sys_platform == "linux"
-selenium==4.11.2 ; python_version >= "3.7" and python_version < "3.12"
-seletools==1.4.0 ; python_version >= "3.7" and python_version < "3.12"
-setuptools==68.0.0 ; python_version >= "3.7" and python_version < "3.12"
-six==1.16.0 ; python_version >= "3.7" and python_version < "3.12"
-sniffio==1.3.0 ; python_version >= "3.7" and python_version < "3.12"
-snowballstemmer==2.2.0 ; python_version >= "3.7" and python_version < "3.12"
-sortedcontainers==2.4.0 ; python_version >= "3.7" and python_version < "3.12"
-sphinx-rtd-theme==1.3.0 ; python_version >= "3.7" and python_version < "3.12"
-sphinx==5.3.0 ; python_version >= "3.7" and python_version < "3.12"
-sphinxcontrib-applehelp==1.0.2 ; python_version >= "3.7" and python_version < "3.12"
-sphinxcontrib-devhelp==1.0.2 ; python_version >= "3.7" and python_version < "3.12"
-sphinxcontrib-htmlhelp==2.0.0 ; python_version >= "3.7" and python_version < "3.12"
-sphinxcontrib-jquery==4.1 ; python_version >= "3.7" and python_version < "3.12"
-sphinxcontrib-jsmath==1.0.1 ; python_version >= "3.7" and python_version < "3.12"
-sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.7" and python_version < "3.12"
-sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.7" and python_version < "3.12"
-statsd==4.0.1 ; python_version >= "3.7" and python_version < "3.12"
-testfixtures==7.2.2 ; python_version >= "3.7" and python_version < "3.12"
-text-unidecode==1.3 ; python_version >= "3.7" and python_version < "3.12"
-tinydb==4.8.0 ; python_version >= "3.7" and python_version < "3.12"
-toml==0.10.2 ; python_version >= "3.7" and python_version < "3.12"
-tomli==2.0.1 ; python_version >= "3.7" and python_full_version <= "3.11.0a6"
-trio-websocket==0.11.1 ; python_version >= "3.7" and python_version < "3.12"
-trio==0.22.2 ; python_version >= "3.7" and python_version < "3.12"
-tuspy==1.0.1 ; python_version >= "3.7" and python_version < "3.12"
-twill==3.1 ; python_version >= "3.7" and python_version < "3.12"
-twine==4.0.2 ; python_version >= "3.7" and python_version < "3.12"
-typed-ast==1.5.5 ; python_version < "3.8" and implementation_name == "cpython" and python_version >= "3.7"
-types-pyyaml==6.0.12.12 ; python_version >= "3.7" and python_version < "3.12"
-typing-extensions==4.7.1 ; python_version >= "3.7" and python_version < "3.12"
-urllib3==1.26.18 ; python_version >= "3.7" and python_version < "3.12"
-urllib3[socks]==1.26.18 ; python_version >= "3.7" and python_version < "3.12"
-vine==5.1.0 ; python_version >= "3.7" and python_version < "3.12"
-watchdog==3.0.0 ; python_version >= "3.7" and python_version < "3.12"
-wcwidth==0.2.12 ; python_version >= "3.7" and python_version < "3.12"
-webencodings==0.5.1 ; python_version >= "3.7" and python_version < "3.12"
-werkzeug==2.2.3 ; python_version >= "3.7" and python_version < "3.12"
-wrapt==1.16.0 ; python_version >= "3.7" and python_version < "3.12"
-wsproto==1.2.0 ; python_version >= "3.7" and python_version < "3.12"
-yarl==1.9.3 ; python_version >= "3.7" and python_version < "3.12"
-zipp==3.15.0 ; python_version >= "3.7" and python_version < "3.12"
+scipy==1.12.0 ; python_version >= "3.9" and python_version < "3.13"
+secretstorage==3.3.3 ; python_version >= "3.8" and python_version < "3.13" and sys_platform == "linux"
+selenium==4.18.1 ; python_version >= "3.8" and python_version < "3.13"
+seletools==1.4.0 ; python_version >= "3.8" and python_version < "3.13"
+setuptools==69.1.1 ; python_version >= "3.8" and python_version < "3.13"
+six==1.16.0 ; python_version >= "3.8" and python_version < "3.13"
+sniffio==1.3.1 ; python_version >= "3.8" and python_version < "3.13"
+snowballstemmer==2.2.0 ; python_version >= "3.8" and python_version < "3.13"
+sortedcontainers==2.4.0 ; python_version >= "3.8" and python_version < "3.13"
+sphinx-rtd-theme==1.3.0 ; python_version >= "3.8" and python_version < "3.13"
+sphinx==7.1.2 ; python_version >= "3.8" and python_version < "3.13"
+sphinxcontrib-applehelp==1.0.4 ; python_version >= "3.8" and python_version < "3.13"
+sphinxcontrib-devhelp==1.0.2 ; python_version >= "3.8" and python_version < "3.13"
+sphinxcontrib-htmlhelp==2.0.1 ; python_version >= "3.8" and python_version < "3.13"
+sphinxcontrib-jquery==4.1 ; python_version >= "3.8" and python_version < "3.13"
+sphinxcontrib-jsmath==1.0.1 ; python_version >= "3.8" and python_version < "3.13"
+sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.8" and python_version < "3.13"
+sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.8" and python_version < "3.13"
+statsd==4.0.1 ; python_version >= "3.8" and python_version < "3.13"
+testfixtures==8.1.0 ; python_version >= "3.8" and python_version < "3.13"
+text-unidecode==1.3 ; python_version >= "3.8" and python_version < "3.13"
+tinydb==4.8.0 ; python_version >= "3.8" and python_version < "3.13"
+toml==0.10.2 ; python_version >= "3.8" and python_version < "3.13"
+tomli==2.0.1 ; python_version >= "3.8" and python_full_version <= "3.11.0a6"
+trio-websocket==0.11.1 ; python_version >= "3.8" and python_version < "3.13"
+trio==0.24.0 ; python_version >= "3.8" and python_version < "3.13"
+tuspy==1.0.3 ; python_version >= "3.8" and python_version < "3.13"
+twill==3.2.2 ; python_version >= "3.8" and python_version < "3.13"
+twine==5.0.0 ; python_version >= "3.8" and python_version < "3.13"
+typing-extensions==4.10.0 ; python_version >= "3.8" and python_version < "3.13"
+tzdata==2024.1 ; python_version >= "3.8" and python_version < "3.13"
+urllib3==1.26.18 ; python_version >= "3.8" and python_version < "3.13"
+urllib3[socks]==1.26.18 ; python_version >= "3.8" and python_version < "3.13"
+vine==5.1.0 ; python_version >= "3.8" and python_version < "3.13"
+watchdog==4.0.0 ; python_version >= "3.8" and python_version < "3.13"
+wcwidth==0.2.13 ; python_version >= "3.8" and python_version < "3.13"
+werkzeug==3.0.1 ; python_version >= "3.8" and python_version < "3.13"
+wrapt==1.16.0 ; python_version >= "3.8" and python_version < "3.13"
+wsproto==1.2.0 ; python_version >= "3.8" and python_version < "3.13"
+yarl==1.9.4 ; python_version >= "3.8" and python_version < "3.13"
+zipp==3.17.0 ; python_version >= "3.8" and python_version < "3.13"
```

### Comparing `galaxy-app-23.2.1/galaxy/dependencies/pinned-requirements.txt` & `galaxy-app-24.0.0/galaxy/dependencies/pinned-requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,221 +1,222 @@
-a2wsgi==1.7.0 ; python_version >= "3.7" and python_version < "3.12"
-adal==1.2.7 ; python_version >= "3.7" and python_version < "3.12"
-aiobotocore==2.4.2 ; python_version >= "3.7" and python_version < "3.12"
-aiodataloader==0.4.0 ; python_version >= "3.7" and python_version < "3.12"
-aiofiles==23.2.1 ; python_version >= "3.7" and python_version < "3.12"
-aiohttp==3.8.6 ; python_version >= "3.7" and python_version < "3.12"
-aioitertools==0.11.0 ; python_version >= "3.7" and python_version < "3.12"
-aiosignal==1.3.1 ; python_version >= "3.7" and python_version < "3.12"
-alembic==1.12.1 ; python_version >= "3.7" and python_version < "3.12"
-amqp==5.2.0 ; python_version >= "3.7" and python_version < "3.12"
-aniso8601==9.0.1 ; python_version >= "3.7" and python_version < "3.12"
-anyio==3.7.1 ; python_version >= "3.7" and python_version < "3.12"
-apispec==6.3.0 ; python_version >= "3.7" and python_version < "3.12"
-appdirs==1.4.4 ; python_version >= "3.7" and python_version < "3.12"
-arcp==0.2.1 ; python_version >= "3.7" and python_version < "3.12"
-argcomplete==3.1.2 ; python_version >= "3.7" and python_version < "3.12"
-async-timeout==4.0.3 ; python_version >= "3.7" and python_version < "3.12"
-asynctest==0.13.0 ; python_version >= "3.7" and python_version < "3.8"
-attmap==0.13.2 ; python_version >= "3.7" and python_version < "3.12"
-attrs==23.1.0 ; python_version >= "3.7" and python_version < "3.12"
-babel==2.13.1 ; python_version >= "3.7" and python_version < "3.12"
-backports-zoneinfo==0.2.1 ; python_version >= "3.7" and python_version < "3.9"
-bagit-profile==1.3.1 ; python_version >= "3.7" and python_version < "3.12"
-bagit==1.8.1 ; python_version >= "3.7" and python_version < "3.12"
-bcrypt==4.0.1 ; python_version >= "3.7" and python_version < "3.12"
-bdbag==1.7.1 ; python_version >= "3.7" and python_version < "3.12"
-beaker==1.12.1 ; python_version >= "3.7" and python_version < "3.12"
-billiard==3.6.4.0 ; python_version >= "3.7" and python_version < "3.8"
-billiard==4.2.0 ; python_version >= "3.8" and python_version < "3.12"
-bioblend==1.2.0 ; python_version >= "3.7" and python_version < "3.12"
-bleach==6.0.0 ; python_version >= "3.7" and python_version < "3.12"
-boltons==23.1.1 ; python_version >= "3.7" and python_version < "3.12"
-boto==2.49.0 ; python_version >= "3.7" and python_version < "3.12"
-botocore==1.27.59 ; python_version >= "3.7" and python_version < "3.12"
-bx-python==0.10.0 ; python_version >= "3.7" and python_version < "3.12"
-cachecontrol[filecache]==0.13.1 ; python_version >= "3.7" and python_version < "3.12"
-cached-property==1.5.2 ; python_version >= "3.7" and python_version < "3.8"
-celery==5.2.7 ; python_version >= "3.7" and python_version < "3.8"
-celery==5.3.6 ; python_version >= "3.8" and python_version < "3.12"
-certifi==2023.11.17 ; python_version >= "3.7" and python_version < "3.12"
-cffi==1.15.1 ; python_version >= "3.7" and python_version < "3.12"
-charset-normalizer==3.3.2 ; python_version >= "3.7" and python_version < "3.12"
-cheetah3==3.2.6.post1 ; python_version >= "3.7" and python_version < "3.12"
-circus==0.18.0 ; python_version >= "3.7" and python_version < "3.12"
-click-didyoumean==0.3.0 ; python_version >= "3.7" and python_version < "3.12"
-click-plugins==1.1.1 ; python_version >= "3.7" and python_version < "3.12"
-click-repl==0.3.0 ; python_version >= "3.7" and python_version < "3.12"
-click==8.1.7 ; python_version >= "3.7" and python_version < "3.12"
-cloudauthz==0.6.0 ; python_version >= "3.7" and python_version < "3.12"
-cloudbridge==3.2.0 ; python_version >= "3.7" and python_version < "3.12"
-colorama==0.4.6 ; python_version >= "3.7" and python_version < "3.12" and platform_system == "Windows"
-coloredlogs==15.0.1 ; python_version >= "3.7" and python_version < "3.12"
-conda-package-streaming==0.9.0 ; python_version >= "3.7" and python_version < "3.12"
-cryptography==41.0.5 ; python_version >= "3.7" and python_version < "3.12"
-cwl-upgrader==1.2.8 ; python_version >= "3.7" and python_version < "3.12"
-cwl-utils==0.28 ; python_version >= "3.7" and python_version < "3.12"
-cwltool==3.1.20221109155812 ; python_version >= "3.7" and python_version < "3.12"
-decorator==5.1.1 ; python_version >= "3.7" and python_version < "3.12"
-defusedxml==0.7.1 ; python_version >= "3.7" and python_version < "3.12"
-deprecation==2.1.0 ; python_version >= "3.7" and python_version < "3.12"
-dictobj==0.4 ; python_version >= "3.7" and python_version < "3.12"
-dnspython==2.3.0 ; python_version >= "3.7" and python_version < "3.12"
-docopt==0.6.2 ; python_version >= "3.7" and python_version < "3.12"
-docutils==0.18.1 ; python_version >= "3.7" and python_version < "3.12"
-dparse==0.6.3 ; python_version >= "3.7" and python_version < "3.12"
-ecdsa==0.18.0 ; python_version >= "3.7" and python_version < "3.12"
-edam-ontology==1.25.2 ; python_version >= "3.7" and python_version < "3.12"
-email-validator==2.0.0.post2 ; python_version >= "3.7" and python_version < "3.12"
-exceptiongroup==1.2.0 ; python_version >= "3.7" and python_version < "3.11"
-fastapi-utils==0.2.1 ; python_version >= "3.7" and python_version < "3.12"
-fastapi==0.98.0 ; python_version >= "3.7" and python_version < "3.12"
-filelock==3.12.2 ; python_version >= "3.7" and python_version < "3.12"
-frozenlist==1.3.3 ; python_version >= "3.7" and python_version < "3.12"
-fs==2.4.16 ; python_version >= "3.7" and python_version < "3.12"
-fsspec==2023.1.0 ; python_version >= "3.7" and python_version < "3.12"
-future==0.18.3 ; python_version >= "3.7" and python_version < "3.12"
-galaxy-sequence-utils==1.1.5 ; python_version >= "3.7" and python_version < "3.12"
-galaxy2cwl==0.1.4 ; python_version >= "3.7" and python_version < "3.12"
-graphene-sqlalchemy==3.0.0b3 ; python_version >= "3.7" and python_version < "3.12"
-graphene==3.3 ; python_version >= "3.7" and python_version < "3.12"
-graphql-core==3.2.3 ; python_version >= "3.7" and python_version < "3.12"
-graphql-relay==3.2.0 ; python_version >= "3.7" and python_version < "3.12"
-gravity==1.0.4 ; python_version >= "3.7" and python_version < "3.12"
-greenlet==2.0.2 ; python_version >= "3.7" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32") and python_version < "3.12"
-gunicorn==21.2.0 ; python_version >= "3.7" and python_version < "3.12"
-gxformat2==0.18.0 ; python_version >= "3.7" and python_version < "3.12"
-h11==0.14.0 ; python_version >= "3.7" and python_version < "3.12"
-h5grove==1.3.0 ; python_version >= "3.7" and python_version < "3.12"
-h5py==3.8.0 ; python_version >= "3.7" and python_version < "3.12"
-humanfriendly==10.0 ; python_version >= "3.7" and python_version < "3.12"
-idna==3.5 ; python_version >= "3.7" and python_version < "3.12"
-importlib-metadata==4.13.0 ; python_version >= "3.7" and python_version < "3.12"
-importlib-resources==5.12.0 ; python_version >= "3.7" and python_version < "3.12"
-isa-rwval==0.10.10 ; python_version >= "3.7" and python_version < "3.12"
-isal==1.3.0 ; python_version >= "3.7" and python_version < "3.12"
-isodate==0.6.1 ; python_version >= "3.7" and python_version < "3.12"
-jinja2==3.1.2 ; python_version >= "3.7" and python_version < "3.12"
-jmespath==1.0.1 ; python_version >= "3.7" and python_version < "3.12"
-jsonref==1.1.0 ; python_version >= "3.7" and python_version < "3.12"
-jsonschema==4.17.3 ; python_version >= "3.7" and python_version < "3.12"
-kombu==5.2.4 ; python_version >= "3.7" and python_version < "3.8"
-kombu==5.3.5 ; python_version >= "3.8" and python_version < "3.12"
-lagom==2.6.0 ; python_version >= "3.7" and python_version < "3.12"
-lxml==4.9.3 ; python_version >= "3.7" and python_version < "3.12"
-mako==1.2.4 ; python_version >= "3.7" and python_version < "3.12"
-markdown-it-py==2.2.0 ; python_version >= "3.7" and python_version < "3.12"
-markdown==3.4.4 ; python_version >= "3.7" and python_version < "3.12"
-markupsafe==2.1.3 ; python_version >= "3.7" and python_version < "3.12"
-mdurl==0.1.2 ; python_version >= "3.7" and python_version < "3.12"
-mercurial==6.6 ; python_version >= "3.7" and python_version < "3.12"
-mistune==2.0.5 ; python_version >= "3.7" and python_version < "3.12"
-mrcfile==1.4.3 ; python_version >= "3.7" and python_version < "3.12"
-msal==1.25.0 ; python_version >= "3.7" and python_version < "3.12"
-msgpack==1.0.5 ; python_version >= "3.7" and python_version < "3.12"
-multidict==6.0.4 ; python_version >= "3.7" and python_version < "3.12"
-mypy-extensions==1.0.0 ; python_version >= "3.7" and python_version < "3.12"
-networkx==2.5 ; python_version >= "3.7" and python_version < "3.12"
-nodeenv==1.8.0 ; python_version >= "3.7" and python_version < "3.12"
-numpy==1.21.6 ; python_version >= "3.7" and python_version < "3.8"
+--extra-index-url https://wheels.galaxyproject.org/simple
+
+a2wsgi==1.10.2 ; python_version >= "3.8" and python_version < "3.13"
+adal==1.2.7 ; python_version >= "3.8" and python_version < "3.13"
+aiobotocore==2.12.0 ; python_version >= "3.8" and python_version < "3.13"
+aiodataloader==0.4.0 ; python_version >= "3.8" and python_version < "3.13"
+aiofiles==23.2.1 ; python_version >= "3.8" and python_version < "3.13"
+aiohttp==3.9.3 ; python_version >= "3.8" and python_version < "3.13"
+aioitertools==0.11.0 ; python_version >= "3.8" and python_version < "3.13"
+aiosignal==1.3.1 ; python_version >= "3.8" and python_version < "3.13"
+alembic==1.13.1 ; python_version >= "3.8" and python_version < "3.13"
+amqp==5.2.0 ; python_version >= "3.8" and python_version < "3.13"
+aniso8601==9.0.1 ; python_version >= "3.8" and python_version < "3.13"
+annotated-types==0.6.0 ; python_version >= "3.8" and python_version < "3.13"
+anyio==4.3.0 ; python_version >= "3.8" and python_version < "3.13"
+apispec==6.5.0 ; python_version >= "3.8" and python_version < "3.13"
+appdirs==1.4.4 ; python_version >= "3.8" and python_version < "3.13"
+arcp==0.2.1 ; python_version >= "3.8" and python_version < "3.13"
+argcomplete==3.2.2 ; python_version >= "3.8" and python_version < "3.13"
+async-timeout==4.0.3 ; python_version >= "3.8" and python_version < "3.11"
+attmap==0.13.2 ; python_version >= "3.8" and python_version < "3.13"
+attrs==23.2.0 ; python_version >= "3.8" and python_version < "3.13"
+babel==2.14.0 ; python_version >= "3.8" and python_version < "3.13"
+backports-zoneinfo==0.2.1 ; python_version >= "3.8" and python_version < "3.9"
+backports-zoneinfo[tzdata]==0.2.1 ; python_version >= "3.8" and python_version < "3.9"
+bagit-profile==1.3.1 ; python_version >= "3.8" and python_version < "3.13"
+bagit==1.8.1 ; python_version >= "3.8" and python_version < "3.13"
+bcrypt==4.1.2 ; python_version >= "3.8" and python_version < "3.13"
+bdbag==1.7.1 ; python_version >= "3.8" and python_version < "3.13"
+beaker==1.12.1 ; python_version >= "3.8" and python_version < "3.13"
+billiard==4.2.0 ; python_version >= "3.8" and python_version < "3.13"
+bioblend==1.2.0 ; python_version >= "3.8" and python_version < "3.13"
+bleach==6.1.0 ; python_version >= "3.8" and python_version < "3.13"
+boltons==23.1.1 ; python_version >= "3.8" and python_version < "3.13"
+boto==2.49.0 ; python_version >= "3.8" and python_version < "3.13"
+botocore==1.34.51 ; python_version >= "3.8" and python_version < "3.13"
+bx-python==0.11.0 ; python_version >= "3.8" and python_version < "3.13"
+cachecontrol[filecache]==0.13.1 ; python_version >= "3.8" and python_version < "3.13"
+celery==5.3.6 ; python_version >= "3.8" and python_version < "3.13"
+certifi==2024.2.2 ; python_version >= "3.8" and python_version < "3.13"
+cffi==1.16.0 ; python_version >= "3.8" and python_version < "3.13"
+charset-normalizer==3.3.2 ; python_version >= "3.8" and python_version < "3.13"
+cheetah3==3.2.6.post1 ; python_version >= "3.8" and python_version < "3.13"
+circus==0.18.0 ; python_version >= "3.8" and python_version < "3.13"
+click-didyoumean==0.3.0 ; python_version >= "3.8" and python_version < "3.13"
+click-plugins==1.1.1 ; python_version >= "3.8" and python_version < "3.13"
+click-repl==0.3.0 ; python_version >= "3.8" and python_version < "3.13"
+click==8.1.7 ; python_version >= "3.8" and python_version < "3.13"
+cloudauthz==0.6.0 ; python_version >= "3.8" and python_version < "3.13"
+cloudbridge==3.2.0 ; python_version >= "3.8" and python_version < "3.13"
+colorama==0.4.6 ; python_version >= "3.8" and python_version < "3.13" and platform_system == "Windows"
+coloredlogs==15.0.1 ; python_version >= "3.8" and python_version < "3.13"
+conda-package-streaming==0.9.0 ; python_version >= "3.8" and python_version < "3.13"
+cryptography==42.0.5 ; python_version >= "3.8" and python_version < "3.13"
+cwl-upgrader==1.2.11 ; python_version >= "3.8" and python_version < "3.13"
+cwl-utils==0.32 ; python_version >= "3.8" and python_version < "3.13"
+cwltool==3.1.20240112164112 ; python_version >= "3.8" and python_version < "3.13"
+decorator==5.1.1 ; python_version >= "3.8" and python_version < "3.13"
+defusedxml==0.7.1 ; python_version >= "3.8" and python_version < "3.13"
+deprecation==2.1.0 ; python_version >= "3.8" and python_version < "3.13"
+dictobj==0.4 ; python_version >= "3.8" and python_version < "3.13"
+dnspython==2.6.1 ; python_version >= "3.8" and python_version < "3.13"
+docopt==0.6.2 ; python_version >= "3.8" and python_version < "3.13"
+docutils==0.18.1 ; python_version >= "3.8" and python_version < "3.13"
+dparse==0.6.3 ; python_version >= "3.8" and python_version < "3.13"
+ecdsa==0.18.0 ; python_version >= "3.8" and python_version < "3.13"
+edam-ontology==1.25.2 ; python_version >= "3.8" and python_version < "3.13"
+email-validator==2.1.1 ; python_version >= "3.8" and python_version < "3.13"
+exceptiongroup==1.2.0 ; python_version >= "3.8" and python_version < "3.11"
+fastapi==0.110.0 ; python_version >= "3.8" and python_version < "3.13"
+filelock==3.13.1 ; python_version >= "3.8" and python_version < "3.13"
+frozenlist==1.4.1 ; python_version >= "3.8" and python_version < "3.13"
+fs==2.4.16 ; python_version >= "3.8" and python_version < "3.13"
+fsspec==2023.12.2 ; python_version >= "3.8" and python_version < "3.13"
+future==1.0.0 ; python_version >= "3.8" and python_version < "3.13"
+galaxy-sequence-utils==1.1.5 ; python_version >= "3.8" and python_version < "3.13"
+galaxy2cwl==0.1.4 ; python_version >= "3.8" and python_version < "3.13"
+graphene-sqlalchemy==3.0.0rc1 ; python_version >= "3.8" and python_version < "3.13"
+graphene==3.3 ; python_version >= "3.8" and python_version < "3.13"
+graphql-core==3.2.3 ; python_version >= "3.8" and python_version < "3.13"
+graphql-relay==3.2.0 ; python_version >= "3.8" and python_version < "3.13"
+gravity==1.0.6 ; python_version >= "3.8" and python_version < "3.13"
+greenlet==3.0.3 ; python_version >= "3.8" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32") and python_version < "3.13"
+gunicorn==21.2.0 ; python_version >= "3.8" and python_version < "3.13"
+gxformat2==0.18.0 ; python_version >= "3.8" and python_version < "3.13"
+h11==0.14.0 ; python_version >= "3.8" and python_version < "3.13"
+h5grove==2.0.0 ; python_version >= "3.8" and python_version < "3.13"
+h5py==3.10.0 ; python_version >= "3.8" and python_version < "3.13"
+humanfriendly==10.0 ; python_version >= "3.8" and python_version < "3.13"
+idna==3.6 ; python_version >= "3.8" and python_version < "3.13"
+importlib-metadata==7.0.1 ; python_version >= "3.8" and python_version < "3.13"
+importlib-resources==6.1.2 ; python_version >= "3.8" and python_version < "3.9"
+isa-rwval==0.10.10 ; python_version >= "3.8" and python_version < "3.13"
+isal==1.6.0 ; python_version >= "3.8" and python_version < "3.13"
+isodate==0.6.1 ; python_version >= "3.8" and python_version < "3.13"
+jinja2==3.1.3 ; python_version >= "3.8" and python_version < "3.13"
+jmespath==1.0.1 ; python_version >= "3.8" and python_version < "3.13"
+jsonref==1.1.0 ; python_version >= "3.8" and python_version < "3.13"
+jsonschema-specifications==2023.12.1 ; python_version >= "3.8" and python_version < "3.13"
+jsonschema==4.21.1 ; python_version >= "3.8" and python_version < "3.13"
+kombu==5.3.5 ; python_version >= "3.8" and python_version < "3.13"
+lagom==2.6.0 ; python_version >= "3.8" and python_version < "3.13"
+lxml==4.9.4 ; python_version >= "3.8" and python_version < "3.13"
+mako==1.3.2 ; python_version >= "3.8" and python_version < "3.13"
+markdown-it-py==3.0.0 ; python_version >= "3.8" and python_version < "3.13"
+markdown==3.5.2 ; python_version >= "3.8" and python_version < "3.13"
+markupsafe==2.1.5 ; python_version >= "3.8" and python_version < "3.13"
+mdurl==0.1.2 ; python_version >= "3.8" and python_version < "3.13"
+mercurial==6.6.3 ; python_version >= "3.8" and python_version < "3.13"
+mistune==2.0.5 ; python_version >= "3.8" and python_version < "3.13"
+mrcfile==1.5.0 ; python_version >= "3.8" and python_version < "3.13"
+msal==1.27.0 ; python_version >= "3.8" and python_version < "3.13"
+msgpack==1.0.8 ; python_version >= "3.8" and python_version < "3.13"
+multidict==6.0.5 ; python_version >= "3.8" and python_version < "3.13"
+mypy-extensions==1.0.0 ; python_version >= "3.8" and python_version < "3.13"
+networkx==2.5 ; python_version >= "3.8" and python_version < "3.13"
+nodeenv==1.8.0 ; python_version >= "3.8" and python_version < "3.13"
 numpy==1.24.4 ; python_version >= "3.8" and python_version < "3.9"
-numpy==1.26.2 ; python_version >= "3.9" and python_version < "3.12"
-oauthlib==3.2.2 ; python_version >= "3.7" and python_version < "3.12"
-orjson==3.9.7 ; python_version >= "3.7" and python_version < "3.12"
-oyaml==1.0 ; python_version >= "3.7" and python_version < "3.12"
-packaging==23.2 ; python_version >= "3.7" and python_version < "3.12"
-paramiko==3.3.1 ; python_version >= "3.7" and python_version < "3.12"
-parsley==1.3 ; python_version >= "3.7" and python_version < "3.12"
-paste==3.7.1 ; python_version >= "3.7" and python_version < "3.12"
-pastedeploy==3.1.0 ; python_version >= "3.7" and python_version < "3.12"
-pebble==5.0.4 ; python_version >= "3.7" and python_version < "3.12"
-pkgutil-resolve-name==1.3.10 ; python_version >= "3.7" and python_version < "3.9"
-promise==2.3 ; python_version >= "3.7" and python_version < "3.12"
-prompt-toolkit==3.0.41 ; python_version >= "3.7" and python_version < "3.12"
-prov==1.5.1 ; python_version >= "3.7" and python_version < "3.12"
-psutil==5.9.6 ; python_version >= "3.7" and python_version < "3.12"
-pulsar-galaxy-lib==0.15.5 ; python_version >= "3.7" and python_version < "3.12"
-pyasn1==0.5.1 ; python_version >= "3.7" and python_version < "3.12"
-pycparser==2.21 ; python_version >= "3.7" and python_version < "3.12"
-pycryptodome==3.19.0 ; python_version >= "3.7" and python_version < "3.12"
-pydantic-tes==0.1.5 ; python_version >= "3.7" and python_version < "3.12"
-pydantic==1.10.13 ; python_version >= "3.7" and python_version < "3.12"
-pydantic[email]==1.10.13 ; python_version >= "3.7" and python_version < "3.12"
-pydot==1.4.2 ; python_version >= "3.7" and python_version < "3.12"
-pyeventsystem==0.1.0 ; python_version >= "3.7" and python_version < "3.12"
-pyfaidx==0.7.2.2 ; python_version >= "3.7" and python_version < "3.12"
-pygments==2.17.2 ; python_version >= "3.7" and python_version < "3.12"
-pyjwt==2.8.0 ; python_version >= "3.7" and python_version < "3.12"
-pyjwt[crypto]==2.8.0 ; python_version >= "3.7" and python_version < "3.12"
-pykwalify==1.8.0 ; python_version >= "3.7" and python_version < "3.12"
-pylibmagic==0.5.0 ; python_version >= "3.7" and python_version < "3.12"
-pynacl==1.5.0 ; python_version >= "3.7" and python_version < "3.12"
-pyparsing==3.0.9 ; python_version >= "3.7" and python_version < "3.12"
-pyreadline3==3.4.1 ; sys_platform == "win32" and python_version >= "3.8" and python_version < "3.12"
-pyreadline==2.1 ; sys_platform == "win32" and python_version < "3.8" and python_version >= "3.7"
-pyrsistent==0.19.3 ; python_version >= "3.7" and python_version < "3.12"
-pysam==0.22.0 ; python_version >= "3.7" and python_version < "3.12"
-python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "3.12"
-python-jose==3.3.0 ; python_version >= "3.7" and python_version < "3.12"
-python-magic==0.4.27 ; python_version >= "3.7" and python_version < "3.12"
-python-multipart==0.0.7 ; python_version >= "3.7" and python_version < "3.12"
-python3-openid==3.2.0 ; python_version >= "3.7" and python_version < "3.12"
-pytz==2023.3.post1 ; python_version >= "3.7" and python_version < "3.12"
-pyyaml==6.0.1 ; python_version >= "3.7" and python_version < "3.12"
-pyzmq==25.1.1 ; python_version >= "3.7" and python_version < "3.12"
-rdflib==6.2.0 ; python_version >= "3.7" and python_version < "3.12"
-refgenconf==0.12.2 ; python_version >= "3.7" and python_version < "3.12"
-regex==2023.10.3 ; python_version >= "3.7" and python_version < "3.12"
-repoze-lru==0.7 ; python_version >= "3.7" and python_version < "3.12"
-requests-oauthlib==1.3.1 ; python_version >= "3.7" and python_version < "3.12"
-requests-toolbelt==1.0.0 ; python_version >= "3.7" and python_version < "3.12"
-requests-unixsocket==0.3.0 ; python_version >= "3.7" and python_version < "3.12"
-requests==2.31.0 ; python_version >= "3.7" and python_version < "3.12"
-rich==13.7.0 ; python_version >= "3.7" and python_version < "3.12"
-rocrate==0.9.0 ; python_version >= "3.7" and python_version < "3.12"
-routes==2.5.1 ; python_version >= "3.7" and python_version < "3.12"
-rsa==4.9 ; python_version >= "3.7" and python_version < "3.12"
-ruamel-yaml-clib==0.2.8 ; platform_python_implementation == "CPython" and python_version < "3.11" and python_version >= "3.7"
-ruamel-yaml==0.17.21 ; python_version >= "3.7" and python_version < "3.12"
-s3fs==2023.1.0 ; python_version >= "3.7" and python_version < "3.12"
-schema-salad==8.4.20230808163024 ; python_version >= "3.7" and python_version < "3.12"
-setuptools-scm==5.0.2 ; python_version >= "3.7" and python_version < "3.12"
-setuptools==68.0.0 ; python_version >= "3.7" and python_version < "3.12"
-shellescape==3.8.1 ; python_version >= "3.7" and python_version < "3.12"
-six==1.16.0 ; python_version >= "3.7" and python_version < "3.12"
-sniffio==1.3.0 ; python_version >= "3.7" and python_version < "3.12"
-social-auth-core[openidconnect]==4.0.3 ; python_version >= "3.7" and python_version < "3.12"
-sortedcontainers==2.4.0 ; python_version >= "3.7" and python_version < "3.12"
-sqlalchemy==1.4.50 ; python_version >= "3.7" and python_version < "3.12"
-sqlitedict==2.1.0 ; python_version >= "3.7" and python_version < "3.12"
-sqlparse==0.4.4 ; python_version >= "3.7" and python_version < "3.12"
-starlette-context==0.3.5 ; python_version >= "3.7" and python_version < "3.12"
-starlette-graphene3==0.6.0 ; python_version >= "3.7" and python_version < "3.12"
-starlette==0.27.0 ; python_version >= "3.7" and python_version < "3.12"
-supervisor==4.2.5 ; python_version >= "3.7" and python_version < "3.12"
-svgwrite==1.4.3 ; python_version >= "3.7" and python_version < "3.12"
-tenacity==8.2.3 ; python_version >= "3.7" and python_version < "3.12"
-tifffile==2021.11.2 ; python_version >= "3.7" and python_version < "3.12"
-tinydb==4.8.0 ; python_version >= "3.7" and python_version < "3.12"
-tomli==2.0.1 ; python_version >= "3.7" and python_version < "3.11"
-tornado==6.2 ; python_version >= "3.7" and python_version < "3.12"
-tqdm==4.66.1 ; python_version >= "3.7" and python_version < "3.12"
-tuspy==1.0.1 ; python_version >= "3.7" and python_version < "3.12"
-tuswsgi==0.5.5 ; python_version >= "3.7" and python_version < "3.12"
-typing-extensions==4.7.1 ; python_version >= "3.7" and python_version < "3.12"
-tzdata==2023.3 ; python_version >= "3.7" and python_version < "3.12" and platform_system == "Windows"
-tzlocal==5.1 ; python_version >= "3.7" and python_version < "3.12"
-ubiquerg==0.6.3 ; python_version >= "3.7" and python_version < "3.12"
-urllib3==1.26.18 ; python_version >= "3.7" and python_version < "3.12"
-uvicorn==0.22.0 ; python_version >= "3.7" and python_version < "3.12"
-uvloop==0.18.0 ; python_version >= "3.7" and python_version < "3.12"
-vine==5.1.0 ; python_version >= "3.7" and python_version < "3.12"
-wcwidth==0.2.12 ; python_version >= "3.7" and python_version < "3.12"
-webencodings==0.5.1 ; python_version >= "3.7" and python_version < "3.12"
-webob==1.8.7 ; python_version >= "3.7" and python_version < "3.12"
-whoosh==2.7.4 ; python_version >= "3.7" and python_version < "3.12"
-wrapt==1.16.0 ; python_version >= "3.7" and python_version < "3.12"
-yacman==0.9.2 ; python_version >= "3.7" and python_version < "3.12"
-yarl==1.9.3 ; python_version >= "3.7" and python_version < "3.12"
-zipp==3.15.0 ; python_version >= "3.7" and python_version < "3.12"
-zipstream-new==1.1.8 ; python_version >= "3.7" and python_version < "3.12"
-zstandard==0.21.0 ; python_version >= "3.7" and python_version < "3.12"
+numpy==1.26.4 ; python_version >= "3.9" and python_version < "3.13"
+oauthlib==3.2.2 ; python_version >= "3.8" and python_version < "3.13"
+orjson==3.9.15 ; python_version >= "3.8" and python_version < "3.13"
+oyaml==1.0 ; python_version >= "3.8" and python_version < "3.13"
+packaging==23.2 ; python_version >= "3.8" and python_version < "3.13"
+paramiko==3.4.0 ; python_version >= "3.8" and python_version < "3.13"
+parsley==1.3 ; python_version >= "3.8" and python_version < "3.13"
+paste==3.7.1 ; python_version >= "3.8" and python_version < "3.13"
+pastedeploy==3.1.0 ; python_version >= "3.8" and python_version < "3.13"
+pebble==5.0.6 ; python_version >= "3.8" and python_version < "3.13"
+pillow==10.2.0 ; python_version >= "3.8" and python_version < "3.13"
+pkgutil-resolve-name==1.3.10 ; python_version >= "3.8" and python_version < "3.9"
+promise==2.3 ; python_version >= "3.8" and python_version < "3.13"
+prompt-toolkit==3.0.43 ; python_version >= "3.8" and python_version < "3.13"
+prov==1.5.1 ; python_version >= "3.8" and python_version < "3.13"
+psutil==5.9.8 ; python_version >= "3.8" and python_version < "3.13"
+pulsar-galaxy-lib==0.15.6 ; python_version >= "3.8" and python_version < "3.13"
+pyasn1==0.5.1 ; python_version >= "3.8" and python_version < "3.13"
+pycparser==2.21 ; python_version >= "3.8" and python_version < "3.13"
+pycryptodome==3.20.0 ; python_version >= "3.8" and python_version < "3.13"
+pydantic-core==2.14.6 ; python_version >= "3.8" and python_version < "3.13"
+pydantic-tes==0.1.5 ; python_version >= "3.8" and python_version < "3.13"
+pydantic==2.5.3 ; python_version >= "3.8" and python_version < "3.13"
+pydantic[email]==2.5.3 ; python_version >= "3.8" and python_version < "3.13"
+pydot==2.0.0 ; python_version >= "3.8" and python_version < "3.13"
+pyeventsystem==0.1.0 ; python_version >= "3.8" and python_version < "3.13"
+pyfaidx==0.8.1.1 ; python_version >= "3.8" and python_version < "3.13"
+pygments==2.17.2 ; python_version >= "3.8" and python_version < "3.13"
+pyjwt==2.8.0 ; python_version >= "3.8" and python_version < "3.13"
+pyjwt[crypto]==2.8.0 ; python_version >= "3.8" and python_version < "3.13"
+pykwalify==1.8.0 ; python_version >= "3.8" and python_version < "3.13"
+pylibmagic==0.5.0 ; python_version >= "3.8" and python_version < "3.13"
+pynacl==1.5.0 ; python_version >= "3.8" and python_version < "3.13"
+pyparsing==3.1.1 ; python_version >= "3.8" and python_version < "3.13"
+pyreadline3==3.4.1 ; sys_platform == "win32" and python_version >= "3.8" and python_version < "3.13"
+pysam==0.22.0 ; python_version >= "3.8" and python_version < "3.13"
+python-dateutil==2.9.0.post0 ; python_version >= "3.8" and python_version < "3.13"
+python-jose==3.3.0 ; python_version >= "3.8" and python_version < "3.13"
+python-magic==0.4.27 ; python_version >= "3.8" and python_version < "3.13"
+python-multipart==0.0.9 ; python_version >= "3.8" and python_version < "3.13"
+python3-openid==3.2.0 ; python_version >= "3.8" and python_version < "3.13"
+pytz==2024.1 ; python_version >= "3.8" and python_version < "3.13"
+pyyaml==6.0.1 ; python_version >= "3.8" and python_version < "3.13"
+pyzmq==25.1.2 ; python_version >= "3.8" and python_version < "3.13"
+rdflib==6.3.2 ; python_version >= "3.8" and python_version < "3.13"
+referencing==0.33.0 ; python_version >= "3.8" and python_version < "3.13"
+refgenconf==0.12.2 ; python_version >= "3.8" and python_version < "3.13"
+regex==2023.12.25 ; python_version >= "3.8" and python_version < "3.13"
+repoze-lru==0.7 ; python_version >= "3.8" and python_version < "3.13"
+requests-oauthlib==1.3.1 ; python_version >= "3.8" and python_version < "3.13"
+requests-toolbelt==1.0.0 ; python_version >= "3.8" and python_version < "3.13"
+requests-unixsocket==0.3.0 ; python_version >= "3.8" and python_version < "3.13"
+requests==2.31.0 ; python_version >= "3.8" and python_version < "3.13"
+rich==13.7.1 ; python_version >= "3.8" and python_version < "3.13"
+rocrate==0.9.0 ; python_version >= "3.8" and python_version < "3.13"
+routes==2.5.1 ; python_version >= "3.8" and python_version < "3.13"
+rpds-py==0.18.0 ; python_version >= "3.8" and python_version < "3.13"
+rsa==4.9 ; python_version >= "3.8" and python_version < "3.13"
+ruamel-yaml-clib==0.2.8 ; platform_python_implementation == "CPython" and python_version < "3.13" and python_version >= "3.8"
+ruamel-yaml==0.18.6 ; python_version >= "3.8" and python_version < "3.13"
+s3fs==2023.12.2 ; python_version >= "3.8" and python_version < "3.13"
+schema-salad==8.5.20240102191335 ; python_version >= "3.8" and python_version < "3.13"
+setuptools-scm==5.0.2 ; python_version >= "3.8" and python_version < "3.13"
+setuptools==69.1.1 ; python_version >= "3.8" and python_version < "3.13"
+shellescape==3.8.1 ; python_version >= "3.8" and python_version < "3.13"
+six==1.16.0 ; python_version >= "3.8" and python_version < "3.13"
+sniffio==1.3.1 ; python_version >= "3.8" and python_version < "3.13"
+social-auth-core[openidconnect]==4.0.3 ; python_version >= "3.8" and python_version < "3.13"
+sortedcontainers==2.4.0 ; python_version >= "3.8" and python_version < "3.13"
+spython==0.3.13 ; python_version >= "3.8" and python_version < "3.13"
+sqlalchemy==1.4.51 ; python_version >= "3.8" and python_version < "3.13"
+sqlitedict==2.1.0 ; python_version >= "3.8" and python_version < "3.13"
+sqlparse==0.4.4 ; python_version >= "3.8" and python_version < "3.13"
+starlette-context==0.3.6 ; python_version >= "3.8" and python_version < "3.13"
+starlette-graphene3==0.6.0 ; python_version >= "3.8" and python_version < "3.13"
+starlette==0.36.3 ; python_version >= "3.8" and python_version < "3.13"
+supervisor==4.2.5 ; python_version >= "3.8" and python_version < "3.13"
+svgwrite==1.4.3 ; python_version >= "3.8" and python_version < "3.13"
+tenacity==8.2.3 ; python_version >= "3.8" and python_version < "3.13"
+tifffile==2023.7.10 ; python_version >= "3.8" and python_version < "3.13"
+tinydb==4.8.0 ; python_version >= "3.8" and python_version < "3.13"
+tomli==2.0.1 ; python_version >= "3.8" and python_version < "3.11"
+tornado==6.4 ; python_version >= "3.8" and python_version < "3.13"
+tqdm==4.66.2 ; python_version >= "3.8" and python_version < "3.13"
+tuspy==1.0.3 ; python_version >= "3.8" and python_version < "3.13"
+tuswsgi==0.5.5 ; python_version >= "3.8" and python_version < "3.13"
+typing-extensions==4.10.0 ; python_version >= "3.8" and python_version < "3.13"
+tzdata==2024.1 ; python_version >= "3.8" and python_version < "3.13"
+tzlocal==5.2 ; python_version >= "3.8" and python_version < "3.13"
+ubiquerg==0.7.0 ; python_version >= "3.8" and python_version < "3.13"
+urllib3==1.26.18 ; python_version >= "3.8" and python_version < "3.13"
+uvicorn==0.27.1 ; python_version >= "3.8" and python_version < "3.13"
+uvloop==0.19.0 ; python_version >= "3.8" and python_version < "3.13"
+vine==5.1.0 ; python_version >= "3.8" and python_version < "3.13"
+wcwidth==0.2.13 ; python_version >= "3.8" and python_version < "3.13"
+webencodings==0.5.1 ; python_version >= "3.8" and python_version < "3.13"
+webob==1.8.7 ; python_version >= "3.8" and python_version < "3.13"
+whoosh==2.7.4 ; python_version >= "3.8" and python_version < "3.13"
+wrapt==1.16.0 ; python_version >= "3.8" and python_version < "3.13"
+yacman==0.9.3 ; python_version >= "3.8" and python_version < "3.13"
+yarl==1.9.4 ; python_version >= "3.8" and python_version < "3.13"
+zipp==3.17.0 ; python_version >= "3.8" and python_version < "3.13"
+zipstream-new==1.1.8 ; python_version >= "3.8" and python_version < "3.13"
+zstandard==0.22.0 ; python_version >= "3.8" and python_version < "3.13"
```

### Comparing `galaxy-app-23.2.1/galaxy/dependencies/update.sh` & `galaxy-app-24.0.0/galaxy/dependencies/update.sh`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 # This script installs poetry if it's not already installed in the user account.
 # It then runs poetry inside Galaxy's root directory, potentially updating 
 # pyproject.toml and poetry.lock, and the pinned and dev requirements files.
 
 set -e
 
-SUPPORTED_PYTHON_VERSIONS="3.7 3.8 3.9 3.10 3.11"
-NOT_SUPPORTED_NEXT_PYTHON_VERSION="3.12"
+SUPPORTED_PYTHON_VERSIONS="3.8 3.9 3.10 3.11 3.12"
+NOT_SUPPORTED_NEXT_PYTHON_VERSION="3.13"
 
 this_directory="$(cd "$(dirname "$0")" > /dev/null && pwd)"
 
 usage() {
     printf "Usage: %s: [-a] [pkg_spec...]\n" "${0##*/}" >&2
 }
 
@@ -82,13 +82,13 @@
         NEW_REQUIREMENTS="$NEW_REQUIREMENTS and python_version < \"$NOT_SUPPORTED_NEXT_PYTHON_VERSION\""
     fi
 
     sed -i.orig -e "s/^$PACKAGE_NAME==.*/$NEW_REQUIREMENTS/" "$PINNED_REQUIREMENTS_FILE" "$PINNED_DEV_REQUIREMENTS_FILE"
 }
 
 # For some packages there is no recent version that works on all Python versions
-# supported by Galaxy, so Poetry resorts to an old version that didn't have a
-# maximum Python version pin. Here we replace any such requirement with multiple
-# Python-version-specific requirements.
+# supported by Galaxy, so Poetry resorts to an old version. Here we replace any
+# such requirement with multiple Python-version-specific requirements.
+# Packages which specify a maximum Python version pin:
 split_requirement matplotlib
 split_requirement numpy
 split_requirement scipy
```

### Comparing `galaxy-app-23.2.1/galaxy/dependencies/update_lint_requirements.sh` & `galaxy-app-24.0.0/galaxy/dependencies/update_lint_requirements.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/bin/sh
 
 set -e
 
 # This script updates the pinned requirements for linting.
-# The lint requirements are split from the other ones due to incompatible
-# dependencies: flake8 requires importlib-metadata 4.2, while the Galaxy's core
-# dependencies depend on importlib-metadata 4.13.
+# The lint requirements are split from the other ones since they often have
+# incompatible dependencies.
 
 THIS_DIRECTORY="$(cd "$(dirname "$0")" > /dev/null && pwd)"
 
 update_pinned_reqs() {
     VENV=$(mktemp -d "${TMPDIR:-/tmp}/$1_venv.XXXXXXXXXX")
-    python3.7 -m venv "${VENV}"
+    python3.8 -m venv "${VENV}"
     . "${VENV}/bin/activate"
     pip install --upgrade pip setuptools
     pip install -r "${THIS_DIRECTORY}/$1-requirements.txt"
     # The grep below is needed to workaround https://github.com/pypa/pip/issues/8331
     pip freeze -l | grep -v 'pkg_resources==0.0.0' > "${THIS_DIRECTORY}/pinned-$1-requirements.txt"
     rm -rf "${VENV}"
 }
```

### Comparing `galaxy-app-23.2.1/galaxy/di.py` & `galaxy-app-24.0.0/galaxy/di.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dependency injection framework for Galaxy-type apps."""
+
 from typing import (
     Optional,
     Type,
     TypeVar,
 )
 
 from lagom import Container as LagomContainer
```

### Comparing `galaxy-app-23.2.1/galaxy/forms/forms.py` & `galaxy-app-24.0.0/galaxy/forms/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FormDefinition and field factories
 """
+
 # TODO: A FormDefinitionField is closely linked to a form_builder result.
 # Can this functionality be further abstracted and merged with form_builder?
 from galaxy.model import (
     FormDefinition,
     FormDefinitionCurrent,
 )
 from galaxy.util import string_as_bool
@@ -50,24 +51,22 @@
         Return FormDefinition created from an xml element.
         """
         name = elem.get("name", None)
         description = elem.get("description", None)
         form_type = elem.get("type", None)
         # load layout
         layout = []
-        layouts_elem = elem.find("layout")
-        if layouts_elem:
+        if layouts_elem := elem.find("layout"):
             for layout_elem in layouts_elem.findall("grid"):
                 layout_name = layout_elem.get("name", None)
                 assert layout_name and layout_name not in layout, "Layout grid element requires a unique name."
                 layout.append(layout_name)
         # load fields
         fields = []
-        fields_elem = elem.find("fields")
-        if fields_elem is not None:
+        if (fields_elem := elem.find("fields")) is not None:
             for field_elem in fields_elem.findall("field"):
                 field_type = field_elem.get("type")
                 assert field_type in self.field_type_factories, f"Invalid form field type ( {field_type} )."
                 fields.append(self.field_type_factories[field_type].from_elem(field_elem, layout))
         # create and return new form
         return self.new(
             form_type,
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/__init__.py` & `galaxy-app-24.0.0/galaxy/jobs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Support for running a tool in Galaxy via an internal job management system
 """
+
 import copy
 import datetime
 import errno
 import json
 import logging
 import os
 import pwd
@@ -62,28 +63,29 @@
 from galaxy.metadata import get_metadata_compute_strategy
 from galaxy.model import (
     Job,
     store,
     Task,
 )
 from galaxy.model.base import transaction
+from galaxy.model.store import copy_dataset_instance_metadata_attributes
 from galaxy.model.store.discover import MaxDiscoveredFilesExceededError
 from galaxy.objectstore import ObjectStorePopulator
 from galaxy.structured_app import MinimalManagerApp
 from galaxy.tool_util.deps import requirements
 from galaxy.tool_util.output_checker import (
     check_output,
     DETECTED_JOB_STATE,
 )
+from galaxy.tool_util.parser.stdio import StdioErrorLevel
 from galaxy.tools.evaluation import (
     PartialToolEvaluator,
     ToolEvaluator,
 )
 from galaxy.util import (
-    etree,
     parse_xml_string,
     RWXRWXRWX,
     safe_makedirs,
     unicodify,
 )
 from galaxy.util.bunch import Bunch
 from galaxy.util.expressions import ExpressionContext
@@ -161,16 +163,15 @@
 def job_config_xml_to_dict(config, root):
     config_dict = {}
 
     runners = {}
     config_dict["runners"] = runners
 
     # Parser plugins section populate 'runners' and 'dynamic' in config_dict.
-    plugins = root.find("plugins")
-    if plugins is not None:
+    if (plugins := root.find("plugins")) is not None:
         for plugin in ConfiguresHandlers._findall_with_required(plugins, "plugin", ("id", "type", "load")):
             if plugin.get("type") == "runner":
                 workers = plugin.get("workers", plugins.get("workers", JobConfiguration.DEFAULT_NWORKERS))
                 runner_kwds = JobConfiguration.get_params(config, plugin)
                 plugin_id = plugin.get("id")
                 runner_info = dict(id=plugin_id, load=plugin.get("load"), workers=int(workers), kwds=runner_kwds)
                 runners[plugin_id] = runner_info
@@ -239,48 +240,45 @@
     if default_destination:
         config_dict["execution"]["default"] = default_destination
 
     resources_config_dict = {}
     resource_groups = {}
 
     # Parse resources...
-    resources = root.find("resources")
-    if resources is not None:
+    if (resources := root.find("resources")) is not None:
         default_resource_group = resources.get("default", None)
         if default_resource_group:
             resources_config_dict["default"] = default_resource_group
 
         for group in ConfiguresHandlers._findall_with_required(resources, "group"):
             group_id = group.get("id")
             fields_str = group.get("fields", None) or group.text or ""
             fields = [f for f in fields_str.split(",") if f]
             resource_groups[group_id] = fields
 
     resources_config_dict["groups"] = resource_groups
     config_dict["resources"] = resources_config_dict
 
     # Parse tool mappings
-    tools = root.find("tools")
     config_dict["tools"] = []
-    if tools is not None:
+    if (tools := root.find("tools")) is not None:
         for tool in tools.findall("tool"):
             # There can be multiple definitions with identical ids, but different params
             tool_mapping_conf = {}
             for key in ["handler", "destination", "id", "resources", "class"]:
                 value = tool.get(key)
                 if value:
                     if key == "destination":
                         key = "environment"
                     tool_mapping_conf[key] = value
             tool_mapping_conf["params"] = JobConfiguration.get_params(config, tool)
             config_dict["tools"].append(tool_mapping_conf)
 
     limits_config = []
-    limits = root.find("limits")
-    if limits is not None:
+    if (limits := root.find("limits")) is not None:
         for limit in JobConfiguration._findall_with_required(limits, "limit", ("type",)):
             limit_dict = {}
             for key in ["type", "tag", "id", "window"]:
                 if key == "type" and key.startswith("destination_"):
                     key = f"environment_{key[len('destination_'):]}"
                 value = limit.get(key)
                 if value:
@@ -643,15 +641,15 @@
                 fields = []
                 for field_name in fields_names:
                     if field_name not in self.resource_parameters:
                         message = "Failed to find field for resource {} in resource parameters {}".format(
                             field_name, self.resource_parameters
                         )
                         raise KeyError(message)
-                    fields.append(etree.fromstring(self.resource_parameters[field_name]))
+                    fields.append(parse_xml_string(self.resource_parameters[field_name]))
 
                 if fields:
                     conditional_element = parse_xml_string(self.JOB_RESOURCE_CONDITIONAL_XML)
                     when_yes_elem = conditional_element.findall("when")[1]
                     for parameter in fields:
                         when_yes_elem.append(parameter)
                     return conditional_element
@@ -1233,16 +1231,15 @@
         if not os.path.exists(self.working_directory):
             os.mkdir(self.working_directory)
 
         job = self._load_job()
 
         def get_special():
             stmt = select(model.JobExportHistoryArchive).filter_by(job=job).limit(1)
-            jeha = self.sa_session.scalars(stmt).first()
-            if jeha:
+            if jeha := self.sa_session.scalars(stmt).first():
                 return jeha.fda
             stmt = select(model.GenomeIndexToolData).filter_by(job=job).limit(1)
             return self.sa_session.scalars(stmt).first()
 
         # TODO: The upload tool actions that create the paramfile can probably be turned in to a configfile to remove this special casing
         if job.tool_id == "upload1":
             self.__prepare_upload_paramfile(job)
@@ -1504,16 +1501,15 @@
             job.set_state(job.states.PAUSED)
             self.sa_session.add(job)
 
     def is_ready_for_resubmission(self, job=None):
         if job is None:
             job = self.get_job()
 
-        destination_params = job.destination_params
-        if "__resubmit_delay_seconds" in destination_params:
+        if "__resubmit_delay_seconds" in (destination_params := job.destination_params):
             delay = float(destination_params["__resubmit_delay_seconds"])
             if job.seconds_since_updated < delay:
                 return False
 
         return True
 
     def mark_as_resubmitted(self, info=None):
@@ -1941,28 +1937,38 @@
 
         if not extended_metadata:
             # importing metadata will discover outputs if extended metadata
             try:
                 self.discover_outputs(job, inp_data, out_data, out_collections, final_job_state=final_job_state)
             except MaxDiscoveredFilesExceededError as e:
                 final_job_state = job.states.ERROR
-                job.job_messages = [str(e)]
+                job.job_messages = [
+                    {
+                        "type": "internal",
+                        "desc": str(e),
+                        "error_level": StdioErrorLevel.FATAL,
+                    }
+                ]
 
             for dataset_assoc in output_dataset_associations:
-                if getattr(dataset_assoc.dataset, "discovered", False):
-                    # skip outputs that have been discovered
-                    continue
+                is_discovered_dataset = getattr(dataset_assoc.dataset, "discovered", False)
                 context = self.get_dataset_finish_context(job_context, dataset_assoc)
                 # should this also be checking library associations? - can a library item be added from a history before the job has ended? -
                 # lets not allow this to occur
                 # need to update all associated output hdas, i.e. history was shared with job running
                 for dataset in (
                     dataset_assoc.dataset.dataset.history_associations
                     + dataset_assoc.dataset.dataset.library_associations
                 ):
+                    if is_discovered_dataset:
+                        if dataset is dataset_assoc.dataset:
+                            continue
+                        elif dataset.extension == dataset_assoc.dataset.extension or dataset.extension == "auto":
+                            copy_dataset_instance_metadata_attributes(dataset_assoc.dataset, dataset)
+                            continue
                     output_name = dataset_assoc.name
 
                     # Handles retry internally on error for instance...
                     self._finish_dataset(output_name, dataset, job, context, final_job_state, remote_metadata_directory)
                 if (
                     not final_job_state == job.states.ERROR
                     and not dataset_assoc.dataset.dataset.state == job.states.ERROR
@@ -1980,15 +1986,16 @@
                 for dep_job_assoc in dataset_assoc.dataset.dependent_jobs:
                     self.pause(
                         dep_job_assoc.job,
                         "Execution of this dataset's job is paused because its input datasets are in an error state.",
                     )
 
         for pja in job.post_job_actions:
-            ActionBox.execute(self.app, self.sa_session, pja.post_job_action, job, final_job_state=final_job_state)
+            if pja.post_job_action.action_type not in ActionBox.immediate_actions:
+                ActionBox.execute(self.app, self.sa_session, pja.post_job_action, job, final_job_state=final_job_state)
 
         # The exit code will be null if there is no exit code to be set.
         # This is so that we don't assign an exit code, such as 0, that
         # is either incorrect or has the wrong semantics.
         if tool_exit_code is not None:
             job.exit_code = tool_exit_code
         # custom post process setup
@@ -2090,20 +2097,16 @@
             inp_data=inp_data,
             input_ext=input_ext,
             input_dbkey=input_dbkey,
             final_job_state=final_job_state,
         )
 
     def check_tool_output(self, tool_stdout, tool_stderr, tool_exit_code, job, job_stdout=None, job_stderr=None):
-        job_id_tag = "<unknown job id>"
-        if job is not None:
-            job_id_tag = job.get_id_tag()
-
         state, tool_stdout, tool_stderr, job_messages = check_output(
-            self.tool.stdio_regexes, self.tool.stdio_exit_codes, tool_stdout, tool_stderr, tool_exit_code, job_id_tag
+            self.tool.stdio_regexes, self.tool.stdio_exit_codes, tool_stdout, tool_stderr, tool_exit_code
         )
 
         # Store the modified stdout and stderr in the job:
         if job is not None:
             job.set_streams(
                 tool_stdout, tool_stderr, job_messages=job_messages, job_stdout=job_stdout, job_stderr=job_stderr
             )
@@ -2404,16 +2407,15 @@
             _monitor_py = shlex.quote(os.path.join(exec_dir, "lib/galaxy_ext/container_monitor/monitor.py"))
             monitor_command = f"python {_monitor_py}"
         return f"({monitor_command} &); sleep 1 "
 
     @property
     def user(self):
         job = self.get_job()
-        user_email = job.get_user_email()
-        if user_email:
+        if user_email := job.get_user_email():
             return user_email
         elif job.galaxy_session is not None:
             return f"anonymous@{job.galaxy_session.remote_addr.split()[-1]}"
         else:
             return "anonymous@unknown"
 
     def __update_output(self, job, hda, clean_only=False):
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/command_factory.py` & `galaxy-app-24.0.0/galaxy/jobs/command_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,15 @@
 
         # Copy working and outputs before job submission so that these can be restored on resubmission
         # xref https://github.com/galaxyproject/galaxy/issues/3289
         commands_builder.prepend_command(PREPARE_DIRS)
 
     __handle_remote_command_line_building(commands_builder, job_wrapper, for_pulsar=for_pulsar)
 
-    container_monitor_command = job_wrapper.container_monitor_command(container)
-    if container_monitor_command:
+    if container_monitor_command := job_wrapper.container_monitor_command(container):
         commands_builder.prepend_command(container_monitor_command)
 
     working_directory = remote_job_directory or job_wrapper.working_directory
     commands_builder.capture_return_code(default_exit_code_file(working_directory, job_wrapper.job_id))
 
     if job_wrapper.is_cwl_job:
         # Minimal metadata needed by the relocate script
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/dynamic_tool_destination.py` & `galaxy-app-24.0.0/galaxy/jobs/dynamic_tool_destination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1643,22 +1643,22 @@
             log.debug(message)
 
     if job_config_location:
         job_conf = parse_xml(job_config_location, strip_whitespace=False)
 
         # Add all destination IDs from the job configuration xml file
         for destination in job_conf.getroot().iter("destination"):
-            if isinstance(destination.get("id"), str):
-                destination_list.add(destination.get("id"))
-
+            destination_id = destination.get("id")
+            if destination_id:
+                destination_list.add(destination_id)
             else:
                 error = f"Destination ID '{str(destination)}"
                 error += "' in job configuration file cannot be"
                 error += " parsed. Things may not work as expected!"
-                log.debug(error)
+                log.warning(error)
 
     return destination_list
 
 
 def get_edit_distance(source, target):
     """
     returns the edit distance (levenshtein distance) between two strings.
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/handler.py` & `galaxy-app-24.0.0/galaxy/jobs/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Galaxy job handler, prepares, runs, tracks, and finishes Galaxy jobs
 """
+
 import datetime
 import os
 import time
 from collections import defaultdict
 from queue import (
     Empty,
     Queue,
@@ -881,15 +882,15 @@
                     and_(
                         model.Job.table.c.state.in_((model.Job.states.QUEUED, model.Job.states.RUNNING)),
                         (model.Job.table.c.user_id == user_id),
                     )
                 )
                 .group_by(model.Job.table.c.destination_id)
             )
-            for row in result:
+            for row in result.mappings():
                 # Add the count from the database to the cached count
                 rval[row["destination_id"]] = rval.get(row["destination_id"], 0) + row["job_count"]
         return rval
 
     def __cache_user_job_count_per_destination(self):
         # Cache the job count if necessary
         if self.user_job_count_per_destination is None and self.app.config.cache_user_job_count:
@@ -899,15 +900,15 @@
                     model.Job.table.c.user_id,
                     model.Job.table.c.destination_id,
                     func.count(model.Job.table.c.user_id).label("job_count"),
                 )
                 .where(and_(model.Job.table.c.state.in_((model.Job.states.QUEUED, model.Job.states.RUNNING))))
                 .group_by(model.Job.table.c.user_id, model.Job.table.c.destination_id)
             )
-            for row in result:
+            for row in result.mappings():
                 if row["user_id"] not in self.user_job_count_per_destination:
                     self.user_job_count_per_destination[row["user_id"]] = {}
                 self.user_job_count_per_destination[row["user_id"]][row["destination_id"]] = row["job_count"]
         elif self.user_job_count_per_destination is None:
             self.user_job_count_per_destination = {}
 
     def increase_running_job_count(self, user_id, destination_id):
@@ -1252,16 +1253,15 @@
         # The runner name is not set until the job has started.
         # If we're stopping a task, then the runner_name may be
         # None, in which case it hasn't been scheduled.
         if self.app.config.enable_celery_tasks and job.tool_id == "__DATA_FETCH__":
             from galaxy.celery import celery_app
 
             celery_app.control.revoke(job.job_runner_external_id)
-        job_runner_name = job.get_job_runner_name()
-        if job_runner_name is not None:
+        if (job_runner_name := job.get_job_runner_name()) is not None:
             runner_name = job_runner_name.split(":", 1)[0]
             log.debug(f"Stopping job {job_wrapper.get_id_tag()} in {runner_name} runner")
             try:
                 self.job_runners[runner_name].stop_job(job_wrapper)
             except KeyError:
                 log.error(f"stop(): ({job_wrapper.get_id_tag()}) Invalid job runner: {runner_name}")
                 # Job and output dataset states have already been updated, so nothing is done here.
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/manager.py` & `galaxy-app-24.0.0/galaxy/jobs/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Top-level Galaxy job manager, moves jobs to handler(s)
 """
+
 import logging
 from functools import partial
 
 from galaxy.exceptions import (
     HandlerAssignmentError,
     ToolExecutionError,
 )
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/mapper.py` & `galaxy-app-24.0.0/galaxy/jobs/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,15 @@
         Returns the function that matches the rule. If a rules_module override
         is specified, search within that rules_module, or default to the plugin's
         top level rules_module.
         """
         rules_module_name = destination.params.get("rules_module")
         rule_modules = self.__get_rule_modules_or_defaults(rules_module_name)
         expand_function = None
-        expand_function_name = destination.params.get("function")
-        if expand_function_name:
+        if expand_function_name := destination.params.get("function"):
             expand_function = self.__last_matching_function_in_modules(rule_modules, expand_function_name)
             if not expand_function:
                 message = ERROR_MESSAGE_RULE_FUNCTION_NOT_FOUND % expand_function_name
                 raise JobMappingConfigurationException(message)
         else:
             expand_function = self.__find_function_by_tool_id(rule_modules)
             if not expand_function:
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/rule_helper.py` & `galaxy-app-24.0.0/galaxy/jobs/rule_helper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/__init__.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Base classes for job runner plugins.
 """
+
 import datetime
 import os
 import string
 import subprocess
 import sys
 import threading
 import time
@@ -30,15 +31,18 @@
 from galaxy.jobs.runners.util import runner_states
 from galaxy.jobs.runners.util.env import env_to_statement
 from galaxy.jobs.runners.util.job_script import (
     DescribesScriptIntegrityChecks,
     job_script,
     write_script,
 )
-from galaxy.model.base import transaction
+from galaxy.model.base import (
+    check_database_connection,
+    transaction,
+)
 from galaxy.tool_util.deps.dependencies import (
     JobInfo,
     ToolInfo,
 )
 from galaxy.tool_util.output_checker import DETECTED_JOB_STATE
 from galaxy.util import (
     asbool,
@@ -195,17 +199,18 @@
     def put(self, job_wrapper: "MinimalJobWrapper"):
         """Add a job to the queue (by job identifier), indicate that the job is ready to run."""
         put_timer = ExecutionTimer()
         try:
             queue_job = job_wrapper.enqueue()
         except Exception as e:
             queue_job = False
-            # Required for exceptions thrown by object store incompatiblity.
+            # Required for exceptions thrown by object store incompatibility.
             # tested by test/integration/objectstore/test_private_handling.py
-            job_wrapper.fail(str(e), exception=e)
+            message = e.client_message if hasattr(e, "client_message") else str(e)
+            job_wrapper.fail(message, exception=e)
             log.debug(f"Job [{job_wrapper.job_id}] failed to queue {put_timer}")
             return
         if queue_job:
             self.mark_as_queued(job_wrapper)
             log.debug(f"Job [{job_wrapper.job_id}] queued {put_timer}")
 
     def mark_as_queued(self, job_wrapper: "MinimalJobWrapper"):
@@ -214,16 +219,15 @@
     def shutdown(self):
         """Attempts to gracefully shut down the worker threads"""
         log.info("%s: Sending stop signal to %s job worker threads", self.runner_name, len(self.work_threads))
         self._should_stop = True
         for _ in range(len(self.work_threads)):
             self.work_queue.put((STOP_SIGNAL, None))
 
-        join_timeout = self.app.config.monitor_thread_join_timeout
-        if join_timeout > 0:
+        if (join_timeout := self.app.config.monitor_thread_join_timeout) > 0:
             log.info("Waiting up to %d seconds for job worker threads to shutdown...", join_timeout)
             start = time.time()
             # NOTE: threads that have already joined by now are not going to be logged
             for thread in self._alive_worker_threads(cycle=True):
                 if time.time() > (start + join_timeout):
                     break
                 try:
@@ -831,14 +835,15 @@
             # Ideally we'd construct a sqlalchemy session now and pass it into `check_watched_items`
             # and have that be the only session being used. The next best thing is to scope
             # the session and discard it after each check_watched_item loop
             scoped_id = str(uuid.uuid4())
             self.app.model.set_request_id(scoped_id)
             # Iterate over the list of watched jobs and check state
             try:
+                check_database_connection(self.sa_session)
                 self.check_watched_items()
             except Exception:
                 log.exception("Unhandled exception checking active jobs")
             finally:
                 self.app.model.unset_request_id(scoped_id)
             # Sleep a bit before the next state check
             time.sleep(self.app.config.job_runner_monitor_sleep)
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/aws.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Galaxy job runners to use Amazon AWS native compute resources, such as AWS Batch.
 """
+
 import bisect
 import hashlib
 import json
 import logging
 import os
 import re
 import time
@@ -74,16 +75,15 @@
 
 
 def _add_resource_requirements(destination_params):
     rval = [
         {"type": "VCPU", "value": str(destination_params.get("vcpu"))},
         {"type": "MEMORY", "value": str(destination_params.get("memory"))},
     ]
-    n_gpu = destination_params.get("gpu")
-    if n_gpu:
+    if n_gpu := destination_params.get("gpu"):
         rval.append({"type": "GPU", "value": str(n_gpu)})
     return rval
 
 
 class AWSBatchJobRunner(AsynchronousJobRunner):
     """
     This runner uses container only. It requires that an AWS EFS is mounted as a local drive
@@ -275,16 +275,15 @@
                 "readOnly": False,
                 "sourceVolume": "efs_whole",
             },
         )
         if destination_params.get("platform") == 'Fargate':   # Fargate doesn't support host volumes
             return volumes, mount_points
 
-        ec2_host_volumes = destination_params.get("ec2_host_volumes")
-        if ec2_host_volumes:
+        if (ec2_host_volumes := destination_params.get("ec2_host_volumes")):
             for ix, vol in enumerate(ec2_host_volumes.split(",")):
                 vol = vol.strip()
                 vol_name = "host_vol_" + str(ix)
                 volumes.append(
                     {
                         "name": vol_name,
                         "host": {"sourcePath": vol},
@@ -352,16 +351,15 @@
                 {
                     "networkConfiguration": {"assignPublicIp": "ENABLED"},
                     "fargatePlatformConfiguration": {"platformVersion": destination_params.get("fargate_version")},
                     "logConfiguration": {"logDriver": "awslogs"},
                 }
             )
         other_kwargs = {}
-        retry_strategy = self._get_retry_strategy(destination_params)
-        if retry_strategy:
+        if (retry_strategy := self._get_retry_strategy(destination_params)):
             other_kwargs["retryStrategy"] = retry_strategy
 
         res = self._batch_client.register_job_definition(
             jobDefinitionName=jd_name,
             type="container",
             platformCapabilities=[platform],
             containerProperties=containerProperties,
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/chronos.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/chronos.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,17 +197,16 @@
             ajs.old_state = model.Job.states.QUEUED
             ajs.running = False
             self.monitor_queue.put(ajs)
 
     @handle_exception_call
     def check_watched_item(self, job_state):
         job_name = job_state.job_id
-        job = self._retrieve_job(job_name)
         # TODO: how can stopped GxIT jobs be handled here?
-        if job:
+        if job := self._retrieve_job(job_name):
             succeeded = job["successCount"]
             errors = job["errorCount"]
             if succeeded > 0:
                 return self._mark_as_successful(job_state)
             elif not succeeded and not errors:
                 return self._mark_as_active(job_state)
             elif errors:
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/cli.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/cli.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/condor.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/condor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 and checking the status of jobs please check out the CLI runner (cli.py in this directory)
 start by writing a new job plugin in for that (see examples in
 /galaxy/jobs/runners/util/cli/job). That approach will result in less boilerplate and allow
 greater reuse of the DRM specific hooks you'll need to write. Ideally this plugin would
 have been written to target that framework, but we don't have the bandwidth to rewrite
 it at this time.
 """
+
 import logging
 import os
 import subprocess
 
 from galaxy import model
 from galaxy.jobs.runners import (
     AsynchronousJobRunner,
@@ -72,16 +73,15 @@
         universe = query_params.get("universe", None)
         if universe and universe.strip().lower() == "docker":
             container = self._find_container(job_wrapper)
             if container:
                 # HTCondor needs the image as 'docker_image'
                 query_params.update({"docker_image": container.container_id})
 
-        galaxy_slots = query_params.get("request_cpus", None)
-        if galaxy_slots:
+        if galaxy_slots := query_params.get("request_cpus", None):
             galaxy_slots_statement = f'GALAXY_SLOTS="{galaxy_slots}"; export GALAXY_SLOTS; GALAXY_SLOTS_CONFIGURED="1"; export GALAXY_SLOTS_CONFIGURED;'
         else:
             galaxy_slots_statement = 'GALAXY_SLOTS="1"; export GALAXY_SLOTS;'
 
         # define job attributes
         cjs = CondorJobState(files_dir=job_wrapper.working_directory, job_wrapper=job_wrapper)
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/drmaa.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/drmaa.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,16 +101,15 @@
 
         self.redact_email_in_job_name = self.app.config.redact_email_in_job_name
 
     def url_to_destination(self, url):
         """Convert a legacy URL to a job destination"""
         if not url:
             return
-        native_spec = url.split("/")[2]
-        if native_spec:
+        if native_spec := url.split("/")[2]:
             params = dict(nativeSpecification=native_spec)
             log.debug(f"Converted URL '{url}' to destination runner=drmaa, params={params}")
             return JobDestination(runner="drmaa", params=params)
         else:
             log.debug(f"Converted URL '{url}' to destination runner=drmaa")
             return JobDestination(runner="drmaa")
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/godocker.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/godocker.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/kubernetes.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/kubernetes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Offload jobs to a Kubernetes cluster.
 """
 
+import json  # for debugging of API objects
 import logging
 import math
 import os
 import re
+import time
 from datetime import datetime
 
 import yaml
 
 from galaxy import model
 from galaxy.jobs.runners import (
     AsynchronousJobRunner,
@@ -39,14 +41,15 @@
     Pod,
     produce_k8s_job_prefix,
     pull_policy,
     pykube_client_from_dict,
     Service,
     service_object_dict,
 )
+from galaxy.util import unicodify
 from galaxy.util.bytesize import ByteSize
 
 log = logging.getLogger(__name__)
 
 __all__ = ("KubernetesJobRunner",)
 
 
@@ -91,19 +94,25 @@
             k8s_run_as_group_id=dict(
                 map=str, valid=lambda s: s == "$gid" or isinstance(s, int) or not s or s.isdigit(), default=None
             ),
             k8s_fs_group_id=dict(
                 map=str, valid=lambda s: s == "$gid" or isinstance(s, int) or not s or s.isdigit(), default=None
             ),
             k8s_cleanup_job=dict(map=str, valid=lambda s: s in {"onsuccess", "always", "never"}, default="always"),
-            k8s_pod_retries=dict(map=int, valid=lambda x: int(x) >= 0, default=3),
+            k8s_pod_retries=dict(
+                map=int, valid=lambda x: int(x) >= 0, default=1
+            ),  # note that if the backOffLimit is lower, this paramer will have no effect.
+            k8s_job_spec_back_off_limit=dict(
+                map=int, valid=lambda x: int(x) >= 0, default=0
+            ),  # this means that it will stop retrying after 1 failure.
             k8s_walltime_limit=dict(map=int, valid=lambda x: int(x) >= 0, default=172800),
             k8s_unschedulable_walltime_limit=dict(map=int, valid=lambda x: not x or int(x) >= 0, default=None),
             k8s_interactivetools_use_ssl=dict(map=bool, default=False),
             k8s_interactivetools_ingress_annotations=dict(map=str),
+            k8s_interactivetools_ingress_class=dict(map=str, default=None),
         )
 
         if "runner_param_specs" not in kwargs:
             kwargs["runner_param_specs"] = dict()
         kwargs["runner_param_specs"].update(runner_param_specs)
 
         # Start the job runner parent object
@@ -209,15 +218,19 @@
         # define job attributes in the AsyncronousJobState for follow-up
         ajs.job_id = job_id
         # store runner information for tracking if Galaxy restarts
         job_wrapper.set_external_id(job_id)
         self.monitor_queue.put(ajs)
 
     def __has_guest_ports(self, job_wrapper):
-        return bool(job_wrapper.guest_ports)
+        # Check if job has guest ports or interactive tool entry points that would signal that
+        log.debug(
+            f"Checking if job {job_wrapper.get_id_tag()} is an interactive tool. guest ports: {job_wrapper.guest_ports}. interactive entry points: {job_wrapper.get_job().interactivetool_entry_points}"
+        )
+        return bool(job_wrapper.guest_ports) or bool(job_wrapper.get_job().interactivetool_entry_points)
 
     def __configure_port_routing(self, ajs):
         # Configure interactive tool entry points first
         guest_ports = ajs.job_wrapper.guest_ports
         ports_dict = {}
         for guest_port in guest_ports:
             ports_dict[str(guest_port)] = dict(host="manual", port=guest_port, protocol="https")
@@ -226,14 +239,17 @@
         # Configure additional k8s service and ingress for tools with guest ports
         k8s_job_prefix = self.__produce_k8s_job_prefix()
         k8s_job_name = self.__get_k8s_job_name(k8s_job_prefix, ajs.job_wrapper)
         log.debug(f"Configuring entry points and deploying service/ingress for job with ID {ajs.job_id}")
         k8s_service_obj = service_object_dict(self.runner_params, k8s_job_name, self.__get_k8s_service_spec(ajs))
 
         k8s_ingress_obj = ingress_object_dict(self.runner_params, k8s_job_name, self.__get_k8s_ingress_spec(ajs))
+        log.debug(f"Kubernetes service object: {json.dumps(k8s_service_obj, indent=4)}")
+        log.debug(f"Kubernetes ingress object: {json.dumps(k8s_ingress_obj, indent=4)}")
+        # We avoid creating service and ingress if they already exist (e.g. when Galaxy is restarted or resubmitting a job)
         service = Service(self._pykube_api, k8s_service_obj)
         service.create()
         ingress = Ingress(self._pykube_api, k8s_ingress_obj)
         ingress.create()
 
     def __get_overridable_params(self, job_wrapper, param_key):
         dest_params = self.__get_destination_params(job_wrapper)
@@ -315,14 +331,15 @@
         k8s_job_spec = {
             "template": self.__get_k8s_job_spec_template(ajs),
             "activeDeadlineSeconds": int(self.runner_params["k8s_walltime_limit"]),
         }
         job_ttl = self.runner_params["k8s_job_ttl_secs_after_finished"]
         if self.runner_params["k8s_cleanup_job"] != "never" and job_ttl is not None:
             k8s_job_spec["ttlSecondsAfterFinished"] = job_ttl
+        k8s_job_spec["backoffLimit"] = self.runner_params["k8s_job_spec_back_off_limit"]
         return k8s_job_spec
 
     def __force_label_conformity(self, value):
         """
         Make sure that a label conforms to k8s requirements.
         A valid label must be an empty string or consist of alphanumeric characters, '-', '_' or '.',
         and must start and end with an alphanumeric character (e.g. 'MyValue',  or 'my_value',  or '12345',
@@ -453,29 +470,34 @@
                 "rules": [
                     {
                         "host": ep["domain"],
                         "http": {
                             "paths": [
                                 {
                                     "backend": {
-                                        "serviceName": self.__get_k8s_job_name(
-                                            self.__produce_k8s_job_prefix(), ajs.job_wrapper
-                                        ),
-                                        "servicePort": int(ep["tool_port"]),
+                                        "service": {
+                                            "name": self.__get_k8s_job_name(
+                                                self.__produce_k8s_job_prefix(), ajs.job_wrapper
+                                            ),
+                                            "port": {"number": int(ep["tool_port"])},
+                                        }
                                     },
                                     "path": ep.get("entry_path", "/"),
                                     "pathType": "Prefix",
                                 }
                             ]
                         },
                     }
                     for ep in entry_points
-                ]
+                ],
             },
         }
+        default_ingress_class = self.runner_params.get("k8s_interactivetools_ingress_class")
+        if default_ingress_class:
+            k8s_spec_template["spec"]["ingressClassName"] = default_ingress_class
         if self.runner_params.get("k8s_interactivetools_use_ssl"):
             domains = list({e["domain"] for e in entry_points})
             k8s_spec_template["spec"]["tls"] = [
                 {"hosts": [domain], "secretName": re.sub("[^a-z0-9-]", "-", domain)} for domain in domains
             ]
         if self.runner_params.get("k8s_interactivetools_ingress_annotations"):
             new_ann = yaml.safe_load(self.runner_params.get("k8s_interactivetools_ingress_annotations"))
@@ -518,21 +540,21 @@
         k8s_container = {
             "name": self.__get_k8s_container_name(ajs.job_wrapper),
             "image": container.container_id,
             # this form of command overrides the entrypoint and allows multi command
             # command line execution, separated by ;, which is what Galaxy does
             # to assemble the command.
             "command": [ajs.job_wrapper.shell],
-            "args": ["-c", ajs.job_file],
+            # Make sure that the exit code is propagated to k8s, so k8s knows why the tool failed (e.g. OOM)
+            "args": ["-c", f"{ajs.job_file}; exit $(cat {ajs.exit_code_file})"],
             "workingDir": ajs.job_wrapper.working_directory,
             "volumeMounts": deduplicate_entries(mounts),
         }
 
-        resources = self.__get_resources(ajs.job_wrapper)
-        if resources:
+        if resources := self.__get_resources(ajs.job_wrapper):
             envs = []
             cpu_val = None
             if "requests" in resources:
                 requests = resources["requests"]
                 if "cpu" in requests:
                     cpu_val = int(math.ceil(float(requests["cpu"])))
                     envs.append({"name": "GALAXY_SLOTS", "value": str(cpu_val)})
@@ -581,31 +603,25 @@
 
         if self._default_pull_policy:
             k8s_container["imagePullPolicy"] = self._default_pull_policy
 
         return [k8s_container]
 
     def __get_resources(self, job_wrapper):
-        mem_request = self.__get_memory_request(job_wrapper)
-        cpu_request = self.__get_cpu_request(job_wrapper)
-
-        mem_limit = self.__get_memory_limit(job_wrapper)
-        cpu_limit = self.__get_cpu_limit(job_wrapper)
-
         requests = {}
         limits = {}
 
-        if mem_request:
+        if mem_request := self.__get_memory_request(job_wrapper):
             requests["memory"] = mem_request
-        if cpu_request:
+        if cpu_request := self.__get_cpu_request(job_wrapper):
             requests["cpu"] = cpu_request
 
-        if mem_limit:
+        if mem_limit := self.__get_memory_limit(job_wrapper):
             limits["memory"] = mem_limit
-        if cpu_limit:
+        if cpu_limit := self.__get_cpu_limit(job_wrapper):
             limits["cpu"] = cpu_limit
 
         resources = {}
         if requests:
             resources["requests"] = requests
         if limits:
             resources["limits"] = limits
@@ -707,14 +723,18 @@
             if "max_pod_retries" in job_destination.params:
                 max_pod_retries = int(job_destination.params["max_pod_retries"])
             elif "k8s_pod_retries" in self.runner_params:
                 max_pod_retries = int(self.runner_params["k8s_pod_retries"])
             else:
                 max_pod_retries = 1
 
+            # make sure that we don't have any conditions by which the runner
+            # would wait forever for a pod that never gets sent.
+            max_pod_retries = min(max_pod_retries, self.runner_params["k8s_job_spec_back_off_limit"])
+
             # Check if job.obj['status'] is empty,
             # return job_state unchanged if this is the case
             # as probably this means that the k8s API server hasn't
             # had time to fill in the object status since the
             # job was created only too recently.
             if len(job.obj["status"]) == 0:
                 return job_state
@@ -727,50 +747,74 @@
 
             job_persisted_state = job_state.job_wrapper.get_state()
 
             # This assumes jobs dependent on a single pod, single container
             if succeeded > 0 or job_state == model.Job.states.STOPPED:
                 job_state.running = False
                 self.mark_as_finished(job_state)
+                log.debug(f"Job id: {job_state.job_id} with k8s id: {job.name} succeeded")
                 return None
-            elif active > 0 and failed <= max_pod_retries:
+            elif active > 0 and failed < max_pod_retries + 1:
                 if not job_state.running:
                     if self.__job_pending_due_to_unschedulable_pod(job_state):
+                        log.debug(f"Job id: {job_state.job_id} with k8s id: {job.name}  pending...")
                         if self.runner_params.get("k8s_unschedulable_walltime_limit"):
                             creation_time_str = job.obj["metadata"].get("creationTimestamp")
                             creation_time = datetime.strptime(creation_time_str, "%Y-%m-%dT%H:%M:%SZ")
                             elapsed_seconds = (datetime.utcnow() - creation_time).total_seconds()
                             if elapsed_seconds > self.runner_params["k8s_unschedulable_walltime_limit"]:
                                 return self._handle_unschedulable_job(job, job_state)
                             else:
                                 pass
                         else:
                             pass
                     else:
+                        log.debug("Job set to running...")
                         job_state.running = True
                         job_state.job_wrapper.change_state(model.Job.states.RUNNING)
                 return job_state
             elif job_persisted_state == model.Job.states.DELETED:
                 # Job has been deleted via stop_job and job has not been deleted,
                 # remove from watched_jobs by returning `None`
+                log.debug(f"Job id: {job_state.job_id} has been already deleted...")
                 if job_state.job_wrapper.cleanup_job in ("always", "onsuccess"):
                     job_state.job_wrapper.cleanup()
                 return None
             else:
-                return self._handle_job_failure(job, job_state)
+                log.debug(
+                    f"Job id: {job_state.job_id} failed and it is not a deletion case. Current state: {job_state.job_wrapper.get_state()}"
+                )
+                if self._handle_job_failure(job, job_state):
+                    # changes for resubmission (removed self.mark_as_failed from handle_job_failure)
+                    self.work_queue.put((self.mark_as_failed, job_state))
+                else:
+                    # Job failure was not due to a k8s issue or something that k8s can handle, so it's a tool error.
+                    job_state.running = False
+                    self.mark_as_finished(job_state)
+                    return None
+
+                return None
 
         elif len(jobs.response["items"]) == 0:
             if job_state.job_wrapper.get_job().state == model.Job.states.DELETED:
-                # Job has been deleted via stop_job and job has been deleted,
-                # cleanup and remove from watched_jobs by returning `None`
                 if job_state.job_wrapper.cleanup_job in ("always", "onsuccess"):
                     job_state.job_wrapper.cleanup()
                 return None
+            if job_state.job_wrapper.get_job().state == model.Job.states.STOPPED and self.__has_guest_ports(
+                job_state.job_wrapper
+            ):
+                # Interactive job has been stopped via stop_job (most likely by the user),
+                # cleanup and remove from watched_jobs by returning `None`. STOPPED jobs are cleaned up elsewhere.
+                # Marking as finished makes sure that the interactive job output is available in the UI.
+                self.mark_as_finished(job_state)
+                return None
             # there is no job responding to this job_id, it is either lost or something happened.
-            log.error("No Jobs are available under expected selector app=%s", job_state.job_id)
+            log.error(
+                f"No Jobs are available under expected selector app={job_state.job_id} and they are not deleted or stopped either."
+            )
             self.mark_as_failed(job_state)
             # job is no longer viable - remove from watched jobs
             return None
         else:
             # there is more than one job associated to the expected unique job id used as selector.
             log.error("More than one Kubernetes Job associated to job id '%s'", job_state.job_id)
             self.mark_as_failed(job_state)
@@ -789,45 +833,60 @@
             self.__cleanup_k8s_job(job)
         except Exception:
             log.exception("Could not clean up k8s batch job. Ignoring...")
         return None
 
     def _handle_job_failure(self, job, job_state):
         # Figure out why job has failed
+        mark_failed = True
         with open(job_state.error_file, "a") as error_file:
+            log.debug("Trying with error file in _handle_job_failure")
             if self.__job_failed_due_to_low_memory(job_state):
+                log.debug(f"OOM detected for job: {job_state.job_id}")
                 error_file.write("Job killed after running out of memory. Try with more memory.\n")
                 job_state.fail_message = "Tool failed due to insufficient memory. Try with more memory."
                 job_state.runner_state = JobState.runner_states.MEMORY_LIMIT_REACHED
             elif self.__job_failed_due_to_walltime_limit(job):
+                log.debug(f"Walltime limit reached for job: {job_state.job_id}")
                 error_file.write("DeadlineExceeded")
                 job_state.fail_message = "Job was active longer than specified deadline"
                 job_state.runner_state = JobState.runner_states.WALLTIME_REACHED
+            elif self.__job_failed_due_to_unknown_exit_code(job_state):
+                msg = f"Job: {job_state.job_id} failed due to an unknown exit code from the tool."
+                log.debug(msg)
+                job_state.fail_message = msg
+                job_state.runner_state = JobState.runner_states.TOOL_DETECT_ERROR
+                mark_failed = False
             else:
-                error_file.write("Exceeded max number of Kubernetes pod retries allowed for job\n")
-                job_state.fail_message = "More pods failed than allowed. See stdout for pods details."
-        job_state.running = False
-        self.mark_as_failed(job_state)
+                msg = f"An unknown error occurred in this job and the maximum number of retries have been exceeded for job: {job_state.job_id}."
+                log.debug(msg)
+                error_file.write(msg)
+                job_state.fail_message = (
+                    "An unknown error occurered with this job. See standard output within the info section for details."
+                )
+        # changes for resubmission
+        # job_state.running = False
+        # self.mark_as_failed(job_state)
         try:
             if self.__has_guest_ports(job_state.job_wrapper):
                 self.__cleanup_k8s_guest_ports(job_state.job_wrapper, job)
             self.__cleanup_k8s_job(job)
         except Exception:
             log.exception("Could not clean up k8s batch job. Ignoring...")
-        return None
+        return mark_failed
 
     def __cleanup_k8s_job(self, job):
         k8s_cleanup_job = self.runner_params["k8s_cleanup_job"]
         delete_job(job, k8s_cleanup_job)
 
-    def __cleanup_k8s_ingress(self, ingress, job_failed):
+    def __cleanup_k8s_ingress(self, ingress, job_failed=False):
         k8s_cleanup_job = self.runner_params["k8s_cleanup_job"]
         delete_ingress(ingress, k8s_cleanup_job, job_failed)
 
-    def __cleanup_k8s_service(self, service, job_failed):
+    def __cleanup_k8s_service(self, service, job_failed=False):
         k8s_cleanup_job = self.runner_params["k8s_cleanup_job"]
         delete_service(service, k8s_cleanup_job, job_failed)
 
     def __job_failed_due_to_walltime_limit(self, job):
         conditions = job.obj["status"].get("conditions") or []
         return any(True for c in conditions if c["type"] == "Failed" and c["reason"] == "DeadlineExceeded")
 
@@ -847,19 +906,20 @@
         for being out of memory (pod status OOMKilled). If that is the case
         marks the job for resubmission (resubmit logic is part of destinations).
         """
         pods = find_pod_object_by_name(self._pykube_api, job_state.job_id, self.runner_params["k8s_namespace"])
         if not pods.response["items"]:
             return False
 
-        pod = self._get_pod_for_job(job_state)
+        # pod = self._get_pod_for_job(job_state) # this was always None
+        pod = pods.response["items"][0]
         if (
             pod
-            and pod.obj["status"]["phase"] == "Failed"
-            and pod.obj["status"]["containerStatuses"][0]["state"]["terminated"]["reason"] == "OOMKilled"
+            and "terminated" in pod["status"]["containerStatuses"][0]["state"]
+            and pod["status"]["containerStatuses"][0]["state"]["terminated"]["reason"] == "OOMKilled"
         ):
             return True
 
         return False
 
     def __job_pending_due_to_unschedulable_pod(self, job_state):
         """
@@ -868,44 +928,79 @@
         pods = find_pod_object_by_name(self._pykube_api, job_state.job_id, self.runner_params["k8s_namespace"])
         if not pods.response["items"]:
             return False
 
         pod = Pod(self._pykube_api, pods.response["items"][0])
         return is_pod_unschedulable(self._pykube_api, pod, self.runner_params["k8s_namespace"])
 
+    def __job_failed_due_to_unknown_exit_code(self, job_state):
+        """
+        checks whether the pod exited prematurely due to an unknown exit code (i.e. not an exit code like OOM that
+        we can handle). This would mean that the tool failed, but the job should be considered to have succeeded.
+        """
+        pods = find_pod_object_by_name(self._pykube_api, job_state.job_id, self.runner_params["k8s_namespace"])
+        if not pods.response["items"]:
+            return False
+
+        pod = pods.response["items"][0]
+        if (
+            pod
+            and "terminated" in pod["status"]["containerStatuses"][0]["state"]
+            and pod["status"]["containerStatuses"][0]["state"]["terminated"].get("exitCode")
+        ):
+            return True
+
+        return False
+
     def __cleanup_k8s_guest_ports(self, job_wrapper, k8s_job):
         k8s_job_prefix = self.__produce_k8s_job_prefix()
         k8s_job_name = f"{k8s_job_prefix}-{self.__force_label_conformity(job_wrapper.get_id_tag())}"
         log.debug(f"Deleting service/ingress for job with ID {job_wrapper.get_id_tag()}")
-        job_failed = k8s_job.obj["status"]["failed"] > 0 if "failed" in k8s_job.obj["status"] else False
         ingress_to_delete = find_ingress_object_by_name(
             self._pykube_api, k8s_job_name, self.runner_params["k8s_namespace"]
         )
         if ingress_to_delete and len(ingress_to_delete.response["items"]) > 0:
             k8s_ingress = Ingress(self._pykube_api, ingress_to_delete.response["items"][0])
-            self.__cleanup_k8s_ingress(k8s_ingress, job_failed)
+            self.__cleanup_k8s_ingress(k8s_ingress)
+        else:
+            log.debug(f"No ingress found for job with k8s_job_name {k8s_job_name}")
         service_to_delete = find_service_object_by_name(
             self._pykube_api, k8s_job_name, self.runner_params["k8s_namespace"]
         )
         if service_to_delete and len(service_to_delete.response["items"]) > 0:
             k8s_service = Service(self._pykube_api, service_to_delete.response["items"][0])
-            self.__cleanup_k8s_service(k8s_service, job_failed)
+            self.__cleanup_k8s_service(k8s_service)
+        else:
+            log.debug(f"No service found for job with k8s_job_name {k8s_job_name}")
+        # remove the interactive environment entrypoints
+        eps = job_wrapper.get_job().interactivetool_entry_points
+        if eps:
+            log.debug(f"Removing entry points for job with ID {job_wrapper.get_id_tag()}")
+            self.app.interactivetool_manager.remove_entry_points(eps)
 
     def stop_job(self, job_wrapper):
         """Attempts to delete a dispatched job to the k8s cluster"""
         job = job_wrapper.get_job()
         try:
+            log.debug(f"Attempting to stop job {job.id} ({job.job_runner_external_id})")
             job_to_delete = find_job_object_by_name(
                 self._pykube_api, job.get_job_runner_external_id(), self.runner_params["k8s_namespace"]
             )
             if job_to_delete and len(job_to_delete.response["items"]) > 0:
                 k8s_job = Job(self._pykube_api, job_to_delete.response["items"][0])
+                log.debug(f"Found job with id {job.get_job_runner_external_id()} to delete")
+                # For interactive jobs, at this point because the job stopping has been partly handled by the
+                # interactive tool manager, the job wrapper no longer shows any guest ports. We need another way
+                # to check if the job is an interactive job.
                 if self.__has_guest_ports(job_wrapper):
+                    log.debug(f"Job {job.id} ({job.job_runner_external_id}) has guest ports, cleaning them up")
                     self.__cleanup_k8s_guest_ports(job_wrapper, k8s_job)
                 self.__cleanup_k8s_job(k8s_job)
+            else:
+                log.debug(f"Could not find job with id {job.get_job_runner_external_id()} to delete")
             # TODO assert whether job parallelism == 0
             # assert not job_to_delete.exists(), "Could not delete job,"+job.job_runner_external_id+" it still exists"
             log.debug(f"({job.id}/{job.job_runner_external_id}) Terminated at user's request")
 
         except Exception as e:
             log.exception(
                 "({}/{}) User killed running job, but error encountered during termination: {}".format(
@@ -942,14 +1037,81 @@
                     job.id, job.job_runner_external_id
                 )
             )
             ajs.old_state = model.Job.states.QUEUED
             ajs.running = False
             self.monitor_queue.put(ajs)
 
+    # added to make sure that stdout and stderr is captured for Kubernetes
+    def fail_job(self, job_state: "JobState", exception=False, message="Job failed", full_status=None):
+        log.debug("PP Getting into fail_job in k8s runner")
+        job = job_state.job_wrapper.get_job()
+
+        # Get STDOUT and STDERR from the job and tool to be stored in the database #
+        # This is needed because when calling finish_job on a failed job, the check_output method
+        # overrides the job error state and tries to figure it out from the job output files
+        # breaking OOM resubmissions.
+        # To ensure that files below are readable, ownership must be reclaimed first
+        job_state.job_wrapper.reclaim_ownership()
+
+        # wait for the files to appear
+        which_try = 0
+        while which_try < self.app.config.retry_job_output_collection + 1:
+            try:
+                with open(job_state.output_file, "rb") as stdout_file, open(job_state.error_file, "rb") as stderr_file:
+                    job_stdout = self._job_io_for_db(stdout_file)
+                    job_stderr = self._job_io_for_db(stderr_file)
+                break
+            except Exception as e:
+                if which_try == self.app.config.retry_job_output_collection:
+                    job_stdout = ""
+                    job_stderr = job_state.runner_states.JOB_OUTPUT_NOT_RETURNED_FROM_CLUSTER
+                    log.error(f"{job.id}/{job.job_runner_external_id} {job_stderr}: {unicodify(e)}")
+                else:
+                    time.sleep(1)
+                which_try += 1
+
+        # get stderr and stdout to database
+        outputs_directory = os.path.join(job_state.job_wrapper.working_directory, "outputs")
+        if not os.path.exists(outputs_directory):
+            outputs_directory = job_state.job_wrapper.working_directory
+
+        tool_stdout_path = os.path.join(outputs_directory, "tool_stdout")
+        tool_stderr_path = os.path.join(outputs_directory, "tool_stderr")
+
+        # TODO: These might not exist for running jobs at the upgrade to 19.XX, remove that
+        # assumption in 20.XX.
+        tool_stderr = "Galaxy issue: stderr could not be retrieved from the job working directory."
+        tool_stdout = "Galaxy issue: stdout could not be retrieved from the job working directory."
+        if os.path.exists(tool_stdout_path):
+            with open(tool_stdout_path, "rb") as stdout_file:
+                tool_stdout = self._job_io_for_db(stdout_file)
+        else:
+            # Legacy job, were getting a merged output - assume it is mostly tool output.
+            tool_stdout = job_stdout
+            job_stdout = None
+
+        if os.path.exists(tool_stderr_path):
+            with open(tool_stderr_path, "rb") as stdout_file:
+                tool_stderr = self._job_io_for_db(stdout_file)
+        else:
+            # Legacy job, were getting a merged output - assume it is mostly tool output.
+            tool_stderr = job_stderr
+            job_stderr = None
+
+        # full status empty leaves the UI without stderr/stdout
+        full_status = {"stderr": tool_stderr, "stdout": tool_stdout}
+        log.debug(f"({job.id}/{job.job_runner_external_id}) tool_stdout: {tool_stdout}")
+        log.debug(f"({job.id}/{job.job_runner_external_id}) tool_stderr: {tool_stderr}")
+        log.debug(f"({job.id}/{job.job_runner_external_id}) job_stdout: {job_stdout}")
+        log.debug(f"({job.id}/{job.job_runner_external_id}) job_stderr: {job_stderr}")
+
+        # run super method
+        super().fail_job(job_state, exception, message, full_status)
+
     def finish_job(self, job_state):
         self._handle_metadata_externally(job_state.job_wrapper, resolve_requirements=True)
         super().finish_job(job_state)
         jobs = find_job_object_by_name(self._pykube_api, job_state.job_id, self.runner_params["k8s_namespace"])
         if len(jobs.response["items"]) > 1:
             log.warning(
                 "More than one job matches selector: %s. Possible configuration error in job id '%s'",
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/local.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Job runner plugin for executing jobs on the local system via the command line.
 """
+
 import datetime
 import logging
 import os
 import subprocess
 import tempfile
 import threading
 from time import sleep
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/pbs.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/pbs.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,16 +128,15 @@
         if server == "":
             server = self.default_pbs_server
         if server is None:
             raise Exception("Could not find TORQUE server")
 
         # Determine the queue, set the PBS destination (not the same thing as a Galaxy job destination)
         pbs_destination = f"@{server}"
-        pbs_queue = url_split[3] or None
-        if pbs_queue is not None:
+        if (pbs_queue := url_split[3] or None) is not None:
             pbs_destination = f"{pbs_queue}{pbs_destination}"
 
         params = dict(destination=pbs_destination)
 
         # Determine the args (long-format args were never supported in URLs so they are not supported here)
         try:
             opts = url.split("/")[4].strip().lstrip("-").split(" -")
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/pulsar.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/pulsar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Job runner used to execute Galaxy jobs through Pulsar.
 
 More information on Pulsar can be found at https://pulsar.readthedocs.io/ .
 """
+
 import copy
 import errno
 import logging
 import os
 import re
 import subprocess
 from time import sleep
@@ -596,16 +597,15 @@
         return [str(i) for i in input_paths]  # Force job_path from DatasetPath objects.
 
     def get_client_from_wrapper(self, job_wrapper):
         job_id = job_wrapper.job_id
         if hasattr(job_wrapper, "task_id"):
             job_id = f"{job_id}_{job_wrapper.task_id}"
         params = job_wrapper.job_destination.params.copy()
-        user = job_wrapper.get_job().user
-        if user:
+        if user := job_wrapper.get_job().user:
             for key, value in params.items():
                 if value and isinstance(value, str):
                     params[key] = model.User.expand_user_properties(user, value)
 
         env = getattr(job_wrapper.job_destination, "env", [])
         return self.get_client(params, job_id, env)
 
@@ -973,16 +973,16 @@
         galaxy_job_id = None
         remote_job_id = None
         try:
             check_database_connection(self.sa_session)
             remote_job_id = full_status["job_id"]
             if len(remote_job_id) == 32:
                 # It is a UUID - assign_ids = uuid in destination params...
-                stmt = select(model.Job).filter(model.Job.job_runner_external_id == remote_job_id)
-                galaxy_job_id = self.app.model.session.execute(stmt).scalar_one().id
+                stmt = select(model.Job.id).filter(model.Job.job_runner_external_id == remote_job_id)
+                galaxy_job_id = self.app.model.session.execute(stmt).scalar_one()
             else:
                 galaxy_job_id = remote_job_id
             job, job_wrapper = self.app.job_manager.job_handler.job_queue.job_pair_for_id(galaxy_job_id)
             job_state = self._job_state(job, job_wrapper)
             self._update_job_state_for_status(job_state, full_status["status"], full_status=full_status)
         except Exception:
             log.exception(f"Failed to update Pulsar job status for job_id ({galaxy_job_id}/{remote_job_id})")
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/slurm.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/slurm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 SLURM job control via the DRMAA API.
 """
+
 import os
 import time
 
 from galaxy import model
 from galaxy.jobs.runners.drmaa import DRMAAJobRunner
 from galaxy.util import commands
 from galaxy.util.custom_logging import get_logger
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/state_handler_factory.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/state_handler_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/state_handlers/_safe_eval.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/_safe_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from ast import (
-    Module,
     parse,
     walk,
 )
 
 AST_NODE_TYPE_ALLOWLIST = [
     "Expr",
     "Load",
@@ -123,16 +122,14 @@
     if allowed_variables is None:
         allowed_variables = []
     try:
         module = parse(text)
     except SyntaxError:
         return False
 
-    if not isinstance(module, Module):
-        return False
     statements = module.body
     if not len(statements) == 1:
         return False
     expression = statements[0]
     if expression.__class__.__name__ != "Expr":
         return False
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/state_handlers/resubmit.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/resubmit.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/tasks.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/tasks.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/univa.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/univa.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   - extend the job runner to cover s_rt cases (some ideas):
 
     * I'm unsure if the programs reaction to SIGUSR1 can be determined easily
       because it depends on the program. It seems that exit code is in most
       cases 10.
     * The sheduler logs contains quite useful information.
 """
+
 import logging
 import re
 import signal
 import time
 from math import inf
 
 from galaxy.jobs.runners.drmaa import DRMAAJobRunner
@@ -563,16 +564,15 @@
         else:
             log.error(f"DRMAAUniva: job {job_id} unknown state from qstat: {state}")
             return self.drmaa.JobState.UNDETERMINED
 
 
 def _parse_time(tstring):
     tme = None
-    m = re.search("([0-9:.]+)", tstring)
-    if m is not None:
+    if (m := re.search("([0-9:.]+)", tstring)) is not None:
         timespl = m.group(1).split(":")
         tme = float(timespl[-1])  # sec
         if len(timespl) > 1:  # min
             tme += float(timespl[-2]) * 60
         if len(timespl) > 2:  # hour
             tme += float(timespl[-3]) * 3600
         if len(timespl) > 3:  # day
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/__init__.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module and its submodules contains utilities for running external
 processes and interfacing with job managers. This module should contain
 functionality shared between Galaxy and the Pulsar.
 """
+
 from galaxy.util.bunch import Bunch
 from .kill import kill_pid
 
 runner_states = Bunch(
     WALLTIME_REACHED="walltime_reached",
     MEMORY_LIMIT_REACHED="memory_limit_reached",
     JOB_OUTPUT_NOT_RETURNED_FROM_CLUSTER="Job output not returned from cluster",
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/__init__.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 """
+
 import json
 
 from galaxy.util.plugin_config import plugins_dict
 
 DEFAULT_SHELL_PLUGIN = "LocalShell"
 
 ERROR_MESSAGE_NO_JOB_PLUGIN = "No job plugin parameter found, cannot create CLI job interface"
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/__init__.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """
 Abstract base class for cli job plugins.
 """
+
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 from enum import Enum
+from typing import (
+    Dict,
+    List,
+)
+
+from typing_extensions import TypeAlias
 
 try:
     from galaxy.model import Job
 
-    job_states = Job.states
+    job_states: TypeAlias = Job.states
 except ImportError:
     # Not in Galaxy, map Galaxy job states to Pulsar ones.
     class job_states(str, Enum):  # type: ignore[no-redef]
         RUNNING = "running"
         OK = "complete"
         QUEUED = "queued"
         ERROR = "failed"
@@ -56,21 +63,21 @@
     @abstractmethod
     def get_single_status(self, job_id):
         """
         Return command to get the status of a single, specified job.
         """
 
     @abstractmethod
-    def parse_status(self, status, job_ids):
+    def parse_status(self, status: str, job_ids: List[str]) -> Dict[str, job_states]:
         """
         Parse the statuses of output from get_status command.
         """
 
     @abstractmethod
-    def parse_single_status(self, status, job_id):
+    def parse_single_status(self, status: str, job_id: str) -> job_states:
         """
         Parse the status of output from get_single_status command.
         """
 
     def get_failure_reason(self, job_id):
         """
         Return the failure reason for the given job_id.
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/lsf.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/lsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         for line in reason.splitlines():
             if "TERM_MEMLIMIT" in line:
                 return runner_states.MEMORY_LIMIT_REACHED
             if "TERM_RUNLIMIT" in line:
                 return runner_states.WALLTIME_REACHED
         return None
 
-    def _get_job_state(self, state):
+    def _get_job_state(self, state: str) -> str:
         # based on:
         # https://www.ibm.com/support/knowledgecenter/en/SSETD4_9.1.3/lsf_admin/job_state_lsf.html
         # https://www.ibm.com/support/knowledgecenter/en/SSETD4_9.1.2/lsf_command_ref/bjobs.1.html
         try:
             return {
                 "EXIT": job_states.ERROR,
                 "RUN": job_states.RUNNING,
@@ -111,15 +111,15 @@
                 "DONE": job_states.OK,
                 "PSUSP": job_states.ERROR,
                 "USUSP": job_states.ERROR,
                 "SSUSP": job_states.ERROR,
                 "UNKWN": job_states.ERROR,
                 "WAIT": job_states.QUEUED,
                 "ZOMBI": job_states.ERROR,
-            }.get(state)
+            }[state]
         except KeyError:
             raise KeyError(f"Failed to map LSF status code [{state}] to job state.")
 
     def _get_excluded_hosts(self):
         """
         Reads a file in the set path with one node name per line. All these nodes will be added
         to the exclusion list for execution.
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/pbs.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/pbs.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/slurm.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/slurm.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,21 +60,21 @@
         if len(status) > 1:
             # Job still on cluster and has state.
             id, state = status[1].split()
             return self._get_job_state(state)
         # else line like "slurm_load_jobs error: Invalid job id specified"
         return job_states.OK
 
-    def _get_job_state(self, state):
+    def _get_job_state(self, state: str) -> str:
         try:
             return {
                 "F": job_states.ERROR,
                 "R": job_states.RUNNING,
                 "CG": job_states.RUNNING,
                 "PD": job_states.QUEUED,
                 "CD": job_states.OK,
-            }.get(state)
+            }[state]
         except KeyError:
             raise KeyError(f"Failed to map slurm status code [{state}] to job state.")
 
 
 __all__ = ("Slurm",)
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/slurm_torque.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/slurm_torque.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/job/torque.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/torque.py`

 * *Files 15% similar despite different names*

```diff
@@ -73,35 +73,38 @@
                 tree = parse_xml_string(line.strip())
                 assert tree.tag == "Data"
                 break
             except Exception:
                 tree = None
         if tree is None:
             log.warning(f"No valid qstat XML return from `qstat -x`, got the following: {status}")
-            return None
+            return {}
         else:
             for job in tree.findall("Job"):
-                id = job.find("Job_Id").text
-                if id in job_ids:
-                    state = job.find("job_state").text
+                job_id_elem = job.find("Job_Id")
+                assert job_id_elem is not None
+                id_ = job_id_elem.text
+                if id_ in job_ids:
+                    job_state_elem = job.find("job_state")
+                    assert job_state_elem is not None
+                    state = job_state_elem.text
+                    assert state
                     # map PBS job states to Galaxy job states.
-                    rval[id] = self._get_job_state(state)
+                    rval[id_] = self._get_job_state(state)
         return rval
 
     def parse_single_status(self, status, job_id):
         for line in status.splitlines():
             line = line.split(" = ")
             if line[0].strip() == "job_state":
                 return self._get_job_state(line[1].strip())
         # no state found, job has exited
         return job_states.OK
 
-    def _get_job_state(self, state):
+    def _get_job_state(self, state: str) -> job_states:
         try:
-            return {"E": job_states.RUNNING, "R": job_states.RUNNING, "Q": job_states.QUEUED, "C": job_states.OK}.get(
-                state
-            )
+            return {"E": job_states.RUNNING, "R": job_states.RUNNING, "Q": job_states.QUEUED, "C": job_states.OK}[state]
         except KeyError:
             raise KeyError(f"Failed to map torque status code [{state}] to job state.")
 
 
 __all__ = ("Torque",)
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/shell/local.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/local.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/cli/shell/rsh.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/rsh.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/condor/__init__.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/condor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Condor helper utilities.
 """
+
 from subprocess import (
     CalledProcessError,
     check_call,
 )
 
 from galaxy.util import (
     commands,
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/env.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,19 +17,17 @@
     ". 'RAW $FILE'"
     >>> # Source file takes precedence
     >>> env_to_statement(dict(name='X', value='"A","B","C"', file="S"))
     '. "S"'
     >>> env_to_statement(dict(execute="module load java/1.5.1"))
     'module load java/1.5.1'
     """
-    source_file = env.get("file", None)
-    if source_file:
+    if source_file := env.get("file", None):
         return f". {__escape(source_file, env)}"
-    execute = env.get("execute", None)
-    if execute:
+    if execute := env.get("execute", None):
         return execute
     name = env["name"]
     value = __escape(env["value"], env)
     return f"{name}={value}; export {name}"
 
 
 def __escape(value, env):
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/external.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/external.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/fork_safe_write.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/fork_safe_write.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/job_script/CLUSTER_SLOTS_STATEMENT.sh` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/CLUSTER_SLOTS_STATEMENT.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/job_script/MEMORY_STATEMENT_TEMPLATE.sh` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/MEMORY_STATEMENT_TEMPLATE.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/job_script/__init__.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/kill.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/kill.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/process_groups.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/process_groups.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/pykube_util.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/pykube_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Interface layer for pykube library shared between Galaxy and Pulsar."""
+
 import logging
 import os
 import re
 from pathlib import PurePath
 
 try:
     from pykube.config import KubeConfig
@@ -27,15 +28,15 @@
         "following error:\nImportError %s" % str(exc)
     )
 
 log = logging.getLogger(__name__)
 
 DEFAULT_JOB_API_VERSION = "batch/v1"
 DEFAULT_SERVICE_API_VERSION = "v1"
-DEFAULT_INGRESS_API_VERSION = "extensions/v1beta1"
+DEFAULT_INGRESS_API_VERSION = "networking.k8s.io/v1"
 DEFAULT_NAMESPACE = "default"
 INSTANCE_ID_INVALID_MESSAGE = (
     "Galaxy instance [%s] is either too long "
     "(>20 characters) or it includes non DNS "
     "acceptable characters, ignoring it."
 )
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/runners/util/sudo.py` & `galaxy-app-24.0.0/galaxy/jobs/runners/util/sudo.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 
 def sudo_popen(*args, **kwargs):
     """
     Helper method for building and executing Popen command. This is potentially
     sensetive code so should probably be centralized.
     """
-    user = kwargs.get("user", None)
     full_command = [SUDO_PATH, SUDO_PRESERVE_ENVIRONMENT_ARG]
-    if user:
+    if user := kwargs.get("user", None):
         full_command.extend([SUDO_USER_ARG, user])
     full_command.extend(args)
     log.info(f"About to execute the following sudo command - [{' '.join(full_command)}]")
     p = Popen(full_command, shell=False, stdout=PIPE, stderr=PIPE)
     return p
```

### Comparing `galaxy-app-23.2.1/galaxy/jobs/splitters/basic.py` & `galaxy-app-24.0.0/galaxy/jobs/splitters/basic.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/splitters/multi.py` & `galaxy-app-24.0.0/galaxy/jobs/splitters/multi.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/jobs/stock_rules.py` & `galaxy-app-24.0.0/galaxy/jobs/stock_rules.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/main.py` & `galaxy-app-24.0.0/galaxy/main.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/main_config.py` & `galaxy-app-24.0.0/galaxy/main_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utilities for finding Galaxy's configuration file.
 
 This is for use by web framework code and scripts (e.g. scripts/galaxy_main.py).
 """
+
 import os
 from typing import (
     List,
     NamedTuple,
     Optional,
 )
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/__init__.py` & `galaxy-app-24.0.0/galaxy/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/annotatable.py` & `galaxy-app-24.0.0/galaxy/managers/annotatable.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,15 @@
 
 
 class AnnotatableManagerMixin:
     #: class of AnnotationAssociation (e.g. HistoryAnnotationAssociation)
     annotation_assoc: type
 
     @abc.abstractmethod
-    def session(self) -> scoped_session:
-        ...
+    def session(self) -> scoped_session: ...
 
     def annotation(self, item) -> Optional[str]:
         """
         Return the annotation string made by the `item`'s owner or `None` if there
         is no annotation.
         """
         # NOTE: only works with sharable (.user)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/api_keys.py` & `galaxy-app-24.0.0/galaxy/managers/api_keys.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/base.py` & `galaxy-app-24.0.0/galaxy/managers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ModelSerializers allow flexible conversion of model objects to dictionaries.
 They control what keys are sent, how values are simplified, can remap keys,
 and allow both predefined and user controlled key sets.
 
 ModelDeserializers control how a model validates and process an incoming
 attribute change to a model object.
 """
+
 # TODO: it may be there's a better way to combine the above three classes
 #   such as: a single flat class, serializers being singletons in the manager, etc.
 #   instead of the three separate classes. With no 'apparent' perfect scheme
 #   I'm opting to just keep them separate.
 import datetime
 import logging
 import re
@@ -55,27 +56,25 @@
 )
 from galaxy.model import tool_shed_install
 from galaxy.model.base import (
     check_database_connection,
     transaction,
 )
 from galaxy.schema import ValueFilterQueryParams
-from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.storage_cleaner import (
     CleanableItemsSummary,
     StorageItemsCleanupResult,
     StoredItem,
     StoredItemOrderBy,
 )
 from galaxy.security.idencoding import IdEncodingHelper
 from galaxy.structured_app import (
     BasicSharedApp,
     MinimalManagerApp,
 )
-from galaxy.web import url_for as gx_url_for
 
 log = logging.getLogger(__name__)
 
 
 class ParsedFilter(NamedTuple):
     filter_type: str  # orm_function, function, or orm
     filter: Any
@@ -147,21 +146,18 @@
     else:
         if not hasattr(model, class_name):
             raise exceptions.MessageException(f"Item class '{class_name}' not available.")
         item_class = getattr(model, class_name)
     return item_class
 
 
-def decode_id(app: BasicSharedApp, id: Any, kind: Optional[str] = None):
+def decode_id(app: BasicSharedApp, id: Any, kind: Optional[str] = None) -> int:
     # note: use str - occasionally a fully numeric id will be placed in post body and parsed as int via JSON
     #   resulting in error for valid id
-    if isinstance(id, DecodedDatabaseIdField):
-        return int(id)
-    else:
-        return decode_with_security(app.security, id, kind=kind)
+    return decode_with_security(app.security, id, kind=kind)
 
 
 def decode_with_security(security: IdEncodingHelper, id: Any, kind: Optional[str] = None):
     return security.decode_id(str(id), kind=kind)
 
 
 def encode_with_security(security: IdEncodingHelper, id: Any, kind: Optional[str] = None):
@@ -300,22 +296,22 @@
         if limit is not None:
             query = query.limit(limit)
         if offset is not None:
             query = query.offset(offset)
         return query
 
     # .... query resolution
-    def one(self, **kwargs) -> Query:
+    def one(self, **kwargs) -> U:
         """
         Sends kwargs to build the query and returns one and only one model.
         """
         query = self.query(**kwargs)
         return self._one_with_recast_errors(query)
 
-    def _one_with_recast_errors(self, query: Query) -> Query:
+    def _one_with_recast_errors(self, query: Query) -> U:
         """
         Call sqlalchemy's one and recast errors to serializable errors if any.
 
         :raises exceptions.ObjectNotFound: if no model is found
         :raises exceptions.InconsistentDatabase: if more than one model is found
         """
         check_database_connection(self.session())
@@ -324,15 +320,15 @@
             return query.one()
         except sqlalchemy.orm.exc.NoResultFound:
             raise exceptions.ObjectNotFound(f"{self.model_class.__name__} not found")
         except sqlalchemy.orm.exc.MultipleResultsFound:
             raise exceptions.InconsistentDatabase(f"found more than one {self.model_class.__name__}")
 
     # NOTE: at this layer, all ids are expected to be decoded and in int form
-    def by_id(self, id: int) -> Query:
+    def by_id(self, id: int) -> U:
         """
         Gets a model by primary id.
         """
         id_filter = self.model_class.__table__.c.id == id
         return self.one(filters=id_filter)
 
     # .... multirow queries
@@ -354,15 +350,15 @@
         query = self.query(filters=orm_filters, order_by=order_by, limit=None, offset=None, **kwargs)
         items = query.all()
 
         # apply limit, offset after SQL filtering
         items = self._apply_fn_filters_gen(items, fn_filters)
         return list(self._apply_fn_limit_offset_gen(items, limit, offset))
 
-    def count(self, filters=None, **kwargs):
+    def count(self, filters=None, **kwargs) -> int:
         """
         Returns the number of objects matching the given filters.
 
         If the filters include functional filters, this function will raise an exception as they might cause
         performance issues.
         """
         self._handle_filters_case_sensitivity(filters)
@@ -404,15 +400,15 @@
                 fn_filters.append(filter_.filter)
             elif filter_.filter_type == "orm_function":
                 orm_filters.append(filter_.filter(self.model_class))
             else:
                 orm_filters.append(filter_.filter)
         return (orm_filters, fn_filters)
 
-    def _orm_list(self, query=None, **kwargs):
+    def _orm_list(self, query: Optional[Query] = None, **kwargs) -> List[U]:
         """
         Sends kwargs to build the query return all models found.
         """
         query = query or self.query(**kwargs)
         return query.all()
 
     def _apply_fn_filters_gen(self, items, filters):
@@ -495,21 +491,21 @@
         self.session().add(item)
         if flush:
             session = self.session()
             with transaction(session):
                 session.commit()
         return item
 
-    def copy(self, item, **kwargs):
+    def copy(self, item, **kwargs) -> U:
         """
         Clone or copy an item.
         """
         raise exceptions.NotImplemented("Abstract method")
 
-    def update(self, item, new_values, flush=True, **kwargs):
+    def update(self, item, new_values, flush=True, **kwargs) -> U:
         """
         Given a dictionary of new values, update `item` and return it.
 
         ..note: NO validation or deserialization occurs here.
         """
         self.session().add(item)
         for key, value in new_values.items():
@@ -595,16 +591,22 @@
     """
     Raise this inside a serializer to prevent the returned dictionary from having
     a the associated key or value for this attribute.
     """
 
 
 class Serializer(Protocol):
-    def __call__(self, item: Any, key: str, **context) -> Any:
-        ...
+    def __call__(self, item: Any, key: str, **context) -> Any: ...
+
+
+# TODO: eventually all urls should be generated by the url builder and this can be safely removed.
+# Using it for now to identify in which contexts the url builder is not available
+def url_for_not_available(*args, **kwargs):
+    args_str = [str(arg) for arg in args]
+    raise NotImplementedError(f"url_for is not available in this context - args: {args_str} ")
 
 
 class ModelSerializer(HasAModelManager[T]):
     """
     Turns models into JSONable dicts.
 
     Maintains a map of requestable keys and the Callable() serializer functions
@@ -646,15 +648,15 @@
         #   inspired by model.dict_{view}_visible_keys
         self.views = {}
         self.default_view = None
 
     @staticmethod
     def url_for(*args, context=None, **kwargs):
         trans = context and context.get("trans")
-        url_for = trans and trans.url_builder or gx_url_for
+        url_for = trans and trans.url_builder or url_for_not_available
         return url_for(*args, **kwargs)
 
     def add_serializers(self):
         """
         Register a map of attribute keys -> serializing functions that will serialize
         the attribute.
         """
@@ -728,21 +730,21 @@
     def serialize_date(self, item: Any, key: str, **context):
         """
         Serialize a date attribute of `item`.
         """
         date = getattr(item, key)
         return date.isoformat() if date is not None else None
 
-    def serialize_id(self, item: Any, key: str, **context):
+    def serialize_id(self, item: Any, key: str, encode_id=True, **context):
         """
         Serialize an id attribute of `item`.
         """
         id = getattr(item, key)
         # Note: it may not be best to encode the id at this layer
-        return self.app.security.encode_id(id) if id is not None else None
+        return self.app.security.encode_id(id) if id is not None and encode_id else id
 
     def serialize_type_id(self, item: Any, key: str, **context):
         """
         Serialize an type-id for `item`.
         """
         TYPE_ID_SEP = "-"
         type_id = getattr(item, key)
@@ -877,16 +879,15 @@
 
     # def slug( self, item, key, val ):
     #    """validate slug"""
     #    pass
 
 
 class Deserializer(Protocol):
-    def __call__(self, item: Any, key: Any, val: Any, **kwargs) -> Any:
-        ...
+    def __call__(self, item: Any, key: Any, val: Any, **kwargs) -> Any: ...
 
 
 class ModelDeserializer(HasAModelManager[T]):
     """
     An object that converts an incoming serialized dict into values that can be
     directly assigned to an item's attributes and assigns them.
     """
@@ -1049,15 +1050,15 @@
         filter_value_key: str = "qv",
         attr_op_split_char: str = "-",
     ) -> List[Tuple[str, str, str]]:
         """
         Builds a list of tuples containing filtering information in the form of (attribute, operator, value).
         """
         DEFAULT_OP = "eq"
-        qdict = query_params.dict(exclude_defaults=True)
+        qdict = query_params.model_dump(exclude_defaults=True)
         if filter_attr_key not in qdict:
             return []
         # precondition: attrs/value pairs are in-order in the qstring
         attrs = qdict.get(filter_attr_key)
         if not isinstance(attrs, list):
             attrs = [attrs]
         # ops are strings placed after the attr strings and separated by a split char (e.g. 'create_time-lt')
@@ -1139,16 +1140,15 @@
             return None
         allowed_ops = attr_map["op"]
         # allowed ops is a map here, op => fn
         filter_fn = allowed_ops.get(op, None)
         if not filter_fn:
             return None
         # parse the val from string using the 'val' parser if present (otherwise, leave as string)
-        val_parser = attr_map.get("val", None)
-        if val_parser:
+        if val_parser := attr_map.get("val", None):
             val = val_parser(val)
 
         # curry/partial and fold the val in there now
         return self.parsed_filter(filter_type="function", filter=lambda i: filter_fn(i, val))
 
     # ---- ORM filters
     def _parse_orm_filter(self, attr, op, val) -> Optional[ParsedFilter]:
@@ -1262,16 +1262,15 @@
         try:
             epoch = float(date_string)
             datetime_obj = datetime.datetime.fromtimestamp(epoch)
             return datetime_obj.isoformat(sep=" ")
         except ValueError:
             pass
 
-        match = self.date_string_re.match(date_string)
-        if match:
+        if match := self.date_string_re.match(date_string):
             date_string = " ".join(group for group in match.groups() if group)
             return date_string
         raise ValueError("datetime strings must be in the ISO 8601 format and in the UTC")
 
     def contains_non_orm_filter(self, filters: List[ParsedFilter]) -> bool:
         """Whether the list of filters contains any non-orm filter."""
         return any(filter.filter_type == "function" for filter in filters)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/citations.py` & `galaxy-app-24.0.0/galaxy/managers/citations.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/cloud.py` & `galaxy-app-24.0.0/galaxy/managers/cloud.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/cloudauthzs.py` & `galaxy-app-24.0.0/galaxy/managers/cloudauthzs.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,17 @@
         # **c: a dictionary containing 'trans' and 'user' objects.
         serializers: Dict[str, base.Serializer] = {
             "id": lambda item, key, **context: self.app.security.encode_id(item.id),
             "model_class": lambda item, key, **context: "CloudAuthz",
             "user_id": lambda item, key, **context: self.app.security.encode_id(item.user_id),
             "provider": lambda item, key, **context: str(item.provider),
             "config": lambda item, key, **context: item.config,
-            "authn_id": lambda item, key, **context: self.app.security.encode_id(item.authn_id)
-            if item.authn_id
-            else None,
+            "authn_id": lambda item, key, **context: (
+                self.app.security.encode_id(item.authn_id) if item.authn_id else None
+            ),
             "last_update": lambda item, key, **context: str(item.last_update),
             "last_activity": lambda item, key, **context: str(item.last_activity),
             "create_time": lambda item, key, **context: item.create_time.isoformat(),
             "description": lambda item, key, **context: str(item.description),
         }
         self.serializers.update(serializers)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/collections.py` & `galaxy-app-24.0.0/galaxy/managers/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,19 +39,19 @@
 from galaxy.model.dataset_collections.matching import MatchingCollections
 from galaxy.model.dataset_collections.registry import DATASET_COLLECTION_TYPES_REGISTRY
 from galaxy.model.dataset_collections.type_description import COLLECTION_TYPE_DESCRIPTION_FACTORY
 from galaxy.model.mapping import GalaxyModelMapping
 from galaxy.schema.schema import DatasetCollectionInstanceType
 from galaxy.schema.tasks import PrepareDatasetCollectionDownload
 from galaxy.security.idencoding import IdEncodingHelper
-from galaxy.util import validation
-from galaxy.web.short_term_storage import (
+from galaxy.short_term_storage import (
     ShortTermStorageMonitor,
     storage_context,
 )
+from galaxy.util import validation
 
 log = logging.getLogger(__name__)
 
 ERROR_INVALID_ELEMENTS_SPECIFICATION = "Create called with invalid parameters, must specify element identifiers."
 ERROR_NO_COLLECTION_TYPE = "Create called without specifying a collection type."
 
 
@@ -627,17 +627,16 @@
             raise MessageException(f"Dataset collection element definition ({element_identifier}) not dictionary-like.")
         element_id = element_identifier.get("id")
         if not src_type or not element_id:
             message_template = "Problem decoding element identifier %s - must contain a 'src' and a 'id'."
             message = message_template % element_identifier
             raise RequestParameterInvalidException(message)
 
-        tags = element_identifier.pop("tags", None)
         tag_str = ""
-        if tags:
+        if tags := element_identifier.pop("tags", None):
             tag_str = ",".join(str(_) for _ in tags)
         if src_type == "hda":
             hda = self.hda_manager.get_accessible(element_id, trans.user)
             if copy_elements:
                 element: model.HistoryDatasetAssociation = self.hda_manager.copy(
                     hda, history=history or trans.history, hide_copy=True, flush=False
                 )
@@ -668,22 +667,20 @@
         get plugin types involved so it will likely make sense in the future.
         """
         return MatchingCollections.for_collections(collections_to_match, self.collection_type_descriptions)
 
     @overload
     def get_dataset_collection_instance(
         self, trans: ProvidesHistoryContext, instance_type: Literal["history"], id, **kwds: Any
-    ) -> model.HistoryDatasetCollectionAssociation:
-        ...
+    ) -> model.HistoryDatasetCollectionAssociation: ...
 
     @overload
     def get_dataset_collection_instance(
         self, trans: ProvidesHistoryContext, instance_type: Literal["library"], id, **kwds: Any
-    ) -> model.LibraryDatasetCollectionAssociation:
-        ...
+    ) -> model.LibraryDatasetCollectionAssociation: ...
 
     def get_dataset_collection_instance(
         self, trans: ProvidesHistoryContext, instance_type: DatasetCollectionInstanceType, id, **kwds: Any
     ) -> Union[model.HistoryDatasetCollectionAssociation, model.LibraryDatasetCollectionAssociation]:
         """ """
         if instance_type == "history":
             return self.__get_history_collection_instance(trans, id, **kwds)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/collections_util.py` & `galaxy-app-24.0.0/galaxy/managers/collections_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,28 +140,31 @@
         elements, rest_fuzzy_counts = get_fuzzy_count_elements(collection, rank_fuzzy_counts)
         if view == "element":
             dict_value["populated"] = collection.populated
             element_func = dictify_element
         else:
             element_func = dictify_element_reference
         dict_value["elements"] = [element_func(_, rank_fuzzy_counts=rest_fuzzy_counts) for _ in elements]
+        icj = dataset_collection_instance.implicit_collection_jobs
+        if icj:
+            dict_value["implicit_collection_jobs_id"] = icj.id
+        else:
+            dict_value["implicit_collection_jobs_id"] = None
 
-    security.encode_all_ids(dict_value, recursive=True)  # TODO: Use Kyle's recursive formulation of this.
     return dict_value
 
 
 def dictify_element_reference(element, rank_fuzzy_counts=None, recursive=True, security=None):
     """Load minimal details of elements required to show outline of contents in history panel.
 
     History panel can use this reference to expand to full details if individual dataset elements
     are clicked.
     """
     dictified = element.to_dict(view="element")
-    element_object = element.element_object
-    if element_object is not None:
+    if (element_object := element.element_object) is not None:
         object_details = dict(
             id=element_object.id,
             model_class=element_object.__class__.__name__,
         )
         if element.child_collection:
             object_details["collection_type"] = element_object.collection_type
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/configuration.py` & `galaxy-app-24.0.0/galaxy/managers/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Managers, serializers for Galaxy config file data. ConfigSerializer for all users
 and a more expanded set of data for admin in AdminConfigSerializer.
 
 Used by both the API and bootstrapped data.
 """
+
 import logging
 import sys
 from typing import (
     Any,
     Dict,
     List,
 )
 
 from galaxy.managers import base
 from galaxy.managers.context import ProvidesUserContext
 from galaxy.managers.markdown_util import weasyprint_available
 from galaxy.schema import SerializationParams
 from galaxy.structured_app import StructuredApp
-from galaxy.web.framework.base import server_starttime
 
 log = logging.getLogger(__name__)
 
 
 class ConfigurationManager:
     """Interface/service object for interacting with configuration and related data."""
 
@@ -31,15 +31,15 @@
     def get_configuration(
         self, trans: ProvidesUserContext, serialization_params: SerializationParams
     ) -> Dict[str, Any]:
         is_admin = trans.user_is_admin
         host = getattr(trans, "host", None)
         serializer_class = AdminConfigSerializer if is_admin else ConfigSerializer
         serializer = serializer_class(self._app)
-        return serializer.serialize_to_view(self._app.config, host=host, **serialization_params.dict())
+        return serializer.serialize_to_view(self._app.config, host=host, **serialization_params.model_dump())
 
     def version(self) -> Dict[str, Any]:
         version_info = {
             "version_major": self._app.config.version_major,
             "version_minor": self._app.config.version_minor,
         }
         if self._app.config.version_extra:
@@ -52,14 +52,21 @@
     ) -> Dict[str, int]:
         # Handle the special case for library folders
         if (len(encoded_id) % 16 == 1) and encoded_id.startswith("F"):
             encoded_id = encoded_id[1:]
         decoded_id = self._app.security.decode_id(encoded_id)
         return {"decoded_id": decoded_id}
 
+    def encode_id(
+        self,
+        decoded_id: int,
+    ) -> Dict[str, str]:
+        encoded_id = self._app.security.encode_id(decoded_id)
+        return {"encoded_id": encoded_id}
+
     def tool_lineages(self) -> List[Dict[str, Dict]]:
         rval = []
         for id, tool in self._app.toolbox.tools():
             try:
                 lineage_dict = tool.lineage.to_dict()
             except AttributeError:
                 pass
@@ -179,15 +186,15 @@
             "carbon_intensity": _use_config,
             "geographical_server_location_name": _use_config,
             "geographical_server_location_code": _use_config,
             "power_usage_effectiveness": _use_config,
             "message_box_content": _use_config,
             "message_box_visible": _use_config,
             "message_box_class": _use_config,
-            "server_startttime": lambda item, key, **context: server_starttime,
+            "server_starttime": lambda item, key, **context: self.app.server_starttime,
             "mailing_join_addr": _defaults_to("galaxy-announce-join@bx.psu.edu"),  # should this be the schema default?
             "server_mail_configured": lambda item, key, **context: bool(item.smtp_server),
             "registration_warning_message": _use_config,
             "welcome_url": _use_config,
             "show_welcome_with_login": _defaults_to(True),  # schema default is False
             "cookie_domain": _use_config,
             "python": _defaults_to((sys.version_info.major, sys.version_info.minor)),
@@ -202,14 +209,16 @@
             "enable_tool_source_display": _use_config,
             "enable_celery_tasks": _use_config,
             "quota_source_labels": lambda item, key, **context: list(
                 object_store.get_quota_source_map().get_quota_source_labels()
             ),
             "object_store_allows_id_selection": lambda item, key, **context: object_store.object_store_allows_id_selection(),
             "object_store_ids_allowing_selection": lambda item, key, **context: object_store.object_store_ids_allowing_selection(),
+            "object_store_always_respect_user_selection": _use_config,
+            "user_activation_on": _use_config,
             "user_library_import_dir_available": lambda item, key, **context: bool(item.get("user_library_import_dir")),
             "welcome_directory": _use_config,
             "themes": _use_config,
             "tool_training_recommendations": _use_config,
             "tool_training_recommendations_link": _use_config,
             "tool_training_recommendations_api_url": _use_config,
             "enable_notification_system": _use_config,
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/context.py` & `galaxy-app-24.0.0/galaxy/managers/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 include :class:`galaxy.managers.context.ProvidesAppContext`,
 :class:`galaxy.managers.context.ProvidesUserContext`,
 and :class:`galaxy.managers.context.ProvidesHistoryContext`. Methods
 should annotate their dependency on the narrowest context they require.
 A method that requires a user but not a history should declare its
 ``trans`` argument as requiring type :class:`galaxy.managers.context.ProvidesUserContext`.
 """
+
 # TODO: Refactor this class so that galaxy.managers depends on a package
 # containing this.
 # TODO: Provide different classes for real users and potentially bootstrapped
 # users so the framework can provide consistent web exceptions for incorrect
 # user being used in that context and so that the type system can provide
 # more checks against this issue.
 import abc
@@ -230,16 +231,15 @@
         return user
 
     @property
     def anonymous(self) -> bool:
         return self.user is None
 
     def get_current_user_roles(self) -> List[Role]:
-        user = self.user
-        if user:
+        if user := self.user:
             roles = user.all_roles()
         else:
             roles = []
         return roles
 
     @property
     def user_is_admin(self) -> bool:
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/datasets.py` & `galaxy-app-24.0.0/galaxy/managers/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Manager and Serializer for Datasets.
 """
+
 import glob
 import logging
 import os
 from typing import (
     Any,
     Dict,
     List,
@@ -56,14 +57,16 @@
     # TODO:?? get + error_if_uploading is common pattern, should upload check be worked into access/owed?
 
     def __init__(self, app: MinimalManagerApp):
         super().__init__(app)
         self.permissions = DatasetRBACPermissions(app)
         # needed for admin test
         self.user_manager = users.UserManager(app)
+        self.quota_agent = app.quota_agent
+        self.security_agent = app.model.security_agent
 
     def create(self, manage_roles=None, access_roles=None, flush=True, **kwargs):
         """
         Create and return a new Dataset object.
         """
         # default to NEW state on new datasets
         kwargs.update(dict(state=(kwargs.get("state", model.Dataset.states.NEW))))
@@ -139,28 +142,58 @@
     def has_access_permission(self, dataset, user):
         """
         Return T/F if the user has role-based access to the dataset.
         """
         roles = user.all_roles_exploiting_cache() if user else []
         return self.app.security_agent.can_access_dataset(roles, dataset)
 
+    def update_object_store_id(self, trans, dataset, object_store_id: str):
+        device_source_map = self.app.object_store.get_device_source_map()
+        old_object_store_id = dataset.object_store_id
+        new_object_store_id = object_store_id
+        if old_object_store_id == new_object_store_id:
+            return None
+        old_device_id = device_source_map.get_device_id(old_object_store_id)
+        new_device_id = device_source_map.get_device_id(new_object_store_id)
+        if old_device_id != new_device_id:
+            raise exceptions.RequestParameterInvalidException(
+                "Cannot swap object store IDs for object stores that don't share a device ID."
+            )
+
+        if not self.security_agent.can_change_object_store_id(trans.user, dataset):
+            # TODO: probably want separate exceptions for doesn't own the dataset and dataset
+            # has been shared.
+            raise exceptions.InsufficientPermissionsException("Cannot change dataset permissions...")
+
+        quota_source_map = self.app.object_store.get_quota_source_map()
+        if quota_source_map:
+            old_label = quota_source_map.get_quota_source_label(old_object_store_id)
+            new_label = quota_source_map.get_quota_source_label(new_object_store_id)
+            if old_label != new_label:
+                self.quota_agent.relabel_quota_for_dataset(dataset, old_label, new_label)
+        sa_session = self.app.model.context
+        with transaction(sa_session):
+            dataset.object_store_id = new_object_store_id
+            sa_session.add(dataset)
+            sa_session.commit()
+
     def compute_hash(self, request: ComputeDatasetHashTaskRequest):
         # For files in extra_files_path
         dataset = self.by_id(request.dataset_id)
         extra_files_path = request.extra_files_path
         if extra_files_path:
             extra_dir = dataset.extra_files_path_name
             file_path = self.app.object_store.get_filename(dataset, extra_dir=extra_dir, alt_name=extra_files_path)
         else:
             file_path = dataset.get_file_name()
         hash_function = request.hash_function
         calculated_hash_value = memory_bound_hexdigest(hash_func_name=hash_function, path=file_path)
         extra_files_path = request.extra_files_path
         dataset_hash = model.DatasetHash(
-            hash_function=hash_function.value,
+            hash_function=hash_function,
             hash_value=calculated_hash_value,
             extra_files_path=extra_files_path,
         )
         dataset_hash.dataset = dataset
         # TODO: replace/update if the combination of dataset_id/hash_function has already
         # been stored.
         sa_session = self.session()
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/datatypes.py` & `galaxy-app-24.0.0/galaxy/managers/datatypes.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/dbkeys.py` & `galaxy-app-24.0.0/galaxy/managers/dbkeys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functionality for dealing with dbkeys.
 """
+
 import logging
 import os.path
 import re
 from json import loads
 from typing import (
     Dict,
     List,
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/deletable.py` & `galaxy-app-24.0.0/galaxy/managers/deletable.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Other models are deletable and also may be purged. Most often these are
 models have some backing/supporting resources that can be removed as well
 (e.g. Datasets have data files on a drive). Purging these models removes
 the supporting resources as well. These models also have the boolean
 attribute 'purged'.
 """
+
 from typing import (
     Any,
     Dict,
     Set,
 )
 
 from galaxy.model import Base
@@ -28,16 +29,15 @@
     A mixin/interface for a model that is deletable (i.e. has a 'deleted' attr).
 
     Many resources in Galaxy can be marked as deleted - meaning (in most cases)
     that they are no longer needed, should not be displayed, or may be actually
     removed by an admin/script.
     """
 
-    def _session_setattr(self, item: Base, attr: str, val: Any, flush: bool = True):
-        ...
+    def _session_setattr(self, item: Base, attr: str, val: Any, flush: bool = True): ...
 
     def delete(self, item, flush=True, **kwargs):
         """
         Mark as deleted and return.
         """
         return self._session_setattr(item, "deleted", True, flush=flush)
 
@@ -87,16 +87,15 @@
 class PurgableManagerMixin(DeletableManagerMixin):
     """
     A manager interface/mixin for a resource that allows deleting and purging where
     purging is often removal of some additional, non-db resource (e.g. a dataset's
     file).
     """
 
-    def _session_setattr(self, item: Base, attr: str, val: Any, flush: bool = True):
-        ...
+    def _session_setattr(self, item: Base, attr: str, val: Any, flush: bool = True): ...
 
     def purge(self, item, flush=True, **kwargs):
         """
         Mark as purged and return.
 
         Override this in subclasses to do the additional resource removal.
         """
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/display_applications.py` & `galaxy-app-24.0.0/galaxy/managers/display_applications.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/executables.py` & `galaxy-app-24.0.0/galaxy/managers/executables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for loading tools and workflows from paths for admin user requests."""
+
 from typing import (
     Any,
     Dict,
     Optional,
 )
 
 import yaml
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/export_tracker.py` & `galaxy-app-24.0.0/galaxy/managers/export_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,19 @@
         self, object_id: int, object_type: ExportObjectType, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> List[StoreExportAssociation]:
         stmt = (
             select(
                 StoreExportAssociation,
             )
             .where(
-                and_(StoreExportAssociation.object_type == object_type, StoreExportAssociation.object_id == object_id)
+                and_(
+                    StoreExportAssociation.object_type == object_type,
+                    StoreExportAssociation.object_id == object_id,
+                    StoreExportAssociation.task_uuid.is_not(None),
+                )
             )
             .order_by(StoreExportAssociation.create_time.desc())
         )
         if offset:
             stmt = stmt.offset(offset)
         if limit:
             stmt = stmt.limit(limit)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/folders.py` & `galaxy-app-24.0.0/galaxy/managers/folders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Manager and Serializer for Library Folders.
 """
+
 import logging
 from dataclasses import dataclass
 from typing import (
     List,
     Optional,
     Tuple,
     Union,
@@ -45,15 +46,14 @@
     LibraryDatasetDatasetAssociation,
     LibraryDatasetPermissions,
     LibraryFolder,
     LibraryFolderPermissions,
 )
 from galaxy.model.base import transaction
 from galaxy.model.scoped_session import galaxy_scoped_session
-from galaxy.schema.fields import LibraryFolderDatabaseIdField
 from galaxy.schema.schema import LibraryFolderContentsIndexQueryPayload
 from galaxy.security import RBACAgent
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
@@ -182,18 +182,14 @@
         :type   folder:       LibraryFolder
 
         :returns:   dict with data about the folder
         :rtype:     dictionary
 
         """
         folder_dict = folder.to_dict(view="element")
-        folder_dict = trans.security.encode_all_ids(folder_dict, True)
-        folder_dict["id"] = f"F{folder_dict['id']}"
-        if folder_dict["parent_id"] is not None:
-            folder_dict["parent_id"] = f"F{folder_dict['parent_id']}"
         folder_dict["update_time"] = folder.update_time
         return folder_dict
 
     def create(self, trans, parent_folder_id, new_folder_name, new_folder_description=""):
         """
         Create a new folder under the given folder.
 
@@ -543,19 +539,19 @@
     ) -> List[Tuple[str, str]]:
         """
         Returns the folder path from root to the given folder.
 
         The path items are tuples with the name and id of each folder for breadcrumb building purposes.
         """
         current_folder = folder
-        path_to_root = [(LibraryFolderDatabaseIdField.encode(current_folder.id), current_folder.name)]
+        path_to_root = [(current_folder.id, current_folder.name)]
         while current_folder.parent_id is not None:
             parent_folder = sa_session.get(LibraryFolder, current_folder.parent_id)
             current_folder = parent_folder
-            path_to_root.insert(0, (LibraryFolderDatabaseIdField.encode(current_folder.id), current_folder.name))
+            path_to_root.insert(0, (current_folder.id, current_folder.name))
         return path_to_root
 
 
 def get_folder(session, folder_id):
     stmt = select(LibraryFolder).where(LibraryFolder.id == folder_id)
     return session.execute(stmt).scalar_one()
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/genomes.py` & `galaxy-app-24.0.0/galaxy/managers/genomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     Any,
     List,
+    Optional,
     TYPE_CHECKING,
 )
 
 from sqlalchemy import (
     func,
     text,
 )
@@ -23,18 +24,18 @@
 
 
 class GenomesManager:
     def __init__(self, app: StructuredApp):
         self._app = app
         self.genomes = app.genomes
 
-    def get_dbkeys(self, user: m.User, chrom_info: bool) -> List[List[str]]:
+    def get_dbkeys(self, user: Optional[m.User], chrom_info: bool) -> List[List[str]]:
         return self.genomes.get_dbkeys(user, chrom_info)
 
-    def is_registered_dbkey(self, dbkey: str, user: m.User) -> bool:
+    def is_registered_dbkey(self, dbkey: str, user: Optional[m.User]) -> bool:
         dbkeys = self.get_dbkeys(user, chrom_info=False)
         for _, key in dbkeys:
             if dbkey == key:
                 return True
         return False
 
     def get_genome(
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/group_roles.py` & `galaxy-app-24.0.0/galaxy/managers/group_roles.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/group_users.py` & `galaxy-app-24.0.0/galaxy/managers/group_users.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/groups.py` & `galaxy-app-24.0.0/galaxy/managers/groups.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 from sqlalchemy.orm import Session
 
 from galaxy import model
 from galaxy.exceptions import (
     Conflict,
     ObjectAttributeMissingException,
     ObjectNotFound,
+    RequestParameterInvalidException,
 )
 from galaxy.managers.context import ProvidesAppContext
 from galaxy.managers.roles import get_roles_by_ids
 from galaxy.managers.users import get_users_by_ids
 from galaxy.model import Group
 from galaxy.model.base import transaction
 from galaxy.model.scoped_session import galaxy_scoped_session
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.fields import Security
 from galaxy.schema.groups import GroupCreatePayload
 from galaxy.structured_app import MinimalManagerApp
 
 
 class GroupsManager:
     """Interface/service object shared by controllers for interacting with groups."""
 
@@ -29,17 +30,17 @@
 
     def index(self, trans: ProvidesAppContext):
         """
         Displays a collection (list) of groups.
         """
         rval = []
         for group in get_not_deleted_groups(trans.sa_session):
-            item = group.to_dict(value_mapper={"id": DecodedDatabaseIdField.encode})
-            encoded_id = DecodedDatabaseIdField.encode(group.id)
-            item["url"] = self._url_for(trans, "show_group", group_id=encoded_id)
+            item = group.to_dict()
+            encoded_id = Security.security.encode_id(group.id)
+            item["url"] = self._url_for(trans, "group", id=encoded_id)
             rval.append(item)
         return rval
 
     def create(self, trans: ProvidesAppContext, payload: GroupCreatePayload):
         """
         Creates a new group.
         """
@@ -55,57 +56,92 @@
         users = get_users_by_ids(sa_session, user_ids)
         role_ids = payload.role_ids
         roles = get_roles_by_ids(sa_session, role_ids)
         trans.app.security_agent.set_entity_group_associations(groups=[group], roles=roles, users=users)
         with transaction(sa_session):
             sa_session.commit()
 
-        encoded_id = DecodedDatabaseIdField.encode(group.id)
-        item = group.to_dict(view="element", value_mapper={"id": DecodedDatabaseIdField.encode})
-        item["url"] = self._url_for(trans, "show_group", group_id=encoded_id)
+        encoded_id = Security.security.encode_id(group.id)
+        item = group.to_dict(view="element")
+        item["url"] = self._url_for(trans, "group", id=encoded_id)
         return [item]
 
     def show(self, trans: ProvidesAppContext, group_id: int):
         """
         Displays information about a group.
         """
-        encoded_id = DecodedDatabaseIdField.encode(group_id)
+        encoded_id = Security.security.encode_id(group_id)
         group = self._get_group(trans.sa_session, group_id)
-        item = group.to_dict(view="element", value_mapper={"id": DecodedDatabaseIdField.encode})
-        item["url"] = self._url_for(trans, "show_group", group_id=encoded_id)
+        item = group.to_dict(view="element")
+        item["url"] = self._url_for(trans, "group", id=encoded_id)
         item["users_url"] = self._url_for(trans, "group_users", group_id=encoded_id)
         item["roles_url"] = self._url_for(trans, "group_roles", group_id=encoded_id)
         return item
 
     def update(self, trans: ProvidesAppContext, group_id: int, payload: GroupCreatePayload):
         """
         Modifies a group.
         """
         sa_session = trans.sa_session
         group = self._get_group(sa_session, group_id)
-        name = payload.name
-        if name:
+        if name := payload.name:
             self._check_duplicated_group_name(sa_session, name)
             group.name = name
             sa_session.add(group)
         user_ids = payload.user_ids
         users = get_users_by_ids(sa_session, user_ids)
         role_ids = payload.role_ids
         roles = get_roles_by_ids(sa_session, role_ids)
         self._app.security_agent.set_entity_group_associations(
             groups=[group], roles=roles, users=users, delete_existing_assocs=False
         )
         with transaction(sa_session):
             sa_session.commit()
 
-        encoded_id = DecodedDatabaseIdField.encode(group.id)
-        item = group.to_dict(view="element", value_mapper={"id": DecodedDatabaseIdField.encode})
+        encoded_id = Security.security.encode_id(group.id)
+        item = group.to_dict(view="element")
         item["url"] = self._url_for(trans, "show_group", group_id=encoded_id)
         return item
 
+    def delete(self, trans: ProvidesAppContext, group_id: int):
+        group = self._get_group(trans.sa_session, group_id)
+        group.deleted = True
+        trans.sa_session.add(group)
+        with transaction(trans.sa_session):
+            trans.sa_session.commit()
+
+    def purge(self, trans: ProvidesAppContext, group_id: int):
+        sa_session = trans.sa_session
+        group = self._get_group(sa_session, group_id)
+        if not group.deleted:
+            raise RequestParameterInvalidException(
+                f"Group '{group.name}' has not been deleted, so it cannot be purged."
+            )
+        # Delete UserGroupAssociations
+        for uga in group.users:
+            sa_session.delete(uga)
+        # Delete GroupRoleAssociations
+        for gra in group.roles:
+            sa_session.delete(gra)
+        # Delete the group
+        sa_session.delete(group)
+        with transaction(sa_session):
+            sa_session.commit()
+
+    def undelete(self, trans: ProvidesAppContext, group_id: int):
+        group = self._get_group(trans.sa_session, group_id)
+        if not group.deleted:
+            raise RequestParameterInvalidException(
+                f"Group '{group.name}' has not been deleted, so it cannot be undeleted."
+            )
+        group.deleted = False
+        trans.sa_session.add(group)
+        with transaction(trans.sa_session):
+            trans.sa_session.commit()
+
     def _url_for(self, trans, name, **kwargs):
         return trans.url_builder(name, **kwargs)
 
     def _check_duplicated_group_name(self, sa_session: galaxy_scoped_session, group_name: str) -> None:
         if get_group_by_name(sa_session, group_name):
             raise Conflict(f"A group with name '{group_name}' already exists")
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/hdas.py` & `galaxy-app-24.0.0/galaxy/managers/hdas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Manager and Serializer for HDAs.
 
 HistoryDatasetAssociations (HDAs) are datasets contained or created in a
 history.
 """
+
 import gettext
 import logging
 import os
 from typing import (
     Any,
     Dict,
     List,
@@ -415,15 +416,15 @@
                 hda.deleted = True
                 quota_amount = int(hda.quota_amount(user))
                 hda.purge_usage_from_quota(user, hda.dataset.quota_source_info)
                 hda.purged = True
                 dataset_ids_to_remove.add(hda.dataset.id)
                 success_item_count += 1
                 total_free_bytes += quota_amount
-            except BaseException as e:
+            except Exception as e:
                 errors.append(StorageItemCleanupError(item_id=hda_id, error=str(e)))
 
         if success_item_count:
             session = self.hda_manager.session()
             with transaction(session):
                 session.commit()
 
@@ -477,29 +478,30 @@
                 "purged",
                 "visible",
                 "tags",
                 "type",
                 "url",
                 "create_time",
                 "update_time",
+                "object_store_id",
+                "quota_source_label",
             ],
         )
         self.add_view(
             "detailed",
             [
                 "model_class",
                 "history_id",
                 "hid",
                 # why include if model_class is there?
                 "hda_ldda",
                 "copied_from_ldda_id",
                 # TODO: accessible needs to go away
                 "accessible",
                 # remapped
-                "genome_build",
                 "misc_info",
                 "misc_blurb",
                 "file_ext",
                 "file_size",
                 "resubmitted",
                 "metadata",
                 "meta_files",
@@ -590,14 +592,16 @@
             ),
             "parent_id": self.serialize_id,
             # TODO: to DatasetAssociationSerializer
             "accessible": lambda item, key, user=None, **c: self.manager.is_accessible(item, user, **c),
             "api_type": lambda item, key, **context: "file",
             "type": lambda item, key, **context: "file",
             "created_from_basename": lambda item, key, **context: item.created_from_basename,
+            "object_store_id": lambda item, key, **context: item.object_store_id,
+            "quota_source_label": lambda item, key, **context: item.dataset.quota_source_label,
             "hashes": lambda item, key, **context: [h.to_dict() for h in item.hashes],
             "sources": lambda item, key, **context: [s.to_dict() for s in item.sources],
             "drs_id": lambda item, key, **context: f"hda-{self.app.security.encode_id(item.id, kind='drs')}",
         }
         self.serializers.update(serializers)
 
     def serialize(self, hda, keys, user=None, **context):
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/hdcas.py` & `galaxy-app-24.0.0/galaxy/managers/hdcas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Manager and Serializer for HDCAs.
 
 HistoryDatasetCollectionAssociations (HDCAs) are datasets contained or created in a
 history.
 """
+
 import logging
 from typing import Dict
 
 from galaxy import model
 from galaxy.managers import (
     annotatable,
     base,
@@ -267,15 +268,14 @@
                 "populated_state",
                 "populated_state_message",
                 "element_count",
                 "job_source_id",
                 "job_source_type",
                 "job_state_summary",
                 "name",
-                "type_id",
                 "deleted",
                 "visible",
                 "type",
                 "url",
                 "create_time",
                 "update_time",
                 "tags",
@@ -306,14 +306,15 @@
             "type_id": self.serialize_type_id,
             "job_source_id": self.serialize_id,
             "url": lambda item, key, **context: self.url_for(
                 "history_content_typed",
                 history_id=self.app.security.encode_id(item.history_id),
                 id=self.app.security.encode_id(item.id),
                 type=self.hdca_manager.model_class.content_type,
+                context=context,
             ),
             "contents_url": self.generate_contents_url,
             "job_state_summary": self.serialize_job_state_summary,
             "elements_datatypes": self.serialize_elements_datatypes,
             "collection_id": self.serialize_id,
         }
         self.serializers.update(serializers)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/histories.py` & `galaxy-app-24.0.0/galaxy/managers/histories.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,74 @@
 """
 Manager and Serializer for histories.
 
 Histories are containers for datasets or dataset collections
 created (or copied) by users over the course of an analysis.
 """
+
 import logging
 from typing import (
     Any,
     cast,
     Dict,
     List,
     Optional,
     Set,
+    Tuple,
     Union,
 )
 
 from sqlalchemy import (
     asc,
     desc,
+    exists,
     false,
     func,
+    or_,
     select,
     true,
 )
+from sqlalchemy.orm import aliased
 from typing_extensions import Literal
 
-from galaxy import (
-    exceptions as glx_exceptions,
-    model,
+from galaxy import model
+from galaxy.exceptions import (
+    MessageException,
+    ObjectNotFound,
+    RequestParameterInvalidException,
 )
 from galaxy.managers import (
     deletable,
     hdas,
     history_contents,
     sharable,
 )
 from galaxy.managers.base import (
     combine_lists,
     ModelDeserializingError,
     Serializer,
     SortableManager,
     StorageCleanerManager,
 )
+from galaxy.managers.context import ProvidesUserContext
 from galaxy.managers.export_tracker import StoreExportTracker
 from galaxy.model import (
     History,
     HistoryUserShareAssociation,
     Job,
 )
 from galaxy.model.base import transaction
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.model.index_filter_util import (
+    append_user_filter,
+    raw_text_column_filter,
+    tag_filter,
+    text_column_filter,
+)
+from galaxy.schema.fields import Security
+from galaxy.schema.history import HistoryIndexQueryPayload
 from galaxy.schema.schema import (
     ExportObjectMetadata,
     ExportObjectType,
     HDABasicInfo,
     ShareHistoryExtra,
 )
 from galaxy.schema.storage_cleaner import (
@@ -61,17 +76,29 @@
     StorageItemCleanupError,
     StorageItemsCleanupResult,
     StoredItem,
     StoredItemOrderBy,
 )
 from galaxy.security.validate_user_input import validate_preferred_object_store_id
 from galaxy.structured_app import MinimalManagerApp
+from galaxy.util.search import (
+    FilteredTerm,
+    parse_filters_structured,
+    RawTextTerm,
+)
 
 log = logging.getLogger(__name__)
 
+INDEX_SEARCH_FILTERS = {
+    "name": "name",
+    "user": "user",
+    "tag": "tag",
+    "is": "is",
+}
+
 
 class HistoryManager(sharable.SharableModelManager, deletable.PurgableManagerMixin, SortableManager):
     model_class = model.History
     foreign_key_name = "history"
     user_share_model = model.HistoryUserShareAssociation
 
     tag_assoc = model.HistoryTagAssociation
@@ -88,14 +115,129 @@
         contents_filters: history_contents.HistoryContentsFilters,
     ) -> None:
         super().__init__(app)
         self.hda_manager = hda_manager
         self.contents_manager = contents_manager
         self.contents_filters = contents_filters
 
+    def index_query(
+        self, trans: ProvidesUserContext, payload: HistoryIndexQueryPayload, include_total_count: bool = False
+    ) -> Tuple[List[model.History], int]:
+        show_deleted = False
+        show_own = payload.show_own
+        show_published = payload.show_published
+        show_purged = False
+        show_shared = payload.show_shared
+        show_archived = payload.show_archived
+        is_admin = trans.user_is_admin
+        user = trans.user
+
+        if not user and not show_published:
+            message = "Requires user to log in."
+            raise RequestParameterInvalidException(message)
+
+        stmt = select(self.model_class).outerjoin(model.User)
+
+        filters = []
+        if show_own or (not show_published and not show_shared and not is_admin):
+            filters = [self.model_class.user == user]
+        if show_published:
+            filters.append(self.model_class.published == true())
+        if show_shared:
+            filters.append(self.user_share_model.user == user)
+            stmt = stmt.outerjoin(self.model_class.users_shared_with)
+        stmt = stmt.where(or_(*filters))
+
+        if payload.search:
+            search_query = payload.search
+            parsed_search = parse_filters_structured(search_query, INDEX_SEARCH_FILTERS)
+
+            def p_tag_filter(term_text: str, quoted: bool):
+                nonlocal stmt
+                alias = aliased(model.HistoryTagAssociation)
+                stmt = stmt.outerjoin(self.model_class.tags.of_type(alias))
+                return tag_filter(alias, term_text, quoted)
+
+            for term in parsed_search.terms:
+                if isinstance(term, FilteredTerm):
+                    key = term.filter
+                    q = term.text
+                    if key == "tag":
+                        pg = p_tag_filter(term.text, term.quoted)
+                        stmt = stmt.where(pg)
+                    elif key == "name":
+                        stmt = stmt.where(text_column_filter(self.model_class.name, term))
+                    elif key == "user":
+                        stmt = append_user_filter(stmt, self.model_class, term)
+                    elif key == "is":
+                        if q == "deleted":
+                            show_deleted = True
+                        elif q == "importable":
+                            stmt = stmt.where(self.model_class.importable == true())
+                        elif q == "published":
+                            stmt = stmt.where(self.model_class.published == true())
+                        elif q == "purged":
+                            show_purged = True
+                        elif q == "shared_with_me":
+                            if not show_shared:
+                                message = "Can only use tag is:shared_with_me if show_shared parameter also true."
+                                raise RequestParameterInvalidException(message)
+                            stmt = stmt.where(self.user_share_model.user == user)
+                elif isinstance(term, RawTextTerm):
+                    tf = p_tag_filter(term.text, False)
+                    alias = aliased(model.User)
+                    stmt = stmt.outerjoin(self.model_class.user.of_type(alias))
+                    stmt = stmt.where(
+                        raw_text_column_filter(
+                            [
+                                self.model_class.name,
+                                tf,
+                                alias.username,
+                            ],
+                            term,
+                        )
+                    )
+
+        if (show_published or show_shared) and not is_admin:
+            show_deleted = False
+            show_purged = False
+
+        if show_purged:
+            stmt = stmt.where(self.model_class.purged == true())
+        else:
+            stmt = stmt.where(self.model_class.purged == false()).where(
+                self.model_class.deleted == (true() if show_deleted else false())
+            )
+
+        # By default, return only non-archived histories when we are showing the current user's histories
+        # if listing other users' histories, we don't filter out archived histories as they may be
+        # public or shared with the current user
+        if show_own and not show_archived:
+            stmt = stmt.where(self.model_class.archived == false())
+
+        stmt = stmt.distinct()
+
+        if include_total_count:
+            total_matches = get_count(trans.sa_session, stmt)
+        else:
+            total_matches = None
+        if payload.sort_by == "username":
+            sort_column = model.User.username
+            stmt = stmt.add_columns(sort_column)
+        else:
+            sort_column = getattr(model.History, payload.sort_by)
+        if payload.sort_desc:
+            sort_column = sort_column.desc()
+        stmt = stmt.order_by(sort_column)
+        if payload.limit is not None:
+            stmt = stmt.limit(payload.limit)
+        if payload.offset is not None:
+            stmt = stmt.offset(payload.offset)
+        return trans.sa_session.scalars(stmt), total_matches
+
     def copy(self, history, user, **kwargs):
         """
         Copy and return the given `history`.
         """
         return history.copy(target_user=user, **kwargs)
 
     # .... sharable
@@ -205,15 +347,15 @@
         if order_by_string in ("size", "size-dsc"):
             return desc(self.model_class.disk_size)
         if order_by_string == "size-asc":
             return asc(self.model_class.disk_size)
         # TODO: add functional/non-orm orders (such as rating)
         if default:
             return self.parse_order_by(default)
-        raise glx_exceptions.RequestParameterInvalidException(
+        raise RequestParameterInvalidException(
             "Unknown order_by", order_by=order_by_string, available=["create_time", "update_time", "name", "size"]
         )
 
     def non_ready_jobs(self, history):
         """Return the currently running job objects associated with this history.
 
         Where running is defined as new, waiting, queued, running, resubmitted,
@@ -281,15 +423,15 @@
         history_exp_tool = trans.app.toolbox.get_tool(export_tool_id)
         job, *_ = history_exp_tool.execute(trans, incoming=params, history=history, set_output_hid=True)
         trans.app.job_manager.enqueue(job, tool=history_exp_tool)
         return job
 
     def get_sharing_extra_information(
         self, trans, item, users: Set[model.User], errors: Set[str], option: Optional[sharable.SharingOptions] = None
-    ) -> Optional[sharable.ShareWithExtra]:
+    ) -> ShareHistoryExtra:
         """Returns optional extra information about the datasets of the history that can be accessed by the users."""
         extra = ShareHistoryExtra()
         history = cast(model.History, item)
         if history.empty:
             errors.add("You cannot share an empty history.")
             return extra
 
@@ -317,15 +459,15 @@
                 )
                 if option and owner_can_manage_dataset:
                     if option == sharable.SharingOptions.make_accessible_to_shared:
                         trans.app.security_agent.privately_share_dataset(hda.dataset, users=[owner, user])
                     elif option == sharable.SharingOptions.make_public:
                         trans.app.security_agent.make_dataset_public(hda.dataset)
                 else:
-                    hda_id = trans.security.encode_id(hda.id)
+                    hda_id = hda.id
                     hda_info = HDABasicInfo(id=hda_id, name=hda.name)
                     if owner_can_manage_dataset:
                         can_change_dict[hda_id] = hda_info
                     else:
                         cannot_change_dict[hda_id] = hda_info
 
         extra.can_change = list(can_change_dict.values())
@@ -336,21 +478,20 @@
                 "The history you are sharing do not contain any datasets that can be accessed by the users with which you are sharing."
             )
 
         extra.can_share = not errors and (extra.accessible_count == total_dataset_count or option is not None)
         return extra
 
     def is_history_shared_with(self, history: model.History, user: model.User) -> bool:
-        stmt = (
-            select(HistoryUserShareAssociation.id)
+        stmt = select(
+            exists()
             .where(HistoryUserShareAssociation.user_id == user.id)
             .where(HistoryUserShareAssociation.history_id == history.id)
-            .limit(1)
         )
-        return bool(self.session().execute(stmt).first())
+        return self.session().scalar(stmt)
 
     def make_members_public(self, trans, item):
         """Make the non-purged datasets in history public.
         Performs permissions check.
         """
         for hda in item.activatable_datasets:
             dataset = hda.dataset
@@ -382,15 +523,15 @@
         in this case by passing `force=True`.
 
         Please note that histories that are associated with an archive export are usually purged after export, so un-archiving them
         will not restore the datasets that were in the history before it was archived. You will need to import the archive export
         record to restore the history and its datasets as a new copy.
         """
         if history.archive_export_id is not None and history.purged and not force:
-            raise glx_exceptions.RequestParameterInvalidException(
+            raise RequestParameterInvalidException(
                 "Cannot restore an archived (and purged) history that is associated with an archive export record. "
                 "Please try importing it back as a new copy from the associated archive export record instead. "
                 "You can still force the un-archiving of the purged history by setting the 'force' parameter."
             )
 
         history.archived = False
         with transaction(self.session()):
@@ -494,15 +635,15 @@
         for history_id in item_ids:
             try:
                 history = self.history_manager.get_owned(history_id, user)
                 self._unarchive_if_needed(history)
                 self.history_manager.purge(history, flush=False, user=user)
                 success_item_count += 1
                 total_free_bytes += int(history.disk_size)
-            except BaseException as e:
+            except Exception as e:
                 errors.append(StorageItemCleanupError(item_id=history_id, error=str(e)))
 
         if success_item_count:
             session = self.history_manager.session()
             with transaction(session):
                 session.commit()
 
@@ -571,16 +712,16 @@
         history = self._history(trans, history_id)
         matching_exports = history.exports
         return [self.serialize(trans, history_id, e) for e in matching_exports]
 
     def serialize(self, trans, history_id: int, jeha: model.JobExportHistoryArchive) -> dict:
         rval = jeha.to_dict()
         rval["type"] = "job"
-        encoded_jeha_id = DecodedDatabaseIdField.encode(jeha.id)
-        encoded_history_id = DecodedDatabaseIdField.encode(history_id)
+        encoded_jeha_id = Security.security.encode_id(jeha.id)
+        encoded_history_id = Security.security.encode_id(history_id)
         api_url = trans.url_builder("history_archive_download", history_id=encoded_history_id, jeha_id=encoded_jeha_id)
         external_url = trans.url_builder(
             "history_archive_download", history_id=encoded_history_id, jeha_id="latest", qualified=True
         )
         external_permanent_url = trans.url_builder(
             "history_archive_download", history_id=encoded_history_id, jeha_id=encoded_jeha_id, qualified=True
         )
@@ -592,19 +733,19 @@
 
     def get_ready_jeha(self, trans, history_id: int, jeha_id: Union[int, Literal["latest"]] = "latest"):
         history = self._history(trans, history_id)
         matching_exports = history.exports
         if jeha_id != "latest":
             matching_exports = [e for e in matching_exports if e.id == jeha_id]
         if len(matching_exports) == 0:
-            raise glx_exceptions.ObjectNotFound("Failed to find target history export")
+            raise ObjectNotFound("Failed to find target history export")
 
         jeha = matching_exports[0]
         if not jeha.ready:
-            raise glx_exceptions.MessageException("Export not available or not yet ready.")
+            raise MessageException("Export not available or not yet ready.")
 
         return jeha
 
     def _history(self, trans, history_id: int) -> model.History:
         history = self.app.history_manager.get_accessible(history_id, trans.user, current_history=trans.history)
         return history
 
@@ -708,28 +849,30 @@
             "state": self.serialize_history_state,
             "url": lambda item, key, **context: self.url_for(
                 "history", history_id=self.app.security.encode_id(item.id), context=context
             ),
             "contents_url": lambda item, key, **context: self.url_for(
                 "history_contents", history_id=self.app.security.encode_id(item.id), context=context
             ),
-            "hdas": lambda item, key, **context: [self.app.security.encode_id(hda.id) for hda in item.datasets],
+            "hdas": lambda item, key, encode_id=True, **context: [
+                self.app.security.encode_id(hda.id) if encode_id else hda.id for hda in item.datasets
+            ],
             "state_details": self.serialize_state_counts,
             "state_ids": self.serialize_state_ids,
             "contents": self.serialize_contents,
-            "non_ready_jobs": lambda item, key, **context: [
+            "non_ready_jobs": lambda item, key, encode_id=True, **context: [
                 self.app.security.encode_id(job.id) for job in self.manager.non_ready_jobs(item)
             ],
             "contents_states": self.serialize_contents_states,
             "contents_active": self.serialize_contents_active,
             #  TODO: Use base manager's serialize_id for user_id (and others)
             #  after refactoring hierarchy here?
-            "user_id": lambda item, key, **context: self.app.security.encode_id(item.user_id)
-            if item.user_id is not None
-            else None,
+            "user_id": lambda item, key, encode_id=True, **context: (
+                self.app.security.encode_id(item.user_id) if item.user_id is not None and encode_id else item.user_id
+            ),
         }
         self.serializers.update(serializers)
 
     # remove this
     def serialize_state_ids(self, item, key, **context):
         """
         Return a dictionary keyed to possible dataset states and valued with lists
@@ -891,7 +1034,12 @@
         )
 
     def username_eq(self, item, val: str) -> bool:
         return val.lower() == str(item.user.username).lower()
 
     def username_contains(self, item, val: str) -> bool:
         return val.lower() in str(item.user.username).lower()
+
+
+def get_count(session, statement):
+    stmt = select(func.count()).select_from(statement)
+    return session.scalar(stmt)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/history_contents.py` & `galaxy-app-24.0.0/galaxy/managers/history_contents.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Heterogenous lists/contents are difficult to query properly since unions are
 not easily made.
 """
+
 import json
 import logging
 from typing import (
     Any,
     Dict,
     List,
 )
@@ -79,14 +80,15 @@
         "hid",
         # joining columns
         "extension",
         "dataset_id",
         "collection_id",
         "name",
         "state",
+        "object_store_id",
         "size",
         "deleted",
         "purged",
         "visible",
         "create_time",
         "update_time",
     )
@@ -177,20 +179,20 @@
         Note: counts for deleted and hidden overlap; In other words, a dataset that's
         both deleted and hidden will be added to both totals.
         """
         hda_select = self._active_counts_statement(model.HistoryDatasetAssociation, history.id)
         hdca_select = self._active_counts_statement(model.HistoryDatasetCollectionAssociation, history.id)
         subquery = hda_select.union_all(hdca_select).subquery()
         statement = select(
-            cast(func.sum(subquery.c.deleted), Integer).label("deleted"),
-            cast(func.sum(subquery.c.hidden), Integer).label("hidden"),
-            cast(func.sum(subquery.c.active), Integer).label("active"),
+            cast(func.coalesce(func.sum(subquery.c.deleted), 0), Integer).label("deleted"),
+            cast(func.coalesce(func.sum(subquery.c.hidden), 0), Integer).label("hidden"),
+            cast(func.coalesce(func.sum(subquery.c.active), 0), Integer).label("active"),
         )
         returned = self.app.model.context.execute(statement).one()
-        return dict(returned)
+        return dict(returned._mapping)
 
     def _active_counts_statement(self, model_class, history_id):
         deleted_attr = model_class.deleted
         visible_attr = model_class.visible
         table_attr = model_class.table
         return (
             select(
@@ -349,14 +351,16 @@
         component_class = self.contained_class
         # TODO: and now a join with Dataset - this is getting sad
         columns = self._contents_common_columns(
             component_class,
             history_content_type=literal("dataset"),
             size=model.Dataset.file_size,
             state=model.Dataset.state,
+            object_store_id=model.Dataset.object_store_id,
+            quota_source_label=model.Dataset.object_store_id,
             # do not have inner collections
             collection_id=literal(None),
         )
         subquery = self._session().query(*columns)
         # for the HDA's we need to join the Dataset since it has an actual state column
         subquery = subquery.join(model.Dataset, model.Dataset.id == component_class.table.c.dataset_id)
         if history_id:
@@ -375,14 +379,16 @@
         columns = self._contents_common_columns(
             component_class,
             history_content_type=literal("dataset_collection"),
             # do not have datasets
             dataset_id=literal(None),
             size=literal(None),
             state=model.DatasetCollection.populated_state,
+            object_store_id=literal(None),
+            quota_source_label=literal(None),
             # TODO: should be purgable? fix
             purged=literal(False),
             extension=literal(None),
         )
         subquery = self._session().query(*columns)
         # for the HDCA's we need to join the DatasetCollection since it has the populated_state
         subquery = subquery.join(model.DatasetCollection, model.DatasetCollection.id == component_class.collection_id)
@@ -564,16 +570,39 @@
                     states = [s for s in val.split(",") if s]
                     for state in states:
                         if state not in valid_states:
                             raise_filter_err(attr, op, state, "invalid state in filter")
                     return sql.column("state").in_(states)
                 raise_filter_err(attr, op, val, "bad op in filter")
 
-        column_filter = get_filter(attr, op, val)
-        if column_filter is not None:
+            if attr == "object_store_id":
+                if op == "eq":
+                    return sql.column("object_store_id") == val
+
+                if op == "in":
+                    object_store_ids = [s for s in val.split(",") if s]
+                    return sql.column("object_store_id").in_(object_store_ids)
+
+                raise_filter_err(attr, op, val, "bad op in filter")
+
+            if attr == "quota_source_label":
+                if op == "eq":
+                    ids = self.app.object_store.get_quota_source_map().ids_per_quota_source(
+                        include_default_quota_source=True
+                    )
+                    if val == "__null__":
+                        val = None
+                    if val not in ids:
+                        raise KeyError(f"Could not find key {val} in object store keys {list(ids.keys())}")
+                    object_store_ids = ids[val]
+                    return sql.column("object_store_id").in_(object_store_ids)
+
+                raise_filter_err(attr, op, val, "bad op in filter")
+
+        if (column_filter := get_filter(attr, op, val)) is not None:
             return self.parsed_filter(filter_type="orm", filter=column_filter)
         return super()._parse_orm_filter(attr, op, val)
 
     def get_query_filters_with_relations(self, query_filters: ValueFilterQueryParams, related_q: str, history_id):
         """Return `query_filters_with_relations` changing `related:hid` to `related:[hid1, hid2, ...]`."""
         if query_filters.q and query_filters.qv:
             qv_index = query_filters.q.index(related_q)
@@ -621,12 +650,14 @@
                 "history_content_type": {"op": ("eq")},
                 "type_id": {"op": ("eq", "in"), "val": self.parse_type_id_list},
                 "hid": {"op": ("eq", "ge", "le", "gt", "lt"), "val": int},
                 # TODO: needs a different val parser - but no way to add to the above
                 # 'hid-in'        : { 'op': ( 'in' ), 'val': self.parse_int_list },
                 "name": {"op": ("eq", "contains", "like")},
                 "state": {"op": ("eq", "in")},
+                "object_store_id": {"op": ("eq", "in")},
+                "quota_source_label": {"op": ("eq")},
                 "visible": {"op": ("eq"), "val": parse_bool},
                 "create_time": {"op": ("le", "ge", "lt", "gt"), "val": self.parse_date},
                 "update_time": {"op": ("le", "ge", "lt", "gt"), "val": self.parse_date},
             }
         )
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/interactivetool.py` & `galaxy-app-24.0.0/galaxy/managers/interactivetool.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/item_tags.py` & `galaxy-app-24.0.0/galaxy/managers/item_tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/job_connections.py` & `galaxy-app-24.0.0/galaxy/managers/job_connections.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/jobs.py` & `galaxy-app-24.0.0/galaxy/managers/jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     Safety,
 )
 from galaxy.managers.collections import DatasetCollectionManager
 from galaxy.managers.datasets import DatasetManager
 from galaxy.managers.hdas import HDAManager
 from galaxy.managers.lddas import LDDAManager
 from galaxy.model import (
+    ImplicitCollectionJobs,
     ImplicitCollectionJobsJobAssociation,
     Job,
     JobParameter,
     User,
     Workflow,
     WorkflowInvocation,
     WorkflowInvocationStep,
@@ -101,20 +102,26 @@
 
 class JobManager:
     def __init__(self, app: StructuredApp):
         self.app = app
         self.dataset_manager = DatasetManager(app)
 
     def index_query(self, trans, payload: JobIndexQueryPayload) -> sqlalchemy.engine.Result:
+        """The caller is responsible for security checks on the resulting job if
+        history_id, invocation_id, or implicit_collection_jobs_id is set.
+        Otherwise this will only return the user's jobs or all jobs if the requesting
+        user is acting as an admin.
+        """
         is_admin = trans.user_is_admin
         user_details = payload.user_details
         decoded_user_id = payload.user_id
         history_id = payload.history_id
         workflow_id = payload.workflow_id
         invocation_id = payload.invocation_id
+        implicit_collection_jobs_id = payload.implicit_collection_jobs_id
         search = payload.search
         order_by = payload.order_by
 
         def build_and_apply_filters(stmt, objects, filter_func):
             if objects is not None:
                 if isinstance(objects, (str, date, datetime)):
                     stmt = stmt.where(filter_func(objects))
@@ -196,29 +203,39 @@
 
         if is_admin:
             if decoded_user_id is not None:
                 stmt = stmt.where(Job.user_id == decoded_user_id)
             if user_details:
                 stmt = stmt.outerjoin(Job.user)
         else:
-            stmt = stmt.where(Job.user_id == trans.user.id)
+            if history_id is None and invocation_id is None and implicit_collection_jobs_id is None:
+                stmt = stmt.where(Job.user_id == trans.user.id)
+            # caller better check security
 
         stmt = build_and_apply_filters(stmt, payload.states, lambda s: model.Job.state == s)
         stmt = build_and_apply_filters(stmt, payload.tool_ids, lambda t: model.Job.tool_id == t)
         stmt = build_and_apply_filters(stmt, payload.tool_ids_like, lambda t: model.Job.tool_id.like(t))
         stmt = build_and_apply_filters(stmt, payload.date_range_min, lambda dmin: model.Job.update_time >= dmin)
         stmt = build_and_apply_filters(stmt, payload.date_range_max, lambda dmax: model.Job.update_time <= dmax)
 
         if history_id is not None:
             stmt = stmt.where(Job.history_id == history_id)
 
         order_by_columns = Job
         if workflow_id or invocation_id:
             stmt, order_by_columns = add_workflow_jobs()
-
+        elif implicit_collection_jobs_id:
+            stmt = (
+                stmt.join(ImplicitCollectionJobsJobAssociation, ImplicitCollectionJobsJobAssociation.job_id == Job.id)
+                .join(
+                    ImplicitCollectionJobs,
+                    ImplicitCollectionJobs.id == ImplicitCollectionJobsJobAssociation.implicit_collection_jobs_id,
+                )
+                .where(ImplicitCollectionJobsJobAssociation.implicit_collection_jobs_id == implicit_collection_jobs_id)
+            )
         if search:
             stmt = add_search_criteria(stmt)
 
         if order_by == JobIndexSortByEnum.create_time:
             stmt = stmt.order_by(order_by_columns.create_time.desc())
         else:
             stmt = stmt.order_by(order_by_columns.update_time.desc())
@@ -232,15 +249,15 @@
 
     def update_job_lock(self, job_lock: JobLock):
         self.app.queue_worker.send_control_task(
             "admin_job_lock", kwargs={"job_lock": job_lock.active}, get_response=True
         )
         return self.job_lock()
 
-    def get_accessible_job(self, trans, decoded_job_id):
+    def get_accessible_job(self, trans, decoded_job_id) -> Job:
         job = trans.sa_session.get(Job, decoded_job_id)
         if job is None:
             raise ObjectNotFound()
         belongs_to_user = (
             (job.user_id == trans.user.id)
             if job.user_id and trans.user
             else (job.session_id == trans.get_galaxy_session().id)
@@ -370,27 +387,24 @@
             and_(
                 model.Job.any_output_dataset_collection_instances_deleted == false(),
                 model.Job.any_output_dataset_deleted == false(),
             )
         )
 
         for k, v in wildcard_param_dump.items():
-            wildcard_value = None
             if v == {"__class__": "RuntimeValue"}:
                 # TODO: verify this is always None. e.g. run with runtime input input
                 v = None
             elif k.endswith("|__identifier__"):
                 # We've taken care of this while constructing the conditions based on ``input_data`` above
                 continue
             elif k == "chromInfo" and "?.len" in v:
                 continue
-                wildcard_value = '"%?.len"'
-            if not wildcard_value:
-                value_dump = json.dumps(v, sort_keys=True)
-                wildcard_value = value_dump.replace('"id": "__id_wildcard__"', '"id": %')
+            value_dump = json.dumps(v, sort_keys=True)
+            wildcard_value = value_dump.replace('"id": "__id_wildcard__"', '"id": %')
             a = aliased(JobParameter)
             if value_dump == wildcard_value:
                 subq = subq.join(a).where(
                     and_(
                         Job.id == a.job_id,
                         a.name == k,
                         a.value == value_dump,
@@ -580,17 +594,14 @@
                         # TODO: verify this is always None. e.g. run with runtime input input
                         v = None
                     elif k.endswith("|__identifier__"):
                         # We've taken care of this while constructing the conditions based on ``input_data`` above
                         continue
                     elif k == "chromInfo" and "?.len" in v:
                         continue
-                        wildcard_value = '"%?.len"'
-                    if not wildcard_value:
-                        wildcard_value = json.dumps(v, sort_keys=True).replace('"id": "__id_wildcard__"', '"id": %')
                     a = aliased(model.JobParameter)
                     job_parameter_conditions.append(
                         and_(model.Job.id == a.job_id, a.name == k, a.value == json.dumps(v, sort_keys=True))
                     )
             else:
                 job_parameter_conditions = [model.Job.id == job[0]]
             job = get_job(self.sa_session, *job_parameter_conditions)
@@ -615,17 +626,17 @@
                 continue
             log.info("Found equivalent job %s", search_timer)
             return job
         log.info("No equivalent jobs found %s", search_timer)
         return None
 
 
-def view_show_job(trans, job, full: bool) -> typing.Dict:
+def view_show_job(trans, job: Job, full: bool) -> typing.Dict:
     is_admin = trans.user_is_admin
-    job_dict = trans.app.security.encode_all_ids(job.to_dict("element", system_details=is_admin), True)
+    job_dict = job.to_dict("element", system_details=is_admin)
     if trans.app.config.expose_dataset_path and "command_line" not in job_dict:
         job_dict["command_line"] = job.command_line
     if full:
         job_dict.update(
             dict(
                 tool_stdout=job.tool_stdout,
                 tool_stderr=job.tool_stderr,
@@ -864,21 +875,20 @@
     """
 
     destination_params = {
         "Runner": job.job_runner_name,
         "Runner Job ID": job.job_runner_external_id,
         "Handler": job.handler,
     }
-    job_destination_params = job.destination_params
-    if job_destination_params:
+    if job_destination_params := job.destination_params:
         destination_params.update(job_destination_params)
     return destination_params
 
 
-def summarize_job_parameters(trans, job):
+def summarize_job_parameters(trans, job: Job):
     """Produce a dict-ified version of job parameters ready for tabular rendering.
 
     Precondition: the caller has verified the job is accessible to the user
     represented by the trans parameter.
     """
     # More client logic here than is ideal but it is hard to reason about
     # tool parameter types on the client relative to the server.
@@ -887,43 +897,44 @@
         if upgrade_messages is None:
             upgrade_messages = {}
 
         rval = []
 
         for input in input_params.values():
             if input.name in param_values:
+                input_value = param_values[input.name]
                 if input.type == "repeat":
-                    for i in range(len(param_values[input.name])):
-                        rval.extend(inputs_recursive(input.inputs, param_values[input.name][i], depth=depth + 1))
+                    for i in range(len(input_value)):
+                        rval.extend(inputs_recursive(input.inputs, input_value[i], depth=depth + 1))
                 elif input.type == "section":
                     # Get the value of the current Section parameter
                     rval.append(dict(text=input.name, depth=depth))
                     rval.extend(
                         inputs_recursive(
                             input.inputs,
-                            param_values[input.name],
+                            input_value,
                             depth=depth + 1,
                             upgrade_messages=upgrade_messages.get(input.name),
                         )
                     )
                 elif input.type == "conditional":
                     try:
-                        current_case = param_values[input.name]["__current_case__"]
+                        current_case = input_value["__current_case__"]
                         is_valid = True
                     except Exception:
                         current_case = None
                         is_valid = False
                     if is_valid:
                         rval.append(
                             dict(text=input.test_param.label, depth=depth, value=input.cases[current_case].value)
                         )
                         rval.extend(
                             inputs_recursive(
                                 input.cases[current_case].inputs,
-                                param_values[input.name],
+                                input_value,
                                 depth=depth + 1,
                                 upgrade_messages=upgrade_messages.get(input.name),
                             )
                         )
                     else:
                         rval.append(
                             dict(
@@ -934,28 +945,32 @@
                             )
                         )
                 elif input.type == "upload_dataset":
                     rval.append(
                         dict(
                             text=input.group_title(param_values),
                             depth=depth,
-                            value=f"{len(param_values[input.name])} uploaded datasets",
+                            value=f"{len(input_value)} uploaded datasets",
                         )
                     )
-                elif input.type == "data" or input.type == "data_collection":
+                elif (
+                    input.type == "data"
+                    or input.type == "data_collection"
+                    or isinstance(input_value, model.HistoryDatasetAssociation)
+                ):
                     value = []
-                    for element in listify(param_values[input.name]):
-                        encoded_id = trans.security.encode_id(element.id)
+                    for element in listify(input_value):
+                        element_id = element.id
                         if isinstance(element, model.HistoryDatasetAssociation):
                             hda = element
-                            value.append({"src": "hda", "id": encoded_id, "hid": hda.hid, "name": hda.name})
+                            value.append({"src": "hda", "id": element_id, "hid": hda.hid, "name": hda.name})
                         elif isinstance(element, model.DatasetCollectionElement):
-                            value.append({"src": "dce", "id": encoded_id, "name": element.element_identifier})
+                            value.append({"src": "dce", "id": element_id, "name": element.element_identifier})
                         elif isinstance(element, model.HistoryDatasetCollectionAssociation):
-                            value.append({"src": "hdca", "id": encoded_id, "hid": element.hid, "name": element.name})
+                            value.append({"src": "hdca", "id": element_id, "hid": element.hid, "name": element.name})
                         else:
                             raise Exception(
                                 f"Unhandled data input parameter type encountered {element.__class__.__name__}"
                             )
                     rval.append(dict(text=input.label, depth=depth, value=value))
                 elif input.visible:
                     if hasattr(input, "label") and input.label:
@@ -963,15 +978,15 @@
                     else:
                         # value for label not required, fallback to input name (same as tool panel)
                         label = input.name
                     rval.append(
                         dict(
                             text=label,
                             depth=depth,
-                            value=input.value_to_display_text(param_values[input.name]),
+                            value=input.value_to_display_text(input_value),
                             notes=upgrade_messages.get(input.name, ""),
                         )
                     )
             else:
                 # Parameter does not have a stored value.
                 # Get parameter label.
                 if input.type == "conditional":
@@ -1008,30 +1023,30 @@
         parameters = inputs_recursive(tool.inputs, params_objects, depth=1, upgrade_messages=upgrade_messages)
     else:
         has_parameter_errors = True
 
     return {
         "parameters": parameters,
         "has_parameter_errors": has_parameter_errors,
-        "outputs": summarize_job_outputs(job=job, tool=tool, params=params_objects, security=trans.security),
+        "outputs": summarize_job_outputs(job=job, tool=tool, params=params_objects),
     }
 
 
 def get_output_name(tool, output, params):
     try:
         return tool.tool_action.get_output_name(
             output,
             tool=tool,
             params=params,
         )
     except Exception:
         pass
 
 
-def summarize_job_outputs(job: model.Job, tool, params, security):
+def summarize_job_outputs(job: model.Job, tool, params):
     outputs = defaultdict(list)
     output_labels = {}
     possible_outputs = (
         ("hda", "dataset_id", job.output_datasets),
         ("ldda", "ldda_id", job.output_library_datasets),
         ("hdca", "dataset_collection_id", job.output_dataset_collection_instances),
     )
@@ -1043,15 +1058,15 @@
                 output_labels[output_name] = get_output_name(
                     tool=tool, output=tool_output.get(output_name), params=params
                 )
             label = output_labels.get(output_name)
             outputs[output_name].append(
                 {
                     "label": label,
-                    "value": {"src": src, "id": security.encode_id(getattr(output_association, attribute))},
+                    "value": {"src": src, "id": getattr(output_association, attribute)},
                 }
             )
     return outputs
 
 
 def get_jobs_to_check_at_startup(session: Session, track_jobs_in_database: bool, config):
     if track_jobs_in_database:
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/lddas.py` & `galaxy-app-24.0.0/galaxy/managers/lddas.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/libraries.py` & `galaxy-app-24.0.0/galaxy/managers/libraries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Manager and Serializer for libraries.
 """
+
 import logging
 from typing import (
     Dict,
     Optional,
     Set,
     Tuple,
 )
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/library_datasets.py` & `galaxy-app-24.0.0/galaxy/managers/library_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Manager and Serializer for library datasets."""
+
 import logging
 
 from sqlalchemy import select
 
 from galaxy import (
     model,
     util,
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/licenses.json` & `galaxy-app-24.0.0/galaxy/managers/licenses.json`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/licenses.py` & `galaxy-app-24.0.0/galaxy/managers/licenses.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,41 +12,45 @@
 from galaxy.util.resources import resource_string
 
 log = logging.getLogger(__name__)
 
 
 # https://github.com/spdx/license-list-data/blob/master/accessingLicenses.md#license-list-table-of-contents
 class LicenseMetadataModel(BaseModel):
-    licenseId: str = Field(title="Identifier", description="SPDX Identifier", example="Apache-2.0")
-    name: str = Field(title="Name", description="Full name of the license", example="Apache License 2.0")
+    licenseId: str = Field(title="Identifier", description="SPDX Identifier", examples=["Apache-2.0"])
+    name: str = Field(title="Name", description="Full name of the license", examples=["Apache License 2.0"])
     reference: str = Field(
-        title="Reference", description="Reference to the HTML format for the license file", example="./Apache-2.0.html"
+        title="Reference",
+        description="Reference to the HTML format for the license file",
+        examples=["./Apache-2.0.html"],
     )
     referenceNumber: int = Field(
         title="Reference number", description="*Deprecated* - this field is generated and is no longer in use"
     )
     isDeprecatedLicenseId: bool = Field(
-        title="Deprecated License", description="True if the entire license is deprecated", example=False
+        title="Deprecated License", description="True if the entire license is deprecated", examples=[False]
     )
     isOsiApproved: bool = Field(
         title="OSI approved",
         description="Indicates if the [OSI](https://opensource.org/) has approved the license",
-        example=True,
+        examples=[True],
     )
     seeAlso: List[HttpUrl] = Field(
         title="Reference URLs", description="Cross reference URL pointing to additional copies of the license"
     )
     detailsUrl: HttpUrl = Field(
         title="Details URL",
         description="URL to the SPDX json details for this license",
-        example="http://spdx.org/licenses/Apache-2.0.json",
+        examples=["http://spdx.org/licenses/Apache-2.0.json"],
     )
     recommended: bool = Field(title="Recommended", description="True if this license is recommended to be used")
-    url: HttpUrl = Field(title="URL", description="License URL", example="http://www.apache.org/licenses/LICENSE-2.0")
-    spdxUrl: HttpUrl = Field(title="SPDX URL", example="https://spdx.org/licenses/Apache-2.0.html")
+    url: HttpUrl = Field(
+        title="URL", description="License URL", examples=["http://www.apache.org/licenses/LICENSE-2.0"]
+    )
+    spdxUrl: HttpUrl = Field(title="SPDX URL", examples=["https://spdx.org/licenses/Apache-2.0.html"])
 
 
 # https://docs.google.com/document/d/16vnRtDjrx5eHSl4jXs2vMaDTI6luyyLzU6xMvRHsnbI/edit#heading=h.1pihjj16olz2
 RECOMMENDED_LICENSES = [
     "Apache-2.0",
     "Artistic-2.0",
     "BSD-2-Clause",
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/markdown_parse.py` & `galaxy-app-24.0.0/galaxy/managers/markdown_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Utilities for parsing "Galaxy Flavored Markdown".
 
 See markdown_util.py for loading objects and interacting with the rest of Galaxy.
 This file is meant to be relatively self contained and just used to "parse" and validate
 Galaxy Markdown. Keeping things isolated to allow re-use of these utilities in other
 projects (e.g. gxformat2).
 """
+
 import re
 from typing import (
     cast,
     Dict,
     List,
     Union,
 )
@@ -26,28 +27,38 @@
 DYNAMIC_ARGUMENTS = DynamicArguments()
 SHARED_ARGUMENTS: List[str] = ["collapse"]
 VALID_ARGUMENTS: Dict[str, Union[List[str], DynamicArguments]] = {
     "history_link": ["history_id"],
     "history_dataset_display": ["input", "output", "history_dataset_id"],
     "history_dataset_embedded": ["input", "output", "history_dataset_id"],
     "history_dataset_as_image": ["input", "output", "history_dataset_id", "path"],
+    "history_dataset_as_table": [
+        "input",
+        "output",
+        "history_dataset_id",
+        "path",
+        "title",
+        "footer",
+        "show_column_headers",
+        "compact",
+    ],
     "history_dataset_peek": ["input", "output", "history_dataset_id"],
     "history_dataset_info": ["input", "output", "history_dataset_id"],
     "history_dataset_link": ["input", "output", "history_dataset_id", "path", "label"],
     "history_dataset_index": ["input", "output", "history_dataset_id", "path"],
     "history_dataset_name": ["input", "output", "history_dataset_id"],
     "history_dataset_type": ["input", "output", "history_dataset_id"],
     "history_dataset_collection_display": ["input", "output", "history_dataset_collection_id"],
     "workflow_display": ["workflow_id", "workflow_checkpoint"],
     "workflow_license": ["workflow_id"],
     "workflow_image": ["workflow_id", "size", "workflow_checkpoint"],
-    "job_metrics": ["step", "job_id"],
-    "job_parameters": ["step", "job_id"],
-    "tool_stderr": ["step", "job_id"],
-    "tool_stdout": ["step", "job_id"],
+    "job_metrics": ["step", "job_id", "implicit_collection_jobs_id"],
+    "job_parameters": ["step", "job_id", "implicit_collection_jobs_id"],
+    "tool_stderr": ["step", "job_id", "implicit_collection_jobs_id"],
+    "tool_stdout": ["step", "job_id", "implicit_collection_jobs_id"],
     "generate_galaxy_version": [],
     "generate_time": [],
     "instance_access_link": [],
     "instance_resources_link": [],
     "instance_help_link": [],
     "instance_support_link": [],
     "instance_citation_link": [],
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/markdown_util.py` & `galaxy-app-24.0.0/galaxy/managers/markdown_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 The core "Galaxy Flavored Markdown" format should just reference objects
 by encoded IDs - but preprocessing should allow for instance workflow objects
 to be referenced relative to the workflow (inputs, outputs, steps, etc..) and
 potential history flavor would allow objects to be referenced by HID. This
 second idea is unimplemented, it is just an example of the general concept of
 context specific processing.
 """
+
 import abc
 import base64
 import codecs
 import logging
 import os
 import re
 import shutil
@@ -42,25 +43,26 @@
 from galaxy.managers.hdcas import HDCASerializer
 from galaxy.managers.jobs import (
     JobManager,
     summarize_job_metrics,
     summarize_job_parameters,
 )
 from galaxy.managers.licenses import LicensesManager
+from galaxy.model import Job
 from galaxy.model.item_attrs import get_item_annotation_str
 from galaxy.model.orm.now import now
 from galaxy.schema import PdfDocumentType
 from galaxy.schema.tasks import GeneratePdfDownload
-from galaxy.util.markdown import literal_via_fence
-from galaxy.util.resources import resource_string
-from galaxy.util.sanitize_html import sanitize_html
-from galaxy.web.short_term_storage import (
+from galaxy.short_term_storage import (
     ShortTermStorageMonitor,
     storage_context,
 )
+from galaxy.util.markdown import literal_via_fence
+from galaxy.util.resources import resource_string
+from galaxy.util.sanitize_html import sanitize_html
 from .markdown_parse import (
     GALAXY_MARKDOWN_FUNCTION_CALL_LINE,
     validate_galaxy_markdown,
 )
 
 log = logging.getLogger(__name__)
 
@@ -68,33 +70,32 @@
 OUTPUT_LABEL_PATTERN = re.compile(r"output=\s*%s\s*" % ARG_VAL_CAPTURED_REGEX)
 INPUT_LABEL_PATTERN = re.compile(r"input=\s*%s\s*" % ARG_VAL_CAPTURED_REGEX)
 STEP_LABEL_PATTERN = re.compile(r"step=\s*%s\s*" % ARG_VAL_CAPTURED_REGEX)
 PATH_LABEL_PATTERN = re.compile(r"path=\s*%s\s*" % ARG_VAL_CAPTURED_REGEX)
 SIZE_PATTERN = re.compile(r"size=\s*%s\s*" % ARG_VAL_CAPTURED_REGEX)
 # STEP_OUTPUT_LABEL_PATTERN = re.compile(r'step_output=([\w_\-]+)/([\w_\-]+)')
 UNENCODED_ID_PATTERN = re.compile(
-    r"(history_id|workflow_id|history_dataset_id|history_dataset_collection_id|job_id|invocation_id)=([\d]+)"
+    r"(history_id|workflow_id|history_dataset_id|history_dataset_collection_id|job_id|implicit_collection_jobs_id|invocation_id)=([\d]+)"
 )
 ENCODED_ID_PATTERN = re.compile(
-    r"(history_id|workflow_id|history_dataset_id|history_dataset_collection_id|job_id|invocation_id)=([a-z0-9]+)"
+    r"(history_id|workflow_id|history_dataset_id|history_dataset_collection_id|job_id|implicit_collection_jobs_id|invocation_id)=([a-z0-9]+)"
 )
 INVOCATION_SECTION_MARKDOWN_CONTAINER_LINE_PATTERN = re.compile(r"```\s*galaxy\s*")
 GALAXY_FENCED_BLOCK = re.compile(r"^```\s*galaxy\s*(.*?)^```", re.MULTILINE ^ re.DOTALL)
 VALID_CONTAINER_START_PATTERN = re.compile(r"^```\s+[\w]+.*$")
 
 
 def ready_galaxy_markdown_for_import(trans, external_galaxy_markdown):
     """Convert from encoded IDs to decoded numeric IDs for storing in the DB."""
 
     _validate(external_galaxy_markdown, internal=False)
 
     def _remap(container, line):
-        id_match = re.search(ENCODED_ID_PATTERN, line)
         object_id = None
-        if id_match:
+        if id_match := re.search(ENCODED_ID_PATTERN, line):
             object_id = id_match.group(2)
             decoded_id = trans.security.decode_id(object_id)
             line = line.replace(id_match.group(), "%s=%d" % (id_match.group(1), decoded_id))
         return (line, False)
 
     internal_markdown = _remap_galaxy_markdown_calls(_remap, external_galaxy_markdown)
     return internal_markdown
@@ -134,14 +135,18 @@
                 _check_object(object_id, line)
                 hda = hda_manager.get_accessible(object_id, trans.user)
                 rval = self.handle_dataset_embedded(line, hda)
             elif container == "history_dataset_as_image":
                 _check_object(object_id, line)
                 hda = hda_manager.get_accessible(object_id, trans.user)
                 rval = self.handle_dataset_as_image(line, hda)
+            elif container == "history_dataset_as_table":
+                _check_object(object_id, line)
+                hda = hda_manager.get_accessible(object_id, trans.user)
+                rval = self.handle_dataset_as_table(line, hda)
             elif container == "history_dataset_peek":
                 _check_object(object_id, line)
                 hda = hda_manager.get_accessible(object_id, trans.user)
                 rval = self.handle_dataset_peek(line, hda)
             elif container == "history_dataset_info":
                 _check_object(object_id, line)
                 hda = hda_manager.get_accessible(object_id, trans.user)
@@ -228,18 +233,17 @@
                 line, *_ = self._encode_line(trans, line)
                 return self.handle_error(container, line, str(e))
 
         export_markdown = _remap_galaxy_markdown_calls(_remap_container, internal_galaxy_markdown)
         return export_markdown
 
     def _encode_line(self, trans, line):
-        id_match = re.search(UNENCODED_ID_PATTERN, line)
         object_id = None
         encoded_id = None
-        if id_match:
+        if id_match := re.search(UNENCODED_ID_PATTERN, line):
             object_id = int(id_match.group(2))
             encoded_id = trans.security.encode_id(object_id)
             line = line.replace(id_match.group(), f"{id_match.group(1)}={encoded_id}")
         return line, object_id, encoded_id
 
     @abc.abstractmethod
     def handle_history_link(self, line, history):
@@ -250,14 +254,18 @@
         pass
 
     @abc.abstractmethod
     def handle_dataset_as_image(self, line, hda):
         pass
 
     @abc.abstractmethod
+    def handle_dataset_as_table(self, line, hda):
+        pass
+
+    @abc.abstractmethod
     def handle_dataset_peek(self, line, hda):
         pass
 
     @abc.abstractmethod
     def handle_dataset_embedded(self, line, hda):
         pass
 
@@ -409,14 +417,17 @@
     # Following three cases - the client side widgets have everything they need
     # from the encoded ID. Don't implement a default on the base class though because
     # it is good to force both Client and PDF/HTML export to deal with each new directive
     # explicitly.
     def handle_dataset_as_image(self, line, hda):
         pass
 
+    def handle_dataset_as_table(self, line, hda):
+        pass
+
     def handle_job_metrics(self, line, job):
         pass
 
     def handle_job_parameters(self, line, job):
         pass
 
     def handle_generate_galaxy_version(self, line, generate_version):
@@ -520,31 +531,38 @@
             markdown += f"**{header}:**\n"
             markdown += datatype.display_as_markdown(hda)
         return markdown
 
     def handle_dataset_as_image(self, line, hda):
         dataset = hda.dataset
         name = hda.name or ""
-        path_match = re.search(PATH_LABEL_PATTERN, line)
 
-        if path_match:
+        if path_match := re.search(PATH_LABEL_PATTERN, line):
             filepath = path_match.group(2)
             file = os.path.join(hda.extra_files_path, filepath)
         else:
             file = dataset.get_file_name()
 
         with open(file, "rb") as f:
             image_data = f.read()
         rval = (self._embed_image(name, "png", image_data), True)
         return rval
 
     def _embed_image(self, name: str, image_type: str, image_data: bytes):
         base64_image_data = base64.b64encode(image_data).decode("utf-8")
         return f"![{name}](data:image/{image_type};base64,{base64_image_data})"
 
+    def handle_dataset_as_table(self, line, hda):
+        # TODO: this form of the rendering doesn't do anything special with advanced
+        # options yet but could easily be modified in the future. show_column_headers,
+        # compact, title, and footer should be handled in here to bring the PDF and the
+        # web rendering closer.
+        rval = self.handle_dataset_embedded(line, hda)
+        return rval
+
     def handle_history_link(self, line, history):
         if history:
             content = literal_via_fence(history.name)
         else:
             content = "*No History available*"
         return (content, True)
 
@@ -577,17 +595,16 @@
             markdown += "|{}|{}|\n".format(step.label or "Step %d" % (order_index + 1), annotation)
         markdown += "\n---\n"
         return (markdown, True)
 
     def handle_workflow_license(self, line, stored_workflow):
         # workflow_manager = self.trans.app.workflow_manager
         license_manager = LicensesManager()
-        license_id = stored_workflow.latest_workflow.license
         markdown = "*No license specified.*"
-        if license_id:
+        if license_id := stored_workflow.latest_workflow.license:
             try:
                 license_metadata = license_manager.get_license_by_id(license_id)
                 markdown = f"[{license_metadata.name}]({license_metadata.url})"
             except ObjectNotFound:
                 markdown = f"Unknown license ({license_id})"
         return (f"\n\n{markdown}\n\n", True)
 
@@ -636,15 +653,15 @@
         for metric_plugin, metrics_for_plugin in metrics_by_plugin.items():
             markdown += f"**{metric_plugin}**\n\n"
             markdown += "|   |   |\n|---|--|\n"
             for title, value in metrics_for_plugin.items():
                 markdown += f"| {title} | {value} |\n"
         return (markdown, True)
 
-    def handle_job_parameters(self, line, job):
+    def handle_job_parameters(self, line, job: Job):
         markdown = """
 | Input Parameter | Value |
 |-----------------|-------|
 """
         parameters = summarize_job_parameters(self.trans, job)["parameters"]
         for parameter in parameters:
             markdown += "| "
@@ -910,17 +927,21 @@
         elif input_match:
             target_match = input_match
             name = find_non_empty_group(target_match)
             ref_object = invocation.get_input_object(name)
         elif step_match:
             target_match = step_match
             name = find_non_empty_group(target_match)
-            ref_object_type = "job"
             invocation_step = invocation.step_invocation_for_label(name)
-            ref_object = invocation_step and invocation_step.job
+            if invocation_step and invocation_step.job:
+                ref_object_type = "job"
+                ref_object = invocation_step.job
+            elif invocation_step and invocation_step.implicit_collection_jobs:
+                ref_object_type = "implicit_collection_jobs"
+                ref_object = invocation_step.implicit_collection_jobs
         else:
             target_match = None
             ref_object = None
         if ref_object:
             assert target_match  # tell type system, this is set when ref_object is set
             if ref_object_type is None:
                 if ref_object.history_content_type == "dataset":
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/metrics.py` & `galaxy-app-24.0.0/galaxy/managers/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         title="Namespace",
         description="Label indicating the source of the metric.",
     )
     time: str = Field(
         ...,  # Required
         title="Timestamp",
         description="The timestamp in ISO format.",
-        example=SOME_EXAMPLE_DATE,
+        examples=[SOME_EXAMPLE_DATE],
     )
     level: int = Field(
         ...,  # Required
         title="Level",
         description="An integer representing the metric's log level.",
     )
     args: str = Field(
@@ -45,15 +45,17 @@
     )
 
 
 class CreateMetricsPayload(BaseModel):
     metrics: List[Metric] = Field(
         default=[],
         title="List of metrics to be recorded.",
-        example=[Metric(namespace="test-source", time=SOME_EXAMPLE_DATE, level=0, args='{"test":"value"}')],
+        examples=[
+            Metric(namespace="test-source", time=SOME_EXAMPLE_DATE, level=0, args='{"test":"value"}').model_dump()
+        ],
     )
 
 
 TimeSeriesTuple = Tuple[str, datetime, Any]
 TimeSeriesTupleGenerator = Generator[TimeSeriesTuple, None, None]
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/model_stores.py` & `galaxy-app-24.0.0/galaxy/managers/model_stores.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,20 +35,20 @@
     GenerateInvocationDownload,
     ImportModelStoreTaskRequest,
     SetupHistoryExportJob,
     WriteHistoryContentTo,
     WriteHistoryTo,
     WriteInvocationTo,
 )
-from galaxy.structured_app import MinimalManagerApp
-from galaxy.version import VERSION
-from galaxy.web.short_term_storage import (
+from galaxy.short_term_storage import (
     ShortTermStorageMonitor,
     storage_context,
 )
+from galaxy.structured_app import MinimalManagerApp
+from galaxy.version import VERSION
 
 
 class ModelStoreUserContext(ProvidesUserContext):
     def __init__(self, app: MinimalManagerApp, user: model.User) -> None:
         self._app = app
         self._user = user
 
@@ -229,15 +229,15 @@
             raise
 
     def set_history_export_request_metadata(
         self, request: Union[WriteHistoryTo, GenerateHistoryDownload]
     ) -> Optional[ExportObjectMetadata]:
         if request.export_association_id is None:
             return None
-        request_dict = request.dict()
+        request_dict = request.model_dump()
         request_payload = (
             WriteStoreToPayload(**request_dict)
             if isinstance(request, WriteHistoryTo)
             else ShortTermStoreExportPayload(**request_dict)
         )
         export_metadata = ExportObjectMetadata(
             request_data=ExportObjectRequestMetadata(
@@ -261,16 +261,15 @@
             export_metadata.result_data = ExportObjectResultMetadata(success=success, error=error)
             self._export_tracker.set_export_association_metadata(export_association_id, export_metadata)
 
     def import_model_store(self, request: ImportModelStoreTaskRequest):
         import_options = ImportOptions(
             allow_library_creation=request.for_library,
         )
-        history_id = request.history_id
-        if history_id:
+        if history_id := request.history_id:
             history = self._sa_session.get(model.History, history_id)
         else:
             history = None
         user_context = self._build_user_context(request.user.user_id)
         model_import_store = source_to_import_store(
             request.source_uri,
             self._app,
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/notification.py` & `galaxy-app-24.0.0/galaxy/managers/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
             )
         )
         result = self.sa_session.execute(stmt).scalar()
         return result
 
     def get_broadcasted_notification(self, notification_id: int, active_only: Optional[bool] = True):
         stmt = (
-            select(self.broadcast_notification_columns)
+            select(*self.broadcast_notification_columns)
             .select_from(Notification)
             .where(
                 and_(
                     Notification.id == notification_id,
                     Notification.category == MandatoryNotificationCategory.broadcast,
                 )
             )
@@ -319,25 +319,25 @@
         return CleanupResultSummary(deleted_notifications_count, deleted_associations_count)
 
     def _create_notification_model(self, payload: NotificationCreateData):
         notification = Notification(
             payload.source,
             payload.category,
             payload.variant,
-            payload.content.dict(),
+            payload.content.model_dump(),
         )
         notification.publication_time = payload.publication_time
         notification.expiration_time = payload.expiration_time
         return notification
 
     def _user_notifications_query(
         self, user: User, since: Optional[datetime] = None, active_only: Optional[bool] = True
     ):
         stmt = (
-            select(self.user_notification_columns)
+            select(*self.user_notification_columns)
             .select_from(Notification)
             .join(
                 UserNotificationAssociation,
                 UserNotificationAssociation.notification_id == Notification.id,
             )
             .where(UserNotificationAssociation.user_id == user.id)
         )
@@ -352,15 +352,15 @@
             stmt = stmt.where(self._notification_is_active)
             stmt = stmt.where(UserNotificationAssociation.deleted == false())
 
         return stmt
 
     def _broadcasted_notifications_query(self, since: Optional[datetime] = None, active_only: Optional[bool] = True):
         stmt = (
-            select(self.broadcast_notification_columns)
+            select(*self.broadcast_notification_columns)
             .select_from(Notification)
             .where(Notification.category == MandatoryNotificationCategory.broadcast)
         )
         if since is not None:
             stmt = stmt.where(
                 or_(
                     Notification.update_time >= since,
@@ -405,15 +405,15 @@
             set(recipients.group_ids), set(recipients.role_ids)
         )
 
         user_ids_from_groups_stmt = self._get_all_user_ids_from_groups_query(all_group_ids)
         user_ids_from_roles_stmt = self._get_all_user_ids_from_roles_query(all_role_ids)
 
         union_stmt = union(user_ids_from_groups_stmt, user_ids_from_roles_stmt)
-        user_ids_from_groups_and_roles = set([id for id, in self.sa_session.execute(union_stmt)])
+        user_ids_from_groups_and_roles = {id for id, in self.sa_session.execute(union_stmt)}
         unique_user_ids.update(user_ids_from_groups_and_roles)
 
         stmt = select(User).where(User.id.in_(unique_user_ids))
         return self.sa_session.scalars(stmt).all()
 
     def _get_all_user_ids_from_roles_query(self, role_ids: Set[int]) -> Select:
         stmt = (
@@ -444,25 +444,25 @@
             # Get group IDs associated with any of the given role IDs
             stmt = (
                 select(GroupRoleAssociation.group_id)
                 .select_from(GroupRoleAssociation)
                 .where(GroupRoleAssociation.role_id.in_(role_ids))
                 .distinct()
             )
-            group_ids_from_roles = set([id for id, in self.sa_session.execute(stmt) if id is not None])
+            group_ids_from_roles = {id for id, in self.sa_session.execute(stmt) if id is not None}
             new_group_ids = group_ids_from_roles - processed_group_ids
 
             # Get role IDs associated with any of the given group IDs
             stmt = (
                 select(GroupRoleAssociation.role_id)
                 .select_from(GroupRoleAssociation)
                 .where(GroupRoleAssociation.group_id.in_(group_ids))
                 .distinct()
             )
-            role_ids_from_groups = set([id for id, in self.sa_session.execute(stmt) if id is not None])
+            role_ids_from_groups = {id for id, in self.sa_session.execute(stmt) if id is not None}
             new_role_ids = role_ids_from_groups - processed_role_ids
 
             # Stop if there are no new group or role IDs to process
             if not new_group_ids and not new_role_ids:
                 break
 
             # Add new group and role IDs to the respective sets
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/pages.py` & `galaxy-app-24.0.0/galaxy/managers/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Manager and Serializers for Pages.
 
 Pages are markup created and saved by users that can contain Galaxy objects
 (such as datasets) and are often used to describe or present an analysis
 from within Galaxy.
 """
+
 import logging
 import re
 from html.entities import name2codepoint
 from html.parser import HTMLParser
 from typing import (
     Callable,
     Tuple,
@@ -138,44 +139,42 @@
         super().__init__(app)
         self.workflow_manager = app.workflow_manager
 
     def index_query(
         self, trans: ProvidesUserContext, payload: PageIndexQueryPayload, include_total_count: bool = False
     ) -> Tuple[sqlalchemy.engine.Result, int]:
         show_deleted = payload.deleted
+        show_own = payload.show_own
+        show_published = payload.show_published
         show_shared = payload.show_shared
         is_admin = trans.user_is_admin
         user = trans.user
 
-        if show_shared is None:
-            show_shared = not show_deleted
-
-        if show_shared and show_deleted:
+        if show_shared and show_deleted and not is_admin:
             message = "show_shared and show_deleted cannot both be specified as true"
             raise exceptions.RequestParameterInvalidException(message)
 
-        stmt = select(Page)
+        if not user and not show_published:
+            message = "Requires user to log in."
+            raise exceptions.RequestParameterInvalidException(message)
+
+        stmt = select(self.model_class)
 
-        if not is_admin:
-            filters = [Page.user == trans.user]
-            if payload.show_published:
-                filters.append(Page.published == true())
-            if user and show_shared:
-                filters.append(PageUserShareAssociation.user == user)
-                stmt = stmt.outerjoin(Page.users_shared_with)
-            stmt = stmt.where(or_(*filters))
-
-        if not show_deleted:
-            stmt = stmt.where(Page.deleted == false())
-        elif not is_admin:
-            # don't let non-admins see other user's deleted pages
-            stmt = stmt.where(or_(Page.deleted == false(), Page.user == user))
+        filters = []
+        if show_own or (not show_published and not show_shared and not is_admin):
+            filters = [self.model_class.user == user]
+        if show_published:
+            filters.append(self.model_class.published == true())
+        if user and show_shared:
+            filters.append(self.user_share_model.user == user)
+            stmt = stmt.outerjoin(self.model_class.users_shared_with)
+        stmt = stmt.where(or_(*filters))
 
         if payload.user_id:
-            stmt = stmt.where(Page.user_id == payload.user_id)
+            stmt = stmt.where(self.model_class.user_id == payload.user_id)
 
         if payload.search:
             search_query = payload.search
             parsed_search = parse_filters_structured(search_query, INDEX_SEARCH_FILTERS)
 
             def p_tag_filter(term_text: str, quoted: bool):
                 nonlocal stmt
@@ -193,14 +192,16 @@
                     elif key == "title":
                         stmt = stmt.where(text_column_filter(Page.title, term))
                     elif key == "slug":
                         stmt = stmt.where(text_column_filter(Page.slug, term))
                     elif key == "user":
                         stmt = append_user_filter(stmt, Page, term)
                     elif key == "is":
+                        if q == "deleted":
+                            show_deleted = True
                         if q == "published":
                             stmt = stmt.where(Page.published == true())
                         if q == "importable":
                             stmt = stmt.where(Page.importable == true())
                         elif q == "shared_with_me":
                             if not show_shared:
                                 message = "Can only use tag is:shared_with_me if show_shared parameter also true."
@@ -217,14 +218,20 @@
                                 Page.slug,
                                 tf,
                                 alias.username,
                             ],
                             term,
                         )
                     )
+
+        if (show_published or show_shared) and not is_admin:
+            show_deleted = False
+
+        stmt = stmt.where(self.model_class.deleted == (true() if show_deleted else false())).distinct()
+
         if include_total_count:
             total_matches = get_count(trans.sa_session, stmt)
         else:
             total_matches = None
         sort_column = getattr(Page, payload.sort_by)
         if payload.sort_desc:
             sort_column = sort_column.desc()
@@ -259,16 +266,15 @@
             content_format = payload.content_format
         content = self.rewrite_content_for_import(trans, content, content_format)
 
         # Create the new stored page
         page = trans.app.model.Page()
         page.title = payload.title
         page.slug = payload.slug
-        page_annotation = payload.annotation
-        if page_annotation is not None:
+        if (page_annotation := payload.annotation) is not None:
             page_annotation = sanitize_html(page_annotation)
             self.add_item_annotation(trans.sa_session, trans.get_user(), page, page_annotation)
 
         page.user = user
         # And the first (empty) page revision
         page_revision = trans.app.model.PageRevision()
         page_revision.title = payload.title
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/quotas.py` & `galaxy-app-24.0.0/galaxy/managers/quotas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Manager and Serializers for Quotas.
 
 For more information about quotas: https://galaxyproject.org/admin/disk-quotas/
 """
+
 import logging
 from typing import (
     cast,
     Optional,
     Tuple,
     Union,
 )
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/ratable.py` & `galaxy-app-24.0.0/galaxy/managers/ratable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Mixins for Ratable model managers and serializers.
 """
+
 import logging
 from typing import Type
 
 from sqlalchemy import select
 from sqlalchemy.sql.expression import func
 
 from galaxy.model import ItemRatingAssociation
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/rbac_secured.py` & `galaxy-app-24.0.0/galaxy/managers/rbac_secured.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,16 +211,15 @@
 
     def _user_private_role(self, user):
         # error with 401 if no user
         self.user_manager.error_if_anonymous(user)
         return self.user_manager.private_role(user)
 
     def _grant_role(self, dataset, role, flush=True):
-        existing = self.by_role(dataset, role)
-        if existing:
+        if existing := self.by_role(dataset, role):
             return existing
         return self._create(dataset, role, flush=flush)
 
     def _revoke_role(self, dataset, role, flush=True):
         permission = self.by_roles(dataset, [role])
         return self._delete([permission], flush=flush)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/remote_files.py` & `galaxy-app-24.0.0/galaxy/managers/remote_files.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/secured.py` & `galaxy-app-24.0.0/galaxy/managers/secured.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Accessible models can be read and copied but not modified or deleted.
 
 Owned models can be modified and deleted.
 """
+
 from typing import (
     Any,
     Optional,
     Type,
     TYPE_CHECKING,
 )
 
@@ -25,16 +26,15 @@
 
     This can also be thought of as 'read but not modify' privileges.
     """
 
     # declare what we are using from base ModelManager
     model_class: Type[Any]
 
-    def by_id(self, id: int):
-        ...
+    def by_id(self, id: int): ...
 
     # don't want to override by_id since consumers will also want to fetch w/o any security checks
     def is_accessible(self, item: "Query", user: model.User, **kwargs: Any) -> bool:
         """
         Return True if the item accessible to user.
         """
         # override in subclasses
@@ -92,16 +92,15 @@
 
     This can also be thought of as write/edit privileges.
     """
 
     # declare what we are using from base ModelManager
     model_class: Type[Any]
 
-    def by_id(self, id: int):
-        ...
+    def by_id(self, id: int): ...
 
     def is_owner(self, item: model.Base, user: Optional[model.User], **kwargs: Any) -> bool:
         """
         Return True if user owns the item.
         """
         # override in subclasses
         raise exceptions.NotImplemented("Abstract interface Method")
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/session.py` & `galaxy-app-24.0.0/galaxy/managers/session.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/sharable.py` & `galaxy-app-24.0.0/galaxy/managers/sharable.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     has an owner/creator User
     is sharable with other, specific Users
     is importable (copyable) by users that have access
     has a slug which can be used as a link to view the resource
     can be published effectively making it available to all other Users
     can be rated
 """
+
 import logging
 import re
 from typing import (
     Any,
     List,
     Optional,
     Set,
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/taggable.py` & `galaxy-app-24.0.0/galaxy/managers/taggable.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/tags.py` & `galaxy-app-24.0.0/galaxy/managers/tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 class TagsManager:
     """Interface/service object shared by controllers for interacting with tags."""
 
     def update(self, trans: ProvidesUserContext, payload: ItemTagsPayload) -> None:
         """Apply a new set of tags to an item; previous tags are deleted."""
         user = trans.user
         new_tags: Optional[str] = None
-        if payload.item_tags and len(payload.item_tags.__root__) > 0:
-            new_tags = ",".join(payload.item_tags.__root__)
+        if payload.item_tags and len(payload.item_tags.root) > 0:
+            new_tags = ",".join(payload.item_tags.root)
         item = self._get_item(trans.tag_handler, payload)
         trans.tag_handler.delete_item_tags(user, item)
         trans.tag_handler.apply_item_tags(user, item, new_tags)
         with transaction(trans.sa_session):
             trans.sa_session.commit()
 
     def _get_item(self, tag_handler: GalaxyTagHandlerSession, payload: ItemTagsPayload):
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/tasks.py` & `galaxy-app-24.0.0/galaxy/managers/tasks.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/tool_data.py` & `galaxy-app-24.0.0/galaxy/managers/tool_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,20 @@
         """Return all tool data tables."""
         return self._app.tool_data_tables.index()
 
     def show(self, table_name: str) -> ToolDataDetails:
         """Get details of a given data table"""
         data_table = self._data_table(table_name)
         element_view = data_table.to_dict(view="element")
-        return ToolDataDetails.construct(**element_view)
+        return ToolDataDetails.model_construct(**element_view)
 
     def show_field(self, table_name: str, field_name: str) -> ToolDataField:
         """Get information about a partiular field in a tool data table"""
         field = self._data_table_field(table_name, field_name)
-        return ToolDataField.construct(**field.to_dict())
+        return ToolDataField.model_construct(**field.to_dict())
 
     def reload(self, table_name: str) -> ToolDataDetails:
         """Reloads a tool data table."""
         data_table = self._data_table(table_name)
         data_table.reload_from_files()
         return self._reload_data_table(table_name)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/tools.py` & `galaxy-app-24.0.0/galaxy/managers/tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/managers/users.py` & `galaxy-app-24.0.0/galaxy/managers/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Manager and Serializer for Users.
 """
+
 import hashlib
 import logging
 import random
 import re
 import string
 import time
 from datetime import datetime
@@ -35,14 +36,15 @@
 from galaxy.config import templates
 from galaxy.managers import (
     base,
     deletable,
 )
 from galaxy.managers.base import combine_lists
 from galaxy.model import (
+    Job,
     User,
     UserAddress,
     UserQuotaUsage,
 )
 from galaxy.model.base import transaction
 from galaxy.security.validate_user_input import (
     VALID_EMAIL_RE,
@@ -52,15 +54,14 @@
     validate_publicname,
 )
 from galaxy.structured_app import (
     BasicSharedApp,
     MinimalManagerApp,
 )
 from galaxy.util.hash_util import new_secure_hash_v2
-from galaxy.web import url_for
 
 log = logging.getLogger(__name__)
 
 PASSWORD_RESET_TEMPLATE = """
 To reset your Galaxy password for the instance at %s use the following link,
 which will expire %s.
 
@@ -157,14 +158,29 @@
     def delete(self, user, flush=True):
         """Mark the given user deleted."""
         if not self.app.config.allow_user_deletion:
             raise exceptions.ConfigDoesNotAllowException(
                 "The configuration of this Galaxy instance does not allow admins to delete users."
             )
         super().delete(user, flush=flush)
+        self._stop_all_jobs_from_user(user)
+
+    def _stop_all_jobs_from_user(self, user):
+        active_jobs = self._get_all_active_jobs_from_user(user)
+        session = self.session()
+        for job in active_jobs:
+            job.mark_deleted(self.app.config.track_jobs_in_database)
+        with transaction(session):
+            session.commit()
+
+    def _get_all_active_jobs_from_user(self, user: User) -> List[Job]:
+        """Get all jobs that are not ready yet and belong to the given user."""
+        stmt = select(Job).where(and_(Job.user_id == user.id, Job.state.in_(Job.non_ready_states)))
+        jobs = self.session().scalars(stmt)
+        return jobs
 
     def undelete(self, user, flush=True):
         """Remove the deleted flag for the given user."""
         if not self.app.config.allow_user_deletion:
             raise exceptions.ConfigDoesNotAllowException(
                 "The configuration of this Galaxy instance does not allow admins to undelete users."
             )
@@ -291,14 +307,21 @@
             raise exceptions.AuthenticationFailed("User account is deactivated, please contact an administrator.")
         sa_session.refresh(provided_key.user)
         newest_key = provided_key.user.api_keys[0]
         if newest_key.key != provided_key.key:
             raise exceptions.AuthenticationFailed("Provided API key has expired.")
         return provided_key.user
 
+    def by_oidc_access_token(self, access_token: str):
+        if hasattr(self.app, "authnz_manager") and self.app.authnz_manager:
+            user = self.app.authnz_manager.match_access_token_to_user(self.app.model.session, access_token)  # type: ignore[attr-defined]
+            return user
+        else:
+            return None
+
     def check_bootstrap_admin_api_key(self, api_key):
         bootstrap_admin_api_key = getattr(self.app.config, "bootstrap_admin_api_key", None)
         if not bootstrap_admin_api_key:
             return False
         # Hash keys to make them the same size, so we can do safe comparison.
         bootstrap_hash = hashlib.sha256(util.smart_str(bootstrap_admin_api_key)).hexdigest()
         provided_hash = hashlib.sha256(util.smart_str(api_key)).hexdigest()
@@ -490,21 +513,33 @@
                 trans.sa_session.add(user)
                 with transaction(trans.sa_session):
                     trans.sa_session.commit()
                 trans.log_event("User change password")
         else:
             return "Failed to determine user, access denied."
 
+    def impersonate(self, trans, user):
+        if not trans.app.config.allow_user_impersonation:
+            raise exceptions.Message("User impersonation is not enabled in this instance of Galaxy.")
+        if user:
+            trans.handle_user_logout()
+            trans.handle_user_login(user)
+        else:
+            raise exceptions.Message("Please provide a valid user.")
+
     def send_activation_email(self, trans, email, username):
         """
         Send the verification email containing the activation link to the user's email.
         """
         activation_token = self.__get_activation_token(trans, email)
-        activation_link = url_for(
-            controller="user", action="activate", activation_token=activation_token, email=escape(email), qualified=True
+        activation_link = trans.url_builder(
+            "/user/activate",
+            activation_token=activation_token,
+            email=escape(email),
+            qualified=True,
         )
         template_context = {
             "name": escape(username),
             "user_email": escape(email),
             "date": datetime.utcnow().strftime("%D"),
             "hostname": trans.request.host,
             "activation_url": activation_link,
@@ -549,15 +584,15 @@
             return "Please provide your email."
         message = validate_email(trans, email, check_dup=False)
         if message:
             return message
         else:
             reset_user, prt = self.get_reset_token(trans, email)
             if prt:
-                reset_url = url_for(controller="login", action="start", token=prt.token)
+                reset_url = trans.url_builder("/login/start", token=prt.token)
                 body = PASSWORD_RESET_TEMPLATE % (
                     trans.app.config.hostname,
                     prt.expiration_time.strftime(trans.app.config.pretty_datetime_format),
                     trans.request.host,
                     reset_url,
                 )
                 subject = "Galaxy Password Reset"
@@ -753,19 +788,20 @@
     update/alter users.
     """
 
     model_manager_class = UserManager
 
     def add_deserializers(self):
         super().add_deserializers()
-        history_deserializers: Dict[str, base.Deserializer] = {
+        user_deserializers: Dict[str, base.Deserializer] = {
+            "active": self.default_deserializer,
             "username": self.deserialize_username,
             "preferred_object_store_id": self.deserialize_preferred_object_store_id,
         }
-        self.deserializers.update(history_deserializers)
+        self.deserializers.update(user_deserializers)
 
     def deserialize_preferred_object_store_id(self, item: Any, key: Any, val: Any, **context):
         preferred_object_store_id = val
         validation_error = validate_preferred_object_store_id(self.app.object_store, preferred_object_store_id)
         if validation_error:
             raise base.ModelDeserializingError(validation_error)
         return self.default_deserializer(item, key, preferred_object_store_id, **context)
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/visualizations.py` & `galaxy-app-24.0.0/galaxy/managers/visualizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Manager and Serializers for Visualizations.
 
 Visualizations are saved configurations/variables used to
 reproduce a specific view in a Galaxy visualization.
 """
+
 import logging
 from typing import (
     Dict,
     List,
     Tuple,
 )
 
@@ -71,31 +72,28 @@
     annotation_assoc = model.VisualizationAnnotationAssociation
     rating_assoc = model.VisualizationRatingAssociation
 
     def index_query(
         self, trans: ProvidesUserContext, payload: VisualizationIndexQueryPayload, include_total_count: bool = False
     ) -> Tuple[List[model.Visualization], int]:
         show_deleted = payload.deleted
-        show_shared = payload.show_shared
-        show_published = payload.show_published
         show_own = payload.show_own
+        show_published = payload.show_published
+        show_shared = payload.show_shared
         is_admin = trans.user_is_admin
         user = trans.user
 
-        if show_shared is None:
-            show_shared = not show_deleted
-
-        if show_shared and show_deleted:
-            message = "show_shared and show_deleted cannot both be specified as true"
+        if not user and not show_published:
+            message = "Requires user to log in."
             raise exceptions.RequestParameterInvalidException(message)
 
         query = trans.sa_session.query(self.model_class)
 
         filters = []
-        if show_own or (not show_published and not is_admin):
+        if show_own or (not show_published and not show_shared and not is_admin):
             filters = [self.model_class.user == user]
         if show_published:
             filters.append(self.model_class.published == true())
         if user and show_shared:
             filters.append(self.user_share_model.user == user)
             query = query.outerjoin(self.model_class.users_shared_with)
         query = query.filter(or_(*filters))
@@ -150,15 +148,18 @@
                                 tf,
                                 alias.username,
                             ],
                             term,
                         )
                     )
 
-        query = query.filter(self.model_class.deleted == (true() if show_deleted else false()))
+        if (show_published or show_shared) and not is_admin:
+            show_deleted = False
+
+        query = query.filter(self.model_class.deleted == (true() if show_deleted else false())).distinct()
 
         if include_total_count:
             total_matches = query.count()
         else:
             total_matches = None
         sort_column = getattr(model.Visualization, payload.sort_by)
         if payload.sort_desc:
```

### Comparing `galaxy-app-23.2.1/galaxy/managers/workflows.py` & `galaxy-app-24.0.0/galaxy/managers/workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,29 +19,34 @@
     ImporterGalaxyInterface,
     ImportOptions,
     python_to_workflow,
 )
 from gxformat2.abstract import from_dict
 from gxformat2.cytoscape import to_cytoscape
 from gxformat2.yaml import ordered_dump
-from pydantic import BaseModel
+from pydantic import (
+    BaseModel,
+    SerializerFunctionWrapHandler,
+    WrapSerializer,
+)
 from sqlalchemy import (
     desc,
     false,
     func,
     or_,
     select,
     true,
 )
 from sqlalchemy.orm import (
     aliased,
     joinedload,
     Query,
     subqueryload,
 )
+from typing_extensions import Annotated
 
 from galaxy import (
     exceptions,
     model,
     util,
 )
 from galaxy.job_execution.actions.post import ActionBox
@@ -60,16 +65,20 @@
     StoredWorkflow,
     StoredWorkflowTagAssociation,
     StoredWorkflowUserShareAssociation,
     User,
     Workflow,
     WorkflowInvocation,
     WorkflowInvocationStep,
+    WorkflowInvocationToSubworkflowInvocationAssociation,
+)
+from galaxy.model.base import (
+    ensure_object_added_to_session,
+    transaction,
 )
-from galaxy.model.base import transaction
 from galaxy.model.index_filter_util import (
     append_user_filter,
     raw_text_column_filter,
     tag_filter,
     text_column_filter,
 )
 from galaxy.model.item_attrs import UsesAnnotations
@@ -77,31 +86,31 @@
 from galaxy.schema.schema import WorkflowIndexQueryPayload
 from galaxy.structured_app import MinimalManagerApp
 from galaxy.tools.parameters import (
     params_to_incoming,
     visit_input_values,
 )
 from galaxy.tools.parameters.basic import (
+    ConnectedValue,
     DataCollectionToolParameter,
     DataToolParameter,
     RuntimeValue,
-    workflow_building_modes,
 )
+from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
 from galaxy.util.hash_util import md5_hash_str
 from galaxy.util.json import (
     safe_dumps,
     safe_loads,
 )
 from galaxy.util.sanitize_html import sanitize_html
 from galaxy.util.search import (
     FilteredTerm,
     parse_filters_structured,
     RawTextTerm,
 )
-from galaxy.web import url_for
 from galaxy.work.context import WorkRequestContext
 from galaxy.workflow.modules import (
     module_factory,
     ToolModule,
     WorkflowModule,
     WorkflowModuleInjector,
 )
@@ -180,15 +189,15 @@
         stmt = select(StoredWorkflow)
         if show_shared:
             stmt = stmt.outerjoin(StoredWorkflow.users_shared_with)
         stmt = stmt.outerjoin(StoredWorkflow.tags)
 
         latest_workflow_load = joinedload(StoredWorkflow.latest_workflow)
         if not payload.skip_step_counts:
-            latest_workflow_load = latest_workflow_load.undefer("step_count")
+            latest_workflow_load = latest_workflow_load.undefer(Workflow.step_count)
         latest_workflow_load = latest_workflow_load.lazyload(Workflow.steps)
 
         stmt = stmt.options(joinedload(StoredWorkflow.annotations))
         stmt = stmt.options(latest_workflow_load)
         stmt = stmt.where(or_(*filters))
         stmt = stmt.where(StoredWorkflow.hidden == (true() if show_hidden else false()))
         if payload.search:
@@ -390,15 +399,15 @@
                 module_name,
                 module_data_inputs,
                 module_data_outputs,
             )
         workflow_canvas.add_steps()
         return workflow_canvas.finish(for_embed=for_embed)
 
-    def get_invocation(self, trans, decoded_invocation_id, eager=False) -> WorkflowInvocation:
+    def get_invocation(self, trans, decoded_invocation_id: int, eager=False) -> WorkflowInvocation:
         workflow_invocation = _get_invocation(trans.sa_session, eager, decoded_invocation_id)
         if not workflow_invocation:
             encoded_wfi_id = trans.security.encode_id(decoded_invocation_id)
             message = f"'{encoded_wfi_id}' is not a valid workflow invocation id"
             raise exceptions.ObjectNotFound(message)
         self.check_security(trans, workflow_invocation, check_ownership=True, check_accessible=False)
         return workflow_invocation
@@ -475,14 +484,15 @@
         job_id=None,
         user_id=None,
         include_terminal=True,
         limit=None,
         offset=None,
         sort_by=None,
         sort_desc=None,
+        include_nested_invocations=True,
     ) -> Tuple[Query, int]:
         """Get invocations owned by the current user."""
 
         stmt = select(WorkflowInvocation)
         if stored_workflow_id is not None:
             stored_workflow = trans.sa_session.get(StoredWorkflow, stored_workflow_id)
             if not stored_workflow:
@@ -492,14 +502,24 @@
             stmt = stmt.join(History).where(History.user_id == user_id)
         if history_id is not None:
             stmt = stmt.where(WorkflowInvocation.history_id == history_id)
         if job_id is not None:
             stmt = stmt.join(WorkflowInvocationStep).where(WorkflowInvocationStep.job_id == job_id)
         if not include_terminal:
             stmt = stmt.where(WorkflowInvocation.state.in_(WorkflowInvocation.non_terminal_states))
+        if not include_nested_invocations:
+            subquery = (
+                select(WorkflowInvocationToSubworkflowInvocationAssociation.id)
+                .where(
+                    WorkflowInvocationToSubworkflowInvocationAssociation.subworkflow_invocation_id
+                    == WorkflowInvocation.id
+                )
+                .exists()
+            )
+            stmt = stmt.where(~subquery)
 
         total_matches = get_count(trans.sa_session, stmt)
 
         if sort_by:
             sort_column = getattr(WorkflowInvocation, sort_by)
             if sort_desc:
                 sort_column = sort_column.desc()
@@ -780,17 +800,16 @@
         # Create each step
         steps: List[model.WorkflowStep] = []
         # The editor will provide ids for each step that we don't need to save,
         # but do need to use to make connections
         steps_by_external_id: Dict[str, model.WorkflowStep] = {}
 
         # Preload dependent workflows with locally defined content_ids.
-        subworkflows = data.get("subworkflows")
         subworkflow_id_map = None
-        if subworkflows:
+        if subworkflows := data.get("subworkflows"):
             subworkflow_id_map = {}
             for key, subworkflow_dict in subworkflows.items():
                 subworkflow = self.__build_embedded_subworkflow(
                     trans, subworkflow_dict, workflow_state_resolution_options
                 )
                 subworkflow_id_map[key] = subworkflow
 
@@ -800,15 +819,15 @@
         missing_tool_tups = []
         for step_dict in self.__walk_step_dicts(data):
             if not dry_run:
                 self.__load_subworkflows(
                     trans, step_dict, subworkflow_id_map, workflow_state_resolution_options, dry_run=dry_run
                 )
 
-        module_kwds = workflow_state_resolution_options.dict()
+        module_kwds = workflow_state_resolution_options.model_dump()
         module_kwds.update(kwds)  # TODO: maybe drop this?
         for step_dict in self.__walk_step_dicts(data):
             module, step = self.__module_from_dict(trans, steps, steps_by_external_id, step_dict, **module_kwds)
             if isinstance(module, ToolModule) and module.tool is None:
                 missing_tool_tup = (module.tool_id, module.get_name(), module.tool_version, step_dict["id"])
                 if missing_tool_tup not in missing_tool_tups:
                     missing_tool_tups.append(missing_tool_tup)
@@ -816,14 +835,19 @@
                 workflow.has_errors = True
 
         # Second pass to deal with connections between steps
         self.__connect_workflow_steps(steps, steps_by_external_id, dry_run)
 
         workflow.has_cycles = True
         workflow.steps = steps
+        # Safeguard: workflow was implicitly merged into this Session prior to SQLAlchemy 2.0.
+        # when AT LEAST ONE step in steps belonged to a session.
+        for step in steps:
+            if ensure_object_added_to_session(workflow, object_in_session=step):
+                break
 
         comments: List[model.WorkflowComment] = []
         comments_by_external_id: Dict[str, model.WorkflowComment] = {}
         for comment_dict in data.get("comments", []):
             comment = model.WorkflowComment.from_dict(comment_dict)
             comments.append(comment)
             external_id = comment_dict.get("id")
@@ -870,17 +894,17 @@
             version = int(version)
         workflow = stored.get_internal_version(version)
         if style == "export":
             style = self.app.config.default_workflow_export_format
         if style == "editor":
             wf_dict = self._workflow_to_dict_editor(trans, stored, workflow)
         elif style == "legacy":
-            wf_dict = self._workflow_to_dict_instance(stored, workflow=workflow, legacy=True)
+            wf_dict = self._workflow_to_dict_instance(trans, stored, workflow=workflow, legacy=True)
         elif style == "instance":
-            wf_dict = self._workflow_to_dict_instance(stored, workflow=workflow, legacy=False)
+            wf_dict = self._workflow_to_dict_instance(trans, stored, workflow=workflow, legacy=False)
         elif style == "run":
             wf_dict = self._workflow_to_dict_run(trans, stored, workflow=workflow, history=history or trans.history)
         elif style == "preview":
             wf_dict = self._workflow_to_dict_preview(trans, workflow=workflow)
         elif style == "format2":
             wf_dict = self._workflow_to_dict_export(trans, stored, workflow=workflow)
             wf_dict = to_format_2(wf_dict)
@@ -1119,24 +1143,27 @@
 
         module_injector = WorkflowModuleInjector(trans)
         module_injector.inject_all(workflow, ignore_tool_missing_exception=True, exact_tools=False)
         step_dicts = []
         for step in workflow.steps:
             step_dict = {}
             step_dict["order_index"] = step.order_index
+            step_dict["type"] = step.type
             if step.annotations:
                 step_dict["annotation"] = step.annotations[0].annotation
             try:
                 module_injector.compute_runtime_state(step)
             except exceptions.ToolMissingException as e:
                 step_dict["label"] = f"Unknown Tool with id '{e.tool_id}'"
                 step_dicts.append(step_dict)
                 continue
             if step.type == "tool":
                 tool = trans.app.toolbox.get_tool(step.tool_id, step.tool_version)
+                step_dict["tool_id"] = step.tool_id
+                step_dict["tool_version"] = step.tool_version
                 step_dict["label"] = step.label or tool.name
                 step_dict["inputs"] = do_inputs(tool.inputs, step.state.inputs, "", step)
             elif step.type == "subworkflow":
                 step_dict["label"] = step.label or (step.subworkflow.name if step.subworkflow else "Missing workflow.")
                 errors = step.module.get_errors()
                 if errors:
                     step_dict["errors"] = errors
@@ -1202,15 +1229,15 @@
                 "annotation": annotation_str,
                 "post_job_actions": module.get_post_job_actions({}),
                 "uuid": str(step.uuid) if step.uuid else None,
                 "when": step.when_expression,
                 "workflow_outputs": [],
             }
             if tooltip:
-                step_dict["tooltip"] = module.get_tooltip(static_path=url_for("/static"))
+                step_dict["tooltip"] = module.get_tooltip(static_path="/static")
             # Connections
             input_connections = step.input_connections
             input_connections_type = {}
             multiple_input = {}  # Boolean value indicating if this can be multiple
             if isinstance(module, ToolModule) and module.tool:
                 # Serialize tool version
                 step_dict["tool_version"] = module.tool.version
@@ -1249,17 +1276,17 @@
                             if output_label not in output_label_duplicate:
                                 output_label_duplicate.add(output_label)
                         else:
                             output_label_index.add(output_label)
             step_dict["workflow_outputs"] = outputs
             if len(output_label_duplicate) > 0:
                 output_label_duplicate_string = ", ".join(output_label_duplicate)
-                upgrade_message_dict[
-                    "output_label_duplicate"
-                ] = f"Ignoring duplicate labels: {output_label_duplicate_string}."
+                upgrade_message_dict["output_label_duplicate"] = (
+                    f"Ignoring duplicate labels: {output_label_duplicate_string}."
+                )
             if upgrade_message_dict:
                 data["upgrade_messages"][step.order_index] = upgrade_message_dict
 
             # Encode input connections as dictionary
             input_conn_dict: model.InputConnDictType = {}
             for conn in input_connections:
                 input_type = "dataset"
@@ -1490,20 +1517,20 @@
             input_dicts = []
             step_state = module.state.inputs or {}
             if module.type != "tool":
                 name = step_state.get("name") or module.label
                 if name:
                     input_dicts.append({"name": name, "description": annotation_str})
             for name, val in step_state.items():
-                if isinstance(val, RuntimeValue):
+                if isinstance(val, RuntimeValue) and not isinstance(val, ConnectedValue):
                     input_dicts.append({"name": name, "description": f"runtime parameter for tool {module.get_name()}"})
                 elif isinstance(val, dict):
                     # Input type is described by a dict, e.g. indexed parameters.
                     for partval in val.values():
-                        if isinstance(partval, RuntimeValue):
+                        if isinstance(partval, RuntimeValue) and not isinstance(val, ConnectedValue):
                             input_dicts.append(
                                 {"name": name, "description": f"runtime parameter for tool {module.get_name()}"}
                             )
             step_dict["inputs"] = input_dicts
 
             # User outputs
             workflow_outputs_dicts = []
@@ -1581,20 +1608,20 @@
             step_dict["input_connections"] = back_compat_input_conn_dict
             # Position
             step_dict["position"] = step.position
             # Add to return value
             steps[step.order_index] = step_dict
         return data
 
-    def _workflow_to_dict_instance(self, stored, workflow, legacy=True):
+    def _workflow_to_dict_instance(self, trans, stored, workflow, legacy=True):
         encode = self.app.security.encode_id
         sa_session = self.app.model.context
-        item = stored.to_dict(view="element", value_mapper={"id": encode})
+        item = stored.to_dict(view="element")
         item["name"] = workflow.name
-        item["url"] = url_for("workflow", id=item["id"])
+        item["url"] = trans.url_builder("workflow", id=encode(stored.id))
         item["owner"] = stored.user.username
         item["email_hash"] = md5_hash_str(stored.user.email)
         item["slug"] = stored.slug
         inputs = {}
         for step in workflow.input_steps:
             step_type = step.type
             step_label = step.label or step.tool_inputs.get("name")
@@ -1637,15 +1664,15 @@
                 "when": step.when_expression,
             }
 
             if step_type == "subworkflow":
                 del step_dict["tool_id"]
                 del step_dict["tool_version"]
                 del step_dict["tool_inputs"]
-                step_dict["workflow_id"] = encode(step.subworkflow.id)
+                step_dict["workflow_id"] = step.subworkflow.id
 
             for conn in step.input_connections:
                 step_id = step.id if legacy else step.order_index
                 source_id = conn.output_step_id
                 source_step = source_id if legacy else steps_to_order_index[source_id]
                 step_dict["input_steps"][conn.input_name] = {
                     "source_step": source_step,
@@ -1745,16 +1772,15 @@
         if "label" in step_dict:
             step.label = step_dict["label"]
 
         module = module_factory.from_dict(trans, step_dict, detached=dry_run, **kwds)
         self.__set_default_label(step, module, step_dict.get("tool_state"))
         module.save_to_step(step, detached=dry_run)
 
-        annotation = step_dict.get("annotation")
-        if annotation:
+        if annotation := step_dict.get("annotation"):
             annotation = sanitize_html(annotation)
             sa_session = None if dry_run else trans.sa_session
             self.add_item_annotation(sa_session, trans.get_user(), step, annotation)
 
         # Stick this in the step temporarily
         DictConnection = Dict[str, Union[int, str]]
         temp_input_connections: Dict[str, Union[List[DictConnection], DictConnection]] = step_dict.get(
@@ -1946,24 +1972,26 @@
         return tools
 
 
 class RefactorRequest(RefactorActions):
     style: str = "export"
 
 
+def safe_wraps(v: Any, nxt: SerializerFunctionWrapHandler) -> str:
+    try:
+        return nxt(v)
+    except Exception:
+        return safe_dumps(v)
+
+
 class RefactorResponse(BaseModel):
     action_executions: List[RefactorActionExecution]
-    workflow: dict
+    workflow: Annotated[dict, WrapSerializer(safe_wraps, when_used="json")]
     dry_run: bool
 
-    class Config:
-        # Workflows have dictionaries with integer keys, which pydantic doesn't coerce to strings.
-        # Integer object keys aren't valid JSON, so the client fails.
-        json_dumps = safe_dumps
-
 
 class WorkflowStateResolutionOptions(BaseModel):
     # fill in default tool state when updating, may change tool_state
     fill_defaults: bool = False
     # If True, assume all tool state coming from generated form instead of potentially simpler json stored in DB/exported
     from_tool_form: bool = False
     # If False, allow running with less exact tool versions
@@ -2072,9 +2100,9 @@
             .joinedload(Job.input_datasets)
         )
     stmt = stmt.where(WorkflowInvocation.id == invocation_id).limit(1)
     return session.scalars(stmt).first()
 
 
 def get_count(session, statement):
-    stmt = select(func.count()).select_from(statement)
+    stmt = select(func.count()).select_from(statement.subquery())
     return session.scalar(stmt)
```

### Comparing `galaxy-app-23.2.1/galaxy/queue_worker.py` & `galaxy-app-24.0.0/galaxy/queue_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,17 +212,16 @@
 
 def reload_sanitize_allowlist(app):
     log.debug("Executing reload sanitize allowlist control task.")
     app.config.reload_sanitize_allowlist()
 
 
 def recalculate_user_disk_usage(app, **kwargs):
-    user_id = kwargs.get("user_id", None)
     sa_session = app.model.context
-    if user_id:
+    if user_id := kwargs.get("user_id", None):
         user = sa_session.get(User, user_id)
         if user:
             user.calculate_and_set_disk_usage(app.object_store)
         else:
             log.error(f"Recalculate user disk usage task failed, user {user_id} not found")
     else:
         log.error("Recalculate user disk usage task received without user_id.")
```

### Comparing `galaxy-app-23.2.1/galaxy/queues.py` & `galaxy-app-24.0.0/galaxy/queues.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 
 All message queues used by Galaxy
 
 """
+
 import socket
 from typing import Optional
 
 from kombu import (
     Connection,
     Exchange,
     Queue,
```

### Comparing `galaxy-app-23.2.1/galaxy/structured_app.py` & `galaxy-app-24.0.0/galaxy/structured_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Typed description of Galaxy's app object."""
+
 import abc
 from typing import (
     Any,
     Optional,
     TYPE_CHECKING,
 )
 
@@ -91,14 +92,15 @@
 class MinimalApp(BasicSharedApp):
     is_webapp: bool  # is_webapp will be set to true when building WSGI app
     tag_handler: GalaxyTagHandler
     model: GalaxyModelMapping
     install_model: ModelMapping
     security_agent: GalaxyRBACAgent
     host_security_agent: HostAgent
+    server_starttime: int
 
 
 class MinimalManagerApp(MinimalApp):
     # Minimal App that is sufficient to run Celery tasks
     file_sources: ConfiguredFileSources
     genome_builds: GenomeBuilds
     dataset_collection_manager: "DatasetCollectionManager"
@@ -120,19 +122,17 @@
     error_reports: "ErrorReports"
     notification_manager: Any  # 'galaxy.managers.notification.NotificationManager'
     object_store: BaseObjectStore
     tool_shed_registry: ToolShedRegistry
 
     @property
     @abc.abstractmethod
-    def is_job_handler(self) -> bool:
-        ...
+    def is_job_handler(self) -> bool: ...
 
-    def wait_for_toolbox_reload(self, old_toolbox: "ToolBox") -> None:
-        ...
+    def wait_for_toolbox_reload(self, old_toolbox: "ToolBox") -> None: ...
 
 
 class StructuredApp(MinimalManagerApp):
     """Interface defining typed description of the Galaxy UniverseApplication.
 
     Ideally nothing that depends on StructuredApp should require
     StructuredApp so we can have a clean import dag. This will
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/cache.py` & `galaxy-app-24.0.0/galaxy/tool_shed/cache.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/client.py` & `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,36 +26,30 @@
     import galaxy.tool_shed.metadata.installed_repository_manger
 
 
 class DataManagerInterface(Protocol):
     GUID_TYPE: str = "data_manager"
     DEFAULT_VERSION: str = "0.0.1"
 
-    def process_result(self, out_data):
-        ...
+    def process_result(self, out_data): ...
 
-    def write_bundle(self, out: Dict[str, OutputDataset]) -> Dict[str, OutputDataset]:
-        ...
+    def write_bundle(self, out: Dict[str, OutputDataset]) -> Dict[str, OutputDataset]: ...
 
 
 class DataManagersInterface(Protocol):
     @property
-    def _reload_count(self) -> int:
-        ...
+    def _reload_count(self) -> int: ...
 
     def load_manager_from_elem(
         self, data_manager_elem, tool_path=None, add_manager=True
-    ) -> Optional[DataManagerInterface]:
-        ...
+    ) -> Optional[DataManagerInterface]: ...
 
-    def get_manager(self, data_manager_id: str) -> Optional[DataManagerInterface]:
-        ...
+    def get_manager(self, data_manager_id: str) -> Optional[DataManagerInterface]: ...
 
-    def remove_manager(self, manager_ids: Union[str, List[str]]) -> None:
-        ...
+    def remove_manager(self, manager_ids: Union[str, List[str]]) -> None: ...
 
 
 ToolBoxType = TypeVar("ToolBoxType", bound="AbstractToolBox")
 
 
 class InstallationTarget(HasToolBox, Generic[ToolBoxType]):
     data_managers: DataManagersInterface
@@ -65,9 +59,8 @@
     config: Any
     installed_repository_manager: "galaxy.tool_shed.metadata.installed_repository_manger.InstalledRepositoryManager"
     watchers: Any  # TODO: interface...
     _toolbox_lock: threading.RLock
     tool_shed_repository_cache: Optional[ToolShedRepositoryCache]
     tool_data_tables: ToolDataTableManager
 
-    def wait_for_toolbox_reload(self, old_toolbox: ToolBoxType) -> None:
-        ...
+    def wait_for_toolbox_reload(self, old_toolbox: ToolBoxType) -> None: ...
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/install_manager.py` & `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/install_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/installed_repository_manager.py` & `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/installed_repository_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Class encapsulating the management of repositories installed into Galaxy from the Tool Shed.
 """
+
 import copy
 import logging
 import os
 import shutil
 from typing import (
     Any,
     Dict,
@@ -166,17 +167,17 @@
         # Add an entry to self.installed_repository_dependencies_of_installed_repositories.
         if repository_tup not in self.installed_repository_dependencies_of_installed_repositories:
             debug_msg = (
                 f"Adding an entry for revision {installed_changeset_revision} of repository {name} owned by {owner} "
             )
             debug_msg += "to installed_repository_dependencies_of_installed_repositories."
             log.debug(debug_msg)
-            self.installed_repository_dependencies_of_installed_repositories[
-                repository_tup
-            ] = repository_dependency_tups
+            self.installed_repository_dependencies_of_installed_repositories[repository_tup] = (
+                repository_dependency_tups
+            )
         # Use the repository_dependency_tups to add entries to the reverse dictionary
         # self.installed_dependent_repositories_of_installed_repositories.
         for required_repository_tup in repository_dependency_tups:
             debug_msg = f"Appending revision {installed_changeset_revision} of repository {name} owned by {owner} "
             debug_msg += "to all dependent repositories in installed_dependent_repositories_of_installed_repositories."
             log.debug(debug_msg)
             if required_repository_tup in self.installed_dependent_repositories_of_installed_repositories:
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/metadata/installed_repository_metadata_manager.py` & `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/metadata/installed_repository_metadata_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,18 +148,17 @@
             )
 
     def reset_metadata_on_selected_repositories(self, user, **kwd):
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
                     repository = get_installed_tool_shed_repository(self.app, repository_id)
                     self.set_repository(repository)
                     self.reset_all_metadata_on_installed_repository()
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/repository_dependencies/repository_dependency_manager.py` & `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/repository_dependencies/repository_dependency_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Class encapsulating the management of repository dependencies installed or being installed
 into Galaxy from the Tool Shed.
 """
+
 import json
 import logging
 import os
 from urllib.error import HTTPError
 from urllib.parse import (
     urlencode,
     urlparse,
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/tools/data_manager.py` & `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/data_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,15 @@
         return None
 
     def _data_manager_config_elems_to_xml_file(self, config_elems: List[Element], config_filename: StrPath) -> None:
         """
         Persist the current in-memory list of config_elems to a file named by the value
         of config_filename.
         """
-        data_managers_path = self.data_managers_path
-        if data_managers_path:
+        if data_managers_path := self.data_managers_path:
             root_str = f'<?xml version="1.0"?><data_managers tool_path="{data_managers_path}"></data_managers>'
         else:
             root_str = '<?xml version="1.0"?><data_managers></data_managers>'
         root = parse_xml_string(root_str)
         for elem in config_elems:
             root.append(elem)
         try:
@@ -108,16 +107,16 @@
                 return rval
             root = tree.getroot()
             for elem in root:
                 if elem.tag == "data_manager":
                     data_manager_id = elem.get("id", None)
                     if data_manager_id is None:
                         log.error(
-                            "A data manager was defined that does not have an id and will not be installed:\n%s"
-                            % xml_to_string(elem)
+                            "A data manager was defined that does not have an id and will not be installed:\n%s",
+                            xml_to_string(elem),
                         )
                         continue
                     data_manager_dict = (
                         metadata_dict["data_manager"].get("data_managers", {}).get(data_manager_id, None)
                     )
                     if data_manager_dict is None:
                         log.error(f"Data manager metadata is not defined properly for '{data_manager_id}'.")
@@ -167,15 +166,15 @@
                     )
                     elem.insert(0, tool_elem)
                     data_manager = self.app.data_managers.load_manager_from_elem(
                         elem, tool_path=shed_config_dict.get("tool_path", "")
                     )
                     if data_manager:
                         rval.append(data_manager)
-                elif elem.tag is etree.Comment:
+                elif elem.tag is etree.Comment:  # type: ignore[comparison-overlap]
                     pass
                 else:
                     log.warning(f"Encountered unexpected element '{elem.tag}':\n{xml_to_string(elem)}")
                 config_elems.append(elem)
                 data_manager_config_has_changes = True
             # Persist the altered shed_data_manager_config file.
             if data_manager_config_has_changes:
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/tools/tool_panel_manager.py` & `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/tool_panel_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 from galaxy.exceptions import RequestParameterInvalidException
 from galaxy.model.base import transaction
 from galaxy.tool_shed.galaxy_install.client import InstallationTarget
 from galaxy.tool_shed.util.basic_util import strip_path
 from galaxy.tool_shed.util.repository_util import get_repository_owner
 from galaxy.tool_shed.util.shed_util_common import get_tool_panel_config_tool_path_install_dir
 from galaxy.util import (
-    etree,
+    Element,
     parse_xml_string,
+    SubElement,
     xml_to_string,
 )
 from galaxy.util.renamed_temporary_file import RenamedTemporaryFile
 from galaxy.util.tool_shed.common_util import remove_protocol_and_user_from_clone_url
 from galaxy.util.tool_shed.xml_util import parse_xml
 
 log = logging.getLogger(__name__)
@@ -150,35 +151,35 @@
             with RenamedTemporaryFile(config_filename, mode="w") as fh:
                 fh.write(xml_to_string(root, pretty=True))
         except Exception:
             log.exception("Exception in ToolPanelManager.config_elems_to_xml_file")
 
     def generate_tool_elem(
         self, tool_shed, repository_name, changeset_revision, owner, tool_file_path, tool, tool_section
-    ):
+    ) -> Element:
         """Create and return an ElementTree tool Element."""
         if tool_section is not None:
-            tool_elem = etree.SubElement(tool_section, "tool")
+            tool_elem = SubElement(tool_section, "tool")
         else:
-            tool_elem = etree.Element("tool")
+            tool_elem = Element("tool")
         tool_elem.attrib["file"] = tool_file_path
         if not tool.guid:
             raise ValueError("tool has no guid")
         tool_elem.attrib["guid"] = tool.guid
-        tool_shed_elem = etree.SubElement(tool_elem, "tool_shed")
+        tool_shed_elem = SubElement(tool_elem, "tool_shed")
         tool_shed_elem.text = tool_shed
-        repository_name_elem = etree.SubElement(tool_elem, "repository_name")
+        repository_name_elem = SubElement(tool_elem, "repository_name")
         repository_name_elem.text = repository_name
-        repository_owner_elem = etree.SubElement(tool_elem, "repository_owner")
+        repository_owner_elem = SubElement(tool_elem, "repository_owner")
         repository_owner_elem.text = owner
-        changeset_revision_elem = etree.SubElement(tool_elem, "installed_changeset_revision")
+        changeset_revision_elem = SubElement(tool_elem, "installed_changeset_revision")
         changeset_revision_elem.text = changeset_revision
-        id_elem = etree.SubElement(tool_elem, "id")
+        id_elem = SubElement(tool_elem, "id")
         id_elem.text = tool.id
-        version_elem = etree.SubElement(tool_elem, "version")
+        version_elem = SubElement(tool_elem, "version")
         version_elem.text = tool.version
         return tool_elem
 
     def generate_tool_panel_dict_for_new_install(self, tool_dicts, tool_section=None):
         """
         When installing a repository that contains tools, all tools must
         currently be defined within the same tool section in the tool panel or
@@ -239,18 +240,17 @@
         repository is being deactivated or un-installed and allows for
         activation or re-installation using the original layout.
         """
         tool_panel_dict: Dict[str, List[Dict[str, Any]]] = {}
         shed_tool_conf, tool_path, relative_install_dir = get_tool_panel_config_tool_path_install_dir(
             self.app, repository
         )
-        metadata = repository.metadata_
         # Create a dictionary of tool guid and tool config file name for each tool in the repository.
         guids_and_configs = {}
-        if "tools" in metadata:
+        if "tools" in (metadata := repository.metadata_):
             for tool_dict in metadata["tools"]:
                 guid = tool_dict["guid"]
                 tool_config = tool_dict["tool_config"]
                 file_name = strip_path(tool_config)
                 guids_and_configs[guid] = file_name
         # Parse the shed_tool_conf file in which all of this repository's tools are defined and generate the tool_panel_dict.
         tree, error_message = parse_xml(shed_tool_conf)
@@ -294,15 +294,15 @@
         repository_clone_url: str,
         changeset_revision: str,
         tool_panel_dict: dict,
         repository_tools_tups: List[tuple],
         owner="",
     ):
         """Generate a list of ElementTree Element objects for each section or tool."""
-        elem_list: List[etree.Element] = []
+        elem_list: List[Element] = []
         tool_elem = None
         cleaned_repository_clone_url = remove_protocol_and_user_from_clone_url(repository_clone_url)
         if not owner:
             owner = get_repository_owner(cleaned_repository_clone_url)
         tool_shed = cleaned_repository_clone_url.split("/repos/")[0].rstrip("/")
         for guid, tool_section_dicts in tool_panel_dict.items():
             for tool_section_dict in tool_section_dicts:
@@ -332,14 +332,15 @@
                     changeset_revision,
                     owner,
                     tool_file_path,
                     tool,
                     tool_section if inside_section else None,
                 )
                 if inside_section:
+                    assert tool_section is not None
                     if section_in_elem_list is not None:
                         elem_list[section_in_elem_list] = tool_section
                     else:
                         elem_list.append(tool_section)
                 else:
                     elem_list.append(tool_elem)
         return elem_list
@@ -363,25 +364,21 @@
                 tool_section_dicts.append(
                     dict(tool_config=tool_config, id=section_id, version=section_version, name=section_name)
                 )
         else:
             tool_section_dicts.append(dict(tool_config=tool_config, id="", version="", name=""))
         return tool_section_dicts
 
-    def generate_tool_section_element_from_dict(self, tool_section_dict):
+    def generate_tool_section_element_from_dict(self, tool_section_dict: Dict[str, str]) -> Element:
         # The value of tool_section_dict looks like the following.
         # { id: <ToolSection id>, version : <ToolSection version>, name : <TooSection name>}
-        if tool_section_dict["id"]:
-            # Create a new tool section.
-            tool_section = etree.Element("section")
-            tool_section.attrib["id"] = tool_section_dict["id"]
-            tool_section.attrib["name"] = tool_section_dict["name"]
-            tool_section.attrib["version"] = tool_section_dict["version"]
-        else:
-            tool_section = None
+        tool_section = Element("section")
+        tool_section.attrib["id"] = tool_section_dict["id"]
+        tool_section.attrib["name"] = tool_section_dict["name"]
+        tool_section.attrib["version"] = tool_section_dict["version"]
         return tool_section
 
     def get_or_create_tool_section(self, toolbox, tool_panel_section_id, new_tool_panel_section_label=None):
         return toolbox.get_section(
             section_id=tool_panel_section_id, new_label=new_tool_panel_section_label, create_if_needed=True
         )
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/galaxy_install/update_repository_manager.py` & `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/update_repository_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Determine if installed tool shed repositories have updates available in their respective tool sheds.
 """
+
 import logging
 import threading
 from typing import NamedTuple
 
 from sqlalchemy import false
 
 from galaxy import util
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/metadata/metadata_generator.py` & `galaxy-app-24.0.0/galaxy/tool_shed/metadata/metadata_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 ]
 
 
 class RepositoryProtocol(Protocol):
     name: str
     id: str
 
-    def repo_path(self, app) -> Optional[str]:
-        ...
+    def repo_path(self, app) -> Optional[str]: ...
 
 
 class BaseMetadataGenerator:
     app: Union["BasicSharedApp", InstallationTarget]
     repository: Optional[RepositoryProtocol]
     invalid_file_tups: List[InvalidFileT]
     changeset_revision: Optional[str]
@@ -131,16 +130,15 @@
         tools = {}
         for tool in metadata_dict.get("tools", []):
             tool_conf_name = tool["tool_config"]
             if tool_path:
                 tool_conf_name = os.path.join(tool_path, tool_conf_name)
             tools[tool_conf_name] = tool
         root = tree.getroot()
-        data_manager_tool_path = root.get("tool_path", None)
-        if data_manager_tool_path:
+        if data_manager_tool_path := root.get("tool_path", None):
             relative_data_manager_dir = os.path.join(relative_data_manager_dir, data_manager_tool_path)
         for i, data_manager_elem in enumerate(root.findall("data_manager")):
             tool_file = data_manager_elem.get("tool_file", None)
             data_manager_id = data_manager_elem.get("id", None)
             if data_manager_id is None:
                 log.error(f'Data Manager entry is missing id attribute in "{data_manager_config_filename}".')
                 invalid_data_managers.append(
@@ -489,17 +487,17 @@
         tree, error_message = parse_xml(repository_dependencies_config)
         if tree is None:
             xml_is_valid = False
         else:
             root = tree.getroot()
             xml_is_valid = root.tag == "repositories"
         if xml_is_valid:
-            invalid_repository_dependencies_dict = dict(description=root.get("description"))
+            invalid_repository_dependencies_dict: Dict[str, Any] = dict(description=root.get("description"))
             invalid_repository_dependency_tups = []
-            valid_repository_dependencies_dict = dict(description=root.get("description"))
+            valid_repository_dependencies_dict: Dict[str, Any] = dict(description=root.get("description"))
             valid_repository_dependency_tups = []
             for repository_elem in root.findall("repository"):
                 repository_dependency_tup, repository_dependency_is_valid, err_msg = self.handle_repository_elem(
                     repository_elem, only_if_compiling_contained_td=False
                 )
                 if repository_dependency_is_valid:
                     valid_repository_dependency_tups.append(repository_dependency_tup)
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/repository_type.py` & `galaxy-app-24.0.0/galaxy/tool_shed/repository_type.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/tools/data_table_manager.py` & `galaxy-app-24.0.0/galaxy/tool_shed/tools/data_table_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,18 @@
     List,
     TYPE_CHECKING,
     Union,
 )
 
 from galaxy.tool_shed.galaxy_install.client import InstallationTarget
 from galaxy.tool_shed.util import hg_util
-from galaxy.util import etree
+from galaxy.util import (
+    Element,
+    SubElement,
+)
 from galaxy.util.tool_shed import xml_util
 
 if TYPE_CHECKING:
     from galaxy.structured_app import BasicSharedApp
 
 log = logging.getLogger(__name__)
 
@@ -25,32 +28,32 @@
     app: RequiredAppT
 
     def __init__(self, app: RequiredAppT):
         self.app = app
 
     def generate_repository_info_elem(
         self, tool_shed: str, repository_name: str, changeset_revision: str, owner: str, parent_elem=None, **kwd
-    ) -> etree.Element:
+    ) -> Element:
         """Create and return an ElementTree repository info Element."""
         if parent_elem is None:
-            elem = etree.Element("tool_shed_repository")
+            elem = Element("tool_shed_repository")
         else:
-            elem = etree.SubElement(parent_elem, "tool_shed_repository")
-        tool_shed_elem = etree.SubElement(elem, "tool_shed")
+            elem = SubElement(parent_elem, "tool_shed_repository")
+        tool_shed_elem = SubElement(elem, "tool_shed")
         tool_shed_elem.text = tool_shed
-        repository_name_elem = etree.SubElement(elem, "repository_name")
+        repository_name_elem = SubElement(elem, "repository_name")
         repository_name_elem.text = repository_name
-        repository_owner_elem = etree.SubElement(elem, "repository_owner")
+        repository_owner_elem = SubElement(elem, "repository_owner")
         repository_owner_elem.text = owner
-        changeset_revision_elem = etree.SubElement(elem, "installed_changeset_revision")
+        changeset_revision_elem = SubElement(elem, "installed_changeset_revision")
         changeset_revision_elem.text = changeset_revision
         # add additional values
         # TODO: enhance additional values to allow e.g. use of dict values that will recurse
         for key, value in kwd.items():
-            new_elem = etree.SubElement(elem, key)
+            new_elem = SubElement(elem, key)
             new_elem.text = value
         return elem
 
     def generate_repository_info_elem_from_repository(self, tool_shed_repository, parent_elem=None, **kwd):
         return self.generate_repository_info_elem(
             tool_shed_repository.tool_shed,
             tool_shed_repository.name,
@@ -159,24 +162,25 @@
             if filename == TOOL_DATA_TABLE_FILE_SAMPLE_NAME:
                 shutil.copy2(source_file, os.path.join(target_dir, filename))
         tool_data_table_conf_filename = os.path.join(target_dir, TOOL_DATA_TABLE_FILE_NAME)
         elems = []
         if os.path.exists(tool_data_table_conf_filename):
             tree, error_message = xml_util.parse_xml(tool_data_table_conf_filename)
             if tree:
-                for elem in tree.getroot():
-                    # Append individual table elems or other elemes, but not tables elems.
-                    if elem.tag == "tables":
-                        # TODO: this code need to be revised
-                        for _table_elem in elems:
-                            elems.append(elem)
-                    else:
-                        elems.append(elem)
+                root = tree.getroot()
+                if root.tag == "tables":
+                    elems = list(root)
+                else:
+                    log.warning(
+                        "The '%s' data table file has '%s' instead of <tables> as root element, skipping.",
+                        tool_data_table_conf_filename,
+                        root.tag,
+                    )
         else:
-            log.debug(
+            log.warning(
                 "The '%s' data table file was not found, but was expected to be copied from '%s' during repository installation.",
                 tool_data_table_conf_filename,
                 TOOL_DATA_TABLE_FILE_SAMPLE_NAME,
             )
         for elem in elems:
             if elem.tag == "table":
                 for file_elem in elem.findall("file"):
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/tools/tool_validator.py` & `galaxy-app-24.0.0/galaxy/tool_shed/tools/tool_validator.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/unittest_utils/__init__.py` & `galaxy-app-24.0.0/galaxy/tool_shed/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/basic_util.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/basic_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/container_util.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/container_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/dependency_display.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/dependency_display.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,16 +193,15 @@
     def populate_containers_dict_from_repository_metadata(self, repository):
         """
         Retrieve necessary information from the received repository's metadata to populate the
         containers_dict for display.  This method is called only from Galaxy (not the tool shed)
         when displaying repository dependencies for installed repositories and when displaying
         them for uninstalled repositories that are being reinstalled.
         """
-        metadata = repository.metadata_
-        if metadata:
+        if metadata := repository.metadata_:
             irm = InstalledRepositoryManager(self.app)
             # Handle repository dependencies.
             (
                 installed_repository_dependencies,
                 missing_repository_dependencies,
             ) = irm.get_installed_and_missing_repository_dependencies(repository)
             # Handle the current repository's tool dependencies.
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/hg_util.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/hg_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def clone_repository(repository_clone_url: str, repository_file_dir: str, ctx_rev=None) -> Tuple[bool, Optional[str]]:
     """
     Clone the repository up to the specified changeset_revision.  No subsequent revisions will be
     present in the cloned repository.
     """
-    cmd = ["hg", "clone"]
+    cmd = ["hg", "clone", "--stream"]
     if ctx_rev:
         cmd.extend(["-r", str(ctx_rev)])
     cmd.extend([repository_clone_url, repository_file_dir])
     # Make sure the destination path actually exists before attempting to clone
     if not os.path.exists(repository_file_dir):
         os.makedirs(repository_file_dir)
     try:
```

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/metadata_util.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/metadata_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/repository_util.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/repository_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/shed_util_common.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/shed_util_common.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/tool_dependency_util.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/tool_dependency_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/tool_util.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/tool_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tool_shed/util/utility_container_manager.py` & `galaxy-app-24.0.0/galaxy/tool_shed/util/utility_container_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,19 @@
         for contained_repository_dependency in self.repository_dependencies:
             if contained_repository_dependency.listify == listified_repository_dependency:
                 return True
         return False
 
     def remove_repository_dependency(self, repository_dependency):
         listified_repository_dependency = repository_dependency.listify
-        for contained_repository_dependency in self.repository_dependencies:
-            if contained_repository_dependency.listify == listified_repository_dependency:
-                self.repository_dependencies.remove(contained_repository_dependency)
+        self.repository_dependencies = [
+            contained_repository_dependency
+            for contained_repository_dependency in self.repository_dependencies
+            if contained_repository_dependency.listify != listified_repository_dependency
+        ]
 
     def to_dict(self):
         folders = []
         if self.folders:
             for folder in self.folders:
                 folders.append(folder.to_dict())
         repository_dependencies = []
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/__init__.py` & `galaxy-app-24.0.0/galaxy/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Classes encapsulating galaxy tools and tool configuration.
 """
+
 import itertools
 import json
 import logging
 import math
 import os
 import re
 import tarfile
@@ -22,15 +23,14 @@
     Type,
     TYPE_CHECKING,
     Union,
 )
 from urllib.parse import unquote_plus
 
 import webob.exc
-from lxml import etree
 from mako.template import Template
 from packaging.version import Version
 from sqlalchemy import (
     delete,
     func,
     select,
 )
@@ -123,15 +123,14 @@
     DataCollectionToolParameter,
     DataToolParameter,
     HiddenToolParameter,
     ImplicitConversionRequired,
     SelectTagParameter,
     SelectToolParameter,
     ToolParameter,
-    workflow_building_modes,
 )
 from galaxy.tools.parameters.dataset_matcher import (
     set_dataset_matcher_factory,
     unset_dataset_matcher_factory,
 )
 from galaxy.tools.parameters.grouping import (
     Conditional,
@@ -139,21 +138,23 @@
     Group,
     Repeat,
     Section,
     UploadDataset,
 )
 from galaxy.tools.parameters.input_translation import ToolInputTranslator
 from galaxy.tools.parameters.meta import expand_meta_parameters
+from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
 from galaxy.tools.parameters.wrapped_json import json_wrap
 from galaxy.tools.test import parse_tests
 from galaxy.util import (
     in_directory,
     listify,
     Params,
     parse_xml_string,
+    parse_xml_string_to_etree,
     rst_to_html,
     string_as_bool,
     unicodify,
     UNKNOWN,
     XML,
 )
 from galaxy.util.bunch import Bunch
@@ -336,16 +337,15 @@
 
 class ToolNotFoundException(Exception):
     pass
 
 
 def create_tool_from_source(app, tool_source, config_file=None, **kwds):
     # Allow specifying a different tool subclass to instantiate
-    tool_module = tool_source.parse_tool_module()
-    if tool_module is not None:
+    if (tool_module := tool_source.parse_tool_module()) is not None:
         module, cls = tool_module
         mod = __import__(module, globals(), locals(), [cls])
         ToolClass = getattr(mod, cls)
     elif tool_source.parse_tool_type():
         tool_type = tool_source.parse_tool_type()
         ToolClass = tool_types.get(tool_type)
     else:
@@ -439,17 +439,18 @@
             config_filenames=config_filenames,
             tool_root_dir=tool_root_dir,
             app=app,
             view_sources=view_sources,
             default_panel_view=default_panel_view,
             save_integrated_tool_panel=save_integrated_tool_panel,
         )
-
-        old_toolbox = getattr(app, "toolbox", None)
-        if old_toolbox:
+        # Load built-in converters
+        if app.config.display_builtin_converters:
+            self.load_builtin_converters()
+        if old_toolbox := getattr(app, "toolbox", None):
             self.dependency_manager = old_toolbox.dependency_manager
         else:
             self._init_dependency_manager()
 
     def tool_tag_manager(self):
         if hasattr(self.app.config, "get_bool") and self.app.config.get_bool("enable_tool_tags", False):
             return PersistentToolTagManager(self.app)
@@ -531,15 +532,15 @@
     def create_tool(self, config_file, tool_cache_data_dir=None, **kwds):
         cache = self.get_cache_region(tool_cache_data_dir)
         if config_file.endswith(".xml") and cache and not cache.disabled:
             tool_document = cache.get(config_file)
             if tool_document:
                 tool_source = self.get_expanded_tool_source(
                     config_file=config_file,
-                    xml_tree=etree.ElementTree(etree.fromstring(tool_document["document"].encode("utf-8"))),
+                    xml_tree=parse_xml_string_to_etree(tool_document["document"]),
                     macro_paths=tool_document["macro_paths"],
                 )
             else:
                 tool_source = self.get_expanded_tool_source(config_file)
                 cache.set(config_file, tool_source)
         else:
             tool_source = self.get_expanded_tool_source(config_file)
@@ -784,15 +785,15 @@
         # differ from the inputs dictionary in that inputs can be page
         # elements like conditionals, but input_params are basic form
         # parameters like SelectField objects.  This enables us to more
         # easily ensure that parameter dependencies like index files or
         # tool_data_table_conf.xml entries exist.
         self.input_params: List[ToolParameter] = []
         # Attributes of tools installed from Galaxy tool sheds.
-        self.tool_shed = None
+        self.tool_shed: Optional[str] = None
         self.repository_name = None
         self.repository_owner = None
         self.changeset_revision = None
         self.installed_changeset_revision = None
         self.sharable_url = None
         self.npages = 0
         # The tool.id value will be the value of guid, but we'll keep the
@@ -822,16 +823,15 @@
             mem_optimize()
         # The job search is only relevant in a galaxy context, and breaks
         # loading tools into the toolshed for validation.
         if self.app.name == "galaxy":
             self.job_search = self.app.job_search
 
     def remove_from_cache(self):
-        source_path = self.tool_source.source_path
-        if source_path:
+        if source_path := self.tool_source.source_path:
             for region in self.app.toolbox.cache_regions.values():
                 region.delete(source_path)
 
     @property
     def history_manager(self):
         return self.app.history_manager
 
@@ -906,21 +906,24 @@
     @property
     def requires_galaxy_python_environment(self):
         """Indicates this tool's runtime requires Galaxy's Python environment."""
         # All special tool types (data source, history import/export, etc...)
         # seem to require Galaxy's Python.
         # FIXME: the (instantiated) tool class should emit this behavior, and not
         #        use inspection by string check
-        if self.tool_type not in ["default", "manage_data", "interactive", "data_source"]:
+        if self.tool_type not in ["default", "manage_data", "interactive", "data_source", "data_source_async"]:
             return True
 
-        if self.tool_type == "manage_data" and self.profile < 18.09:
+        if self.tool_type == "manage_data" and Version(str(self.profile)) < Version("18.09"):
             return True
 
-        if self.tool_type == "data_source" and self.profile < 21.09:
+        if self.tool_type == "data_source" and Version(str(self.profile)) < Version("21.09"):
+            return True
+
+        if self.tool_type == "data_source_async" and self.profile < 24.0:
             return True
 
         config = self.app.config
         preserve_python_environment = config.preserve_python_environment
         if preserve_python_environment == "always":
             return True
         elif preserve_python_environment == "legacy_and_local" and self.tool_shed is None:
@@ -1015,29 +1018,29 @@
         if self.app.name == "galaxy" and profile >= Version("16.04") and Version(VERSION_MAJOR) < profile:
             message = f"The tool [{self.id}] targets version {self.profile} of Galaxy, you should upgrade Galaxy to ensure proper functioning of this tool."
             raise Exception(message)
 
         self.python_template_version = tool_source.parse_python_template_version()
         if self.python_template_version is None:
             # If python_template_version not specified we assume tools with profile versions >= 19.05 are python 3 ready
-            if self.profile >= 19.05:
+            if profile >= Version("19.05"):
                 self.python_template_version = Version("3.5")
             else:
                 self.python_template_version = Version("2.7")
 
         # Get the (user visible) name of the tool
         self.name = tool_source.parse_name()
         if not self.name and dynamic:
             self.name = self.id
         if not dynamic and not self.name:
             raise Exception(f"Missing tool 'name' for tool with id '{self.id}' at '{tool_source}'")
 
         self.version = tool_source.parse_version()
         if not self.version:
-            if self.profile < 16.04:
+            if profile < Version("16.04"):
                 # For backward compatibility, some tools may not have versions yet.
                 self.version = "1.0.0"
             else:
                 raise Exception(f"Missing tool 'version' for tool with id '{self.id}' at '{tool_source}'")
 
         # Legacy feature, ignored by UI.
         self.force_history_refresh = False
@@ -1089,16 +1092,15 @@
             self.redirect_url_params = ""
 
         # Short description of the tool
         self.description = tool_source.parse_description()
 
         # Versioning for tools
         self.version_string_cmd = None
-        version_command = tool_source.parse_version_command()
-        if version_command is not None:
+        if (version_command := tool_source.parse_version_command()) is not None:
             self.version_string_cmd = version_command.strip()
 
             version_cmd_interpreter = tool_source.parse_version_command_interpreter()
             if version_cmd_interpreter:
                 executable = self.version_string_cmd.split()[0]
                 abs_executable = os.path.abspath(os.path.join(self.tool_dir, executable))
                 command_line = self.version_string_cmd.replace(executable, abs_executable, 1)
@@ -1257,27 +1259,25 @@
                         )
                         compiled_code = compile(translated_code, f"futurized_{code_path}", "exec")
                         exec(compiled_code, self.code_namespace)
                     else:
                         raise
 
         # User interface hints
-        uihints_elem = root.find("uihints")
-        if uihints_elem is not None:
+        if (uihints_elem := root.find("uihints")) is not None:
             for key, value in uihints_elem.attrib.items():
                 self.uihints[key] = value
 
     def __parse_config_files(self, tool_source):
         self.config_files = []
         if not hasattr(tool_source, "root"):
             return
 
         root = tool_source.root
-        conf_parent_elem = root.find("configfiles")
-        if conf_parent_elem is not None:
+        if (conf_parent_elem := root.find("configfiles")) is not None:
             inputs_elem = conf_parent_elem.find("inputs")
             if inputs_elem is not None:
                 name = inputs_elem.get("name")
                 filename = inputs_elem.get("filename", None)
                 format = inputs_elem.get("format", "json")
                 data_style = inputs_elem.get("data_style", "skip")
                 content = dict(format=format, handle_files=data_style, type="inputs")
@@ -1296,21 +1296,19 @@
 
     def __parse_trackster_conf(self, tool_source):
         self.trackster_conf = None
         if not hasattr(tool_source, "root"):
             return
 
         # Trackster configuration.
-        trackster_conf = tool_source.root.find("trackster_conf")
-        if trackster_conf is not None:
+        if (trackster_conf := tool_source.root.find("trackster_conf")) is not None:
             self.trackster_conf = TracksterConfig.parse(trackster_conf)
 
     def parse_tests(self):
-        tests_source = self.tool_source
-        if tests_source:
+        if tests_source := self.tool_source:
             try:
                 self.__tests = json.dumps([t.to_dict() for t in parse_tests(self, tests_source)], indent=None)
             except Exception:
                 self.__tests = None
                 log.exception("Failed to parse tool tests for tool '%s'", self.id)
 
     @property
@@ -1331,17 +1329,16 @@
                     return str(repo_dir)
             else:
                 log.error(f"Problem finding repository dir for tool '{self.id}'")
 
         return repository_base_dir
 
     def test_data_path(self, filename):
-        repository_dir = self._repository_dir
         test_data = None
-        if repository_dir:
+        if repository_dir := self._repository_dir:
             test_data = self.__walk_test_data(dir=repository_dir, filename=filename)
         else:
             if self.tool_dir:
                 tool_dir = self.tool_dir
                 if isinstance(self, DataManagerTool):
                     tool_dir = os.path.dirname(self.tool_dir)
                 test_data = self.__walk_test_data(tool_dir, filename=filename)
@@ -1376,16 +1373,15 @@
         return parse_tool_provided_metadata(
             meta_file, provided_metadata_style=self.provided_metadata_style, job_wrapper=job_wrapper
         )
 
     def parse_command(self, tool_source):
         """ """
         # Command line (template). Optional for tools that do not invoke a local program
-        command = tool_source.parse_command()
-        if command is not None:
+        if (command := tool_source.parse_command()) is not None:
             self.command = command.lstrip()  # get rid of leading whitespace
             # Must pre-pend this AFTER processing the cheetah command template
             self.interpreter = tool_source.parse_interpreter()
         else:
             self.command = ""
             self.interpreter = None
 
@@ -1633,16 +1629,15 @@
     def parse_param_elem(self, input_source: InputSource, enctypes, context) -> ToolParameter:
         """
         Parse a single "<param>" element and return a ToolParameter instance.
         Also, if the parameter has a 'required_enctype' add it to the set
         enctypes.
         """
         param = ToolParameter.build(self, input_source)
-        param_enctype = param.get_required_enctype()
-        if param_enctype:
+        if param_enctype := param.get_required_enctype():
             enctypes.add(param_enctype)
         # If parameter depends on any other paramters, we must refresh the
         # form when it changes
         for name in param.get_dependencies():
             # Let it throw exception, but give some hint what the problem might be
             if name not in context:
                 log.error(f"Tool with id '{self.id}': Could not find dependency '{name}' of parameter '{param.name}'")
@@ -1663,14 +1658,15 @@
                     inputs = parse_xml_string("<inputs/>")
                     root.append(inputs)
                 inputs.append(resource_xml)
 
     def populate_tool_shed_info(self, tool_shed_repository):
         if tool_shed_repository:
             self.tool_shed = tool_shed_repository.tool_shed
+            assert self.tool_shed
             self.repository_name = tool_shed_repository.name
             self.repository_owner = tool_shed_repository.owner
             self.changeset_revision = tool_shed_repository.changeset_revision
             self.installed_changeset_revision = tool_shed_repository.installed_changeset_revision
             self.sharable_url = get_tool_shed_repository_url(
                 self.app, self.tool_shed, self.repository_owner, self.repository_name
             )
@@ -2339,16 +2335,15 @@
         # Find and add macros and code files.
         for external_file in tool.get_externally_referenced_paths(os.path.abspath(tool.config_file)):
             external_file_abspath = os.path.abspath(os.path.join(tool_path, external_file))
             tarball_files.append((external_file_abspath, external_file))
         if os.path.exists(os.path.join(tool_path, "Dockerfile")):
             tarball_files.append((os.path.join(tool_path, "Dockerfile"), "Dockerfile"))
         # Find tests, and check them for test data.
-        tests = tool.tests
-        if tests is not None:
+        if (tests := tool.tests) is not None:
             for test in tests:
                 # Add input file tuples to the list.
                 for input in test.inputs:
                     for input_value in test.inputs[input]:
                         input_filename = str(input_value)
                         input_path = os.path.abspath(os.path.join("test-data", input_filename))
                         if os.path.exists(input_path):
@@ -2647,16 +2642,15 @@
                 id = value.dataset.id
                 source = hda_source_dict
             elif isinstance(value, self.app.model.HistoryDatasetCollectionAssociation):
                 id = value.collection.id
                 source = hdca_source_dict
             else:
                 return None
-            key = f"{value.hid}_{id}"
-            if key in source:
+            if (key := f"{value.hid}_{id}") in source:
                 return source[key]
             elif id in source:
                 return source[id]
             else:
                 return None
 
         def mapping_callback(input, value, **kwargs):
@@ -2866,24 +2860,26 @@
         for key, val in self.outputs.items():
             if key not in out_data:
                 # Skip filtered outputs
                 continue
             if val.output_type == "data":
                 with open(out_data[key].get_file_name()) as f:
                     src = json.load(f)
+                if src is None:
+                    continue
                 assert isinstance(src, dict), f"Expected dataset 'src' to be a dictionary - actual type is {type(src)}"
                 dataset_id = src["id"]
                 copy_object = None
                 for input_dataset in inp_data.values():
                     if input_dataset and input_dataset.id == dataset_id:
                         copy_object = input_dataset
                         break
                 if copy_object is None:
                     raise exceptions.MessageException("Failed to find dataset output.")
-                out_data[key].copy_from(copy_object)
+                out_data[key].copy_from(copy_object, include_metadata=True)
 
     def parse_environment_variables(self, tool_source):
         """Setup environment variable for inputs file."""
         environmnt_variables_raw = super().parse_environment_variables(tool_source)
         expression_script_inputs = dict(
             name="GALAXY_EXPRESSION_INPUTS",
             template=ExpressionTool.EXPRESSION_INPUTS_NAME,
@@ -2897,23 +2893,32 @@
     Alternate implementation of Tool for data_source tools -- those that
     allow the user to query and extract data from another web site.
     """
 
     tool_type = "data_source"
     default_tool_action = DataSourceToolAction
 
+    @property
+    def wants_params_cleaned(self):
+        """Indicates whether received, but undeclared request params should be cleaned."""
+        if self.profile < 24.0:
+            return False
+        return True
+
     def _build_GALAXY_URL_parameter(self):
         return ToolParameter.build(
             self, XML(f'<param name="GALAXY_URL" type="baseurl" value="/tool_runner?tool_id={self.id}" />')
         )
 
     def parse_inputs(self, tool_source):
         super().parse_inputs(tool_source)
         # Open all data_source tools in _top.
         self.target = "_top"
+        # data_source tools cannot check param values
+        self.check_values = False
         if "GALAXY_URL" not in self.inputs:
             self.inputs["GALAXY_URL"] = self._build_GALAXY_URL_parameter()
             self.inputs_by_page[0]["GALAXY_URL"] = self.inputs["GALAXY_URL"]
 
     def exec_before_job(self, app, inp_data, out_data, param_dict=None):
         if param_dict is None:
             param_dict = {}
@@ -3195,21 +3200,24 @@
 
 
 class DatabaseOperationTool(Tool):
     default_tool_action = ModelOperationToolAction
     require_terminal_states = True
     require_dataset_ok = True
     tool_type_local = True
+    require_terminal_or_paused_states = False
 
     @property
     def valid_input_states(self):
         if self.require_dataset_ok:
             return (model.Dataset.states.OK,)
         elif self.require_terminal_states:
             return model.Dataset.terminal_states
+        elif self.require_terminal_or_paused_states:
+            return model.Dataset.terminal_states or model.Dataset.states.PAUSED
         else:
             return model.Dataset.valid_input_states
 
     @property
     def allow_errored_inputs(self):
         return not self.require_dataset_ok
 
@@ -3369,18 +3377,17 @@
 
     def produce_outputs(self, trans, out_data, output_collections, incoming, history, **kwds):
         input_lists = []
 
         for incoming_repeat in incoming["inputs"]:
             input_lists.append(incoming_repeat["input"])
 
-        advanced = incoming.get("advanced", None)
         dupl_actions = "keep_first"
         suffix_pattern = None
-        if advanced is not None:
+        if (advanced := incoming.get("advanced", None)) is not None:
             dupl_actions = advanced["conflict"]["duplicate_options"]
 
             if dupl_actions in ["suffix_conflict", "suffix_every", "suffix_conflict_rest"]:
                 suffix_pattern = advanced["conflict"]["suffix_pattern"]
 
         new_element_structure = {}
 
@@ -3495,14 +3502,30 @@
     require_dataset_ok = False
 
     @staticmethod
     def element_is_valid(element: model.DatasetCollectionElement):
         return element.element_object.is_ok
 
 
+class KeepSuccessDatasetsTool(FilterDatasetsTool):
+    tool_type = "keep_success_datasets_collection"
+    require_terminal_states = False
+    require_dataset_ok = False
+    require_terminal_or_paused_states = True
+
+    @staticmethod
+    def element_is_valid(element: model.DatasetCollectionElement):
+        if (
+            element.element_object.state != model.Dataset.states.PAUSED
+            and element.element_object.state in model.Dataset.non_ready_states
+        ):
+            raise ToolInputsNotReadyException("An input dataset is pending.")
+        return element.element_object.is_ok
+
+
 class FilterEmptyDatasetsTool(FilterDatasetsTool):
     tool_type = "filter_empty_datasets_collection"
     require_dataset_ok = False
 
     @staticmethod
     def element_is_valid(element: model.DatasetCollectionElement):
         dataset_instance: model.DatasetInstance = element.element_object
@@ -3593,14 +3616,70 @@
 
         self._add_datasets_to_history(history, new_elements.values())
         output_collections.create_collection(
             next(iter(self.outputs.values())), "output", elements=new_elements, propagate_hda_tags=False
         )
 
 
+class HarmonizeTool(DatabaseOperationTool):
+    tool_type = "harmonize_list"
+    require_terminal_states = False
+    require_dataset_ok = False
+
+    def produce_outputs(self, trans, out_data, output_collections, incoming, history, **kwds):
+        # Get the 2 input collections
+        hdca1 = incoming["input1"]
+        hdca2 = incoming["input2"]
+        # Get the elements of both collections
+        elements1 = hdca1.collection.elements
+        elements2 = hdca2.collection.elements
+        # Put elements in dictionary with identifiers:
+        old_elements1_dict = {}
+        for element in elements1:
+            old_elements1_dict[element.element_identifier] = element
+        old_elements2_dict = {}
+        for element in elements2:
+            old_elements2_dict[element.element_identifier] = element
+        # Get the list of final identifiers
+        final_sorted_identifiers = [
+            element.element_identifier for element in elements1 if element.element_identifier in old_elements2_dict
+        ]
+        # Raise Exception if it is empty
+        if len(final_sorted_identifiers) == 0:
+            # Create empty collections:
+            output_collections.create_collection(
+                next(iter(self.outputs.values())), "output1", elements={}, propagate_hda_tags=False
+            )
+            output_collections.create_collection(
+                next(iter(self.outputs.values())), "output2", elements={}, propagate_hda_tags=False
+            )
+            return
+
+        def output_with_selected_identifiers(old_elements_dict, output_label):
+            # Create a new dictionary with the elements in the good order
+            new_elements = {}
+            for identifier in final_sorted_identifiers:
+                dce_object = old_elements_dict[identifier].element_object
+                if getattr(dce_object, "history_content_type", None) == "dataset":
+                    copied_dataset = dce_object.copy(copy_tags=dce_object.tags, flush=False)
+                else:
+                    copied_dataset = dce_object.copy(flush=False)
+                new_elements[identifier] = copied_dataset
+            # Add datasets:
+            self._add_datasets_to_history(history, new_elements.values())
+            # Create collections:
+            output_collections.create_collection(
+                next(iter(self.outputs.values())), output_label, elements=new_elements, propagate_hda_tags=False
+            )
+
+        # Create outputs:
+        output_with_selected_identifiers(old_elements1_dict, "output1")
+        output_with_selected_identifiers(old_elements2_dict, "output2")
+
+
 class RelabelFromFileTool(DatabaseOperationTool):
     tool_type = "relabel_from_file"
 
     def produce_outputs(self, trans, out_data, output_collections, incoming, history, **kwds):
         hdca = incoming["input"]
         how_type = incoming["how"]["how_select"]
         new_labels_dataset_assoc = incoming["how"]["labels"]
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/actions/__init__.py` & `galaxy-app-24.0.0/galaxy/tools/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     Dict,
     List,
     Set,
     TYPE_CHECKING,
     Union,
 )
 
+from packaging.version import Version
+
 from galaxy import model
 from galaxy.exceptions import ItemAccessibilityException
 from galaxy.job_execution.actions.post import ActionBox
 from galaxy.model import (
     HistoryDatasetAssociation,
     Job,
     LibraryDatasetDatasetAssociation,
@@ -28,14 +30,15 @@
 from galaxy.model.none_like import NoneDataset
 from galaxy.objectstore import ObjectStorePopulator
 from galaxy.tools.parameters import update_dataset_ids
 from galaxy.tools.parameters.basic import (
     DataCollectionToolParameter,
     DataToolParameter,
     RuntimeValue,
+    SelectToolParameter,
 )
 from galaxy.tools.parameters.wrapped import (
     LegacyUnprefixedDict,
     WrappedParameters,
 )
 from galaxy.util import ExecutionTimer
 from galaxy.util.template import fill_template
@@ -172,17 +175,17 @@
                         input_datasets.set_legacy_alias(
                             new_key=prefixed_name + str(i + 1), old_key=prefix + input.name + str(i + 1)
                         )
                         conversions = []
                         for conversion_name, conversion_extensions, conversion_datatypes in input.conversions:
                             new_data = process_dataset(input_datasets[prefixed_name + str(i + 1)], conversion_datatypes)
                             if not new_data or new_data.datatype.matches_any(conversion_datatypes):
-                                input_datasets[
-                                    prefixed_name[: -len(input.name)] + conversion_name + str(i + 1)
-                                ] = new_data
+                                input_datasets[prefixed_name[: -len(input.name)] + conversion_name + str(i + 1)] = (
+                                    new_data
+                                )
                                 input_datasets.set_legacy_alias(
                                     new_key=prefixed_name[: -len(input.name)] + conversion_name + str(i + 1),
                                     old_key=prefix + conversion_name + str(i + 1),
                                 )
                                 conversions.append((conversion_name, new_data))
                             else:
                                 raise Exception(
@@ -217,17 +220,17 @@
                             )
                     target_dict = parent
                     if not target_dict:
                         target_dict = param_values
                     target_dict[input.name] = input_datasets[prefixed_name]
                     for conversion_name, conversion_data in conversions:
                         # allow explicit conversion to be stored in job_parameter table
-                        target_dict[
-                            conversion_name
-                        ] = conversion_data.id  # a more robust way to determine JSONable value is desired
+                        target_dict[conversion_name] = (
+                            conversion_data.id
+                        )  # a more robust way to determine JSONable value is desired
             elif isinstance(input, DataCollectionToolParameter):
                 if not value:
                     return
 
                 collection = None
                 child_collection = False
                 if hasattr(value, "child_collection"):
@@ -279,14 +282,16 @@
                         replacement_dict=processed_dataset_dict,
                     )
                     new_collection = collection_builder.build()
                     if child_collection:
                         value.child_collection = new_collection
                     else:
                         value.collection = new_collection
+            elif isinstance(input, SelectToolParameter) and isinstance(value, HistoryDatasetAssociation):
+                input_datasets[prefixed_name] = value
 
         tool.visit_inputs(param_values, visitor)
         return input_datasets, all_permissions
 
     def collect_input_dataset_collections(self, tool, param_values):
         def append_to_key(the_dict: LegacyUnprefixedDict, key, legacy_key, value):
             if key not in the_dict:
@@ -413,27 +418,27 @@
         ) = self._collect_inputs(tool, trans, incoming, history, current_user_roles, collection_info)
         # Build name for output datasets based on tool name and input names
         on_text = self._get_on_text(inp_data)
 
         # format='input" previously would give you a random extension from
         # the input extensions, now it should just give "input" as the output
         # format.
-        input_ext = "data" if tool.profile < 16.04 else "input"
+        input_ext = "data" if Version(str(tool.profile)) < Version("16.04") else "input"
         input_dbkey = incoming.get("dbkey", "?")
         for name, data in reversed(list(inp_data.items())):
             if not data:
                 data = NoneDataset(datatypes_registry=app.datatypes_registry)
                 continue
 
             # Convert LDDA to an HDA.
             if isinstance(data, LibraryDatasetDatasetAssociation) and not completed_job:
                 data = data.to_history_dataset_association(None)
                 inp_data[name] = data
 
-            if tool.profile < 16.04:
+            if Version(str(tool.profile)) < Version("16.04"):
                 input_ext = data.ext
 
             if data.dbkey not in [None, "?"]:
                 input_dbkey = data.dbkey
 
             identifier = getattr(data, "element_identifier", None)
             if identifier is not None:
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/actions/data_manager.py` & `galaxy-app-24.0.0/galaxy/tools/actions/data_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/actions/data_source.py` & `galaxy-app-24.0.0/galaxy/tools/actions/data_source.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/actions/history_imp_exp.py` & `galaxy-app-24.0.0/galaxy/tools/actions/history_imp_exp.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/actions/metadata.py` & `galaxy-app-24.0.0/galaxy/tools/actions/metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/actions/model_operations.py` & `galaxy-app-24.0.0/galaxy/tools/actions/model_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,16 +122,15 @@
             output_collections,
             incoming,
             history=history,
             tags=tags,
             hdca_tags=hdca_tags,
             tag_handler=tag_handler,
         )
-        mapped_over_elements = output_collections.dataset_collection_elements
-        if mapped_over_elements:
+        if mapped_over_elements := output_collections.dataset_collection_elements:
             for name, value in out_data.items():
                 if name in mapped_over_elements:
                     value.visible = False
                     mapped_over_elements[name].hda = value
 
         # We probably need to mark all outputs as skipped, not just the outputs of whatever the database op tools do ?
         # This is probably not exactly right, but it might also work in most cases
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/actions/upload.py` & `galaxy-app-24.0.0/galaxy/tools/actions/upload.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/actions/upload_common.py` & `galaxy-app-24.0.0/galaxy/tools/actions/upload_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,16 +192,15 @@
         create_dataset=True,
         sa_session=trans.sa_session,
     )
     if uploaded_dataset.get("tag_using_filenames", False):
         tag_from_filename = os.path.splitext(os.path.basename(uploaded_dataset.name))[0]
         tag_handler.apply_item_tag(item=ldda, user=trans.user, name="name", value=tag_from_filename, flush=False)
 
-    tags_list = uploaded_dataset.get("tags", False)
-    if tags_list:
+    if tags_list := uploaded_dataset.get("tags", False):
         for tag in tags_list:
             tag_handler.apply_item_tag(item=ldda, user=trans.user, name="name", value=tag, flush=False)
 
     trans.sa_session.add(ldda)
     if state:
         ldda.state = state
     else:
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/apply_rules.xml` & `galaxy-app-24.0.0/galaxy/tools/apply_rules.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/biotools.py` & `galaxy-app-24.0.0/galaxy/tools/biotools.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/build_list.xml` & `galaxy-app-24.0.0/galaxy/tools/build_list.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/build_list_1.2.0.xml` & `galaxy-app-24.0.0/galaxy/tools/build_list_1.2.0.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_export/export_remote.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_export/export_remote.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_export/export_remote.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_export/export_remote.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_export/send.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_export/send.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_export/send.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_export/send.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/biomart.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart.xml`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/biomart.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart.xml`

```diff
@@ -3,15 +3,15 @@
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 
     TODO: Hack to get biomart to work - the 'add_to_URL' param can be eliminated when the Biomart team encodes URL prior to sending, meanwhile
     everything including and beyond the first '&' is truncated from URL.  They said they'll let us know when this is fixed at their end.
 -->
-<tool name="BioMart" id="biomart" tool_type="data_source" version="1.0.1">
+<tool name="BioMart" id="biomart" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>Ensembl server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/biomart_test.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart_test.xml`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/biomart_test.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart_test.xml`

```diff
@@ -3,15 +3,15 @@
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 
     TODO: Hack to get biomart to work - the 'add_to_URL' param can be eliminated when the Biomart team encodes URL prior to sending, meanwhile
     everything including and beyond the first '&' is truncated from URL.  They said they'll let us know when this is fixed at their end.
 -->
-<tool name="BioMart" id="biomart_test" tool_type="data_source" version="1.0.1">
+<tool name="BioMart" id="biomart_test" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>Test server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/cbi_rice_mart.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/cbi_rice_mart.xml`

 * *Files 4% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/cbi_rice_mart.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/cbi_rice_mart.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="CBI Rice Mart" id="cbi_rice_mart" tool_type="data_source" version="1.0.1">
+<tool name="CBI Rice Mart" id="cbi_rice_mart" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>rice mart</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/data_source.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/data_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,95 @@
 #!/usr/bin/env python
 # Retrieves data from external data source applications and stores in a dataset file.
 # Data source application parameters are temporarily stored in the dataset file.
+import json
 import os
 import sys
-from json import (
-    dumps,
-    loads,
-)
 from urllib.parse import (
     urlencode,
     urlparse,
 )
 from urllib.request import urlopen
 
 from galaxy.datatypes import sniff
 from galaxy.datatypes.registry import Registry
-from galaxy.jobs import TOOL_PROVIDED_JOB_METADATA_FILE
 from galaxy.util import (
     DEFAULT_SOCKET_TIMEOUT,
     get_charset_from_http_headers,
     stream_to_open_named_file,
 )
 
 GALAXY_PARAM_PREFIX = "GALAXY"
 GALAXY_ROOT_DIR = os.path.realpath(os.path.join(os.path.dirname(__file__), os.pardir, os.pardir))
 GALAXY_DATATYPES_CONF_FILE = os.path.join(GALAXY_ROOT_DIR, "datatypes_conf.xml")
 
 
-def stop_err(msg):
-    sys.stderr.write(msg)
-    sys.exit()
-
-
-def load_input_parameters(filename, erase_file=True):
-    datasource_params = {}
-    try:
-        json_params = loads(open(filename).read())
-        datasource_params = json_params.get("param_dict")
-    except Exception:
-        json_params = None
-        for line in open(filename):
-            try:
-                line = line.strip()
-                fields = line.split("\t")
-                datasource_params[fields[0]] = fields[1]
-            except Exception:
-                continue
-    if erase_file:
-        open(filename, "w").close()  # open file for writing, then close, removes params from file
-    return json_params, datasource_params
-
-
 def __main__():
-    filename = sys.argv[1]
-    try:
+    if len(sys.argv) >= 3:
         max_file_size = int(sys.argv[2])
-    except Exception:
+    else:
         max_file_size = 0
 
-    job_params, params = load_input_parameters(filename)
-    if job_params is None:  # using an older tabular file
-        enhanced_handling = False
-        job_params = dict(param_dict=params)
-        job_params["output_data"] = [
-            dict(out_data_name="output", ext="data", file_name=filename, extra_files_path=None)
-        ]
-        job_params["job_config"] = dict(
-            GALAXY_ROOT_DIR=GALAXY_ROOT_DIR,
-            GALAXY_DATATYPES_CONF_FILE=GALAXY_DATATYPES_CONF_FILE,
-            TOOL_PROVIDED_JOB_METADATA_FILE=TOOL_PROVIDED_JOB_METADATA_FILE,
-        )
-    else:
-        enhanced_handling = True
-        json_file = open(
-            job_params["job_config"]["TOOL_PROVIDED_JOB_METADATA_FILE"], "w"
-        )  # specially named file for output junk to pass onto set metadata
+    with open(sys.argv[1]) as fh:
+        params = json.load(fh)
+
+    out_data_name = params["output_data"][0]["out_data_name"]
+
+    URL = params["param_dict"].get("URL", None)  # using exactly URL indicates that only one dataset is being downloaded
+    URL_method = params["param_dict"].get("URL_method", "get")
 
     datatypes_registry = Registry()
     datatypes_registry.load_datatypes(
-        root_dir=job_params["job_config"]["GALAXY_ROOT_DIR"],
-        config=job_params["job_config"]["GALAXY_DATATYPES_CONF_FILE"],
+        root_dir=params["job_config"]["GALAXY_ROOT_DIR"],
+        config=params["job_config"]["GALAXY_DATATYPES_CONF_FILE"],
     )
 
-    URL = params.get("URL", None)  # using exactly URL indicates that only one dataset is being downloaded
-    URL_method = params.get("URL_method", None)
-
-    for data_dict in job_params["output_data"]:
-        cur_filename = data_dict.get("file_name", filename)
-        cur_URL = params.get("%s|%s|URL" % (GALAXY_PARAM_PREFIX, data_dict["out_data_name"]), URL)
+    for data_dict in params["output_data"]:
+        cur_filename = data_dict["file_name"]
+        cur_URL = params["param_dict"].get("%s|%s|URL" % (GALAXY_PARAM_PREFIX, data_dict["out_data_name"]), URL)
         if not cur_URL or urlparse(cur_URL).scheme not in ("http", "https", "ftp"):
             open(cur_filename, "w").write("")
-            stop_err("The remote data source application has not sent back a URL parameter in the request.")
+            sys.exit("The remote data source application has not sent back a URL parameter in the request.")
 
         # The following calls to urlopen() will use the above default timeout
         try:
-            if not URL_method or URL_method == "get":
+            if URL_method == "get":
                 page = urlopen(cur_URL, timeout=DEFAULT_SOCKET_TIMEOUT)
             elif URL_method == "post":
-                page = urlopen(cur_URL, urlencode(params).encode("utf-8"), timeout=DEFAULT_SOCKET_TIMEOUT)
+                page = urlopen(
+                    cur_URL,
+                    urlencode(params["param_dict"]["incoming_request_params"]).encode("utf-8"),
+                    timeout=DEFAULT_SOCKET_TIMEOUT,
+                )
         except Exception as e:
-            stop_err("The remote data source application may be off line, please try again later. Error: %s" % str(e))
+            sys.exit("The remote data source application may be off line, please try again later. Error: %s" % str(e))
         if max_file_size:
             file_size = int(page.info().get("Content-Length", 0))
             if file_size > max_file_size:
-                stop_err(
+                sys.exit(
                     "The size of the data (%d bytes) you have requested exceeds the maximum allowed (%d bytes) on this server."
                     % (file_size, max_file_size)
                 )
         try:
             cur_filename = stream_to_open_named_file(
                 page,
-                os.open(cur_filename, os.O_WRONLY | os.O_CREAT),
+                os.open(cur_filename, os.O_WRONLY | os.O_TRUNC | os.O_CREAT),
                 cur_filename,
                 source_encoding=get_charset_from_http_headers(page.headers),
             )
         except Exception as e:
-            stop_err("Unable to fetch %s:\n%s" % (cur_URL, e))
+            sys.exit("Unable to fetch %s:\n%s" % (cur_URL, e))
 
         # here import checks that upload tool performs
-        if enhanced_handling:
-            try:
-                ext = sniff.handle_uploaded_dataset_file(filename, datatypes_registry, ext=data_dict["ext"])
-            except Exception as e:
-                stop_err(str(e))
-            info = dict(type="dataset", dataset_id=data_dict["dataset_id"], ext=ext)
+        try:
+            ext = sniff.handle_uploaded_dataset_file(cur_filename, datatypes_registry, ext=data_dict["ext"])
+        except Exception as e:
+            sys.exit(str(e))
+
+        tool_provided_metadata = {out_data_name: {"ext": ext}}
 
-            json_file.write("%s\n" % dumps(info))
+        with open(params["job_config"]["TOOL_PROVIDED_JOB_METADATA_FILE"], "w") as json_file:
+            json.dump(tool_provided_metadata, json_file)
 
 
 if __name__ == "__main__":
     __main__()
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ebi_sra.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ebi_sra.xml`

 * *Files 12% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ebi_sra.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ebi_sra.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="EBI SRA" id="ebi_sra_main" tool_type="data_source" version="1.0.1">
+<tool name="EBI SRA" id="ebi_sra_main" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>ENA SRA</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <!-- This paython script imports the file into Galaxy -->
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/eupathdb.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/eupathdb.xml`

 * *Files 12% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/eupathdb.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/eupathdb.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="EuPathDB" id="eupathdb" tool_type="data_source" url_method="post" version="1.0.0">
+<tool name="EuPathDB" id="eupathdb" tool_type="data_source" url_method="post" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/fly_modencode.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/fly_modencode.xml`

 * *Files 4% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/fly_modencode.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/fly_modencode.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="modENCODE fly" id="modENCODEfly" tool_type="data_source" version="1.0.1">
+<tool name="modENCODE fly" id="modENCODEfly" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/flymine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine.xml`

 * *Files 4% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/flymine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="Flymine" id="flymine" tool_type="data_source" version="1.0.0">
+<tool name="Flymine" id="flymine" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/flymine_test.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine_test.xml`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/flymine_test.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine_test.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="Flymine test" id="flymine_test" tool_type="data_source" version="1.0.0">
+<tool name="Flymine test" id="flymine_test" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/genbank.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/genbank.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/genbank.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/genbank.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/gramene_mart.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/gramene_mart.xml`

 * *Files 4% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/gramene_mart.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/gramene_mart.xml`

```diff
@@ -3,15 +3,15 @@
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 
     TODO: Hack to get biomart to work - the 'add_to_URL' param can be eliminated when the Biomart team encodes URL prior to sending, meanwhile
     everything including and beyond the first '&' is truncated from URL.  They said they'll let us know when this is fixed at their end.
 -->
-<tool name="GrameneMart" id="gramenemart" tool_type="data_source" version="1.0.1">
+<tool name="GrameneMart" id="gramenemart" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>Central server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/hapmapmart.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hapmapmart.xml`

 * *Files 1% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/hapmapmart.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hapmapmart.xml`

```diff
@@ -7,15 +7,15 @@
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 
     TODO: Hack to get biomart to work - the 'add_to_URL' param can be eliminated when the Biomart team encodes URL prior to sending, meanwhile
     everything including and beyond the first '&' is truncated from URL.  They said they'll let us know when this is fixed at their end.
 -->
-<tool name="HapMapMart" id="hapmapmart" tool_type="data_source" version="0.0.01">
+<tool name="HapMapMart" id="hapmapmart" tool_type="data_source" version="0.0.01" profile="20.09">
   <description>HapMap Biomart</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/hbvar.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hbvar.xml`

 * *Files 13% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/hbvar.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hbvar.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="HbVar" id="hbvar" tool_type="data_source" version="2.0.0">
+<tool name="HbVar" id="hbvar" tool_type="data_source" version="2.0.0" profile="20.09">
   <description>Human Hemoglobin Variants and Thalassemias</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/import.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/import.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/import.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/import.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/intermine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/intermine.xml`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/intermine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/intermine.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="InterMine" id="intermine" tool_type="data_source" version="1.0.0">
+<tool name="InterMine" id="intermine" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/metabolicmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/metabolicmine.xml`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/metabolicmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/metabolicmine.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="metabolicMine" id="metabolicmine" tool_type="data_source" version="1.0.0">
+<tool name="metabolicMine" id="metabolicmine" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/microbial_import.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/microbial_import.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/microbial_import_code.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import_code.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/modmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/modmine.xml`

 * *Files 11% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/modmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/modmine.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="modENCODE modMine" id="modmine" tool_type="data_source" version="1.0.0">
+<tool name="modENCODE modMine" id="modmine" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/mousemine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/mousemine.xml`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/mousemine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/mousemine.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="MouseMine" id="mousemine" tool_type="data_source" version="1.0.0">
+<tool name="MouseMine" id="mousemine" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ncbi_datasets.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ncbi_datasets.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ratmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ratmine.xml`

 * *Files 5% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ratmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ratmine.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="Ratmine" id="ratmine" tool_type="data_source" version="1.0.0">
+<tool name="Ratmine" id="ratmine" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/sra.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/sra.xml`

 * *Files 8% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/sra.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/sra.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="SRA" id="sra_source" tool_type="data_source" version="1.0.1" profile="16.04">
+<tool name="SRA" id="sra_source" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
     python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit &&
     python '$csv_to_tsv'
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml`

 * *Files 4% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="UCSC Main" id="ucsc_table_direct1" tool_type="data_source" version="1.0.0">
+<tool name="UCSC Main" id="ucsc_table_direct1" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>table browser</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
@@ -23,29 +23,30 @@
   <request_param_translation>
     <request_param galaxy_name="URL_method" remote_name="URL_method" missing="post"/>
     <request_param galaxy_name="URL" remote_name="URL" missing=""/>
     <request_param galaxy_name="dbkey" remote_name="db" missing="?"/>
     <request_param galaxy_name="organism" remote_name="org" missing="unknown species"/>
     <request_param galaxy_name="table" remote_name="hgta_table" missing="unknown table"/>
     <request_param galaxy_name="description" remote_name="hgta_regionType" missing="no description"/>
+    <request_param galaxy_name="position" remote_name="position" missing="unknown position"/>
     <request_param galaxy_name="data_type" remote_name="hgta_outputType" missing="auto">
       <value_translation>
         <value galaxy_value="auto" remote_value="primaryTable"/>
         <value galaxy_value="auto" remote_value="selectedFields"/>
         <value galaxy_value="wig" remote_value="wigData"/>
         <value galaxy_value="interval" remote_value="tab"/>
         <value galaxy_value="html" remote_value="hyperlinks"/>
         <value galaxy_value="fasta" remote_value="sequence"/>
         <value galaxy_value="gtf" remote_value="gff"/>
       </value_translation>
     </request_param>
   </request_param_translation>
   <uihints minwidth="800"/>
   <outputs>
-    <data name="output" format="tabular" label="${tool.name} on ${organism}: ${table} (#if $description == 'range' then $getVar( 'position', 'unknown position' ) else $description#)"/>
+    <data name="output" format="tabular" label="${tool.name} on ${organism}: ${table} (#if $description == 'range' then $position else $description#)"/>
   </outputs>
   <options sanitize="False" refresh="True"/>
   <citations>
     <citation type="doi">10.1093/database/bar011</citation>
     <citation type="doi">10.1101/gr.229102</citation>
   </citations>
 </tool>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml`

 * *Files 3% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="UCSC Archaea" id="ucsc_table_direct_archaea1" tool_type="data_source" version="1.0.0">
+<tool name="UCSC Archaea" id="ucsc_table_direct_archaea1" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>table browser</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
@@ -23,29 +23,30 @@
   <request_param_translation>
     <request_param galaxy_name="URL_method" remote_name="URL_method" missing="post"/>
     <request_param galaxy_name="URL" remote_name="URL" missing=""/>
     <request_param galaxy_name="dbkey" remote_name="db" missing="?"/>
     <request_param galaxy_name="organism" remote_name="org" missing="unknown species"/>
     <request_param galaxy_name="table" remote_name="hgta_table" missing="unknown table"/>
     <request_param galaxy_name="description" remote_name="hgta_regionType" missing="no description"/>
+    <request_param galaxy_name="position" remote_name="position" missing="unknown position"/>
     <request_param galaxy_name="data_type" remote_name="hgta_outputType" missing="auto">
       <value_translation>
         <value galaxy_value="auto" remote_value="primaryTable"/>
         <value galaxy_value="auto" remote_value="selectedFields"/>
         <value galaxy_value="wig" remote_value="wigData"/>
         <value galaxy_value="interval" remote_value="tab"/>
         <value galaxy_value="html" remote_value="hyperlinks"/>
         <value galaxy_value="fasta" remote_value="sequence"/>
         <value galaxy_value="gtf" remote_value="gff"/>
       </value_translation>
     </request_param>
   </request_param_translation>
   <uihints minwidth="800"/>
   <outputs>
-    <data name="output" format="tabular" label="${tool.name} on ${organism}: ${table} (#if $description == 'range' then $getVar( 'position', 'unknown position' ) else $description#)"/>
+    <data name="output" format="tabular" label="${tool.name} on ${organism}: ${table} (#if $description == 'range' then $position else $description#)"/>
   </outputs>
   <options sanitize="False" refresh="True"/>
   <citations>
     <citation type="doi">10.1093/database/bar011</citation>
     <citation type="doi">10.1101/gr.229102</citation>
     <citation type="doi">10.1093/nar/gkj134</citation>
   </citations>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml`

 * *Files 6% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
     If the value of 'URL_method' is 'get', the request will consist of the value of 'URL' coming back in
     the initial response.  If value of 'URL_method' is 'post', any additional params coming back in the
     initial response ( in addition to 'URL' ) will be encoded and appended to URL and a post will be performed.
 -->
-<tool name="UCSC Test" id="ucsc_table_direct_test1" tool_type="data_source" version="1.0.1">
+<tool name="UCSC Test" id="ucsc_table_direct_test1" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>table browser</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
@@ -23,29 +23,30 @@
   <request_param_translation>
     <request_param galaxy_name="URL_method" remote_name="URL_method" missing="post"/>
     <request_param galaxy_name="URL" remote_name="URL" missing=""/>
     <request_param galaxy_name="dbkey" remote_name="db" missing="?"/>
     <request_param galaxy_name="organism" remote_name="org" missing="unknown species"/>
     <request_param galaxy_name="table" remote_name="hgta_table" missing="unknown table"/>
     <request_param galaxy_name="description" remote_name="hgta_regionType" missing="no description"/>
+    <request_param galaxy_name="position" remote_name="position" missing="unknown position"/>
     <request_param galaxy_name="data_type" remote_name="hgta_outputType" missing="auto">
       <value_translation>
         <value galaxy_value="auto" remote_value="primaryTable"/>
         <value galaxy_value="auto" remote_value="selectedFields"/>
         <value galaxy_value="wig" remote_value="wigData"/>
         <value galaxy_value="interval" remote_value="tab"/>
         <value galaxy_value="html" remote_value="hyperlinks"/>
         <value galaxy_value="fasta" remote_value="sequence"/>
         <value galaxy_value="gtf" remote_value="gff"/>
       </value_translation>
     </request_param>
   </request_param_translation>
   <uihints minwidth="800"/>
   <outputs>
-    <data name="output" format="tabular" label="${tool.name} on ${organism}: ${table} (#if $description == 'range' then $getVar( 'position', 'unknown position' ) else $description#)"/>
+    <data name="output" format="tabular" label="${tool.name} on ${organism}: ${table} (#if $description == 'range' then $position else $description#)"/>
   </outputs>
   <options sanitize="False" refresh="True"/>
   <citations>
     <citation type="doi">10.1093/database/bar011</citation>
     <citation type="doi">10.1101/gr.229102</citation>
   </citations>
 </tool>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/upload.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         id, files_path, path = arg.split(":", 2)
         rval[int(id)] = (path, files_path)
     return rval
 
 
 def add_file(dataset, registry, output_path: str) -> Dict[str, str]:
     ext = None
-    compression_type = None
     line_count = None
     link_data_only_str = dataset.get("link_data_only", "copy_files")
     if link_data_only_str not in ["link_to_files", "copy_files"]:
         raise UploadProblemException(
             "Invalid setting '%s' for option link_data_only - upload request misconfigured" % link_data_only_str
         )
     link_data_only = link_data_only_str == "link_to_files"
@@ -146,22 +145,14 @@
         link_data_only=link_data_only,
         in_place=in_place,
         auto_decompress=auto_decompress,
         convert_to_posix_lines=dataset.to_posix_lines,
         convert_spaces_to_tabs=dataset.space_to_tab,
     )
 
-    # Strip compression extension from name
-    if (
-        compression_type
-        and not getattr(datatype, "compressed", False)
-        and dataset.name.endswith("." + compression_type)
-    ):
-        dataset.name = dataset.name[: -len("." + compression_type)]
-
     # Move dataset
     if link_data_only:
         # Never alter a file that will not be copied to Galaxy's local file store.
         if datatype.dataset_content_needs_grooming(dataset.path):
             err_msg = (
                 "The uploaded files need grooming, so change your <b>Copy data into Galaxy?</b> selection to be "
                 + "<b>Copy files into Galaxy</b> instead of <b>Link to files without copying into Galaxy</b> so grooming can be performed."
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/upload.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/upload.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/worm_modencode.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/worm_modencode.xml`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/worm_modencode.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/worm_modencode.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="modENCODE worm" id="modENCODEworm" tool_type="data_source" version="1.0.1">
+<tool name="modENCODE worm" id="modENCODEworm" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/wormbase.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase.xml`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/wormbase.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="WormBase" id="wormbase" tool_type="data_source" version="1.0.1">
+<tool name="WormBase" id="wormbase" tool_type="data_source" version="1.0.1" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/wormbase_test.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase_test.xml`

 * *Files 4% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/wormbase_test.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase_test.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="Wormbase" id="wormbase_test" tool_type="data_source" version="1.0.0">
+<tool name="Wormbase" id="wormbase_test" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>test server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/yeastmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/yeastmine.xml`

 * *Files 10% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/yeastmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/yeastmine.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="YeastMine" id="yeastmine" tool_type="data_source" version="1.0.0">
+<tool name="YeastMine" id="yeastmine" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/zebrafishmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/zebrafishmine.xml`

 * *Files 6% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/data_source/zebrafishmine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/zebrafishmine.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool name="ZebrafishMine" id="zebrafishmine" tool_type="data_source" version="1.0.0">
+<tool name="ZebrafishMine" id="zebrafishmine" tool_type="data_source" version="1.0.0" profile="20.09">
   <description>server</description>
   <edam_operations>
     <edam_operation>operation_0224</edam_operation>
   </edam_operations>
   <command><![CDATA[
 python '$__tool_directory__/data_source.py' '$output' $__app__.config.output_size_limit
     ]]></command>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/expression_tools/expression_macros.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/expression_macros.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/expression_tools/parse_values_from_file.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/parse_values_from_file.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/expression_tools/pick_value.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/pick_value.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/extract/extract_genomic_dna.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/extract/extract_genomic_dna.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/extract/extract_genomic_dna.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/extract/extract_genomic_dna.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/extract/liftOver_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/extract/liftOver_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/extract/liftOver_wrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/extract/liftOver_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/CreateInterval.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/CreateInterval.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_concat_fasta.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_concat_fasta.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_concat_fasta.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_concat_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_fasta.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_fasta.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_fasta.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_lav.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 usage("missing a value in %s=" % arg)
 
         if arg == "--silent" and val is None:
             silent = True
         elif primary is None and val is None:
             primary = arg
         elif secondary is None and val is None:
-            secondary = arg
+            secondary = arg  # type: ignore[unreachable]
         else:
             usage("unknown argument: %s" % arg)
 
     if primary is None:
         usage("missing primary file name and length")
 
     if secondary is None:
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/axt_to_lav.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/bed2gff.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed2gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/bed_to_bigbed.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed_to_bigbed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/bed_to_gff_converter.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed_to_gff_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/catWrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/catWrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/catWrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/catWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/changeCase.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/changeCase.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/changeCase.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/changeCase.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/commWrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/commWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/compare.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/compare.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/condense_characters.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/condense_characters.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/condense_characters.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/condense_characters.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/convert_characters.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/convert_characters.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/convert_characters.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/convert_characters.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/cutWrapper.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/cutWrapper.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/cutWrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/cutWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/fileGrep.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/fileGrep.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/fixedValueColumn.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/fixedValueColumn.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/fixedValueColumn.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/fixedValueColumn.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/extract_GFF_Features.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/extract_GFF_Features.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/extract_GFF_Features.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/extract_GFF_Features.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from __future__ import (
     division,
     print_function,
 )
 
 import sys
 from ast import (
-    Module,
     parse,
     walk,
 )
 from json import loads
 
 AST_NODE_TYPE_WHITELIST = [
     "Expr",
@@ -108,16 +107,14 @@
     False
     """
     try:
         module = parse(text)
     except SyntaxError:
         return False
 
-    if not isinstance(module, Module):
-        return False
     statements = module.body
     if not len(statements) == 1:
         return False
     expression = statements[0]
     if expression.__class__.__name__ != "Expr":
         return False
 
@@ -167,19 +164,17 @@
     False
     """
     try:
         module = parse(text)
     except SyntaxError:
         return False
 
-    if not isinstance(module, Module):
-        return False
     statements = module.body
     if not len(statements) == 1:
-        return False
+        return False  # type: ignore[unreachable]
     expression = statements[0]
     if expression.__class__.__name__ != "Expr":
         return False
 
     for ast_node in walk(expression):
         ast_node_class = ast_node.__class__.__name__
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff2bed.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff2bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gff_to_bed_converter.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff_to_bed_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                         #
                         # No transcript ID, so write last transcript and write current line as its own line.
                         #
 
                         # Write previous transcript.
                         if cur_transcript_id:
                             # Write BED entry.
-                            out.write(
+                            out.write(  # type: ignore[unreachable]
                                 get_bed_line(
                                     cur_transcript_chrome,
                                     cur_transcript_id,
                                     cur_transcript_strand,
                                     cur_transcripts_blocks,
                                 )
                             )
@@ -116,15 +116,15 @@
                     # Line is part of new transcript; write previous transcript and start
                     # new transcript.
                     #
 
                     # Write previous transcript.
                     if cur_transcript_id:
                         # Write BED entry.
-                        out.write(
+                        out.write(  # type: ignore[unreachable]
                             get_bed_line(
                                 cur_transcript_chrome, cur_transcript_id, cur_transcript_strand, cur_transcripts_blocks
                             )
                         )
 
                     # Start new transcript.
                     cur_transcript_chrome = elems[0]
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/grep.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/grep.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/grep_1.0.1.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep_1.0.1.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gtf2bedgraph.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gtf2bedgraph.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/gtf_to_bedgraph_converter.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gtf_to_bedgraph_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/headWrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/headWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/join.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/join.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/joinWrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/joinWrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/joiner.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/joiner.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/joiner2.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/joiner2.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/lav_to_bed.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/lav_to_bed.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/lav_to_bed_code.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed_code.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/mergeCols.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/mergeCols.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/mergeCols.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/mergeCols.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/pasteWrapper.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/pasteWrapper.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/pasteWrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/pasteWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/random_lines_two_pass.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/random_lines_two_pass.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/randomlines.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/randomlines.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/randomlines.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/randomlines.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/remove_beginning.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/remove_beginning.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/remove_beginning.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/remove_beginning.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/secure_hash_message_digest.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/secure_hash_message_digest.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/secure_hash_message_digest.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/secure_hash_message_digest.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/sff_extract.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/sff_extract.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/sff_extractor.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/sff_extractor.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/sorter.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
     Sorts tabular data on one or more columns. All comments of the file are collected
     and placed at the beginning of the sorted output file.
 """
+
 # 03/05/2013 guerler
 
 import argparse
 import subprocess
 import sys
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/sorter.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/sorter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/tailWrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/tailWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/trimmer.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/trimmer.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/trimmer.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/trimmer.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/uniq.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/uniq.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/uniq.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/uniq.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/wc_gnu.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/wc_gnu.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/wig_to_bigwig.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/wig_to_bigwig.xml`

 * *Files 1% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/wig_to_bigwig.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/wig_to_bigwig.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool id="wig_to_bigWig" name="Wig/BedGraph-to-bigWig" version="1.1.1">
+<tool id="wig_to_bigWig" name="Wig/BedGraph-to-bigWig" version="1.1.1" hidden="true">
   <description>converter</description>
   <requirements>
     <requirement type="package" version="357">ucsc-wigtobigwig</requirement>
   </requirements>
   <stdio>
     <!-- Anything other than zero is an error -->
     <regex match="needLargeMem: trying to allocate 0 bytes" description="Your input file might be empty or wrongly formatted"/>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/wiggle_to_simple.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/wiggle_to_simple.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/filters/wiggle_to_simple.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/filters/wiggle_to_simple.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/default_notebook.ipynb` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/default_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_askomics.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_askomics.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_bam_iobio.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_bam_iobio.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_cellxgene_0.16.2.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_cellxgene_0.16.2.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_cellxgene_1.1.1.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_cellxgene_1.1.1.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_climate_notebook.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_climate_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_ethercalc.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_ethercalc.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_geoexplorer.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_geoexplorer.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_guacamole_desktop.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_guacamole_desktop.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_hicbrowser.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_hicbrowser.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_higlass.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_higlass.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_isee.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_isee.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook_1.0.0.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook_1.0.0.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_metashark.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_metashark.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_mgnify_notebook.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_mgnify_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_ml_jupyter_notebook.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_ml_jupyter_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_neo4j.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_neo4j.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_openrefine.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_openrefine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_pangeo_notebook.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pangeo_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_panoply.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_panoply.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_paraview.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_paraview.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_pavian.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pavian.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_phinch.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_phinch.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_pyiron.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pyiron.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_radiant.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_radiant.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml`

 * *Files 6% similar despite different names*

#### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml`

```diff
@@ -1,12 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<tool id="interactive_tool_rstudio" tool_type="interactive" name="RStudio" version="0.2" profile="22.01">
+<tool id="interactive_tool_rstudio" tool_type="interactive" name="RStudio" version="0.3" profile="22.01">
   <requirements>
-    <!--container type="docker">quay.io/erasche/docker-rstudio-notebook:19.09</container-->
-    <container type="docker">quay.io/erasche/docker-rstudio-notebook:ie2</container>
+    <container type="docker">quay.io/galaxy/docker-rstudio-notebook:23.1</container>
   </requirements>
   <entry_points>
     <entry_point name="RStudio" requires_domain="False" requires_path_in_header_named="X-RStudio-Root-Path">
       <port>8787</port>
       <url>/</url>
     </entry_point>
   </entry_points>
@@ -16,31 +15,26 @@
     <environment_variable name="GALAXY_WEB_PORT">8080</environment_variable>
     <environment_variable name="GALAXY_URL">$__galaxy_url__</environment_variable>
     <environment_variable name="DEBUG">true</environment_variable>
     <environment_variable name="DISABLE_AUTH">true</environment_variable>
     <environment_variable name="API_KEY" inject="api_key"/>
   </environment_variables>
   <command><![CDATA[
-        #import re
         export GALAXY_WORKING_DIR=`pwd` &&
         mkdir -p ./rstudio/outputs/ &&
         mkdir -p ./rstudio/data &&
 
         ## change into the directory where the notebooks are located
         cd ./rstudio/ &&
 
-        sed -i 's|/monitor.*||g' /etc/services.d/nginx/run &&
-
-        ##/etc/init.d/syslog-ng start &&
         /init &
-        ##rstudio-server start &&
         sleep 5 &&
 
         chmod 777 /tmp -R &&
-        tail -f /var/log/rstudio-server/rserver.log
+        tail --retry -f /var/log/rstudio/rstudio-server/rserver.log
 
     ]]></command>
   <inputs>
     <!--<param name="input" type="data" optional="true" label="Include data into the environment"/>-->
   </inputs>
   <outputs>
     <data name="jupyter_notebook" format="ipynb" label=""/>
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_simtext_app.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_simtext_app.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_vcf_iobio.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_vcf_iobio.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_vrm_editor.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_vrm_editor.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_wallace.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_wallace.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/interactivetool_wilson.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_wilson.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/interactive/simtext_app.R` & `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/simtext_app.R`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/genebed_maf_to_fasta.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/genebed_maf_to_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval2maf.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval2maf.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval2maf_pairwise.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf_pairwise.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_by_block_number.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_by_block_number.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_by_block_number.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_by_block_number.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_filter.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_filter.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_filter.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_filter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_limit_size.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_size.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_limit_size.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_size.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_limit_to_species.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_to_species.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_limit_to_species.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_to_species.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_reverse_complement.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_reverse_complement.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_reverse_complement.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_reverse_complement.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_split_by_species.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_split_by_species.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_split_by_species.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_split_by_species.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_stats.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_stats.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_stats.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_stats.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_thread_for_species.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_thread_for_species.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_thread_for_species.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_thread_for_species.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_bed.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_bed.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_bed_code.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed_code.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_fasta.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_fasta_concat.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta_concat.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_fasta_multiple_sets.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta_multiple_sets.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_interval.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_interval.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/maf_to_interval.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_interval.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/meme/fimo.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/meme/fimo.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/meme/fimo_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/meme/fimo_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/meme/meme.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/meme/meme.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/blat_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/blat_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/blat_wrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/blat_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/shrimp_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/metag_tools/shrimp_wrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/bwa_solid2fastq_modified.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/bwa_solid2fastq_modified.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/solid2fastq.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid2fastq.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     quality_string = quality_string.rstrip(" ")
     for qv in quality_string.split(" "):
         try:
             if int(qv) < 0:
                 qv = "0"
             if int(qv) < min_qual:
                 return False
-                break
             sanger += chr(int(qv) + 33)
         except Exception:
             pass
     return sanger
 
 
 def Translator(frm="", to="", delete=""):
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/solid2fastq.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid2fastq.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/ngs_simulation/ngs_simulation.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/ngs_simulation.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/ngs_simulation/ngs_simulation.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/ngs_simulation.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/BEAM2_wrapper.sh` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/BEAM2_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/beam.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/beam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/gpass.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/gpass.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/gpass.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/gpass.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/ldtools.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/ldtools.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/ldtools_wrapper.sh` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/ldtools_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/linkToDavid.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToDavid.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/linkToDavid.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToDavid.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/linkToGProfile.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToGProfile.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/linkToGProfile.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToGProfile.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/lped_to_geno.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lped_to_geno.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/lps.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lps.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/lps_tool_wrapper.sh` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lps_tool_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/master2gd_snp.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2gd_snp.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/master2gd_snp.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2gd_snp.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/master2pg.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2pg.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/master2pg.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2pg.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/mergeSnps.pl` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/mergeSnps.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/pagetag.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pagetag.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/pass.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pass.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/senatag.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/senatag.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/sift.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/sift.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/phenotype_association/sift_variants_wrapper.sh` & `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/sift_variants_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/plotting/bar_chart.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/plotting/bar_chart.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/plotting/bar_chart.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/plotting/bar_chart.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/plotting/boxplot.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/plotting/boxplot.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/qualsolid_boxplot_graph.sh` & `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/qualsolid_boxplot_graph.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/solid_qual_boxplot.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_boxplot.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/solid_qual_stats.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_stats.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/solid_tools/solid_qual_stats.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_stats.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/velvetg.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velvetg.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/velvetg_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velvetg_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/velveth.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velveth.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_assembly/velveth_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velveth_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/PerM.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/PerM.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/bfast_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/bfast_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/bfast_wrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/bfast_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/fastq_statistics.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/fastq_statistics.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/mosaik.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/mosaik.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/srma_wrapper.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/srma_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/sr_mapping/srma_wrapper.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/srma_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/aggregate_binned_scores_in_intervals.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/aggregate_binned_scores_in_intervals.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/aggregate_scores_in_intervals.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/aggregate_scores_in_intervals.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/filtering.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     print_function,
 )
 
 import json
 import re
 import sys
 from ast import (
-    Module,
     parse,
     walk,
 )
 
 AST_NODE_TYPE_WHITELIST = [
     "Expr",
     "Load",
@@ -135,16 +134,14 @@
     True
     """
     try:
         module = parse(text)
     except SyntaxError:
         return False
 
-    if not isinstance(module, Module):
-        return False
     statements = module.body
     if not len(statements) == 1:
         return False
     expression = statements[0]
     if expression.__class__.__name__ != "Expr":
         return False
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/filtering.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/filtering_1_1_0.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering_1_1_0.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/grouping.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/grouping.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/grouping.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/grouping.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/gsummary.py` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/gsummary.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/gsummary.xml` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/gsummary.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/bundled/stats/r_wrapper.sh` & `galaxy-app-24.0.0/galaxy/tools/bundled/stats/r_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/cache.py` & `galaxy-app-24.0.0/galaxy/tools/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -267,31 +267,21 @@
         self.path = path
         self._modtime = modtime or os.path.getmtime(path)
         self._tool_hash = None
         if not lazy_hash:
             self.hash  # noqa: B018
 
     def modtime_less_than(self, other_modtime: float):
-        if self._modtime is None:
-            # For the purposes of the tool cache,
-            # if we haven't seen the modtime we consider it not equal
-            return True
         return self._modtime < other_modtime
 
     def hash_equals(self, other_hash: Optional[str]):
-        if self._tool_hash is None or other_hash is None:
-            # For the purposes of the tool cache,
-            # if we haven't seen the hash yet we consider it not equal
-            return False
         return self.hash == other_hash
 
     @property
     def modtime(self) -> float:
-        if self._modtime is None:
-            self._modtime = os.path.getmtime(self.path)
         return self._modtime
 
     @modtime.setter
     def modtime(self, new_value: float):
         self._modtime = new_value
 
     @property
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/data/__init__.py` & `galaxy-app-24.0.0/galaxy/tools/data/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/data_fetch.py` & `galaxy-app-24.0.0/galaxy/tools/data_fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,17 +86,16 @@
 
 
 def _fetch_target(upload_config: "UploadConfig", target):
     destination = target.get("destination", None)
     assert destination, "No destination defined."
 
     def expand_elements_from(target_or_item):
-        elements_from = target_or_item.get("elements_from", None)
         items = None
-        if elements_from:
+        if elements_from := target_or_item.get("elements_from", None):
             if elements_from == "archive":
                 decompressed_directory = _decompress_target(upload_config, target_or_item)
                 items = _directory_to_items(decompressed_directory)
             elif elements_from == "bagit":
                 _, elements_from_path = _has_src_to_path(upload_config, target_or_item, is_dataset=False)
                 items = _bagit_to_items(elements_from_path)
             elif elements_from == "bagit_archive":
@@ -135,19 +134,18 @@
     if "name" in target:
         fetched_target["name"] = target["name"]
 
     def _copy_and_validate_simple_attributes(src_item, target_metadata):
         info = src_item.get("info", None)
         created_from_basename = src_item.get("created_from_basename", None)
         tags = src_item.get("tags", [])
-        object_id = src_item.get("object_id", None)
 
         if info is not None:
             target_metadata["info"] = info
-        if object_id is not None:
+        if (object_id := src_item.get("object_id", None)) is not None:
             target_metadata["object_id"] = object_id
         if tags:
             target_metadata["tags"] = tags
         if created_from_basename:
             target_metadata["created_from_basename"] = created_from_basename
         if "error_message" in src_item:
             target_metadata["error_message"] = src_item["error_message"]
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/data_fetch.xml` & `galaxy-app-24.0.0/galaxy/tools/data_fetch.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/data_manager/manager.py` & `galaxy-app-24.0.0/galaxy/tools/data_manager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     managed_data_tables: Dict[str, "DataManager"]
     __reload_count: int
 
     def __init__(self, app: StructuredApp, xml_filename=None, reload_count: Optional[int] = None):
         self.app = app
         self.data_managers = {}
         self.managed_data_tables = {}
-        self.tool_path = None
+        self.tool_path: Optional[str] = None
         self.__reload_count = reload_count or 0
         self.filename = xml_filename or self.app.config.data_manager_config_file
         for filename in util.listify(self.filename):
             if not filename:
                 continue
             self.load_from_xml(filename)
         if self.app.config.shed_data_manager_config_file:
@@ -139,21 +139,21 @@
 
 class DataManager:
     GUID_TYPE = "data_manager"
     DEFAULT_VERSION = "0.0.1"
 
     tool: Optional[Tool]
 
-    def __init__(self, data_managers: DataManagers, elem: Element = None, tool_path: Optional[str] = None):
+    def __init__(self, data_managers: DataManagers, elem: Optional[Element] = None, tool_path: Optional[str] = None):
         self.data_managers = data_managers
-        self.declared_id = None
-        self.name = None
-        self.description = None
+        self.declared_id: Optional[str] = None
+        self.name: Optional[str] = None
+        self.description: Optional[str] = None
         self.version = self.DEFAULT_VERSION
-        self.guid = None
+        self.guid: Optional[str] = None
         self.tool = None
         self.tool_shed_repository_info: Optional[RepoInfo] = None
         self.undeclared_tables = False
         if elem is not None:
             self._load_from_element(elem, tool_path or self.data_managers.tool_path)
 
     def _load_from_element(self, elem: Element, tool_path: Optional[str]) -> None:
@@ -265,8 +265,8 @@
     def repo_info(self) -> Optional[RepoInfo]:
         return self.tool_shed_repository_info
 
     # legacy stuff because tool shed code calls this...
     # data manager manual integration test provides coverage
     def get_tool_shed_repository_info_dict(self) -> Optional[dict]:
         repo_info = self.repo_info
-        return repo_info.dict() if repo_info else None
+        return repo_info.model_dump(mode="json") if repo_info else None
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/duplicate_file_to_collection.xml` & `galaxy-app-24.0.0/galaxy/tools/duplicate_file_to_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/__init__.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module defines the error reporting framework for Galaxy jobs.
 """
+
 import collections
 import logging
 import os
 
 from galaxy.util import plugin_config
 
 log = logging.getLogger(__name__)
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/__init__.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module describes the abstract interface for :class:`InstrumentPlugin`.
 
 These are responsible for collecting and formatting a coherent set of metrics.
 """
+
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 
 
 class ErrorPlugin(metaclass=ABCMeta):
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/base_git.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/base_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """This module defines the common functions for error reporting for Galaxy jobs towards Git applications (e.g. Github/GitLab).
 """
 
-
 import logging
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 from typing import Dict
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/email.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/email.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/github.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/github.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/gitlab.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/gitlab.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,16 +243,15 @@
         return gitlab_projecturl
 
     def _create_issue(self, issue_cache_key, error_title, error_message, project, **kwargs):
         # Set payload for the issue
         issue_data = {"title": error_title, "description": error_message}
 
         # Assign the user to the issue
-        gl_userid = kwargs.get("gl_userid", None)
-        if gl_userid is not None:
+        if (gl_userid := kwargs.get("gl_userid", None)) is not None:
             issue_data["assignee_ids"] = [gl_userid]
 
         # Create the issue on GitLab
         issue = project.issues.create(issue_data)
 
         # Set labels
         issue.labels = self.gitlab_labels
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/influxdb.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/influxdb.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/json.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/json.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/sentry.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/sentry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The module describes the ``sentry`` error plugin."""
+
 import logging
 from typing import Dict
 
 try:
     import sentry_sdk
 except ImportError:
     sentry_sdk = None
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/error_reports/plugins/slack.py` & `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The module describes the ``slack`` error plugin plugin."""
+
 import logging
 import uuid
 from typing import (
     Any,
     Dict,
 )
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/errors.py` & `galaxy-app-24.0.0/galaxy/tools/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functionality for dealing with tool errors.
 """
+
 import string
 
 import markupsafe
 
 from galaxy import (
     model,
     util,
@@ -249,10 +250,17 @@
         try:
             subject = "{} ({})".format(
                 subject, self.app.toolbox.get_tool(self.job.tool_id, self.job.tool_version).old_id
             )
         except Exception:
             pass
 
+        reply_to = user.email if user else None
         return util.send_mail(
-            self.app.config.email_from, to, subject, self.report, self.app.config, html=self.html_report
+            self.app.config.email_from,
+            to,
+            subject,
+            self.report,
+            self.app.config,
+            html=self.html_report,
+            reply_to=reply_to,
         )
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/evaluation.py` & `galaxy-app-24.0.0/galaxy/tools/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     Callable,
     Dict,
     List,
     Optional,
     Union,
 )
 
+from packaging.version import Version
+
 from galaxy import model
 from galaxy.authnz.util import provider_name_to_backend
 from galaxy.job_execution.compute_environment import ComputeEnvironment
 from galaxy.job_execution.setup import ensure_configs_directory
 from galaxy.model.deferred import (
     materialize_collection_input,
     materializer_factory,
@@ -403,15 +405,15 @@
                 # variables
                 if matches is None:
                     matches = find_instance_nested(param_dict, instances=(DatasetFilenameWrapper, DatasetListWrapper))
                 wrapper = matches.get(name)
                 if wrapper:
                     param_dict[name] = wrapper
                     continue
-            if not isinstance(param_dict_value, (DatasetFilenameWrapper, DatasetListWrapper)):
+            if not isinstance(param_dict_value, ToolParameterValueWrapper):
                 wrapper_kwds = dict(
                     datatypes_registry=self.app.datatypes_registry,
                     tool=self.tool,
                     name=name,
                     compute_environment=self.compute_environment,
                 )
                 param_dict[name] = DatasetFilenameWrapper(data, **wrapper_kwds)
@@ -562,17 +564,17 @@
         skip = ["chromInfo"] + list(self.tool.template_macro_params.keys())
         if not self.tool or not self.tool.options or self.tool.options.sanitize:
             for key, value in list(param_dict.items()):
                 if key not in skip:
                     # Remove key so that new wrapped object will occupy key slot
                     del param_dict[key]
                     # And replace with new wrapped key
-                    param_dict[
-                        wrap_with_safe_string(key, no_wrap_classes=ToolParameterValueWrapper)
-                    ] = wrap_with_safe_string(value, no_wrap_classes=ToolParameterValueWrapper)
+                    param_dict[wrap_with_safe_string(key, no_wrap_classes=ToolParameterValueWrapper)] = (
+                        wrap_with_safe_string(value, no_wrap_classes=ToolParameterValueWrapper)
+                    )
 
     def build(self):
         """
         Build runtime description of job to execute, evaluate command and
         config templates corresponding to this tool with these inputs on this
         compute environment.
         """
@@ -624,16 +626,15 @@
             executable = command_line.split()[0]
             tool_dir = os.path.abspath(self.tool.tool_dir)
             abs_executable = os.path.join(tool_dir, executable)
             command_line = command_line.replace(executable, f"{interpreter} {shlex.quote(abs_executable)}", 1)
         self.command_line = command_line
 
     def _build_version_command(self):
-        version_string_cmd_raw = self.tool.version_string_cmd
-        if version_string_cmd_raw:
+        if version_string_cmd_raw := self.tool.version_string_cmd:
             version_command_template = string.Template(version_string_cmd_raw)
             version_command = version_command_template.safe_substitute(
                 {"__tool_directory__": self.compute_environment.tool_directory()}
             )
             self.version_command_line = f"{version_command} > {self.compute_environment.version_path()} 2>&1;\n"
 
     def _build_config_files(self):
@@ -698,27 +699,25 @@
                 environment_variable_template,
                 param_dict,
                 is_template=is_template,
                 strip=environment_variable_def.get("strip", False),
             )
             config_file_basename = os.path.basename(config_filename)
             # environment setup in job file template happens before `cd $working_directory`
-            environment_variable[
-                "value"
-            ] = f'`cat "{self.compute_environment.env_config_directory()}/{config_file_basename}"`'
+            environment_variable["value"] = (
+                f'`cat "{self.compute_environment.env_config_directory()}/{config_file_basename}"`'
+            )
             environment_variable["raw"] = True
             environment_variable["job_directory_path"] = config_filename
             environment_variables.append(environment_variable)
 
-        home_dir = self.compute_environment.home_directory()
-        tmp_dir = self.compute_environment.tmp_directory()
-        if home_dir:
+        if home_dir := self.compute_environment.home_directory():
             environment_variable = dict(name="HOME", value=f'"{home_dir}"', raw=True)
             environment_variables.append(environment_variable)
-        if tmp_dir:
+        if tmp_dir := self.compute_environment.tmp_directory():
             for tmp_directory_var in self.tool.tmp_directory_vars:
                 environment_variable = dict(name=tmp_directory_var, value=f'"{tmp_dir}"', raw=True)
                 environment_variables.append(environment_variable)
 
     def get_oidc_token(self, inject):
         if not self._user:
             return "token-unavailable"
@@ -740,15 +739,15 @@
     def _build_param_file(self):
         """
         Build temporary file for file based parameter transfer if needed
         """
         param_dict = self.param_dict
         directory = self.local_working_directory
         command = self.tool.command
-        if self.tool.profile < 16.04 and command and "$param_file" in command:
+        if Version(str(self.tool.profile)) < Version("16.04") and command and "$param_file" in command:
             with tempfile.NamedTemporaryFile(mode="w", dir=directory, delete=False) as param:
                 for key, value in param_dict.items():
                     # parameters can be strings or lists of strings, coerce to list
                     if not isinstance(value, list):
                         value = [value]
                     for elem in value:
                         param.write(f"{key}={elem}\n")
@@ -817,16 +816,15 @@
 
     @property
     def _history(self):
         return self.job.history
 
     @property
     def _user(self):
-        history = self._history
-        if history:
+        if history := self._history:
             return history.user
         else:
             return self.job.user
 
 
 class PartialToolEvaluator(ToolEvaluator):
     """
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/execute.py` & `galaxy-app-24.0.0/galaxy/tools/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Once state information has been calculated, handle actually executing tools
 from various states, tracking results, and building implicit dataset
 collections from matched collections.
 """
+
 import collections
 import logging
 import typing
 from abc import abstractmethod
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     NamedTuple,
     Optional,
 )
 
 from boltons.iterutils import remap
+from packaging.version import Version
 
 from galaxy import model
 from galaxy.exceptions import ToolInputsNotOKException
 from galaxy.model.base import transaction
 from galaxy.model.dataset_collections.matching import MatchingCollections
 from galaxy.model.dataset_collections.structure import (
     get_structure,
@@ -136,16 +138,15 @@
                 datasets = [pair[1] for pair in result if type(pair[1]) in instance_types]
                 if datasets:
                     job_datasets[job] = datasets
         else:
             execution_tracker.record_error(result)
 
     tool_action = tool.tool_action
-    check_inputs_ready = getattr(tool_action, "check_inputs_ready", None)
-    if check_inputs_ready:
+    if check_inputs_ready := getattr(tool_action, "check_inputs_ready", None):
         for params in execution_tracker.param_combinations:
             # This will throw an exception if the tool is not ready.
             try:
                 check_inputs_ready(
                     tool,
                     trans,
                     params,
@@ -170,19 +171,14 @@
             break
         else:
             skip = execution_slice.param_combination.pop("__when_value__", None) is False
             execute_single_job(execution_slice, completed_jobs[i], skip=skip)
             history = execution_slice.history or history
             jobs_executed += 1
 
-    if job_datasets:
-        for job, datasets in job_datasets.items():
-            for dataset_instance in datasets:
-                dataset_instance.dataset.job = job
-
     if execution_slice:
         history.add_pending_items()
     # Make sure collections, implicit jobs etc are flushed even if there are no precreated output datasets
     with transaction(trans.sa_session):
         trans.sa_session.commit()
 
     tool_id = tool.id
@@ -306,15 +302,15 @@
             )
         except Exception:
             output_collection_name = f"{self.tool.name} across {on_text}"
 
         return output_collection_name
 
     def sliced_input_collection_structure(self, input_name):
-        unqualified_recurse = self.tool.profile < 18.09 and "|" not in input_name
+        unqualified_recurse = Version(str(self.tool.profile)) < Version("18.09") and "|" not in input_name
 
         def find_collection(input_dict, input_name):
             for key, value in input_dict.items():
                 if key == input_name:
                     return value
                 if isinstance(value, dict):
                     if "|" in input_name:
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/expressions/cwlNodeEngine.js` & `galaxy-app-24.0.0/galaxy/tools/expressions/cwlNodeEngine.js`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/expressions/evaluation.py` & `galaxy-app-24.0.0/galaxy/tools/expressions/evaluation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 import json
 import os
 import subprocess
+from typing import MutableMapping
+
+from cwl_utils.expression import do_eval as _do_eval
 
 from .util import find_engine
 
 FILE_DIRECTORY = os.path.normpath(os.path.dirname(os.path.join(__file__)))
 NODE_ENGINE = os.path.join(FILE_DIRECTORY, "cwlNodeEngine.js")
 
 
+def do_eval(expression: str, context: MutableMapping):
+    return _do_eval(
+        expression,
+        context,
+        [{"class": "InlineJavascriptRequirement"}],
+        None,
+        None,
+        {},
+        cwlVersion="v1.2.1",
+    )
+
+
 def evaluate(config, input):
     application = find_engine(config)
 
     default_context = {
         "engineConfig": [],
         "job": {},
         "context": None,
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/extract_dataset.xml` & `galaxy-app-24.0.0/galaxy/tools/extract_dataset.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/filter_empty_collection.xml` & `galaxy-app-24.0.0/galaxy/tools/filter_empty_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/filter_failed_collection.xml` & `galaxy-app-24.0.0/galaxy/tools/filter_failed_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/filter_from_file.xml` & `galaxy-app-24.0.0/galaxy/tools/filter_from_file.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/flatten_collection.xml` & `galaxy-app-24.0.0/galaxy/tools/flatten_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/imp_exp/__init__.py` & `galaxy-app-24.0.0/galaxy/tools/imp_exp/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/imp_exp/exp_history_to_archive.xml` & `galaxy-app-24.0.0/galaxy/tools/imp_exp/exp_history_to_archive.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/imp_exp/exp_history_to_uri.xml` & `galaxy-app-24.0.0/galaxy/tools/imp_exp/exp_history_to_uri.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/imp_exp/export_history.py` & `galaxy-app-24.0.0/galaxy/tools/imp_exp/export_history.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,17 +36,14 @@
     parser = optparse.OptionParser()
     parser.add_option("-G", "--gzip", dest="gzip", action="store_true", help="Compress archive using gzip.")
     parser.add_option(
         "--galaxy-version", dest="galaxy_version", help="Galaxy version that initiated the command.", default=None
     )
     parser.add_option("--file-sources", type=str, help="file sources json")
     (options, args) = parser.parse_args(argv)
-    galaxy_version = options.galaxy_version
-    if galaxy_version is None:
-        galaxy_version = "19.05"
 
     gzip = bool(options.gzip)
     assert len(args) >= 2
     temp_directory = args[0]
     out_arg = args[1]
 
     destination_uri = None
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/imp_exp/imp_history_from_archive.xml` & `galaxy-app-24.0.0/galaxy/tools/imp_exp/imp_history_from_archive.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/imp_exp/unpack_tar_gz_archive.py` & `galaxy-app-24.0.0/galaxy/tools/imp_exp/unpack_tar_gz_archive.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/merge_collection.xml` & `galaxy-app-24.0.0/galaxy/tools/merge_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/__init__.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/basic.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 
 import contextlib
 import json
 import logging
 import os
 import os.path
 import re
+import typing
 import urllib.parse
+from collections.abc import MutableMapping
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     Tuple,
     TYPE_CHECKING,
     Union,
 )
 
+from packaging.version import Version
 from webob.compat import cgi_FieldStorage
 
 from galaxy import util
 from galaxy.files import ProvidesUserFileSourcesUserContext
 from galaxy.managers.dbkeys import read_dbnames
 from galaxy.model import (
     cached_id,
@@ -35,14 +38,15 @@
     HistoryDatasetAssociation,
     HistoryDatasetCollectionAssociation,
     LibraryDatasetDatasetAssociation,
 )
 from galaxy.model.dataset_collections import builder
 from galaxy.schema.fetch_data import FilesPayload
 from galaxy.tool_util.parser import get_input_source as ensure_input_source
+from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
 from galaxy.util import (
     sanitize_param,
     string_as_bool,
     string_as_bool_or_none,
     unicodify,
     XML,
 )
@@ -62,20 +66,14 @@
     from sqlalchemy.orm import Session
 
     from galaxy.security.idencoding import IdEncodingHelper
 
 log = logging.getLogger(__name__)
 
 
-class workflow_building_modes:
-    DISABLED = False
-    ENABLED = True
-    USE_HISTORY = 1
-
-
 WORKFLOW_PARAMETER_REGULAR_EXPRESSION = re.compile(r"\$\{.+?\}")
 
 
 class ImplicitConversionRequired(Exception):
     pass
 
 
@@ -87,15 +85,15 @@
     if not search and WORKFLOW_PARAMETER_REGULAR_EXPRESSION.match(value):
         return True
     return False
 
 
 def is_runtime_value(value):
     return isinstance(value, RuntimeValue) or (
-        isinstance(value, dict) and value.get("__class__") in ["RuntimeValue", "ConnectedValue"]
+        isinstance(value, MutableMapping) and value.get("__class__") in ["RuntimeValue", "ConnectedValue"]
     )
 
 
 def is_runtime_context(trans, other_values):
     if trans.workflow_building_mode:
         return True
     for context_value in other_values.values():
@@ -106,16 +104,15 @@
                 (hasattr(v, "state") and v.state != Dataset.states.OK) or hasattr(v, "implicit_conversion")
             ):
                 return True
     return False
 
 
 def parse_dynamic_options(param, input_source):
-    options_elem = input_source.parse_dynamic_options_elem()
-    if options_elem is not None:
+    if (options_elem := input_source.parse_dynamic_options_elem()) is not None:
         return dynamic_options.DynamicOptions(options_elem, param)
     return None
 
 
 # Describe a parameter value error where there is no actual supplied
 # parameter - e.g. just a specification issue.
 NO_PARAMETER_VALUE = object()
@@ -176,16 +173,15 @@
         self.hidden = input_source.get_bool("hidden", False)
         self.refresh_on_change = input_source.get_bool("refresh_on_change", False)
         self.optional = input_source.parse_optional()
         self.optionality_inferred = False
         self.is_dynamic = False
         self.label = input_source.parse_label()
         self.help = input_source.parse_help()
-        sanitizer_elem = input_source.parse_sanitizer_elem()
-        if sanitizer_elem is not None:
+        if (sanitizer_elem := input_source.parse_sanitizer_elem()) is not None:
             self.sanitizer = ToolParameterSanitizer.from_element(sanitizer_elem)
         else:
             self.sanitizer = None
         self.validators = []
         for elem in input_source.parse_validator_elems():
             self.validators.append(validation.Validator.from_element(self, elem))
 
@@ -240,15 +236,15 @@
 
     def value_from_basic(self, value, app, ignore_errors=False):
         # Handle Runtime and Unvalidated values
         if is_runtime_value(value):
             if isinstance(self, HiddenToolParameter):
                 raise ParameterValueError(message_suffix="Runtime Parameter not valid", parameter_name=self.name)
             return runtime_to_object(value)
-        elif isinstance(value, dict) and value.get("__class__") == "UnvalidatedValue":
+        elif isinstance(value, MutableMapping) and value.get("__class__") == "UnvalidatedValue":
             return value["value"]
         # Delegate to the 'to_python' method
         if ignore_errors:
             try:
                 return self.to_python(value, app)
             except Exception:
                 return value
@@ -590,15 +586,15 @@
     """
 
     def __init__(self, tool, input_source):
         input_source = ensure_input_source(input_source)
         super().__init__(tool, input_source)
         truevalue = input_source.get("truevalue", "true")
         falsevalue = input_source.get("falsevalue", "false")
-        if tool and tool.profile >= 23.1:
+        if tool and Version(str(tool.profile)) >= Version("23.1"):
             if truevalue == falsevalue:
                 raise ParameterValueError("Cannot set true and false to the same value", self.name)
             if truevalue.lower() == "false":
                 raise ParameterValueError(
                     f"Cannot set truevalue to [{truevalue}], Galaxy state may encounter issues distinguishing booleans and strings in this case.",
                     self.name,
                 )
@@ -665,16 +661,16 @@
         super().__init__(tool, input_source)
 
     def from_json(self, value, trans=None, other_values=None):
         # Middleware or proxies may encode files in special ways (TODO: this
         # should be pluggable)
         if isinstance(value, FilesPayload):
             # multi-part upload handled and persisted in service layer
-            return value.dict()
-        elif isinstance(value, dict):
+            return value.model_dump()
+        elif isinstance(value, MutableMapping):
             if "session_id" in value:
                 # handle api upload
                 session_id = value["session_id"]
                 upload_store = trans.app.config.tus_upload_store or trans.app.config.new_file_path
                 if re.match(r"^[\w-]+$", session_id) is None:
                     raise ValueError("Invalid session id format.")
                 local_filename = os.path.abspath(os.path.join(upload_store, session_id))
@@ -698,15 +694,15 @@
         return "multipart/form-data"
 
     def to_json(self, value, app, use_security):
         if value in [None, ""]:
             return None
         elif isinstance(value, str):
             return value
-        elif isinstance(value, dict):
+        elif isinstance(value, MutableMapping):
             # or should we jsonify?
             try:
                 return value["local_filename"]
             except KeyError:
                 return None
         elif isinstance(value, cgi_FieldStorage):
             return value.file.name
@@ -772,15 +768,15 @@
         if not isinstance(value, list):
             value = [value]
         lst: List[str] = []
         for val in value:
             if val in [None, ""]:
                 lst = []
                 break
-            if isinstance(val, dict):
+            if isinstance(val, MutableMapping):
                 lst.append(val["name"])
             else:
                 lst.append(val)
         if len(lst) == 0:
             if not self.optional and validate:
                 raise ValueError("Please select a valid FTP file.")
             return None
@@ -977,15 +973,18 @@
         else:
             return self.static_options
 
     def get_legal_values(self, trans, other_values, value):
         """
         determine the set of values of legal options
         """
-        return {v for _, v, _ in self.get_options(trans, other_values)}
+        return {
+            history_item_dict_to_python(v, trans.app, self.name) or v
+            for _, v, _ in self.get_options(trans, other_values)
+        }
 
     def get_legal_names(self, trans, other_values):
         """
         determine a mapping from names to values for all legal options
         """
         return {n: v for n, v, _ in self.get_options(trans, other_values)}
 
@@ -1018,15 +1017,15 @@
         elif value is None:
             if self.optional:
                 return None
             raise ParameterValueError(
                 "an invalid option (None) was selected, please verify", self.name, None, is_dynamic=self.is_dynamic
             )
         elif not legal_values:
-            if self.optional and self.tool.profile < 18.09:
+            if self.optional and Version(str(self.tool.profile)) < Version("18.09"):
                 # Covers optional parameters with default values that reference other optional parameters.
                 # These will have a value but no legal_values.
                 # See https://github.com/galaxyproject/tools-iuc/pull/1842#issuecomment-394083768 for context.
                 return None
             raise ParameterValueError(
                 "requires a value, but no legal values defined", self.name, is_dynamic=self.is_dynamic
             )
@@ -1092,16 +1091,21 @@
             else:
                 value = sanitize_param(value)
         if isinstance(value, list):
             value = self.separator.join(value)
         return value
 
     def to_json(self, value, app, use_security):
+        if isinstance(value, HistoryDatasetAssociation):
+            return history_item_to_json(value, app, use_security=use_security)
         return value
 
+    def to_python(self, value, app):
+        return history_item_dict_to_python(value, app, self.name) or super().to_python(value, app)
+
     def get_initial_value(self, trans, other_values):
         try:
             options = list(self.get_options(trans, other_values))
         except ImplicitConversionRequired:
             return None
         if not options:
             return None
@@ -1477,28 +1481,40 @@
         return column_list
 
     def get_options(self, trans, other_values):
         """
         Show column labels rather than c1..cn if use_header_names=True
         """
         options: List[Tuple[str, Union[str, Tuple[str, str]], bool]] = []
-        if self.usecolnames:  # read first row - assume is a header with metadata useful for making good choices
+        # if available use column_names metadata for option names
+        # otherwise read first row - assume is a header with tab separated names
+        if self.usecolnames:
             dataset = other_values.get(self.data_ref, None)
-            try:
-                with open(dataset.get_file_name()) as f:
-                    head = f.readline()
-                cnames = head.rstrip("\n\r ").split("\t")
-                column_list = [("%d" % (i + 1), "c%d: %s" % (i + 1, x)) for i, x in enumerate(cnames)]
-                if self.numerical:  # If numerical was requested, filter columns based on metadata
-                    if hasattr(dataset, "metadata") and hasattr(dataset.metadata, "column_types"):
-                        if len(dataset.metadata.column_types) >= len(cnames):
-                            numerics = [i for i, x in enumerate(dataset.metadata.column_types) if x in ["int", "float"]]
-                            column_list = [column_list[i] for i in numerics]
-            except Exception:
-                column_list = self.get_column_list(trans, other_values)
+            if (
+                hasattr(dataset, "metadata")
+                and hasattr(dataset.metadata, "column_names")
+                and dataset.metadata.element_is_set("column_names")
+            ):
+                log.error(f"column_names {dataset.metadata.column_names}")
+                column_list = [
+                    ("%d" % (i + 1), "c%d: %s" % (i + 1, x)) for i, x in enumerate(dataset.metadata.column_names)
+                ]
+            else:
+                try:
+                    with open(dataset.get_file_name()) as f:
+                        head = f.readline()
+                    cnames = head.rstrip("\n\r ").split("\t")
+                    column_list = [("%d" % (i + 1), "c%d: %s" % (i + 1, x)) for i, x in enumerate(cnames)]
+                except Exception:
+                    column_list = self.get_column_list(trans, other_values)
+            if self.numerical:  # If numerical was requested, filter columns based on metadata
+                if hasattr(dataset, "metadata") and hasattr(dataset.metadata, "column_types"):
+                    if len(dataset.metadata.column_types) >= len(column_list):
+                        numerics = [i for i, x in enumerate(dataset.metadata.column_types) if x in ["int", "float"]]
+                        column_list = [column_list[i] for i in numerics]
         else:
             column_list = self.get_column_list(trans, other_values)
         for col in column_list:
             if isinstance(col, tuple) and len(col) == 2:
                 options.append((col[1], col[0], False))
             else:
                 options.append((f"Column: {col}", col, False))
@@ -1614,16 +1630,15 @@
         # TODO: abstract XML out of here - so non-XML InputSources can
         # specify DrillDown parameters.
         elem = input_source.elem()
         self.multiple = string_as_bool(elem.get("multiple", False))
         self.display = elem.get("display", None)
         self.hierarchy = elem.get("hierarchy", "exact")  # exact or recurse
         self.separator = elem.get("separator", ",")
-        from_file = elem.get("from_file", None)
-        if from_file:
+        if from_file := elem.get("from_file", None):
             if not os.path.isabs(from_file):
                 from_file = os.path.join(tool.app.config.tool_data_path, from_file)
             elem = XML(f"<root>{open(from_file).read()}</root>")
         self.dynamic_options = elem.get("dynamic_options", None)
         if self.dynamic_options:
             self.is_dynamic = True
         self.options = []
@@ -1871,19 +1886,18 @@
                 self.tool.app.datatypes_registry
             )  # can be None if self.tool.app is a ValidationContext
 
     def _parse_formats(self, trans, input_source):
         """
         Build list of classes for supported data formats
         """
-        self.extensions = input_source.get("format", "data").split(",")
+        self.extensions = [extension.strip().lower() for extension in input_source.get("format", "data").split(",")]
         formats = []
         if self.datatypes_registry:  # This may be None when self.tool.app is a ValidationContext
-            normalized_extensions = [extension.strip().lower() for extension in self.extensions]
-            for extension in normalized_extensions:
+            for extension in self.extensions:
                 datatype = self.datatypes_registry.get_datatype_by_extension(extension)
                 if datatype is not None:
                     formats.append(datatype)
                 else:
                     log.warning(
                         f"Datatype class not found for extension '{extension}', which is used in the 'format' attribute of parameter '{self.name}'"
                     )
@@ -1902,69 +1916,45 @@
         self.is_dynamic = self.options is not None
 
     def get_initial_value(self, trans, other_values):
         if trans.workflow_building_mode is workflow_building_modes.ENABLED or trans.app.name == "tool_shed":
             return RuntimeValue()
         if self.optional:
             return None
-        history = trans.history
-        if history is not None:
+        if (history := trans.history) is not None:
             dataset_matcher_factory = get_dataset_matcher_factory(trans)
             dataset_matcher = dataset_matcher_factory.dataset_matcher(self, other_values)
             if isinstance(self, DataToolParameter):
                 for hda in reversed(history.active_visible_datasets_and_roles):
                     match = dataset_matcher.hda_match(hda)
                     if match:
                         return match.hda
             else:
                 dataset_collection_matcher = dataset_matcher_factory.dataset_collection_matcher(dataset_matcher)
                 for hdca in reversed(history.active_visible_dataset_collections):
                     if dataset_collection_matcher.hdca_match(hdca):
                         return hdca
 
     def to_json(self, value, app, use_security):
-        def single_to_json(value):
-            src = None
-            if isinstance(value, dict) and "src" in value and "id" in value:
-                return value
-            elif isinstance(value, DatasetCollectionElement):
-                src = "dce"
-            elif isinstance(value, HistoryDatasetCollectionAssociation):
-                src = "hdca"
-            elif isinstance(value, LibraryDatasetDatasetAssociation):
-                src = "ldda"
-            elif isinstance(value, HistoryDatasetAssociation) or hasattr(value, "id"):
-                # hasattr 'id' fires a query on persistent objects after a flush so better
-                # to do the isinstance check. Not sure we need the hasattr check anymore - it'd be
-                # nice to drop it.
-                src = "hda"
-            if src is not None:
-                object_id = cached_id(value)
-                return {"id": app.security.encode_id(object_id) if use_security else object_id, "src": src}
 
         if value not in [None, "", "None"]:
             if isinstance(value, list) and len(value) > 0:
-                values = [single_to_json(v) for v in value]
+                values = [history_item_to_json(v, app, use_security) for v in value]
             else:
-                values = [single_to_json(value)]
+                values = [history_item_to_json(value, app, use_security)]
             return {"values": values}
         return None
 
     def to_python(self, value, app):
-        def single_to_python(value):
-            if isinstance(value, dict) and "src" in value:
-                if value["src"] not in ("hda", "dce", "ldda", "hdca"):
-                    raise ParameterValueError(f"Invalid value {value}", self.name)
-                return src_id_to_item(sa_session=app.model.context, security=app.security, value=value)
 
-        if isinstance(value, dict) and "values" in value:
+        if isinstance(value, MutableMapping) and "values" in value:
             if hasattr(self, "multiple") and self.multiple is True:
-                return [single_to_python(v) for v in value["values"]]
+                return [history_item_dict_to_python(v, app, self.name) for v in value["values"]]
             elif len(value["values"]) > 0:
-                return single_to_python(value["values"][0])
+                return history_item_dict_to_python(value["values"][0], app, self.name)
 
         # Handle legacy string values potentially stored in databases
         none_values = [None, "", "None"]
         if value in none_values:
             return None
         if isinstance(value, str) and value.find(",") > -1:
             return [
@@ -2030,15 +2020,15 @@
                 raise ValueError("At least %d datasets are required for %s" % (self.min, self.name))
         if self.max is not None:
             if self.max < dataset_count:
                 raise ValueError("At most %d datasets are required for %s" % (self.max, self.name))
 
 
 def src_id_to_item(
-    sa_session: "Session", value: Dict[str, Any], security: "IdEncodingHelper"
+    sa_session: "Session", value: typing.MutableMapping[str, Any], security: "IdEncodingHelper"
 ) -> Union[
     DatasetCollectionElement,
     HistoryDatasetAssociation,
     HistoryDatasetCollectionAssociation,
     LibraryDatasetDatasetAssociation,
 ]:
     src_to_class = {
@@ -2123,30 +2113,30 @@
             return None
         if not value and not self.optional and not self.default_object:
             raise ParameterValueError("specify a dataset of the required format / build for parameter", self.name)
         if value in [None, "None", ""]:
             if self.default_object:
                 return raw_to_galaxy(trans, self.default_object)
             return None
-        if isinstance(value, dict) and "values" in value:
+        if isinstance(value, MutableMapping) and "values" in value:
             value = self.to_python(value, trans.app)
         if isinstance(value, str) and value.find(",") > 0:
             value = [int(value_part) for value_part in value.split(",")]
         rval: List[
             Union[
                 DatasetCollectionElement,
                 HistoryDatasetAssociation,
                 HistoryDatasetCollectionAssociation,
                 LibraryDatasetDatasetAssociation,
             ]
         ] = []
         if isinstance(value, list):
             found_srcs = set()
             for single_value in value:
-                if isinstance(single_value, dict) and "src" in single_value and "id" in single_value:
+                if isinstance(single_value, MutableMapping) and "src" in single_value and "id" in single_value:
                     found_srcs.add(single_value["src"])
                     rval.append(
                         src_id_to_item(sa_session=trans.sa_session, value=single_value, security=trans.security)
                     )
                 elif isinstance(
                     single_value,
                     (
@@ -2167,15 +2157,15 @@
                 if len(found_srcs) > 1 and "hdca" in found_srcs:
                     raise ParameterValueError(
                         "if collections are supplied to multiple data input parameter, only collections may be used",
                         self.name,
                     )
         elif isinstance(value, (HistoryDatasetAssociation, LibraryDatasetDatasetAssociation)):
             rval.append(value)
-        elif isinstance(value, dict) and "src" in value and "id" in value:
+        elif isinstance(value, MutableMapping) and "src" in value and "id" in value:
             rval.append(src_id_to_item(sa_session=trans.sa_session, value=value, security=trans.security))
         elif str(value).startswith("__collection_reduce__|"):
             encoded_ids = [v[len("__collection_reduce__|") :] for v in str(value).split(",")]
             decoded_ids = map(trans.security.decode_id, encoded_ids)
             rval = []
             for decoded_id in decoded_ids:
                 hdca = session.get(HistoryDatasetCollectionAssociation, decoded_id)
@@ -2248,17 +2238,17 @@
         def visitor(prefix, input, value, parent=None):
             if isinstance(input, SelectToolParameter) and self.name in input.get_dependencies():
                 if input.is_dynamic and (
                     input.dynamic_options
                     or (not input.dynamic_options and not input.options)
                     or not input.options.converter_safe
                 ):
-                    converter_safe[
-                        0
-                    ] = False  # This option does not allow for conversion, i.e. uses contents of dataset file to generate options
+                    converter_safe[0] = (
+                        False  # This option does not allow for conversion, i.e. uses contents of dataset file to generate options
+                    )
 
         self.tool.visit_inputs(other_values, visitor)
         return False not in converter_safe
 
     def get_options_filter_attribute(self, value):
         # HACK to get around current hardcoded limitation of when a set of dynamic options is defined for a DataToolParameter
         # it always causes available datasets to be filtered by dbkey
@@ -2463,32 +2453,32 @@
             return None
         if not value and not self.optional and not self.default_object:
             raise ParameterValueError("specify a dataset collection of the correct type", self.name)
         if value in [None, "None"]:
             if self.default_object:
                 return raw_to_galaxy(trans, self.default_object)
             return None
-        if isinstance(value, dict) and "values" in value:
+        if isinstance(value, MutableMapping) and "values" in value:
             value = self.to_python(value, trans.app)
         if isinstance(value, str) and value.find(",") > 0:
             value = [int(value_part) for value_part in value.split(",")]
         elif isinstance(value, HistoryDatasetCollectionAssociation):
             rval = value
         elif isinstance(value, DatasetCollectionElement):
             # When mapping over nested collection - this parameter will receive
             # a DatasetCollectionElement instead of a
             # HistoryDatasetCollectionAssociation.
             rval = value
-        elif isinstance(value, dict) and "src" in value and "id" in value:
+        elif isinstance(value, MutableMapping) and "src" in value and "id" in value:
             if value["src"] == "hdca":
                 rval = session.get(HistoryDatasetCollectionAssociation, trans.security.decode_id(value["id"]))
         elif isinstance(value, list):
             if len(value) > 0:
                 value = value[0]
-                if isinstance(value, dict) and "src" in value and "id" in value:
+                if isinstance(value, MutableMapping) and "src" in value and "id" in value:
                     if value["src"] == "hdca":
                         rval = session.get(HistoryDatasetCollectionAssociation, trans.security.decode_id(value["id"]))
                     elif value["src"] == "dce":
                         rval = session.get(DatasetCollectionElement, trans.security.decode_id(value["id"]))
         elif isinstance(value, str):
             if value.startswith("dce:"):
                 rval = session.get(DatasetCollectionElement, int(value[len("dce:") :]))
@@ -2647,27 +2637,26 @@
         input_source = ensure_input_source(input_source)
         super().__init__(tool, input_source)
         self.data_ref = input_source.get("data_ref", None)
 
     def to_dict(self, trans, other_values=None):
         other_values = other_values or {}
         d = ToolParameter.to_dict(self, trans)
-        target_name = self.data_ref
-        if target_name in other_values:
+        if (target_name := self.data_ref) in other_values:
             target = other_values[target_name]
             if not is_runtime_value(target):
                 d["target"] = {
                     "src": "hdca" if hasattr(target, "collection") else "hda",
                     "id": trans.app.security.encode_id(target.id),
                 }
         return d
 
     def validate(self, value, trans=None):
         super().validate(value, trans=trans)
-        if not isinstance(value, dict):
+        if not isinstance(value, MutableMapping):
             raise ValueError("No rules specified for rules parameter.")
 
         if "rules" not in value:
             raise ValueError("No rules specified for rules parameter")
         mappings = value.get("mapping", None)
         if not mappings:
             raise ValueError("No column definitions defined for rules parameter.")
@@ -2786,24 +2775,24 @@
     directory_uri=DirectoryUriToolParameter,
     drill_down=DrillDownSelectToolParameter,
 )
 
 
 def runtime_to_json(runtime_value):
     if isinstance(runtime_value, ConnectedValue) or (
-        isinstance(runtime_value, dict) and runtime_value["__class__"] == "ConnectedValue"
+        isinstance(runtime_value, MutableMapping) and runtime_value["__class__"] == "ConnectedValue"
     ):
         return {"__class__": "ConnectedValue"}
     else:
         return {"__class__": "RuntimeValue"}
 
 
 def runtime_to_object(runtime_value):
     if isinstance(runtime_value, ConnectedValue) or (
-        isinstance(runtime_value, dict) and runtime_value["__class__"] == "ConnectedValue"
+        isinstance(runtime_value, MutableMapping) and runtime_value["__class__"] == "ConnectedValue"
     ):
         return ConnectedValue()
     else:
         return RuntimeValue()
 
 
 class RuntimeValue:
@@ -2812,7 +2801,34 @@
     """
 
 
 class ConnectedValue(RuntimeValue):
     """
     Wrapper to note a value that is not yet set, but will be inferred from a connection.
     """
+
+
+def history_item_dict_to_python(value, app, name):
+    if isinstance(value, MutableMapping) and "src" in value:
+        if value["src"] not in ("hda", "dce", "ldda", "hdca"):
+            raise ParameterValueError(f"Invalid value {value}", name)
+        return src_id_to_item(sa_session=app.model.context, security=app.security, value=value)
+
+
+def history_item_to_json(value, app, use_security):
+    src = None
+    if isinstance(value, MutableMapping) and "src" in value and "id" in value:
+        return value
+    elif isinstance(value, DatasetCollectionElement):
+        src = "dce"
+    elif isinstance(value, HistoryDatasetCollectionAssociation):
+        src = "hdca"
+    elif isinstance(value, LibraryDatasetDatasetAssociation):
+        src = "ldda"
+    elif isinstance(value, HistoryDatasetAssociation) or hasattr(value, "id"):
+        # hasattr 'id' fires a query on persistent objects after a flush so better
+        # to do the isinstance check. Not sure we need the hasattr check anymore - it'd be
+        # nice to drop it.
+        src = "hda"
+    if src is not None:
+        object_id = cached_id(value)
+        return {"id": app.security.encode_id(object_id) if use_security else object_id, "src": src}
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/dataset_matcher.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/dataset_matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,16 +242,15 @@
     def __valid_element(self, element):
         # Simplify things for now and assume these are hdas and not implicit
         # converts. One could imagine handling both of those cases down the
         # road.
         if element.ldda:
             return False
 
-        child_collection = element.child_collection
-        if child_collection:
+        if child_collection := element.child_collection:
             return self.dataset_collection_match(child_collection)
 
         hda = element.hda
         if not hda:
             return False
         hda_match = self.dataset_matcher.hda_match(hda, ensure_visible=False)
         return hda_match
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/dynamic_options.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/dynamic_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,45 @@
 """
 Support for generating the options for a SelectToolParameter dynamically (based
 on the values of other parameters or other aspects of the current state)
 """
+
 import copy
+import json
 import logging
 import os
 import re
+from dataclasses import dataclass
 from io import StringIO
+from typing import (
+    Any,
+    cast,
+    Dict,
+    get_args,
+    Optional,
+)
+
+from typing_extensions import Literal
 
 from galaxy.model import (
     DatasetCollectionElement,
     HistoryDatasetAssociation,
     HistoryDatasetCollectionAssociation,
     MetadataFile,
     User,
 )
-from galaxy.util import string_as_bool
+from galaxy.tools.expressions import do_eval
+from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
+from galaxy.util import (
+    Element,
+    string_as_bool,
+)
+from galaxy.util.template import fill_template
 from . import validation
+from .cancelable_request import request
 
 log = logging.getLogger(__name__)
 
 
 class Filter:
     """
     A filter takes the current options list and modifies it.
@@ -530,25 +549,25 @@
     sort_by=SortByColumnFilter,
 )
 
 
 class DynamicOptions:
     """Handles dynamically generated SelectToolParameter options"""
 
-    def __init__(self, elem, tool_param):
+    def __init__(self, elem: Element, tool_param):
         def load_from_parameter(from_parameter, transform_lines=None):
             obj = self.tool_param
             for field in from_parameter.split("."):
                 obj = getattr(obj, field)
             if transform_lines:
                 obj = eval(transform_lines, {"self": self, "obj": obj})
             return self.parse_file_fields(obj)
 
         self.tool_param = tool_param
-        self.columns = {}
+        self.columns: Dict[str, int] = {}
         self.filters = []
         self.file_fields = None
         self.largest_index = 0
         self.dataset_ref_name = None
         # True if the options generation depends on one or more other parameters
         # that are dataset inputs
         self.has_dataset_dependencies = False
@@ -560,14 +579,15 @@
         self.line_startswith = elem.get("startswith", None)
         data_file = elem.get("from_file", None)
         self.index_file = None
         self.missing_index_file = None
         dataset_file = elem.get("from_dataset", None)
         from_parameter = elem.get("from_parameter", None)
         self.tool_data_table_name = elem.get("from_data_table", None)
+        self.from_url_options = parse_from_url_options(elem)
         # Options are defined from a data table loaded by the app
         self._tool_data_table = None
         self.elem = elem
         self.column_elem = elem.find("column")
         self.tool_data_table  # noqa: B018 Need to touch tool data table once to populate self.columns
 
         # Options are defined by parsing tabular text data from a data file
@@ -725,22 +745,64 @@
                     # Pass just the first megabyte to parse_file_fields.
                     log.warning("Attempting to load options from large file, reading just first megabyte")
                     with open(path) as fh:
                         contents = fh.read(1048576)
                     options += self.parse_file_fields(StringIO(contents))
         elif self.tool_data_table:
             options = self.tool_data_table.get_fields()
+            if trans and trans.user and trans.workflow_building_mode != workflow_building_modes.ENABLED:
+                options += self.get_user_options(trans.user)
         elif self.file_fields:
             options = list(self.file_fields)
         else:
             options = []
         for filter in self.filters:
             options = filter.filter_options(options, trans, other_values)
         return options
 
+    def get_user_options(self, user: User):
+        # stored metadata are key: value pairs, turn into flat lists of correct order
+        fields = []
+        if self.tool_data_table_name:
+            hdas = user.get_user_data_tables(self.tool_data_table_name)
+            by_dbkey = {}
+            for hda in hdas:
+                try:
+                    table_entries = self.hda_to_table_entries(hda, self.tool_data_table_name)
+                except Exception as e:
+                    # This is a bug, `hda_to_table_entries` is not generic enough for certain loc file
+                    # structures, such as for the dada2_species, which doesn't have a dbkey column
+                    table_entries = {}
+                    log.warning("Failed to read data table bundle entries: %s", e)
+                by_dbkey.update(table_entries)
+            for data_table_entry in by_dbkey.values():
+                field_entry = []
+                for column_key in self.tool_data_table.columns.keys():
+                    field_entry.append(data_table_entry[column_key])
+                fields.append(field_entry)
+        return fields
+
+    @staticmethod
+    def hda_to_table_entries(hda, table_name):
+        table_entries = {}
+        for value in hda._metadata["data_tables"][table_name]:
+            if dbkey := value.get("dbkey"):
+                table_entries[dbkey] = value
+            if path := value.get("path"):
+                # maybe a hack, should probably pass around dataset or src id combinations ?
+                value["path"] = os.path.join(hda.extra_files_path, path)
+                value["value"] = {"src": "hda", "id": hda.id}
+        return table_entries
+
+    def get_option_from_dataset(self, dataset):
+        # TODO: we may have to pass the name/id in case there are multiple entries produced by a single dm run
+        entries = self.hda_to_table_entries(dataset, self.tool_data_table_name)
+        assert len(entries) == 1, "Cannot pass tool data bundle with more than 1 data entry per table"
+        return next(iter(entries.values()))
+
     def get_fields_by_value(self, value, trans, other_values):
         """
         Return a list of fields with column 'value' matching provided value.
         """
         rval = []
         val_index = self.columns["value"]
         for fields in self.get_fields(trans, other_values):
@@ -762,14 +824,57 @@
             value = [value]
         for val in value:
             for fields in self.get_fields_by_value(val, trans, other_values):
                 rval.append(fields[field_index])
         return rval
 
     def get_options(self, trans, other_values):
+        def to_triple(values):
+            if len(values) == 2:
+                return [str(values[0]), str(values[1]), False]
+            else:
+                return [str(values[0]), str(values[1]), bool(values[2])]
+
+        if from_url_options := self.from_url_options:
+            context = User.user_template_environment(trans.user)
+            url = fill_template(from_url_options.from_url, context)
+            request_body = template_or_none(from_url_options.request_body, context)
+            request_headers = template_or_none(from_url_options.request_headers, context)
+            try:
+                unset_value = object()
+                cached_value = trans.get_cache_value(
+                    (url, from_url_options.request_method, request_body, request_headers), unset_value
+                )
+                if cached_value is unset_value:
+                    data = request(
+                        url=url,
+                        method=from_url_options.request_method,
+                        data=json.loads(request_body) if request_body else None,
+                        headers=json.loads(request_headers) if request_headers else None,
+                        timeout=10,
+                    )
+                    trans.set_cache_value((url, from_url_options.request_method, request_body, request_headers), data)
+                else:
+                    data = cached_value
+            except Exception as e:
+                log.warning("Fetching from url '%s' failed: %s", url, str(e))
+                data = None
+
+            if from_url_options.postprocess_expression:
+                try:
+                    data = do_eval(
+                        from_url_options.postprocess_expression,
+                        data,
+                    )
+                except Exception as eval_error:
+                    log.warning("Failed to evaluate postprocess_expression: %s", str(eval_error))
+                    data = []
+
+            # We only support the very specific ["name", "value", "selected"] format for now.
+            return [to_triple(d) for d in data]
         rval = []
         if (
             self.file_fields is not None
             or self.tool_data_table is not None
             or self.dataset_ref_name is not None
             or self.missing_index_file
         ):
@@ -790,14 +895,57 @@
         # Name?
         if column_spec in self.columns:
             return self.columns[column_spec]
         # Int?
         return int(column_spec)
 
 
+REQUEST_METHODS = Literal["GET", "POST"]
+
+
+@dataclass
+class FromUrlOptions:
+    from_url: str
+    request_method: REQUEST_METHODS
+    request_body: Optional[str]
+    request_headers: Optional[str]
+    postprocess_expression: Optional[str]
+
+
+def strip_or_none(maybe_string: Optional[Element]) -> Optional[str]:
+    if maybe_string is not None:
+        if maybe_string.text:
+            return maybe_string.text.strip()
+    return None
+
+
+def parse_from_url_options(elem: Element) -> Optional[FromUrlOptions]:
+    from_url = elem.get("from_url")
+    if from_url:
+        request_method = cast(Literal["GET", "POST"], elem.get("request_method", "GET"))
+        assert request_method in get_args(REQUEST_METHODS)
+        request_headers = strip_or_none(elem.find("request_headers"))
+        request_body = strip_or_none(elem.find("request_body"))
+        postprocess_expression = strip_or_none(elem.find("postprocess_expression"))
+        return FromUrlOptions(
+            from_url,
+            request_method=request_method,
+            request_headers=request_headers,
+            request_body=request_body,
+            postprocess_expression=postprocess_expression,
+        )
+    return None
+
+
+def template_or_none(template: Optional[str], context: Dict[str, Any]) -> Optional[str]:
+    if template:
+        return fill_template(template, context=context)
+    return None
+
+
 def _get_ref_data(other_values, ref_name):
     """
     get the list of data sets from ref_name
     - a KeyError is raised if no such element exists
     - a ValueError is raised if the element is not of the type DatasetFilenameWrapper, HistoryDatasetAssociation, DatasetListWrapper, HistoryDatasetCollectionAssociation, list
     """
     from galaxy.tools.wrappers import (
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/grouping.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Constructs for grouping tool parameters
 """
+
 import io
 import logging
 import os
 import unicodedata
 from typing import (
     Any,
     Callable,
@@ -408,16 +409,15 @@
                     dataset_name = get_file_name(data_file["filename"])
                 return Bunch(type="file", path=data_file["local_filename"], name=dataset_name, purge_source=purge)
             except Exception:
                 # The uploaded file should've been persisted by the upload tool action
                 return Bunch(type=None, path=None, name=None)
 
         def get_url_paste_urls_or_filename(group_incoming, override_name=None, override_info=None):
-            url_paste_file = group_incoming.get("url_paste", None)
-            if url_paste_file is not None:
+            if (url_paste_file := group_incoming.get("url_paste", None)) is not None:
                 url_paste = open(url_paste_file).read()
 
                 def start_of_url(content):
                     start_of_url_paste = content.lstrip()[0:10].lower()
                     looks_like_url = False
                     for url_prefix in URI_PREFIXES:
                         if start_of_url_paste.startswith(url_prefix):
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/history_query.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/history_query.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/input_translation.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/input_translation.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,16 @@
             # trans_list = []
             remote_name = req_param.get("remote_name")
             galaxy_name = req_param.get("galaxy_name")
             missing = req_param.get("missing")
             value_trans = {}
             append_param = None
 
+            rval.vocabulary.add(remote_name)
+
             value_trans_elem = req_param.find("value_translation")
             if value_trans_elem is not None:
                 for value_elem in value_trans_elem.findall("value"):
                     remote_value = value_elem.get("remote_value")
                     galaxy_value = value_elem.get("galaxy_value")
                     if None not in [remote_value, galaxy_value]:
                         value_trans[remote_value] = galaxy_value
@@ -77,26 +79,28 @@
                 join_str = append_param_elem.get("join", "=")
                 append_dict = {}
                 for value_elem in append_param_elem.findall("value"):
                     value_name = value_elem.get("name")
                     value_missing = value_elem.get("missing")
                     if None not in [value_name, value_missing]:
                         append_dict[value_name] = value_missing
+                        rval.vocabulary.add(value_name)
                 append_param = Bunch(
                     separator=separator, first_separator=first_separator, join_str=join_str, append_dict=append_dict
                 )
 
             rval.param_trans_dict[remote_name] = Bunch(
                 galaxy_name=galaxy_name, missing=missing, value_trans=value_trans, append_param=append_param
             )
 
         return rval
 
     def __init__(self):
         self.param_trans_dict = {}
+        self.vocabulary = set()
 
     def translate(self, params):
         """
         update params in-place
         """
         for remote_name, translator in self.param_trans_dict.items():
             galaxy_name = (
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/meta.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/meta.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/sanitize.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/sanitize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tool Parameter specific sanitizing.
 """
+
 import logging
 import string
 
 import galaxy.util
 
 log = logging.getLogger(__name__)
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/validation.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Classes related to parameter validation.
 """
+
 import abc
 import json
 import logging
 import os.path
 
 import regex
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/wrapped.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/wrapped.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/parameters/wrapped_json.py` & `galaxy-app-24.0.0/galaxy/tools/parameters/wrapped_json.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import json
 import logging
 from typing import (
     Any,
     Dict,
     List,
     Sequence,
+    TYPE_CHECKING,
 )
 
 from packaging.version import Version
 
+if TYPE_CHECKING:
+    from galaxy.tools.parameters.wrappers import (
+        DatasetCollectionWrapper,
+        DatasetFilenameWrapper,
+    )
+
 log = logging.getLogger(__name__)
 
 SKIP_INPUT = object()
 
 
 def json_wrap(inputs, input_values, profile, as_dict=None, handle_files="skip"):
     if as_dict is None:
@@ -36,36 +43,49 @@
 
 
 def data_collection_input_to_path(v):
     return v.all_paths
 
 
 def data_collection_input_to_staging_path_and_source_path(
-    v, invalid_chars: Sequence[str] = ("/",), include_collection_name: bool = False
+    v: "DatasetCollectionWrapper", invalid_chars: Sequence[str] = ("/",), include_collection_name: bool = False
 ) -> List[Dict[str, Any]]:
     staging_paths = v.get_all_staging_paths(
         invalid_chars=invalid_chars, include_collection_name=include_collection_name
     )
-    source_paths = v.all_paths
-    metadata_files = v.all_metadata_files
+    if v.element_identifiers_extensions_paths_and_metadata_files:
+        element_identifiers, extensions, source_paths, metadata_files = zip(
+            *v.element_identifiers_extensions_paths_and_metadata_files
+        )
+    else:
+        element_identifiers, extensions, source_paths, metadata_files = (), (), (), ()
     return [
         {
+            "element_identifier": element_identifier,
+            "ext": extension,
             "staging_path": staging_path,
             "source_path": source_path,
             "metadata_files": [
                 {"staging_path": f"{staging_path}.{mf[0]}", "source_path": mf[1]} for mf in metadata_files
             ],
         }
-        for staging_path, source_path, metadata_files in zip(staging_paths, source_paths, metadata_files)
+        for element_identifier, extension, staging_path, source_path, metadata_files in zip(
+            element_identifiers, extensions, staging_paths, source_paths, metadata_files
+        )
     ]
 
 
-def data_input_to_staging_path_and_source_path(v, invalid_chars: Sequence[str] = ("/",)) -> Dict[str, Any]:
+def data_input_to_staging_path_and_source_path(
+    v: "DatasetFilenameWrapper", invalid_chars: Sequence[str] = ("/",)
+) -> Dict[str, Any]:
     staging_path = v.get_staging_path(invalid_chars=invalid_chars)
+    # note that the element identifier should be always a list
     return {
+        "element_identifier": [v.element_identifier],
+        "ext": v.file_ext,
         "staging_path": staging_path,
         "source_path": data_input_to_path(v),
         "metadata_files": [
             {"staging_path": f"{staging_path}.{mf[0]}", "source_path": mf[1]} for mf in v.all_metadata_files
         ],
     }
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/recommendations.py` & `galaxy-app-24.0.0/galaxy/tools/recommendations.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import h5py
 import numpy as np
 import requests
 import yaml
 
 from galaxy.tools.parameters import populate_state
-from galaxy.tools.parameters.basic import workflow_building_modes
+from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
 from galaxy.util import DEFAULT_SOCKET_TIMEOUT
 from galaxy.workflow.modules import module_factory
 
 log = logging.getLogger(__name__)
 
 
 class ToolRecommendations:
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/relabel_from_file.xml` & `galaxy-app-24.0.0/galaxy/tools/relabel_from_file.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/remote_tool_eval.py` & `galaxy-app-24.0.0/galaxy/tools/remote_tool_eval.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/repositories.py` & `galaxy-app-24.0.0/galaxy/tools/repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provides a subset of app for verifying tools."""
+
 import os
 import shutil
 import tempfile
 from contextlib import contextmanager
 from typing import Optional
 
 from galaxy.managers.dbkeys import GenomeBuilds
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/search/__init__.py` & `galaxy-app-24.0.0/galaxy/tools/search/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 Filters - various filters are available for processing content as the index is
     built. A StopFilter removes common articles 'a', 'for', 'and' etc. A
     StemmingFilter removes suffixes from words to create a 'base work' e.g.
     stemming -> stem; opened -> open; philosophy -> philosoph.
 
 """
+
 import logging
 import os
 import re
 import shutil
 from typing import (
     Dict,
     List,
@@ -53,16 +54,18 @@
     BM25F,
     Frequency,
     MultiWeighting,
 )
 from whoosh.writing import AsyncWriter
 
 from galaxy.config import GalaxyAppConfiguration
-from galaxy.util import ExecutionTimer
-from galaxy.web.framework.helpers import to_unicode
+from galaxy.util import (
+    ExecutionTimer,
+    unicodify,
+)
 
 log = logging.getLogger(__name__)
 
 CanConvertToFloat = Union[str, int, float]
 CanConvertToInt = Union[str, int, float]
 
 
@@ -275,47 +278,47 @@
         self,
         tool,
         index_help: bool = True,
     ) -> Dict[str, str]:
         def clean(string):
             """Remove hyphens as they are Whoosh wildcards."""
             if "-" in string:
-                return (" ").join(token.text for token in self.rex(to_unicode(tool.name)))
+                return (" ").join(token.text for token in self.rex(unicodify(tool.name)))
             else:
                 return string
 
         if tool.tool_type == "manage_data":
             #  Do not add data managers to the public index
             return {}
         add_doc_kwds = {
-            "id": to_unicode(tool.id),
-            "id_exact": to_unicode(tool.id),
+            "id": unicodify(tool.id),
+            "id_exact": unicodify(tool.id),
             "name": clean(tool.name),
-            "description": to_unicode(tool.description),
-            "section": to_unicode(tool.get_panel_section()[1] if len(tool.get_panel_section()) == 2 else ""),
+            "description": unicodify(tool.description),
+            "section": unicodify(tool.get_panel_section()[1] if len(tool.get_panel_section()) == 2 else ""),
             "edam_operations": clean(tool.edam_operations),
             "edam_topics": clean(tool.edam_topics),
-            "repository": to_unicode(tool.repository_name),
-            "owner": to_unicode(tool.repository_owner),
-            "help": to_unicode(""),
+            "repository": unicodify(tool.repository_name),
+            "owner": unicodify(tool.repository_owner),
+            "help": unicodify(""),
         }
         if tool.guid:
             # Create a stub consisting of owner, repo, and tool from guid
             slash_indexes = [m.start() for m in re.finditer("/", tool.guid)]
             id_stub = tool.guid[(slash_indexes[1] + 1) : slash_indexes[4]]
             add_doc_kwds["stub"] = clean(id_stub)
         else:
-            add_doc_kwds["stub"] = to_unicode(id)
+            add_doc_kwds["stub"] = unicodify(id)
         if tool.labels:
-            add_doc_kwds["labels"] = to_unicode(" ".join(tool.labels))
+            add_doc_kwds["labels"] = unicodify(" ".join(tool.labels))
         if index_help:
             raw_help = tool.raw_help
             if raw_help:
                 try:
-                    add_doc_kwds["help"] = to_unicode(raw_help)
+                    add_doc_kwds["help"] = unicodify(raw_help)
                 except Exception:
                     # Don't fail to build index when help fails to parse
                     pass
 
         add_doc_kwds["name_exact"] = add_doc_kwds["name"]
 
         return add_doc_kwds
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/sort_collection_list.xml` & `galaxy-app-24.0.0/galaxy/tools/sort_collection_list.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/special_tools.py` & `galaxy-app-24.0.0/galaxy/tools/special_tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/tag_collection_from_file.xml` & `galaxy-app-24.0.0/galaxy/tools/tag_collection_from_file.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/test.py` & `galaxy-app-24.0.0/galaxy/tools/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,16 +365,15 @@
     def __init__(self, name, index=None, parent_context=None):
         self.parent_context = parent_context
         self.name = name
         self.index = None if index is None else int(index)
 
     def for_state(self):
         name = self.name if self.index is None else "%s_%d" % (self.name, self.index)
-        parent_for_state = self.parent_context.for_state()
-        if parent_for_state:
+        if parent_for_state := self.parent_context.for_state():
             return f"{parent_for_state}|{name}"
         else:
             return name
 
     def __str__(self):
         return f"Context[for_state={self.for_state()}]"
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/unzip_collection.xml` & `galaxy-app-24.0.0/galaxy/tools/unzip_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/util/galaxyops/__init__.py` & `galaxy-app-24.0.0/galaxy/tools/util/galaxyops/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/tools/util/maf_utilities.py` & `galaxy-app-24.0.0/galaxy/tools/util/maf_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,17 +654,14 @@
     ends = []
 
     fields = line.split()
     # Requires atleast 12 BED columns
     if len(fields) < 12:
         raise Exception(f"Not a proper 12 column BED line ({line}).")
     tx_start = int(fields[1])
-    strand = fields[5]
-    if strand != "-":
-        strand = "+"  # Default strand is +
     cds_start = int(fields[6])
     cds_end = int(fields[7])
 
     # Calculate and store starts and ends of coding exons
     region_start, region_end = cds_start, cds_end
     exon_starts = list(map(int, fields[11].rstrip(",\n").split(",")))
     exon_starts = [x + tx_start for x in exon_starts]
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/wrappers.py` & `galaxy-app-24.0.0/galaxy/tools/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     Optional,
     Sequence,
     Tuple,
     TYPE_CHECKING,
     Union,
 )
 
+from packaging.version import Version
+
 from galaxy.model import (
     DatasetCollection,
     DatasetCollectionElement,
     DatasetCollectionInstance,
     DatasetInstance,
     HasTags,
     HistoryDatasetCollectionAssociation,
@@ -124,15 +126,15 @@
     ) -> None:
         self.input = input
         if (
             value is None
             and input.type == "text"
             and input.optional
             and input.optionality_inferred
-            and (profile is None or profile < 23.0)
+            and (profile is None or Version(str(profile)) < Version("23.0"))
         ):
             # Tools with old profile versions may treat an optional text parameter as `""`
             value = ""
         self.value = value
         self._other_values: Dict[str, str] = other_values or {}
 
     def _get_cast_values(self, other: Any) -> Tuple[Union[str, int, float, bool, None], Any]:
@@ -210,22 +212,25 @@
             value: Union[str, List[str]],
             other_values: Optional[Dict[str, str]],
             compute_environment: Optional["ComputeEnvironment"],
         ) -> None:
             self._input = input
             self._value = value
             self._other_values = other_values
-            self._fields: Dict[str, str] = {}
+            self._fields: Dict[str, List[str]] = {}
             self._compute_environment = compute_environment
 
         def __getattr__(self, name: str) -> Any:
             if name not in self._fields:
-                self._fields[name] = self._input.options.get_field_by_name_for_value(
-                    name, self._value, None, self._other_values
-                )
+                if isinstance(self._value, DatasetInstance):
+                    self._fields[name] = [self._input.options.get_option_from_dataset(self._value)[name]]
+                else:
+                    self._fields[name] = self._input.options.get_field_by_name_for_value(
+                        name, self._value, None, self._other_values
+                    )
             values = map(str, self._fields[name])
             if name in PATH_ATTRIBUTES and self._compute_environment:
                 # If we infer this is a path, rewrite it if needed.
                 new_values = []
                 for value in values:
                     rewrite_value = self._compute_environment.unstructured_path_rewrite(value)
                     if rewrite_value:
@@ -789,13 +794,12 @@
     def __init__(self, input_datasets: Optional[Dict[str, Any]] = None) -> None:
         if input_datasets is not None:
             self.identifier_key_dict = {v: f"{k}|__identifier__" for k, v in input_datasets.items()}
         else:
             self.identifier_key_dict = {}
 
     def identifier(self, dataset_value: str, input_values: Dict[str, str]) -> Optional[str]:
-        identifier_key = self.identifier_key_dict.get(dataset_value, None)
         element_identifier = None
-        if identifier_key:
+        if identifier_key := self.identifier_key_dict.get(dataset_value, None):
             element_identifier = input_values.get(identifier_key, None)
 
         return element_identifier
```

### Comparing `galaxy-app-23.2.1/galaxy/tools/zip_collection.xml` & `galaxy-app-24.0.0/galaxy/tools/zip_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/visualization/data_providers/basic.py` & `galaxy-app-24.0.0/galaxy/visualization/data_providers/basic.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/visualization/data_providers/cigar.py` & `galaxy-app-24.0.0/galaxy/visualization/data_providers/cigar.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/visualization/data_providers/genome.py` & `galaxy-app-24.0.0/galaxy/visualization/data_providers/genome.py`

 * *Files 0% similar despite different names*

```diff
@@ -1160,16 +1160,15 @@
     """
     BBI data provider for the Galaxy track browser.
     """
 
     dataset_type = "bigwig"
 
     @abc.abstractmethod
-    def _get_dataset(self) -> Tuple[IO[bytes], Union[BigBedFile, BigWigFile]]:
-        ...
+    def _get_dataset(self) -> Tuple[IO[bytes], Union[BigBedFile, BigWigFile]]: ...
 
     def valid_chroms(self):
         # No way to return this info as of now
         return None
 
     def has_data(self, chrom):
         f, bbi = self._get_dataset()
@@ -1229,16 +1228,15 @@
             will return None for all positions.
             """
             result = []
 
             # Get summary; this samples at intervals of length
             # (end - start)/num_points -- i.e. drops any fractional component
             # of interval length.
-            summary = _summarize_bbi(bbi, chrom, start, end, num_points)
-            if summary:
+            if summary := _summarize_bbi(bbi, chrom, start, end, num_points):
                 # mean = summary.sum_data / summary.valid_count
 
                 # Standard deviation by bin, not yet used
                 # var = summary.sum_squares - mean
                 # var /= minimum( valid_count - 1, 1 )
                 # sd = sqrt( var )
```

### Comparing `galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/__init__.py` & `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ Data providers code for PhyloViz """
+
 from typing import (
     Any,
     Dict,
 )
 
 from galaxy.visualization.data_providers.basic import BaseDataProvider
 from galaxy.visualization.data_providers.phyloviz.newickparser import Newick_Parser
```

### Comparing `galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/baseparser.py` & `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/baseparser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/newickparser.py` & `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/newickparser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/nexusparser.py` & `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/nexusparser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/visualization/data_providers/phyloviz/phyloxmlparser.py` & `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/phyloxmlparser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/visualization/data_providers/registry.py` & `galaxy-app-24.0.0/galaxy/visualization/data_providers/registry.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/visualization/genomes.py` & `galaxy-app-24.0.0/galaxy/visualization/genomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import logging
 import os
 import re
 import sys
 from json import loads
-from typing import Dict
+from typing import (
+    Dict,
+    Optional,
+)
 
 from bx.seq.twobit import TwoBitFile
 
 from galaxy.exceptions import (
     ObjectNotFound,
     ReferenceDataError,
 )
 from galaxy.managers.users import get_user_by_username
-from galaxy.model import HistoryDatasetAssociation
+from galaxy.model import (
+    HistoryDatasetAssociation,
+    User,
+)
 from galaxy.structured_app import StructuredApp
 from galaxy.util.bunch import Bunch
 
 log = logging.getLogger(__name__)
 
 # FIXME: copied from tracks.py
 # Message strings returned to browser
@@ -252,15 +258,15 @@
         """Returns build for the given key."""
         self.check_and_reload()
         rval = None
         if dbkey in self.genomes:
             rval = self.genomes[dbkey]
         return rval
 
-    def get_dbkeys(self, user, chrom_info=False):
+    def get_dbkeys(self, user: Optional[User], chrom_info=False):
         """Returns all known dbkeys. If chrom_info is True, only dbkeys with
         chromosome lengths are returned."""
         self.check_and_reload()
         dbkeys = []
 
         # Add user's custom keys to dbkeys.
         if user and "dbkeys" in user.preferences:
```

### Comparing `galaxy-app-23.2.1/galaxy/visualization/plugins/config_parser.py` & `galaxy-app-24.0.0/galaxy/visualization/plugins/config_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,26 +144,23 @@
         if (render_target is not None and render_target.text) and (render_target.text in self.VALID_RENDER_TARGETS):
             returned["render_target"] = render_target.text
         else:
             returned["render_target"] = "galaxy_main"
         # consider unifying the above into its own element and parsing method
 
         # load optional custom configuration specifiers
-        specs_section = xml_tree.find("specs")
-        if specs_section is not None:
+        if (specs_section := xml_tree.find("specs")) is not None:
             returned["specs"] = DictParser(specs_section)
 
         # load group specifiers
-        groups_section = xml_tree.find("groups")
-        if groups_section is not None:
+        if (groups_section := xml_tree.find("groups")) is not None:
             returned["groups"] = ListParser(groups_section)
 
         # load settings specifiers
-        settings_section = xml_tree.find("settings")
-        if settings_section is not None:
+        if (settings_section := xml_tree.find("settings")) is not None:
             returned["settings"] = ListParser(settings_section)
 
         return returned
 
     def parse_entry_point(self, xml_tree):
         """
         Parse the config file for an appropriate entry point: a mako template, a script tag,
@@ -222,16 +219,15 @@
 
         # tests (optional, 0 or more) - data for boolean test: 'is the visualization usable by this object?'
         # when no tests are given, default to isinstance( object, model_class )
         returned["tests"] = self.parse_tests(xml_tree.findall("test"))
 
         # to_params (optional, 0 or more) - tells the registry to set certain params based on the model_clas, tests
         returned["to_params"] = {}
-        to_params = self.parse_to_params(xml_tree.findall("to_param"))
-        if to_params:
+        if to_params := self.parse_to_params(xml_tree.findall("to_param")):
             returned["to_params"] = to_params
 
         return returned
 
     def parse_model_class(self, xml_tree):
         """
         Convert xml model_class element to a galaxy model class
@@ -460,24 +456,22 @@
                 # convert default based on param_type here
             returned["default"] = default
 
         # does the param have to be within a list of certain values
         # NOTE: the interpretation of this list is deferred till parsing and based on param type
         #   e.g. it could be 'val in constrain_to', or 'constrain_to is min, max for number', etc.
         # TODO: currently unused
-        constrain_to = xml_tree.get("constrain_to")
-        if constrain_to:
+        if constrain_to := xml_tree.get("constrain_to"):
             returned["constrain_to"] = constrain_to.split(",")
 
         # is the param a comma-separated-value list?
         returned["csv"] = xml_tree.get("csv") == "true"
 
         # remap keys in the params/query string to the var names used in the template
-        var_name_in_template = xml_tree.get("var_name_in_template")
-        if var_name_in_template:
+        if var_name_in_template := xml_tree.get("var_name_in_template"):
             returned["var_name_in_template"] = var_name_in_template
 
         return returned
 
     def parse_param_type(self, xml_tree):
         """
         Parse a param type from the given `xml_tree`.
```

### Comparing `galaxy-app-23.2.1/galaxy/visualization/plugins/plugin.py` & `galaxy-app-24.0.0/galaxy/visualization/plugins/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Visualization plugins: instantiate/deserialize data and models
 from a query string and render a webpage based on those data.
 """
+
 import copy
 import logging
 import os
 from typing import (
     Any,
     Dict,
 )
```

### Comparing `galaxy-app-23.2.1/galaxy/visualization/plugins/registry.py` & `galaxy-app-24.0.0/galaxy/visualization/plugins/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Lower level of visualization framework which does three main things:
     - associate visualizations with objects
     - create urls to visualizations based on some target object(s)
     - unpack a query string into the desired objects needed for rendering
 """
+
 import logging
 import os
 import weakref
 
 from galaxy.exceptions import ObjectNotFound
 from galaxy.util import (
     config_directories_from_setting,
@@ -243,16 +244,15 @@
 
     def get_visualization(self, trans, visualization_name, target_object):
         """
         Return data to build a url to the visualization with the given
         `visualization_name` if it's applicable to `target_object` or
         `None` if it's not.
         """
-        visualization = self.plugins.get(visualization_name, None)
-        if visualization is not None:
+        if (visualization := self.plugins.get(visualization_name, None)) is not None:
             data_sources = visualization.config["data_sources"]
             for data_source in data_sources:
                 model_class = data_source["model_class"]
                 if isinstance(target_object, model_class):
                     tests = data_source["tests"]
                     if tests is None or self.is_object_applicable(trans, target_object, tests):
                         return visualization.to_dict()
```

### Comparing `galaxy-app-23.2.1/galaxy/visualization/plugins/resource_parser.py` & `galaxy-app-24.0.0/galaxy/visualization/plugins/resource_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Deserialize Galaxy resources (hdas, ldas, datasets, genomes, etc.) from
 a dictionary of string data/ids (often from a query string).
 """
+
 import json
 import logging
 import weakref
 from typing import (
     Callable,
     Dict,
     Optional,
```

### Comparing `galaxy-app-23.2.1/galaxy/visualization/plugins/utils.py` & `galaxy-app-24.0.0/galaxy/visualization/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/webhooks/__init__.py` & `galaxy-app-24.0.0/galaxy/webhooks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module manages loading of Galaxy webhooks.
 """
+
 import logging
 import os
 
 import yaml
 
 from galaxy.util import config_directories_from_setting
```

### Comparing `galaxy-app-23.2.1/galaxy/work/context.py` & `galaxy-app-24.0.0/galaxy/work/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import abc
 from typing import (
+    Any,
+    Dict,
     List,
     Optional,
+    Tuple,
 )
 
 from typing_extensions import Literal
 
 from galaxy.managers.context import ProvidesHistoryContext
 from galaxy.model import (
     GalaxySession,
@@ -38,17 +41,24 @@
         galaxy_session: Optional[GalaxySession] = None,
     ):
         self._app = app
         self.__user = user
         self.__user_current_roles: Optional[List[Role]] = None
         self.__history = history
         self._url_builder = url_builder
+        self._short_term_cache: Dict[Tuple[str, ...], Any] = {}
         self.workflow_building_mode = workflow_building_mode
         self.galaxy_session = galaxy_session
 
+    def set_cache_value(self, args: Tuple[str, ...], value: Any):
+        self._short_term_cache[args] = value
+
+    def get_cache_value(self, args: Tuple[str, ...], default: Any = None) -> Any:
+        return self._short_term_cache.get(args, default)
+
     @property
     def app(self):
         return self._app
 
     @property
     def url_builder(self):
         return self._url_builder
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/extract.py` & `galaxy-app-24.0.0/galaxy/workflow/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """ This module contains functionality to aid in extracting workflows from
 histories.
 """
+
 import logging
 from typing import Optional
 
 from galaxy import (
     exceptions,
     model,
 )
-from galaxy.model.base import transaction
+from galaxy.model.base import (
+    ensure_object_added_to_session,
+    transaction,
+)
 from galaxy.tool_util.parser import ToolOutputCollectionPart
 from galaxy.tools.parameters.basic import (
     DataCollectionToolParameter,
     DataToolParameter,
 )
 from galaxy.tools.parameters.grouping import (
     Conditional,
@@ -67,14 +71,15 @@
     # Store it
     stored = model.StoredWorkflow()
     stored.user = user
     stored.name = workflow_name
     workflow.stored_workflow = stored
     stored.latest_workflow = workflow
     trans.sa_session.add(stored)
+    ensure_object_added_to_session(workflow, session=trans.sa_session)
     with transaction(trans.sa_session):
         trans.sa_session.commit()
     return stored
 
 
 def extract_steps(
     trans,
@@ -292,16 +297,15 @@
     def __summarize_dataset_collection(self, dataset_collection):
         hid_in_history = dataset_collection.hid
         dataset_collection = self.__original_hdca(dataset_collection)
         self.hdca_hid_in_history[dataset_collection.id] = hid_in_history
 
         hid = dataset_collection.hid
         self.collection_types[hid] = dataset_collection.collection.collection_type
-        cja = dataset_collection.creating_job_associations
-        if cja:
+        if cja := dataset_collection.creating_job_associations:
             # Use the "first" job to represent all mapped jobs.
             representative_assoc = cja[0]
             representative_job = representative_assoc.job
             if (
                 representative_job not in self.jobs
                 or self.jobs[representative_job][0][1].history_content_type == "dataset"
             ):
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/modules.py` & `galaxy-app-24.0.0/galaxy/workflow/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Modules used in building workflows
 """
+
 import json
 import logging
 import re
 from collections import defaultdict
 from typing import (
     Any,
     cast,
@@ -13,33 +14,32 @@
     List,
     Optional,
     Type,
     TYPE_CHECKING,
     Union,
 )
 
-from cwl_utils.expression import do_eval
 from typing_extensions import TypedDict
 
 from galaxy import (
     exceptions,
     model,
-    web,
 )
 from galaxy.exceptions import (
     ToolInputsNotReadyException,
     ToolMissingException,
 )
 from galaxy.job_execution.actions.post import ActionBox
 from galaxy.model import (
     PostJobAction,
     Workflow,
     WorkflowStep,
     WorkflowStepConnection,
 )
+from galaxy.model.base import ensure_object_added_to_session
 from galaxy.model.dataset_collections import matching
 from galaxy.schema.invocation import (
     CancelReason,
     FailureReason,
     InvocationCancellationReviewFailed,
     InvocationFailureDatasetFailed,
     InvocationFailureExpressionEvaluationFailed,
@@ -54,14 +54,15 @@
 )
 from galaxy.tools.actions import filter_output
 from galaxy.tools.execute import (
     execute,
     MappingParameters,
     PartialJobExecution,
 )
+from galaxy.tools.expressions import do_eval
 from galaxy.tools.parameters import (
     check_param,
     params_to_incoming,
     visit_input_values,
 )
 from galaxy.tools.parameters.basic import (
     BaseDataToolParameter,
@@ -75,21 +76,21 @@
     IntegerToolParameter,
     is_runtime_value,
     parameter_types,
     raw_to_galaxy,
     runtime_to_json,
     SelectToolParameter,
     TextToolParameter,
-    workflow_building_modes,
 )
 from galaxy.tools.parameters.grouping import (
     Conditional,
     ConditionalWhen,
 )
 from galaxy.tools.parameters.history_query import HistoryQuery
+from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
 from galaxy.tools.parameters.wrapped import make_dict_copy
 from galaxy.util import (
     listify,
     unicodify,
 )
 from galaxy.util.bunch import Bunch
 from galaxy.util.json import safe_loads
@@ -221,18 +222,14 @@
         if when_expression == "${inputs.when}":
             # Fallback for workflows defined on 23.0
             when_expression = "$(inputs.when)"
         try:
             as_cwl_value = do_eval(
                 when_expression,
                 step_state,
-                [{"class": "InlineJavascriptRequirement"}],
-                None,
-                None,
-                {},
             )
         except Exception:
             # Exception contains script and traceback, which could be helpful for debugging workflows,
             # but both could conceivably contain secrets.
             # CWL has a secret hint that should cause values to be sanitized,
             # but Galaxy does not, so we can't really display anything here at this point.
             # In any case I believe the CWL secret hint can be bypassed if the value is passed on
@@ -310,16 +307,15 @@
 
     # ---- Configuration time -----------------------------------------------
 
     def get_state(self, nested=True):
         """Return a serializable representation of the persistable state of
         the step.
         """
-        inputs = self.get_inputs()
-        if inputs:
+        if inputs := self.get_inputs():
             return self.state.encode(Bunch(inputs=inputs), self.trans.app, nested=nested)
         else:
             return self.state.inputs
 
     def get_export_state(self):
         return self.get_state(nested=True)
 
@@ -344,16 +340,15 @@
         from_tool_form = kwds.get("from_tool_form", False)
         if not from_tool_form:
             # I've never seen state here be none except for unit tests so 'or {}' below may only be
             # needed due to test bugs. Doesn't hurt anything though.
             state = self.step_state_to_tool_state(state or {})
 
         self.state = DefaultToolState()
-        inputs = self.get_inputs()
-        if inputs:
+        if inputs := self.get_inputs():
             self.state.decode(state, Bunch(inputs=inputs), self.trans.app)
         else:
             self.state.inputs = safe_loads(state) or {}
 
     def step_state_to_tool_state(self, state):
         return state
 
@@ -644,14 +639,15 @@
         module = super().from_workflow_step(trans, step, **kwds)
         module.subworkflow = step.subworkflow
         return module
 
     def save_to_step(self, step, **kwd):
         step.type = self.type
         step.subworkflow = self.subworkflow
+        ensure_object_added_to_session(step, object_in_session=self.subworkflow)
 
     def get_name(self):
         if hasattr(self.subworkflow, "name"):
             return self.subworkflow.name
         return self.name
 
     def get_all_inputs(self, data_only=False, connectable_only=False):
@@ -1111,24 +1107,23 @@
         return inputs
 
     def get_runtime_inputs(self, step, connections: Optional[Iterable[WorkflowStepConnection]] = None):
         parameter_def = self._parse_state_into_dict()
         collection_type = parameter_def["collection_type"]
         optional = parameter_def["optional"]
         tag = parameter_def["tag"]
-        formats = parameter_def.get("format")
         collection_param_source = dict(
             name="input",
             label=self.label,
             type="data_collection",
             collection_type=collection_type,
             tag=tag,
             optional=optional,
         )
-        if formats:
+        if formats := parameter_def.get("format"):
             collection_param_source["format"] = ",".join(listify(formats))
         input_param = DataCollectionToolParameter(None, collection_param_source, self.trans)
         return dict(input=input_param)
 
     def get_all_outputs(self, data_only=False):
         parameter_def = self._parse_state_into_dict()
         format_def = parameter_def.get("format")
@@ -1145,16 +1140,15 @@
                 collection_type=parameter_def.get("collection_type", self.default_collection_type),
                 optional=optional,
             )
         ]
 
     def _parse_state_into_dict(self):
         state_as_dict = super()._parse_state_into_dict()
-        inputs = self.state.inputs
-        if "collection_type" in inputs:
+        if "collection_type" in (inputs := self.state.inputs):
             collection_type = inputs["collection_type"]
         else:
             collection_type = self.default_collection_type
         state_as_dict["collection_type"] = collection_type
         return state_as_dict
 
 
@@ -1821,16 +1815,15 @@
     def save_to_step(self, step, detached=False):
         super().save_to_step(step, detached=detached)
         step.tool_id = self.tool_id
         if self.tool:
             step.tool_version = self.get_version()
         else:
             step.tool_version = self.tool_version
-        tool_uuid = getattr(self, "tool_uuid", None)
-        if tool_uuid:
+        if tool_uuid := getattr(self, "tool_uuid", None):
             step.dynamic_tool = self.trans.app.dynamic_tool_manager.get_tool_by_uuid(tool_uuid)
         if not detached:
             for k, v in self.post_job_actions.items():
                 pja = self.__to_pja(k, v, step)
                 self.trans.sa_session.add(pja)
 
     # ---- General attributes ------------------------------------------------
@@ -1840,17 +1833,19 @@
 
     def get_content_id(self):
         return self.tool.id if self.tool else self.tool_id
 
     def get_version(self):
         return self.tool.version if self.tool else self.tool_version
 
-    def get_tooltip(self, static_path=""):
+    def get_tooltip(self, static_path=None):
         if self.tool and self.tool.help:
-            return self.tool.help.render(host_url=web.url_for("/"), static_path=static_path)
+            host_url = self.trans.url_builder("/")
+            static_path = self.trans.url_builder(static_path) if static_path else ""
+            return self.tool.help.render(host_url=host_url, static_path=static_path)
 
     # ---- Configuration time -----------------------------------------------
 
     def get_errors(self, include_tool_id=False, **kwargs):
         if not self.tool:
             if include_tool_id:
                 return f"{self.tool_id} is not installed"
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/refactor/execute.py` & `galaxy-app-24.0.0/galaxy/workflow/refactor/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             # action at a time or just performing actions that use raw_workflow_description.
             action_type = action.action_type
             refactor_method_name = f"_apply_{action_type}"
             refactor_method = getattr(self, refactor_method_name, None)
             if refactor_method is None:
                 raise RequestParameterInvalidException(f"Unknown workflow editing action encountered [{action_type}]")
             execution = RefactorActionExecution(
-                action=action.dict(),
+                action=action,
                 messages=[],
             )
             refactor_method(action, execution)
             action_executions.append(execution)
         return action_executions
 
     def _apply_update_step_label(self, action: UpdateStepLabelAction, execution: RefactorActionExecution):
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/refactor/schema.py` & `galaxy-app-24.0.0/galaxy/workflow/refactor/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,18 @@
     Union,
 )
 
 from pydantic import (
     BaseModel,
     Field,
 )
-from typing_extensions import Literal
+from typing_extensions import (
+    Annotated,
+    Literal,
+)
 
 LABEL_DESCRIPTION = "The unique label of the step being referenced."
 INPUT_NAME_DESCRIPTION = "The input name as defined by the workflow module corresponding to the step being referenced. For Galaxy tool steps these inputs should be normalized using '|' (e.g. 'cond|repeat_0|input')."
 input_name_field = Field(description=INPUT_NAME_DESCRIPTION)
 output_name_field = Field(
     description="The output name as defined by the workflow module corresponding to the step being referenced. The default is 'output', corresponding to the output defined by input step types.",
     default="output",
@@ -111,19 +114,20 @@
     After the workflow is updated, an order_index will be assigned
     and this step may cause other steps to have their output_index
     adjusted.
     """
 
     action_type: Literal["add_step"]
     type: str = Field(description="Module type of the step to add, see galaxy.workflow.modules for available types.")
-    tool_state: Optional[Dict[str, Any]]
+    tool_state: Optional[Dict[str, Any]] = None
     label: Optional[str] = Field(
-        description="A unique label for the step being added, must be distinct from the labels already present in the workflow."
+        None,
+        description="A unique label for the step being added, must be distinct from the labels already present in the workflow.",
     )
-    position: Optional[Position] = Field(description="The location of the step in the Galaxy workflow editor.")
+    position: Optional[Position] = Field(None, description="The location of the step in the Galaxy workflow editor.")
 
 
 class ConnectAction(BaseAction):
     action_type: Literal["connect"]
     input: input_reference_union
     output: output_reference_union
 
@@ -133,36 +137,36 @@
     input: input_reference_union
     output: output_reference_union
 
 
 class AddInputAction(BaseAction):
     action_type: Literal["add_input"]
     type: str
-    label: Optional[str]
-    position: Optional[Position]
-    collection_type: Optional[str]
-    restrictions: Optional[List[str]]
-    restrict_on_connections: Optional[bool]
-    suggestions: Optional[List[str]]
+    label: Optional[str] = None
+    position: Optional[Position] = None
+    collection_type: Optional[str] = None
+    restrictions: Optional[List[str]] = None
+    restrict_on_connections: Optional[bool] = None
+    suggestions: Optional[List[str]] = None
     optional: Optional[bool] = False
-    default: Optional[Any]  # this probably needs to be revisited when we have more complex field types
+    default: Optional[Any] = None  # this probably needs to be revisited when we have more complex field types
 
 
 class ExtractInputAction(BaseAction):
     action_type: Literal["extract_input"]
     input: input_reference_union
-    label: Optional[str]
-    position: Optional[Position]
+    label: Optional[str] = None
+    position: Optional[Position] = None
 
 
 class ExtractUntypedParameter(BaseAction):
     action_type: Literal["extract_untyped_parameter"]
     name: str
-    label: Optional[str]  # defaults to name if unset
-    position: Optional[Position]
+    label: Optional[str] = None  # defaults to name if unset
+    position: Optional[Position] = None
 
 
 class RemoveUnlabeledWorkflowOutputs(BaseAction):
     action_type: Literal["remove_unlabeled_workflow_outputs"]
 
 
 class UpdateNameAction(BaseAction):
@@ -178,15 +182,15 @@
 class UpdateLicenseAction(BaseAction):
     action_type: Literal["update_license"]
     license: str
 
 
 class UpdateCreatorAction(BaseAction):
     action_type: Literal["update_creator"]
-    creator: Any
+    creator: Any = None
 
 
 class Report(BaseModel):
     markdown: str
 
 
 class UpdateReportAction(BaseAction):
@@ -210,21 +214,21 @@
 
 
 class UpgradeSubworkflowAction(BaseAction):
     action_type: Literal["upgrade_subworkflow"]
     step: step_reference_union = step_target_field
     # Once we start storing these actions in the database, this needs to be decoded
     # before adding it into the database.
-    content_id: Optional[str]
+    content_id: Optional[str] = None
 
 
 class UpgradeToolAction(BaseAction):
     action_type: Literal["upgrade_tool"]
     step: step_reference_union = step_target_field
-    tool_version: Optional[str]
+    tool_version: Optional[str] = None
 
 
 class UpgradeAllStepsAction(BaseAction):
     action_type: Literal["upgrade_all_steps"]
 
 
 union_action_classes = Union[
@@ -249,27 +253,27 @@
     UpgradeAllStepsAction,
     RemoveUnlabeledWorkflowOutputs,
 ]
 
 
 ACTION_CLASSES_BY_TYPE = {}
 for action_class in union_action_classes.__args__:  # type: ignore[attr-defined]
-    action_type_def = action_class.schema()["properties"]["action_type"]
+    action_type_def = action_class.model_json_schema()["properties"]["action_type"]
     try:
         # pydantic 1.8
         action_type = action_type_def["enum"][0]
     except KeyError:
         # pydantic 1.7
         action_type = action_type_def["const"]
 
     ACTION_CLASSES_BY_TYPE[action_type] = action_class
 
 
 class RefactorActions(BaseModel):
-    actions: List[Action]
+    actions: List[Annotated[union_action_classes, Field(discriminator="action_type")]]
     dry_run: bool = False
 
 
 class RefactorActionExecutionMessageTypeEnum(str, Enum):
     tool_version_change = "tool_version_change"
     tool_state_adjustment = "tool_state_adjustment"
     connection_drop_forced = "connection_drop_forced"
@@ -286,16 +290,20 @@
 step with the previously connected input.
 """
 
 
 class RefactorActionExecutionMessage(BaseModel):
     message: str
     message_type: RefactorActionExecutionMessageTypeEnum
-    step_label: Optional[str] = Field(description=f"Reference to the step the message refers to. ${INPUT_REFERENCE}")
-    order_index: Optional[int] = Field(description=f"Reference to the step the message refers to. ${INPUT_REFERENCE}")
+    step_label: Optional[str] = Field(
+        None, description=f"Reference to the step the message refers to. ${INPUT_REFERENCE}"
+    )
+    order_index: Optional[int] = Field(
+        None, description=f"Reference to the step the message refers to. ${INPUT_REFERENCE}"
+    )
     input_name: Optional[str] = Field(
         None,
         description=f"""If this message is about an input to a step,
 this field describes the target input name. ${INPUT_NAME_DESCRIPTION}""",
     )
     output_name: Optional[str] = Field(
         None,
@@ -315,9 +323,9 @@
     )
     output_label: Optional[str] = Field(
         None, description="If the message_type is workflow_output_drop_forced, this is the output label dropped."
     )
 
 
 class RefactorActionExecution(BaseModel):
-    action: Action
+    action: union_action_classes
     messages: List[RefactorActionExecutionMessage]
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/render.py` & `galaxy-app-24.0.0/galaxy/workflow/render.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/workflow/reports/__init__.py` & `galaxy-app-24.0.0/galaxy/workflow/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/workflow/reports/generators/__init__.py` & `galaxy-app-24.0.0/galaxy/workflow/reports/generators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Module containing Galaxy workflow report generator plugins.
 """
+
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 
 from galaxy.managers import workflows
 from galaxy.managers.markdown_util import (
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/reports/generators/markdown.py` & `galaxy-app-24.0.0/galaxy/workflow/reports/generators/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """The class defines the default stock Galaxy workflow reporting plugin
 """
+
 import logging
 import string
 
 from . import WorkflowMarkdownGeneratorPlugin
 
 log = logging.getLogger(__name__)
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/resources/__init__.py` & `galaxy-app-24.0.0/galaxy/workflow/resources/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This package is something a placeholder for workflow resource parameters.
 
 This file defines the baked in resource mapper types, and this package contains an
 example of a more open, pluggable approach with greater control.
 """
+
 import functools
 import logging
 import os
 import sys
 from copy import deepcopy
 
 import yaml
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/resources/example.py.sample` & `galaxy-app-24.0.0/galaxy/workflow/resources/example.py.sample`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/workflow/run.py` & `galaxy-app-24.0.0/galaxy/workflow/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 
 from galaxy import model
 from galaxy.exceptions import MessageException
 from galaxy.model import (
     WorkflowInvocation,
     WorkflowInvocationStep,
 )
-from galaxy.model.base import transaction
+from galaxy.model.base import (
+    ensure_object_added_to_session,
+    transaction,
+)
 from galaxy.schema.invocation import (
     CancelReason,
     FailureReason,
     InvocationCancellationHistoryDeleted,
     InvocationFailureCollectionFailed,
     InvocationFailureDatasetFailed,
     InvocationFailureJobFailed,
@@ -221,14 +224,15 @@
             try:
                 self.__check_implicitly_dependent_steps(step)
 
                 if not workflow_invocation_step:
                     workflow_invocation_step = WorkflowInvocationStep()
                     assert workflow_invocation_step
                     workflow_invocation_step.workflow_invocation = workflow_invocation
+                    ensure_object_added_to_session(workflow_invocation_step, object_in_session=workflow_invocation)
                     workflow_invocation_step.workflow_step = step
                     workflow_invocation_step.state = "new"
 
                     workflow_invocation.steps.append(workflow_invocation_step)
 
                 assert workflow_invocation_step
                 incomplete_or_none = self._invoke_step(workflow_invocation_step)
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/run_request.py` & `galaxy-app-24.0.0/galaxy/workflow/run_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     HistoryDatasetCollectionAssociation,
     LibraryDataset,
     LibraryDatasetDatasetAssociation,
     WorkflowInvocation,
     WorkflowRequestInputParameter,
     WorkflowRequestStepState,
 )
-from galaxy.model.base import transaction
+from galaxy.model.base import (
+    ensure_object_added_to_session,
+    transaction,
+)
 from galaxy.tools.parameters.meta import expand_workflow_inputs
 from galaxy.workflow.resources import get_resource_mapper_function
 
 if TYPE_CHECKING:
     from galaxy.model import (
         Workflow,
         WorkflowStep,
@@ -198,16 +201,15 @@
     Note that this format allows only one parameter to be set per step.
     """
     param_dict = param_map.get(step.tool_id, {}).copy()
     if legacy:
         param_dict.update(param_map.get(str(step.id), {}))
     else:
         param_dict.update(param_map.get(str(step.order_index), {}))
-    step_uuid = step.uuid
-    if step_uuid:
+    if step_uuid := step.uuid:
         uuid_params = param_map.get(str(step_uuid), {})
         param_dict.update(uuid_params)
     if param_dict:
         if "param" in param_dict and "value" in param_dict:
             param_dict[param_dict["param"]] = param_dict["value"]
             del param_dict["param"]
             del param_dict["value"]
@@ -483,14 +485,15 @@
     trans: "GalaxyWebTransaction", run_config: WorkflowRunConfig, workflow: "Workflow"
 ) -> WorkflowInvocation:
     param_types = WorkflowRequestInputParameter.types
 
     workflow_invocation = WorkflowInvocation()
     workflow_invocation.uuid = uuid.uuid1()
     workflow_invocation.history = run_config.target_history
+    ensure_object_added_to_session(workflow_invocation, object_in_session=run_config.target_history)
 
     def add_parameter(name: str, value: str, type: WorkflowRequestInputParameter.types) -> None:
         parameter = WorkflowRequestInputParameter(
             name=name,
             value=value,
             type=type,
         )
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/schedulers/__init__.py` & `galaxy-app-24.0.0/galaxy/workflow/schedulers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Module containing Galaxy workflow scheduling plugins. Galaxy's interface
 for workflow scheduling is highly experimental and the interface required for
 scheduling plugins will almost certainly change.
 """
+
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 
 
 class WorkflowSchedulingPlugin(metaclass=ABCMeta):
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/schedulers/core.py` & `galaxy-app-24.0.0/galaxy/workflow/schedulers/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ The class defines the stock Galaxy workflow scheduling plugin - currently
 it simply schedules the whole workflow up front when offered.
 """
+
 import logging
 from typing import TYPE_CHECKING
 
 from galaxy.work import context
 from galaxy.workflow import (
     run,
     run_request,
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/scheduling_manager.py` & `galaxy-app-24.0.0/galaxy/workflow/scheduling_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/galaxy/workflow/steps.py` & `galaxy-app-24.0.0/galaxy/workflow/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ This module contains utility methods for reasoning about and ordering
 workflow steps.
 """
+
 import math
 
 from galaxy.util.topsort import (
     CycleError,
     topsort,
     topsort_levels,
 )
@@ -75,15 +76,15 @@
             ordered_comments = freehand_comments
             ordered_comments.extend(sortable_comments)
 
         # normalize steps by min_left and min_top
         for step in steps:
             step.position = {
                 "left": step.position["left"] - min_left,
-                "top": step.position["top"] - min_top
+                "top": step.position["top"] - min_top,
                 # other position attributes can be discarded if present
             }
 
         # order by Euclidean distance to the origin (i.e. pre-normalized (min_left, min_top))
         steps.sort(key=lambda _: math.sqrt(_.position["left"] ** 2 + _.position["top"] ** 2))
     try:
         edges = sorted(edgelist_for_workflow_steps(steps))
```

### Comparing `galaxy-app-23.2.1/galaxy/workflow/trs_proxy.py` & `galaxy-app-24.0.0/galaxy/workflow/trs_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,15 @@
         trs_url = self._server_dict[trs_server]["api_url"]
         return TrsServer(trs_url)
 
     def server_from_url(self, trs_url):
         return TrsServer(trs_url)
 
     def match_url(self, url):
-        matches = re.match(TRS_URL_REGEX, url)
-        if matches:
+        if matches := re.match(TRS_URL_REGEX, url):
             match_dict = matches.groupdict()
             match_dict["tool_id"] = urllib.parse.unquote(match_dict["tool_id"])
             return match_dict
         else:
             return None
```

### Comparing `galaxy-app-23.2.1/galaxy_app.egg-info/PKG-INFO` & `galaxy-app-24.0.0/galaxy_app.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,77 @@
 Metadata-Version: 2.1
 Name: galaxy-app
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy application (backend)
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-auth
+Requires-Dist: galaxy-config
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-files
+Requires-Dist: galaxy-job-execution
+Requires-Dist: galaxy-job-metrics
+Requires-Dist: galaxy-objectstore
+Requires-Dist: galaxy-tool-util[cwl,edam]
+Requires-Dist: galaxy-tours
+Requires-Dist: galaxy-util
+Requires-Dist: galaxy-web-framework
+Requires-Dist: galaxy-web-stack
+Requires-Dist: Beaker
+Requires-Dist: boltons
+Requires-Dist: bx-python
+Requires-Dist: celery
+Requires-Dist: cloudauthz==0.6.0
+Requires-Dist: dparse
+Requires-Dist: gxformat2
+Requires-Dist: kombu>=5.3
+Requires-Dist: lagom
+Requires-Dist: lxml!=4.2.2
+Requires-Dist: Mako
+Requires-Dist: Markdown
+Requires-Dist: MarkupSafe
+Requires-Dist: packaging
+Requires-Dist: paramiko!=2.9.0,!=2.9.1
+Requires-Dist: pebble
+Requires-Dist: pulsar-galaxy-lib>=0.15.0.dev0
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: pysam>=0.21
+Requires-Dist: PyJWT
+Requires-Dist: PyYAML
+Requires-Dist: refgenconf>=0.12.0
+Requires-Dist: regex
+Requires-Dist: requests
+Requires-Dist: SQLAlchemy<2,>=1.4.25
+Requires-Dist: sqlitedict
+Requires-Dist: starlette
+Requires-Dist: svgwrite
+Requires-Dist: typing-extensions
+Requires-Dist: WebOb
+Requires-Dist: Whoosh
 
 
 .. image:: https://badge.fury.io/py/galaxy-app.svg
    :target: https://pypi.org/project/galaxy-app/
 
 
 Overview
@@ -42,14 +85,114 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Reload built-in converters on toolbox reload by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17209 <https://github.com/galaxyproject/galaxy/pull/17209>`_
+* Optional Reply-to SMTP header in tool error reports by `@neoformit <https://github.com/neoformit>`_ in `#17243 <https://github.com/galaxyproject/galaxy/pull/17243>`_
+* Package tests fixes by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17301 <https://github.com/galaxyproject/galaxy/pull/17301>`_
+* Follow-up on #17274 and #17262 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17302 <https://github.com/galaxyproject/galaxy/pull/17302>`_
+* Rollback invalidated transaction: catch them earlier by `@jdavcs <https://github.com/jdavcs>`_ in `#17312 <https://github.com/galaxyproject/galaxy/pull/17312>`_
+* Fixes for flake8-bugbear 24.1.17 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17340 <https://github.com/galaxyproject/galaxy/pull/17340>`_
+* Fix data_source and data_source_async bugs by `@wm75 <https://github.com/wm75>`_ in `#17422 <https://github.com/galaxyproject/galaxy/pull/17422>`_
+* More efficient change_state queries, maybe fix deadlock by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17632 <https://github.com/galaxyproject/galaxy/pull/17632>`_
+* Don't index tasks without task_uuid by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17646 <https://github.com/galaxyproject/galaxy/pull/17646>`_
+* Separate `ConnectedValue` from `RuntimeValue` by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17678 <https://github.com/galaxyproject/galaxy/pull/17678>`_
+* Fix step type serialization for StoredWorkflowDetailed models by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17716 <https://github.com/galaxyproject/galaxy/pull/17716>`_
+* Fix usage of DISTINCT by `@jdavcs <https://github.com/jdavcs>`_ in `#17759 <https://github.com/galaxyproject/galaxy/pull/17759>`_
+* Also set extension and metadata on copies of job outputs when finishing job by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17777 <https://github.com/galaxyproject/galaxy/pull/17777>`_
+* Use ``hg clone --stream`` to clone repos by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17786 <https://github.com/galaxyproject/galaxy/pull/17786>`_
+* Defer job attributes that are usually not needed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17795 <https://github.com/galaxyproject/galaxy/pull/17795>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+* Fix archived histories mixing with active in histories list by `@davelopez <https://github.com/davelopez>`_ in `#17856 <https://github.com/galaxyproject/galaxy/pull/17856>`_
+* Normalize extensions when loading tool by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17868 <https://github.com/galaxyproject/galaxy/pull/17868>`_
+* Ignore user data table errors for now by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17880 <https://github.com/galaxyproject/galaxy/pull/17880>`_
+
+============
+Enhancements
+============
+
+* Add harmonize collections tool (or whatever other name) by `@lldelisle <https://github.com/lldelisle>`_ in `#16662 <https://github.com/galaxyproject/galaxy/pull/16662>`_
+* Add support for Python 3.12 by `@tuncK <https://github.com/tuncK>`_ in `#16796 <https://github.com/galaxyproject/galaxy/pull/16796>`_
+* SQLAlchemy 2.0 upgrades (part 5) by `@jdavcs <https://github.com/jdavcs>`_ in `#16932 <https://github.com/galaxyproject/galaxy/pull/16932>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
+* Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
+* Add select parameter with options from remote resources by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17087 <https://github.com/galaxyproject/galaxy/pull/17087>`_
+*  Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
+* Vueify Admin Roles Grid by `@guerler <https://github.com/guerler>`_ in `#17118 <https://github.com/galaxyproject/galaxy/pull/17118>`_
+* SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17123 <https://github.com/galaxyproject/galaxy/pull/17123>`_
+* Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
+* Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
+* Vueify Admin Forms and Quota grids by `@guerler <https://github.com/guerler>`_ in `#17141 <https://github.com/galaxyproject/galaxy/pull/17141>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17157 <https://github.com/galaxyproject/galaxy/pull/17157>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17201 <https://github.com/galaxyproject/galaxy/pull/17201>`_
+* Vendorize fastapi-utls.cbv by `@jdavcs <https://github.com/jdavcs>`_ in `#17205 <https://github.com/galaxyproject/galaxy/pull/17205>`_
+* Fix usage of graphene-sqlalchemy, bump to 3.0.0rc1 by `@jdavcs <https://github.com/jdavcs>`_ in `#17216 <https://github.com/galaxyproject/galaxy/pull/17216>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17230 <https://github.com/galaxyproject/galaxy/pull/17230>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17235 <https://github.com/galaxyproject/galaxy/pull/17235>`_
+* Allow job files to consume TUS uploads by `@jmchilton <https://github.com/jmchilton>`_ in `#17242 <https://github.com/galaxyproject/galaxy/pull/17242>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17247 <https://github.com/galaxyproject/galaxy/pull/17247>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Consider Null inputs by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17271 <https://github.com/galaxyproject/galaxy/pull/17271>`_
+* Add OIDC backend configuration schema and validation by `@uwwint <https://github.com/uwwint>`_ in `#17274 <https://github.com/galaxyproject/galaxy/pull/17274>`_
+* Adds delete, purge and undelete batch operations to History Grid by `@guerler <https://github.com/guerler>`_ in `#17282 <https://github.com/galaxyproject/galaxy/pull/17282>`_
+* Add ``__KEEP_SUCCESS_DATASETS__`` by `@lldelisle <https://github.com/lldelisle>`_ in `#17294 <https://github.com/galaxyproject/galaxy/pull/17294>`_
+* Improve ModelManager type hints by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17299 <https://github.com/galaxyproject/galaxy/pull/17299>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17333 <https://github.com/galaxyproject/galaxy/pull/17333>`_
+* Add element_identifier and ext to inputs config file export by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17357 <https://github.com/galaxyproject/galaxy/pull/17357>`_
+* Remove unused statements in job search function by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17361 <https://github.com/galaxyproject/galaxy/pull/17361>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Fix type annotation of code using XML etree by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17367 <https://github.com/galaxyproject/galaxy/pull/17367>`_
+* More specific type annotation for ``BaseJobExec.parse_status()`` by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17381 <https://github.com/galaxyproject/galaxy/pull/17381>`_
+* Cancel all active jobs when the user is deleted by `@davelopez <https://github.com/davelopez>`_ in `#17390 <https://github.com/galaxyproject/galaxy/pull/17390>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Purge `groups` and `roles` from DB (for real) by `@davelopez <https://github.com/davelopez>`_ in `#17411 <https://github.com/galaxyproject/galaxy/pull/17411>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17420 <https://github.com/galaxyproject/galaxy/pull/17420>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* Adds published histories to grid list by `@guerler <https://github.com/guerler>`_ in `#17449 <https://github.com/galaxyproject/galaxy/pull/17449>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* `data_column` parameter: use `column_names` metadata if present by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17478 <https://github.com/galaxyproject/galaxy/pull/17478>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17486 <https://github.com/galaxyproject/galaxy/pull/17486>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+* Update k8s docker python to 3.12 by `@nuwang <https://github.com/nuwang>`_ in `#17494 <https://github.com/galaxyproject/galaxy/pull/17494>`_
+* add encode ID API endpoint by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#17510 <https://github.com/galaxyproject/galaxy/pull/17510>`_
+* Fixing data_source tools and incrementing tool profile by `@wm75 <https://github.com/wm75>`_ in `#17515 <https://github.com/galaxyproject/galaxy/pull/17515>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17541 <https://github.com/galaxyproject/galaxy/pull/17541>`_
+* Add `image_diff` comparison method for test output verification using images by `@kostrykin <https://github.com/kostrykin>`_ in `#17556 <https://github.com/galaxyproject/galaxy/pull/17556>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17580 <https://github.com/galaxyproject/galaxy/pull/17580>`_
+* Restore histories API behavior for `keys` query parameter by `@davelopez <https://github.com/davelopez>`_ in `#17779 <https://github.com/galaxyproject/galaxy/pull/17779>`_
+* Fix datasets API custom keys encoding by `@davelopez <https://github.com/davelopez>`_ in `#17793 <https://github.com/galaxyproject/galaxy/pull/17793>`_
+* Improved error messages for runtime sharing problems. by `@jmchilton <https://github.com/jmchilton>`_ in `#17794 <https://github.com/galaxyproject/galaxy/pull/17794>`_
+* Allow admin to sharpen language about selected object stores. by `@jmchilton <https://github.com/jmchilton>`_ in `#17806 <https://github.com/galaxyproject/galaxy/pull/17806>`_
+
+=============
+Other changes
+=============
+
+* consistently compare profile versions by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16492 <https://github.com/galaxyproject/galaxy/pull/16492>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -119,15 +262,15 @@
 * Workflow Comments 💬 by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#16612 <https://github.com/galaxyproject/galaxy/pull/16612>`_
 * Switch out conditional requirement parser by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16636 <https://github.com/galaxyproject/galaxy/pull/16636>`_
 * Add scroll pagination and username filter to `HistoryPublishedList` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#16642 <https://github.com/galaxyproject/galaxy/pull/16642>`_
 * Bump samtools converters by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16668 <https://github.com/galaxyproject/galaxy/pull/16668>`_
 * Galaxy Markdown - add workflow image and license to Galaxy markdown. by `@jmchilton <https://github.com/jmchilton>`_ in `#16672 <https://github.com/galaxyproject/galaxy/pull/16672>`_
 * Implement instance URLs in Galaxy markdown. by `@jmchilton <https://github.com/jmchilton>`_ in `#16675 <https://github.com/galaxyproject/galaxy/pull/16675>`_
 * Change Sentry error reporting plug-in by `@kysrpex <https://github.com/kysrpex>`_ in `#16686 <https://github.com/galaxyproject/galaxy/pull/16686>`_
-*  Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
+* Use fs.onedatarestfs for Onedata files source plugin implementation by `@lopiola <https://github.com/lopiola>`_ in `#16690 <https://github.com/galaxyproject/galaxy/pull/16690>`_
 * Enhance task monitor composable by `@davelopez <https://github.com/davelopez>`_ in `#16695 <https://github.com/galaxyproject/galaxy/pull/16695>`_
 * Misc. edits/refactorings to session handling  by `@jdavcs <https://github.com/jdavcs>`_ in `#16712 <https://github.com/galaxyproject/galaxy/pull/16712>`_
 * SQLAlchemy 2.0 upgrades (part 2) by `@jdavcs <https://github.com/jdavcs>`_ in `#16724 <https://github.com/galaxyproject/galaxy/pull/16724>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16735 <https://github.com/galaxyproject/galaxy/pull/16735>`_
 * Convert ISO to UTC for Date/Time in workflow reports by `@assuntad23 <https://github.com/assuntad23>`_ in `#16758 <https://github.com/galaxyproject/galaxy/pull/16758>`_
 * Replace ELIXIR AAI button with Life Science login by `@sebastian-schaaf <https://github.com/sebastian-schaaf>`_ in `#16762 <https://github.com/galaxyproject/galaxy/pull/16762>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16770 <https://github.com/galaxyproject/galaxy/pull/16770>`_
```

### Comparing `galaxy-app-23.2.1/galaxy_app.egg-info/SOURCES.txt` & `galaxy-app-24.0.0/galaxy_app.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -153,14 +153,15 @@
 galaxy/managers/tags.py
 galaxy/managers/tasks.py
 galaxy/managers/tool_data.py
 galaxy/managers/tools.py
 galaxy/managers/users.py
 galaxy/managers/visualizations.py
 galaxy/managers/workflows.py
+galaxy/short_term_storage/__init__.py
 galaxy/tool_shed/__init__.py
 galaxy/tool_shed/cache.py
 galaxy/tool_shed/repository_type.py
 galaxy/tool_shed/galaxy_install/__init__.py
 galaxy/tool_shed/galaxy_install/client.py
 galaxy/tool_shed/galaxy_install/install_manager.py
 galaxy/tool_shed/galaxy_install/installed_repository_manager.py
@@ -203,14 +204,16 @@
 galaxy/tools/exception_handling.py
 galaxy/tools/execute.py
 galaxy/tools/extract_dataset.xml
 galaxy/tools/filter_empty_collection.xml
 galaxy/tools/filter_failed_collection.xml
 galaxy/tools/filter_from_file.xml
 galaxy/tools/flatten_collection.xml
+galaxy/tools/harmonize_two_collections_list.xml
+galaxy/tools/keep_success_collection.xml
 galaxy/tools/merge_collection.xml
 galaxy/tools/recommendations.py
 galaxy/tools/relabel_from_file.xml
 galaxy/tools/remote_tool_eval.py
 galaxy/tools/repositories.py
 galaxy/tools/sort_collection_list.xml
 galaxy/tools/special_tools.py
@@ -382,14 +385,15 @@
 galaxy/tools/bundled/interactive/interactivetool_openrefine.xml
 galaxy/tools/bundled/interactive/interactivetool_pangeo_notebook.xml
 galaxy/tools/bundled/interactive/interactivetool_panoply.xml
 galaxy/tools/bundled/interactive/interactivetool_paraview.xml
 galaxy/tools/bundled/interactive/interactivetool_pavian.xml
 galaxy/tools/bundled/interactive/interactivetool_phinch.xml
 galaxy/tools/bundled/interactive/interactivetool_pyiron.xml
+galaxy/tools/bundled/interactive/interactivetool_qiskit_jupyter_notebook.xml
 galaxy/tools/bundled/interactive/interactivetool_radiant.xml
 galaxy/tools/bundled/interactive/interactivetool_rstudio.xml
 galaxy/tools/bundled/interactive/interactivetool_simtext_app.xml
 galaxy/tools/bundled/interactive/interactivetool_vcf_iobio.xml
 galaxy/tools/bundled/interactive/interactivetool_vrm_editor.xml
 galaxy/tools/bundled/interactive/interactivetool_wallace.xml
 galaxy/tools/bundled/interactive/interactivetool_wilson.xml
@@ -534,22 +538,24 @@
 galaxy/tools/imp_exp/exp_history_to_archive.xml
 galaxy/tools/imp_exp/exp_history_to_uri.xml
 galaxy/tools/imp_exp/export_history.py
 galaxy/tools/imp_exp/imp_history_from_archive.xml
 galaxy/tools/imp_exp/unpack_tar_gz_archive.py
 galaxy/tools/parameters/__init__.py
 galaxy/tools/parameters/basic.py
+galaxy/tools/parameters/cancelable_request.py
 galaxy/tools/parameters/dataset_matcher.py
 galaxy/tools/parameters/dynamic_options.py
 galaxy/tools/parameters/grouping.py
 galaxy/tools/parameters/history_query.py
 galaxy/tools/parameters/input_translation.py
 galaxy/tools/parameters/meta.py
 galaxy/tools/parameters/sanitize.py
 galaxy/tools/parameters/validation.py
+galaxy/tools/parameters/workflow_building_modes.py
 galaxy/tools/parameters/wrapped.py
 galaxy/tools/parameters/wrapped_json.py
 galaxy/tools/search/__init__.py
 galaxy/tools/util/__init__.py
 galaxy/tools/util/maf_utilities.py
 galaxy/tools/util/galaxyops/__init__.py
 galaxy/visualization/__init__.py
```

### Comparing `galaxy-app-23.2.1/galaxy_app.egg-info/requires.txt` & `galaxy-app-24.0.0/galaxy_app.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 Beaker
 boltons
 bx-python
 celery
 cloudauthz==0.6.0
 dparse
 gxformat2
-importlib-metadata<5
-kombu
+kombu>=5.3
 lagom
-lxml
+lxml!=4.2.2
 Mako
 Markdown
 MarkupSafe
 packaging
 paramiko!=2.9.0,!=2.9.1
 pebble
 pulsar-galaxy-lib>=0.15.0.dev0
-pydantic<2
+pydantic!=2.6.0,!=2.6.1,>=2
 pysam>=0.21
 PyJWT
 PyYAML
 refgenconf>=0.12.0
 regex
 requests
 SQLAlchemy<2,>=1.4.25
```

### Comparing `galaxy-app-23.2.1/galaxy_ext/expressions/handle_job.py` & `galaxy-app-24.0.0/galaxy_ext/expressions/handle_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Execute an external process to evaluate expressions for Galaxy jobs.
 
 Galaxy should be importable on sys.path .
 """
+
 import json
 import logging
 import os
 import sys
 import warnings
 
 # insert *this* galaxy before all others on sys.path
```

### Comparing `galaxy-app-23.2.1/galaxy_ext/metadata/set_metadata.py` & `galaxy-app-24.0.0/galaxy_ext/metadata/set_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-23.2.1/setup.cfg` & `galaxy-app-24.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -5,33 +5,33 @@
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
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy application (backend)
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-app
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-auth
 	galaxy-config
 	galaxy-data
@@ -47,41 +47,40 @@
 	Beaker
 	boltons
 	bx-python
 	celery
 	cloudauthz==0.6.0
 	dparse
 	gxformat2
-	importlib-metadata<5  # Work around https://github.com/celery/kombu/issues/1600
-	kombu
+	kombu>=5.3
 	lagom
-	lxml
+	lxml!=4.2.2
 	Mako
 	Markdown
 	MarkupSafe
 	packaging
 	paramiko!=2.9.0,!=2.9.1
 	pebble
 	pulsar-galaxy-lib>=0.15.0.dev0
-	pydantic<2
+	pydantic>=2,!=2.6.0,!=2.6.1
 	pysam>=0.21
 	PyJWT
 	PyYAML
 	refgenconf>=0.12.0
 	regex
 	requests
 	SQLAlchemy>=1.4.25,<2
 	sqlitedict
 	starlette
 	svgwrite
 	typing-extensions
 	WebOb
 	Whoosh
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	galaxy-main = galaxy.main:main
 
 [options.packages.find]
 exclude =
```

### Comparing `galaxy-app-23.2.1/tool_shed_client/schema/__init__.py` & `galaxy-app-24.0.0/tool_shed_client/schema/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,32 @@
     Optional,
     Tuple,
     Union,
 )
 
 from pydantic import (
     BaseModel,
+    ConfigDict,
     Field,
+    RootModel,
 )
 from typing_extensions import (
     Literal,
     TypedDict,
 )
 
 
 class Repository(BaseModel):
     # element/collection view on the backend have same keys/impl
     id: str
     name: str
     owner: str
     type: str  # TODO: enum
-    remote_repository_url: Optional[str]
-    homepage_url: Optional[str]
+    remote_repository_url: Optional[str] = None
+    homepage_url: Optional[str] = None
     description: str
     user_id: str
     private: bool
     deleted: bool
     times_downloaded: int
     deprecated: bool
     create_time: str
@@ -42,16 +44,16 @@
 
 class RepositoryPermissions(BaseModel):
     allow_push: List[str]
     can_manage: bool  # can the requesting user manage the repository
     can_push: bool
 
 
-class RepositoryRevisionReadmes(BaseModel):
-    __root__: Dict[str, str]
+class RepositoryRevisionReadmes(RootModel):
+    root: Dict[str, str]
 
 
 class CreateUserRequest(BaseModel):
     username: str
     email: str
     password: str
 
@@ -87,16 +89,16 @@
 
 
 class GetOrderedInstallableRevisionsRequest(BaseModel):
     name: str
     owner: str
 
 
-class OrderedInstallableRevisions(BaseModel):
-    __root__: List[str]
+class OrderedInstallableRevisions(RootModel):
+    root: List[str]
 
 
 RepositoryType = Literal[
     "repository_suite_definition",
     "tool_dependency_definition",
     "unrestricted",
 ]
@@ -114,29 +116,27 @@
         title="Type",
     )
     category_ids: Optional[Union[List[str], str]] = Field(
         ...,
         alias="category_ids[]",
         title="Category IDs",
     )
-
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class RepositoryUpdateRequest(BaseModel):
     commit_message: Optional[str] = None
 
 
-class RepositoryUpdate(BaseModel):
-    __root__: Union[ValidRepostiroyUpdateMessage, FailedRepositoryUpdateMessage]
+class RepositoryUpdate(RootModel):
+    root: Union[ValidRepostiroyUpdateMessage, FailedRepositoryUpdateMessage]
 
     @property
     def is_ok(self):
-        return isinstance(self.__root__, ValidRepostiroyUpdateMessage)
+        return isinstance(self.root, ValidRepostiroyUpdateMessage)
 
 
 class RepositoryTool(BaseModel):
     # Added back in post v2 in order for the frontend to render
     # tool descriptions on the repository page.
     description: str
     guid: str
@@ -151,57 +151,54 @@
     # version_string_cmd: Optional[str]
 
 
 class RepositoryRevisionMetadata(BaseModel):
     id: str
     repository: Repository
     repository_dependencies: List["RepositoryDependency"]
-    tools: Optional[List["RepositoryTool"]]
+    tools: Optional[List["RepositoryTool"]] = None
     invalid_tools: List[str]  # added for rendering list of invalid tools in 2.0 frontend
     repository_id: str
     numeric_revision: int
     changeset_revision: str
     malicious: bool
     downloadable: bool
     missing_test_components: bool
     has_repository_dependencies: bool
     includes_tools: bool
     includes_tools_for_display_in_tool_panel: bool
     # Deprecate these...
-    includes_tool_dependencies: Optional[bool]
-    includes_datatypes: Optional[bool]
-    includes_workflows: Optional[bool]
+    includes_tool_dependencies: Optional[bool] = None
+    includes_datatypes: Optional[bool] = None
+    includes_workflows: Optional[bool] = None
 
 
 class RepositoryDependency(RepositoryRevisionMetadata):
     # This only needs properties for tests it seems?
     # e.g. test_0550_metadata_updated_dependencies.py
     pass
 
 
-RepositoryRevisionMetadata.update_forward_refs()
-
-
-class RepositoryMetadata(BaseModel):
-    __root__: Dict[str, RepositoryRevisionMetadata]
+class RepositoryMetadata(RootModel):
+    root: Dict[str, RepositoryRevisionMetadata]
 
     @property
     def latest_revision(self) -> RepositoryRevisionMetadata:
-        return list(self.__root__.values())[-1]
+        return list(self.root.values())[-1]
 
     @property
     def tip(self) -> str:
         if self.is_new:
             return "000000000000"
         else:
             return self.latest_revision.changeset_revision
 
     @property
     def is_new(self) -> bool:
-        return len(self.__root__) == 0
+        return len(self.root) == 0
 
 
 class ResetMetadataOnRepositoryRequest(BaseModel):
     repository_id: str
 
 
 class ResetMetadataOnRepositoryResponse(BaseModel):
@@ -209,16 +206,16 @@
     repository_status: List[str]
     start_time: str
     stop_time: str
 
 
 class ToolSearchRequest(BaseModel):
     q: str
-    page: Optional[int]
-    page_size: Optional[int]
+    page: Optional[int] = None
+    page_size: Optional[int] = None
 
 
 class ToolSearchHitTool(BaseModel):
     id: str
     repo_owner_username: str
     repo_name: str
     name: str
@@ -249,46 +246,46 @@
                 matching_hit = hit
                 break
 
         return matching_hit
 
 
 class RepositoryIndexRequest(BaseModel):
-    owner: Optional[str]
-    name: Optional[str]
+    owner: Optional[str] = None
+    name: Optional[str] = None
     deleted: str = "false"
 
 
 class RepositoriesByCategory(BaseModel):
     id: str
     name: str
     description: str
     repository_count: int
     repositories: List[Repository]
 
 
-class RepositoryIndexResponse(BaseModel):
-    __root__: List[Repository]
+class RepositoryIndexResponse(RootModel):
+    root: List[Repository]
 
 
 class RepositorySearchRequest(BaseModel):
     q: str
-    page: Optional[int]
-    page_size: Optional[int]
+    page: Optional[int] = None
+    page_size: Optional[int] = None
 
 
 class RepositorySearchResult(BaseModel):
     id: str
     name: str
     repo_owner_username: str
     description: str
-    long_description: Optional[str]
-    remote_repository_url: Optional[str]
-    homepage_url: Optional[str]
-    last_update: Optional[str]
+    long_description: Optional[str] = None
+    remote_repository_url: Optional[str] = None
+    homepage_url: Optional[str] = None
+    last_update: Optional[str] = None
     full_last_updated: str
     repo_lineage: str
     approved: bool
     times_downloaded: int
     categories: str
 
 
@@ -370,15 +367,15 @@
 class RepositoryExtraInstallInfo(BaseModel):
     name: str
     description: str
     repository_clone_url: str
     changeset_revision: str
     ctx_rev: str
     repository_owner: str
-    repository_dependencies: Optional[Dict]
+    repository_dependencies: Optional[Dict] = None
     # tool dependencies not longer work so don't transmit them in v2?
     # tool_dependencies: Optional[Dict]
 
     @staticmethod
     def from_legacy_dict(as_dict: ExtraRepoInfo) -> "RepositoryExtraInstallInfo":
         assert len(as_dict) == 1
         repo_name = next(iter(as_dict.keys()))
@@ -401,15 +398,15 @@
     id: str
     name: str
     requirements: list
     tests: list
     tool_config: str
     tool_type: str
     version: str
-    version_string_cmd: Optional[str]
+    version_string_cmd: Optional[str] = None
 
     @staticmethod
     def from_legacy_dict(as_dict: ValidToolDict) -> "ValidTool":
         return ValidTool(**as_dict)
 
     @staticmethod
     def from_legacy_list(as_dicts: List[ValidToolDict]) -> List["ValidTool"]:
@@ -422,15 +419,15 @@
     downloadable: bool
     has_repository_dependencies: bool
     includes_tools: bool
     includes_tools_for_display_in_tool_panel: bool
     malicious: bool
     repository_id: str
     url: str
-    valid_tools: List[ValidToolDict]
+    valid_tools: List[ValidTool]
     # no longer used, don't transmit.
     # has_repository_dependencies_only_if_compiling_contained_td: bool
     # includes_datatypes: bool
     # includes_tool_dependencies: bool
     # includes_workflows: bool
 
     @staticmethod
@@ -446,16 +443,16 @@
             repository_id=as_dict["repository_id"],
             url=as_dict["url"],
             valid_tools=ValidTool.from_legacy_list(as_dict.get("valid_tools", [])),
         )
 
 
 class InstallInfo(BaseModel):
-    metadata_info: Optional[RepositoryMetadataInstallInfo]
-    repo_info: Optional[RepositoryExtraInstallInfo]
+    metadata_info: Optional[RepositoryMetadataInstallInfo] = None
+    repo_info: Optional[RepositoryExtraInstallInfo] = None
 
 
 def from_legacy_install_info(legacy_install_info: LegacyInstallInfoTuple) -> InstallInfo:
     repo_metadata_install_info: Union[RepositoryMetadataInstallInfoDict, EmptyDict]
     extra_info: Union[ExtraRepoInfo, EmptyDict]
     _, repo_metadata_install_info, extra_info = legacy_install_info
     if repo_metadata_install_info:
```

### Comparing `galaxy-app-23.2.1/tool_shed_client/schema/trs.py` & `galaxy-app-24.0.0/tool_shed_client/schema/trs.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,23 @@
     Optional,
     Union,
 )
 
 from pydantic import (
     BaseModel,
     Field,
+    RootModel,
 )
 
 
 class Checksum(BaseModel):
     checksum: str = Field(..., description="The hex-string encoded checksum for the data. ")
     type: str = Field(
         ...,
-        description="The digest method used to create the checksum.\nThe value (e.g. `sha-256`) SHOULD be listed as `Hash Name String` in the https://github.com/ga4gh-discovery/ga4gh-checksum/blob/master/hash-alg.csv[GA4GH Checksum Hash Algorithm Registry].\nOther values MAY be used, as long as implementors are aware of the issues discussed in https://tools.ietf.org/html/rfc6920#section-9.4[RFC6920].\nGA4GH may provide more explicit guidance for use of non-IANA-registered algorithms in the future.",
+        description="The digest method used to create the checksum.\nThe value (e.g. `sha-256`) SHOULD be listed as `Hash Name String` in the https://github.com/ga4gh-discovery/ga4gh-checksum/blob/master/hash-alg.csv[GA4GH Checksum Hash Algorithm Registry].\nOther values MAY be used, as long as implementers are aware of the issues discussed in https://tools.ietf.org/html/rfc6920#section-9.4[RFC6920].\nGA4GH may provide more explicit guidance for use of non-IANA-registered algorithms in the future.",
     )
 
 
 class FileType(Enum):
     TEST_FILE = "TEST_FILE"
     PRIMARY_DESCRIPTOR = "PRIMARY_DESCRIPTOR"
     SECONDARY_DESCRIPTOR = "SECONDARY_DESCRIPTOR"
@@ -61,16 +62,16 @@
     CWL = "CWL"
     WDL = "WDL"
     NFL = "NFL"
     GALAXY = "GALAXY"
     SMK = "SMK"
 
 
-class DescriptorTypeVersion(BaseModel):
-    __root__: str = Field(
+class DescriptorTypeVersion(RootModel):
+    root: str = Field(
         ...,
         description="The language version for a given descriptor type. The version should correspond to the actual declared version of the descriptor. For example, tools defined in CWL could have a version of `v1.0.2` whereas WDL tools may have a version of `1.0` or `draft-2`",
     )
 
 
 class DescriptorTypeWithPlain(Enum):
     CWL = "CWL"
@@ -88,72 +89,74 @@
 class FileWrapper(BaseModel):
     content: Optional[str] = Field(
         None, description="The content of the file itself. One of url or content is required."
     )
     checksum: Optional[List[Checksum]] = Field(
         None,
         description="A production (immutable) tool version is required to have a hashcode. Not required otherwise, but might be useful to detect changes. ",
-        example=[{"checksum": "ea2a5db69bd20a42976838790bc29294df3af02b", "type": "sha1"}],
+        examples=[{"checksum": "ea2a5db69bd20a42976838790bc29294df3af02b", "type": "sha1"}],
     )
     image_type: Optional[Union[ImageType, DescriptorType]] = Field(
         None, description="Optionally return additional information on the type of file this is"
     )
     url: Optional[str] = Field(
         None,
         description="Optional url to the underlying content, should include version information, and can include a git hash.  Note that this URL should resolve to the raw unwrapped content that would otherwise be available in content. One of url or content is required.",
-        example={
-            "descriptorfile": {
-                "url": "https://raw.githubusercontent.com/ICGC-TCGA-PanCancer/pcawg_delly_workflow/ea2a5db69bd20a42976838790bc29294df3af02b/delly_docker/Delly.cwl"
-            },
-            "containerfile": {
-                "url": "https://raw.githubusercontent.com/ICGC-TCGA-PanCancer/pcawg_delly_workflow/c83478829802b4d36374870843821abe1b625a71/delly_docker/Dockerfile"
-            },
-        },
+        examples=[
+            {
+                "descriptorfile": {
+                    "url": "https://raw.githubusercontent.com/ICGC-TCGA-PanCancer/pcawg_delly_workflow/ea2a5db69bd20a42976838790bc29294df3af02b/delly_docker/Delly.cwl"
+                },
+                "containerfile": {
+                    "url": "https://raw.githubusercontent.com/ICGC-TCGA-PanCancer/pcawg_delly_workflow/c83478829802b4d36374870843821abe1b625a71/delly_docker/Dockerfile"
+                },
+            }
+        ],
     )
 
 
 class Error(BaseModel):
     code: int
     message: Optional[str] = "Internal Server Error"
 
 
 class ImageData(BaseModel):
     registry_host: Optional[str] = Field(
         None,
         description="A docker registry or a URL to a Singularity registry. Used along with image_name to locate a specific image.",
-        example=["registry.hub.docker.com"],
+        examples=["registry.hub.docker.com"],
     )
     image_name: Optional[str] = Field(
         None,
         description="Used in conjunction with a registry_url if provided to locate images.",
-        example=["quay.io/seqware/seqware_full/1.1", "ubuntu:latest"],
+        examples=["quay.io/seqware/seqware_full/1.1", "ubuntu:latest"],
     )
     size: Optional[int] = Field(None, description="Size of the container in bytes.")
     updated: Optional[str] = Field(None, description="Last time the container was updated.")
     checksum: Optional[List[Checksum]] = Field(
         None,
         description="A production (immutable) tool version is required to have a hashcode. Not required otherwise, but might be useful to detect changes.  This exposes the hashcode for specific image versions to verify that the container version pulled is actually the version that was indexed by the registry.",
-        example=[{"checksum": "77af4d6b9913e693e8d0b4b294fa62ade6054e6b2f1ffb617ac955dd63fb0182", "type": "sha256"}],
+        examples=[{"checksum": "77af4d6b9913e693e8d0b4b294fa62ade6054e6b2f1ffb617ac955dd63fb0182", "type": "sha256"}],
     )
     image_type: Optional[ImageType] = None
 
 
 class ToolVersion(BaseModel):
     author: Optional[List[str]] = Field(
         None,
         description="Contact information for the author of this version of the tool in the registry. (More complex authorship information is handled by the descriptor).",
     )
     name: Optional[str] = Field(None, description="The name of the version.")
     url: str = Field(
         ...,
         description="The URL for this tool version in this registry.",
-        example="http://agora.broadinstitute.org/tools/123456/versions/1",
+        examples=["http://agora.broadinstitute.org/tools/123456/versions/1"],
     )
     id: str = Field(
-        ..., description="An identifier of the version of this tool for this particular tool registry.", example="v1"
+        ..., description="An identifier of the version of this tool for this particular tool registry.", examples=["v1"]
     )
     is_production: Optional[bool] = Field(
         None,
         description="This version of a tool is guaranteed to not change over time (for example, a  tool built from a tag in git as opposed to a branch). A production quality tool  is required to have a checksum",
     )
     images: Optional[List[ImageData]] = Field(
         None,
@@ -161,15 +164,15 @@
     )
     descriptor_type: Optional[List[DescriptorType]] = Field(
         None, description="The type (or types) of descriptors available."
     )
     descriptor_type_version: Optional[Dict[str, List[DescriptorTypeVersion]]] = Field(
         None,
         description="A map providing information about the language versions used in this tool. The keys should be the same values used in the `descriptor_type` field, and the value should be an array of all the language versions used for the given `descriptor_type`. Depending on the `descriptor_type` (e.g. CWL) multiple version values may be used in a single tool.",
-        example='{\n  "WDL": ["1.0", "1.0"],\n  "CWL": ["v1.0.2"],\n  "NFL": ["DSL2"]\n}\n',
+        examples=['{\n  "WDL": ["1.0", "1.0"],\n  "CWL": ["v1.0.2"],\n  "NFL": ["DSL2"]\n}\n'],
     )
     containerfile: Optional[bool] = Field(
         None,
         description="Reports if this tool has a containerfile available. (For Docker-based tools, this would indicate the presence of a Dockerfile)",
     )
     meta_version: Optional[str] = Field(
         None,
@@ -181,25 +184,25 @@
     verified_source: Optional[List[str]] = Field(
         None, description="Source of metadata that can support a verified tool, such as an email or URL."
     )
     signed: Optional[bool] = Field(None, description="Reports whether this version of the tool has been signed.")
     included_apps: Optional[List[str]] = Field(
         None,
         description="An array of IDs for the applications that are stored inside this tool.",
-        example=["https://bio.tools/tool/mytum.de/SNAP2/1", "https://bio.tools/bioexcel_seqqc"],
+        examples=["https://bio.tools/tool/mytum.de/SNAP2/1", "https://bio.tools/bioexcel_seqqc"],
     )
 
 
 class Tool(BaseModel):
     url: str = Field(
         ...,
         description="The URL for this tool in this registry.",
-        example="http://agora.broadinstitute.org/tools/123456",
+        examples=["http://agora.broadinstitute.org/tools/123456"],
     )
-    id: str = Field(..., description="A unique identifier of the tool, scoped to this registry.", example=123456)
+    id: str = Field(..., description="A unique identifier of the tool, scoped to this registry.", examples=[123456])
     aliases: Optional[List[str]] = Field(
         None,
         description="Support for this parameter is optional for tool registries that support aliases.\nA list of strings that can be used to identify this tool which could be  straight up URLs. \nThis can be used to expose alternative ids (such as GUIDs) for a tool\nfor registries. Can be used to match tools across registries.",
     )
     organization: str = Field(..., description="The organization that published the image.")
     name: Optional[str] = Field(None, description="The name of the tool.")
     toolclass: ToolClass
```

### Comparing `galaxy-app-23.2.1/tool_shed_client/schema/trs_service_info.py` & `galaxy-app-24.0.0/tool_shed_client/schema/trs_service_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,76 +12,76 @@
     BaseModel,
     Field,
 )
 
 
 class Organization(BaseModel):
     name: str = Field(
-        ..., description="Name of the organization responsible for the service", example="My organization"
+        ..., description="Name of the organization responsible for the service", examples=["My organization"]
     )
     url: AnyUrl = Field(
-        ..., description="URL of the website of the organization (RFC 3986 format)", example="https://example.com"
+        ..., description="URL of the website of the organization (RFC 3986 format)", examples=["https://example.com"]
     )
 
 
 class ServiceType(BaseModel):
     group: str = Field(
         ...,
         description="Namespace in reverse domain name format. Use `org.ga4gh` for implementations compliant with official GA4GH specifications. For services with custom APIs not standardized by GA4GH, or implementations diverging from official GA4GH specifications, use a different namespace (e.g. your organization's reverse domain name).",
-        example="org.ga4gh",
+        examples=["org.ga4gh"],
     )
     artifact: str = Field(
         ...,
         description="Name of the API or GA4GH specification implemented. Official GA4GH types should be assigned as part of standards approval process. Custom artifacts are supported.",
-        example="beacon",
+        examples=["beacon"],
     )
     version: str = Field(
         ...,
         description="Version of the API or specification. GA4GH specifications use semantic versioning.",
-        example="1.0.0",
+        examples=["1.0.0"],
     )
 
 
 class Service(BaseModel):
     id: str = Field(
         ...,
         description="Unique ID of this service. Reverse domain name notation is recommended, though not required. The identifier should attempt to be globally unique so it can be used in downstream aggregator services e.g. Service Registry.",
-        example="org.ga4gh.myservice",
+        examples=["org.ga4gh.myservice"],
     )
-    name: str = Field(..., description="Name of this service. Should be human readable.", example="My project")
+    name: str = Field(..., description="Name of this service. Should be human readable.", examples=["My project"])
     type: ServiceType
     description: Optional[str] = Field(
         None,
         description="Description of the service. Should be human readable and provide information about the service.",
-        example="This service provides...",
+        examples=["This service provides..."],
     )
     organization: Organization = Field(..., description="Organization providing the service")
     contactUrl: Optional[AnyUrl] = Field(
         None,
         description="URL of the contact for the provider of this service, e.g. a link to a contact form (RFC 3986 format), or an email (RFC 2368 format).",
-        example="mailto:support@example.com",
+        examples=["mailto:support@example.com"],
     )
     documentationUrl: Optional[AnyUrl] = Field(
         None,
         description="URL of the documentation of this service (RFC 3986 format). This should help someone learn how to use your service, including any specifics required to access data, e.g. authentication.",
-        example="https://docs.myservice.example.com",
+        examples=["https://docs.myservice.example.com"],
     )
     createdAt: Optional[datetime] = Field(
         None,
         description="Timestamp describing when the service was first deployed and available (RFC 3339 format)",
-        example="2019-06-04T12:58:19Z",
+        examples=["2019-06-04T12:58:19Z"],
     )
     updatedAt: Optional[datetime] = Field(
         None,
         description="Timestamp describing when the service was last updated (RFC 3339 format)",
-        example="2019-06-04T12:58:19Z",
+        examples=["2019-06-04T12:58:19Z"],
     )
     environment: Optional[str] = Field(
         None,
         description="Environment the service is running in. Use this to distinguish between production, development and testing/staging deployments. Suggested values are prod, test, dev, staging. However this is advised and not enforced.",
-        example="test",
+        examples=["test"],
     )
     version: str = Field(
         ...,
         description="Version of the service being described. Semantic versioning is recommended, but other identifiers, such as dates or commit hashes, are also allowed. The version should be changed whenever the service is updated.",
-        example="1.0.0",
+        examples=["1.0.0"],
     )
```

### Comparing `galaxy-app-23.2.1/tool_shed_client/trs_util.py` & `galaxy-app-24.0.0/tool_shed_client/trs_util.py`

 * *Files identical despite different names*

