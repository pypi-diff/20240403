# Comparing `tmp/yarn-dev-tools-2.0.0.tar.gz` & `tmp/yarn_dev_tools-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yarn-dev-tools-2.0.0.tar", max compression
+gzip compressed data, was "yarn_dev_tools-2.0.1.tar", max compression
```

## Comparing `yarn-dev-tools-2.0.0.tar` & `yarn_dev_tools-2.0.1.tar`

### file list

```diff
@@ -1,102 +1,101 @@
--rwxr-xr-x   0        0        0     1286 2020-08-18 18:59:10.000000 yarn-dev-tools-2.0.0/LICENSE
--rwxr-xr-x   0        0        0     8774 2023-04-05 01:08:00.058196 yarn-dev-tools-2.0.0/README.md
--rw-r--r--   0        0        0     1516 2023-04-05 01:08:06.458083 yarn-dev-tools-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        8 2022-01-06 12:10:58.591525 yarn-dev-tools-2.0.0/yarndevtools/.gitignore
--rw-r--r--   0        0        0        0 2020-08-18 19:22:37.000000 yarn-dev-tools-2.0.0/yarndevtools/__init__.py
--rw-r--r--   0        0        0     4427 2023-04-05 01:08:00.070672 yarn-dev-tools-2.0.0/yarndevtools/argparser.py
--rw-r--r--   0        0        0       62 2022-01-06 12:10:58.593052 yarn-dev-tools-2.0.0/yarndevtools/cdsw/.gitignore
--rw-r--r--   0        0        0      540 2022-10-07 15:04:39.588060 yarn-dev-tools-2.0.0/yarndevtools/cdsw/Dockerfile
--rw-r--r--   0        0        0        0 2022-01-06 12:10:58.594830 yarn-dev-tools-2.0.0/yarndevtools/cdsw/__init__.py
--rw-r--r--   0        0        0    12351 2023-04-05 01:08:00.071605 yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_common.py
--rw-r--r--   0        0        0    22094 2023-04-05 01:08:00.072542 yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_config.py
--rw-r--r--   0        0        0    16493 2023-04-05 01:08:00.073523 yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_runner.py
--rw-r--r--   0        0        0     3067 2023-04-05 01:08:00.074554 yarn-dev-tools-2.0.0/yarndevtools/cdsw/constants.py
--rw-r--r--   0        0        0        0 2022-01-28 12:46:19.326799 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/__init__.py
--rw-r--r--   0        0        0     3688 2022-03-25 07:44:59.852898 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/branch_comparator_job_config.py
--rw-r--r--   0        0        0     2710 2022-11-14 14:38:31.676456 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/jira_umbrella_data_fetcher_job_config.py
--rw-r--r--   0        0        0     2577 2022-03-25 07:44:59.854589 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/review_sheet_backport_updater_job_config.py
--rw-r--r--   0        0        0     2501 2022-03-25 07:44:59.855487 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/reviewsync_job_config.py
--rw-r--r--   0        0        0     4733 2023-04-05 01:08:00.075302 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/unit_test_result_aggregator_email_job_config.py
--rw-r--r--   0        0        0     5037 2022-01-28 12:46:19.330150 yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/unit_test_result_fetcher_job_config.py
--rw-r--r--   0        0        0        0 2022-01-06 12:12:38.991565 yarn-dev-tools-2.0.0/yarndevtools/cdsw/libreloader/__init__.py
--rw-r--r--   0        0        0     6288 2022-10-08 15:30:26.829864 yarn-dev-tools-2.0.0/yarndevtools/cdsw/libreloader/reload_dependencies.py
--rw-r--r--   0        0        0     9397 2022-01-06 12:12:38.994617 yarn-dev-tools-2.0.0/yarndevtools/cdsw/resources/cdsw_stacktrace_example.txt
--rw-r--r--   0        0        0     2493 2022-01-28 12:46:19.333950 yarn-dev-tools-2.0.0/yarndevtools/cdsw/restarter.py
--rwxr-xr-x   0        0        0     1145 2023-01-17 14:25:07.393686 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/clone_downstream_repos.sh
--rwxr-xr-x   0        0        0      893 2023-01-17 14:25:07.408136 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/clone_upstream_repos.sh
--rw-r--r--   0        0        0      980 2022-01-06 12:10:58.607176 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/clone_repos_python2.sh
--rwxr-xr-x   0        0        0      734 2022-01-06 12:10:58.607369 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/exit-test.py
--rwxr-xr-x   0        0        0      806 2022-01-06 12:10:58.607585 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/exit-test2.py
--rwxr-xr-x   0        0        0      149 2022-01-06 12:10:58.607845 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/test.py
--rwxr-xr-x   0        0        0       56 2022-01-06 12:10:58.608064 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/test.sh
--rw-r--r--   0        0        0     4243 2022-09-23 12:01:04.799569 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/initial-cdsw-setup.sh
--rw-r--r--   0        0        0      491 2022-10-07 15:05:52.226372 yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/install-requirements.sh
--rw-r--r--   0        0        0     2167 2022-11-12 11:48:51.946677 yarn-dev-tools-2.0.0/yarndevtools/cdsw/start_job.py
--rw-r--r--   0        0        0      516 2022-01-20 21:40:52.794108 yarn-dev-tools-2.0.0/yarndevtools/cdsw/unit-test-result-aggregator/skip_aggregation_defaults.txt
--rw-r--r--   0        0        0     2731 2021-03-26 06:41:50.421000 yarn-dev-tools-2.0.0/yarndevtools/cdsw_compat.py
--rw-r--r--   0        0        0        0 2020-08-16 20:16:33.000000 yarn-dev-tools-2.0.0/yarndevtools/commands/__init__.py
--rw-r--r--   0        0        0    11904 2023-04-05 01:08:00.076368 yarn-dev-tools-2.0.0/yarndevtools/commands/backporter.py
--rw-r--r--   0        0        0        0 2021-04-20 19:49:58.360499 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/__init__.py
--rw-r--r--   0        0        0    16165 2023-04-05 01:08:00.077338 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/branch_comparator.py
--rw-r--r--   0        0        0     5844 2021-04-20 19:49:58.361481 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/common.py
--rw-r--r--   0        0        0    17597 2022-03-25 07:44:59.858949 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/common_representation.py
--rw-r--r--   0        0        0    34636 2022-01-06 12:12:39.004030 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/group_matching.py
--rw-r--r--   0        0        0     4589 2021-05-05 17:23:20.255448 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/legacy_script.py
--rw-r--r--   0        0        0    23360 2023-04-05 01:08:00.078314 yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/simple_matching.py
--rw-r--r--   0        0        0     4954 2022-03-25 07:44:59.859747 yarn-dev-tools-2.0.0/yarndevtools/commands/format_patch_saver.py
--rw-r--r--   0        0        0     6268 2022-03-25 07:44:59.861044 yarn-dev-tools-2.0.0/yarndevtools/commands/patch_saver.py
--rw-r--r--   0        0        0     4847 2022-03-25 07:44:59.861741 yarn-dev-tools-2.0.0/yarndevtools/commands/review_branch_creator.py
--rw-r--r--   0        0        0        0 2022-01-06 12:12:39.005164 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/__init__.py
--rw-r--r--   0        0        0     1357 2022-02-23 14:40:39.023806 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/common.py
--rw-r--r--   0        0        0    11076 2022-03-25 07:44:59.862561 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/representation.py
--rw-r--r--   0        0        0     9083 2022-03-25 07:44:59.863362 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/review_sheet_backport_updater.py
--rwxr-xr-x   0        0        0     2499 2022-01-06 12:12:39.005969 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/README.md
--rw-r--r--   0        0        0        0 2022-01-06 12:12:39.006124 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/__init__.py
--rw-r--r--   0        0        0      482 2022-01-06 12:12:39.006438 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/common.py
--rw-r--r--   0        0        0    10819 2022-01-06 12:12:39.006765 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/jira_wrapper.py
--rw-r--r--   0        0        0    10904 2022-03-25 07:44:59.864473 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/representation.py
--rwxr-xr-x   0        0        0    16327 2022-06-21 17:12:39.479946 yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/reviewsync.py
--rw-r--r--   0        0        0     5274 2022-03-25 07:44:59.865969 yarn-dev-tools-2.0.0/yarndevtools/commands/send_latest_command_data_in_mail.py
--rw-r--r--   0        0        0        0 2022-01-06 12:10:58.625913 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 01:08:00.078483 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/__init__.py
--rw-r--r--   0        0        0    30693 2023-04-05 01:08:00.079967 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/aggregation.py
--rw-r--r--   0        0        0    16485 2023-04-05 01:08:00.080474 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/model.py
--rw-r--r--   0        0        0     3393 2023-04-05 01:08:00.081501 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/parser.py
--rw-r--r--   0        0        0      948 2023-04-05 01:08:00.082455 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/constants.py
--rw-r--r--   0        0        0     7395 2023-04-05 01:08:00.083377 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/aggregation.py
--rw-r--r--   0        0        0     1422 2023-04-05 01:08:00.083694 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/model.py
--rw-r--r--   0        0        0      245 2023-04-05 01:08:00.084499 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/parser.py
--rw-r--r--   0        0        0     2977 2023-04-05 01:08:00.084837 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/persistence.py
--rw-r--r--   0        0        0        0 2023-04-05 01:08:00.084984 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/__init__.py
--rw-r--r--   0        0        0     7695 2023-04-05 01:08:00.085978 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/config.py
--rw-r--r--   0        0        0     2106 2023-04-05 01:08:00.086633 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/parser.py
--rw-r--r--   0        0        0     6173 2023-04-05 01:08:00.087520 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/processor.py
--rw-r--r--   0        0        0     3263 2023-04-05 01:08:00.088492 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/gsheet.py
--rw-r--r--   0        0        0    33662 2023-04-05 01:08:00.090043 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/representation.py
--rw-r--r--   0        0        0     4787 2023-04-05 01:08:00.091411 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/unit_test_result_aggregator.py
--rw-r--r--   0        0        0        0 2022-01-06 12:12:39.010105 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/__init__.py
--rw-r--r--   0        0        0    20068 2023-04-05 01:08:00.092008 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/cache.py
--rw-r--r--   0        0        0     2235 2023-04-05 01:08:00.092400 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/common.py
--rw-r--r--   0        0        0     8475 2023-04-05 01:08:00.092749 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/db.py
--rw-r--r--   0        0        0     4344 2023-04-05 01:08:00.093106 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/email.py
--rw-r--r--   0        0        0     8528 2023-04-05 01:08:00.093705 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/jenkins.py
--rw-r--r--   0        0        0     5591 2023-04-05 01:08:00.094084 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/model.py
--rw-r--r--   0        0        0     6924 2023-04-05 01:08:00.094695 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/parser.py
--rwxr-xr-x   0        0        0    20496 2023-04-05 01:08:00.096137 yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/unit_test_result_fetcher.py
--rw-r--r--   0        0        0     5163 2022-03-25 07:44:59.870797 yarn-dev-tools-2.0.0/yarndevtools/commands/upstream_jira_patch_differ.py
--rw-r--r--   0        0        0     4427 2022-03-25 07:44:59.871519 yarn-dev-tools-2.0.0/yarndevtools/commands/upstream_pr_fetcher.py
--rw-r--r--   0        0        0        0 2022-01-06 12:12:39.011215 yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/__init__.py
--rw-r--r--   0        0        0     3116 2022-01-06 12:12:39.011504 yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/common.py
--rw-r--r--   0        0        0    11072 2022-03-25 07:44:59.872666 yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/representation.py
--rw-r--r--   0        0        0    30282 2022-10-07 15:04:28.669991 yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/upstream_jira_umbrella_fetcher.py
--rw-r--r--   0        0        0     5549 2022-03-25 07:44:59.874359 yarn-dev-tools-2.0.0/yarndevtools/commands/zip_latest_command_data.py
--rw-r--r--   0        0        0    21980 2023-04-05 01:08:00.097596 yarn-dev-tools-2.0.0/yarndevtools/commands_common.py
--rw-r--r--   0        0        0        0 2022-01-06 12:10:58.634134 yarn-dev-tools-2.0.0/yarndevtools/common/__init__.py
--rw-r--r--   0        0        0     9647 2023-04-05 01:08:00.098260 yarn-dev-tools-2.0.0/yarndevtools/common/common_model.py
--rw-r--r--   0        0        0     7921 2023-04-05 01:08:00.099136 yarn-dev-tools-2.0.0/yarndevtools/common/db.py
--rw-r--r--   0        0        0    12378 2023-04-05 01:08:00.100462 yarn-dev-tools-2.0.0/yarndevtools/common/shared_command_utils.py
--rw-r--r--   0        0        0     1518 2022-10-07 15:04:28.706599 yarn-dev-tools-2.0.0/yarndevtools/constants.py
--rwxr-xr-x   0        0        0     6349 2023-04-05 01:08:00.101778 yarn-dev-tools-2.0.0/yarndevtools/yarn_dev_tools.py
--rw-r--r--   0        0        0      178 2022-03-25 07:44:59.878538 yarn-dev-tools-2.0.0/yarndevtools/yarn_dev_tools_config.py
--rw-r--r--   0        0        0    10651 1970-01-01 00:00:00.000000 yarn-dev-tools-2.0.0/setup.py
--rw-r--r--   0        0        0     9587 1970-01-01 00:00:00.000000 yarn-dev-tools-2.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1286 2020-08-18 18:59:10.000000 yarn_dev_tools-2.0.1/LICENSE
+-rwxr-xr-x   0        0        0     8774 2024-04-03 01:34:54.385801 yarn_dev_tools-2.0.1/README.md
+-rw-r--r--   0        0        0     1518 2024-04-03 01:40:59.408094 yarn_dev_tools-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0        8 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/.gitignore
+-rw-r--r--   0        0        0        0 2020-08-18 19:22:37.000000 yarn_dev_tools-2.0.1/yarndevtools/__init__.py
+-rw-r--r--   0        0        0     4427 2024-01-13 04:45:01.198501 yarn_dev_tools-2.0.1/yarndevtools/argparser.py
+-rw-r--r--   0        0        0       62 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/.gitignore
+-rw-r--r--   0        0        0      540 2022-10-07 15:04:39.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/Dockerfile
+-rw-r--r--   0        0        0        0 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/__init__.py
+-rw-r--r--   0        0        0    12351 2024-01-13 04:45:01.199270 yarn_dev_tools-2.0.1/yarndevtools/cdsw/cdsw_common.py
+-rw-r--r--   0        0        0    22094 2024-01-13 04:45:01.199968 yarn_dev_tools-2.0.1/yarndevtools/cdsw/cdsw_config.py
+-rw-r--r--   0        0        0    16493 2024-01-13 04:45:01.201048 yarn_dev_tools-2.0.1/yarndevtools/cdsw/cdsw_runner.py
+-rw-r--r--   0        0        0     3207 2024-04-02 21:08:57.498963 yarn_dev_tools-2.0.1/yarndevtools/cdsw/constants.py
+-rw-r--r--   0        0        0        0 2022-01-28 12:46:19.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/__init__.py
+-rw-r--r--   0        0        0     3688 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/branch_comparator_job_config.py
+-rw-r--r--   0        0        0     2710 2022-11-14 14:38:31.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/jira_umbrella_data_fetcher_job_config.py
+-rw-r--r--   0        0        0     2577 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/review_sheet_backport_updater_job_config.py
+-rw-r--r--   0        0        0     2501 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/reviewsync_job_config.py
+-rw-r--r--   0        0        0     4733 2024-01-13 04:45:01.202081 yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/unit_test_result_aggregator_email_job_config.py
+-rw-r--r--   0        0        0     5215 2024-04-02 21:08:57.501962 yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/unit_test_result_fetcher_job_config.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:38.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/libreloader/__init__.py
+-rw-r--r--   0        0        0     6288 2024-01-13 04:45:01.204085 yarn_dev_tools-2.0.1/yarndevtools/cdsw/libreloader/reload_dependencies.py
+-rw-r--r--   0        0        0     9397 2022-01-06 12:12:38.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/resources/cdsw_stacktrace_example.txt
+-rw-r--r--   0        0        0     2493 2022-01-28 12:46:19.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/restarter.py
+-rwxr-xr-x   0        0        0     1145 2023-09-22 22:11:56.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/clone_downstream_repos.sh
+-rwxr-xr-x   0        0        0      893 2023-09-22 22:11:56.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/clone_upstream_repos.sh
+-rw-r--r--   0        0        0      980 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/experiments/clone_repos_python2.sh
+-rwxr-xr-x   0        0        0      734 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/experiments/exit-test.py
+-rwxr-xr-x   0        0        0      806 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/experiments/exit-test2.py
+-rwxr-xr-x   0        0        0      149 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/experiments/test.py
+-rwxr-xr-x   0        0        0       56 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/experiments/test.sh
+-rw-r--r--   0        0        0     4243 2022-09-23 12:01:04.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/initial-cdsw-setup.sh
+-rw-r--r--   0        0        0      491 2024-01-13 04:45:01.204893 yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/install-requirements.sh
+-rw-r--r--   0        0        0     2167 2024-01-13 04:45:01.205626 yarn_dev_tools-2.0.1/yarndevtools/cdsw/start_job.py
+-rw-r--r--   0        0        0      516 2022-01-20 21:40:52.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw/unit-test-result-aggregator/skip_aggregation_defaults.txt
+-rw-r--r--   0        0        0     2731 2021-03-26 06:41:50.000000 yarn_dev_tools-2.0.1/yarndevtools/cdsw_compat.py
+-rw-r--r--   0        0        0        0 2020-08-16 20:16:33.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/__init__.py
+-rw-r--r--   0        0        0    11904 2024-04-02 21:08:57.502983 yarn_dev_tools-2.0.1/yarndevtools/commands/backporter.py
+-rw-r--r--   0        0        0        0 2021-04-20 19:49:58.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/__init__.py
+-rw-r--r--   0        0        0    16165 2024-01-13 04:45:01.207283 yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/branch_comparator.py
+-rw-r--r--   0        0        0     5844 2021-04-20 19:49:58.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/common.py
+-rw-r--r--   0        0        0    17597 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/common_representation.py
+-rw-r--r--   0        0        0    34636 2022-01-06 12:12:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/group_matching.py
+-rw-r--r--   0        0        0     4589 2021-05-05 17:23:20.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/legacy_script.py
+-rw-r--r--   0        0        0    23360 2024-01-13 04:45:01.208027 yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/simple_matching.py
+-rw-r--r--   0        0        0     4954 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/format_patch_saver.py
+-rw-r--r--   0        0        0     6268 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/patch_saver.py
+-rw-r--r--   0        0        0     4847 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/review_branch_creator.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsheetbackportupdater/__init__.py
+-rw-r--r--   0        0        0     1357 2022-02-23 14:40:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsheetbackportupdater/common.py
+-rw-r--r--   0        0        0    11076 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsheetbackportupdater/representation.py
+-rw-r--r--   0        0        0     9083 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsheetbackportupdater/review_sheet_backport_updater.py
+-rwxr-xr-x   0        0        0     2499 2022-01-06 12:12:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/README.md
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/__init__.py
+-rw-r--r--   0        0        0      482 2022-01-06 12:12:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/common.py
+-rw-r--r--   0        0        0    10819 2022-01-06 12:12:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/jira_wrapper.py
+-rw-r--r--   0        0        0    10904 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/representation.py
+-rwxr-xr-x   0        0        0    16327 2023-09-21 03:34:15.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/reviewsync.py
+-rw-r--r--   0        0        0     5274 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/send_latest_command_data_in_mail.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:45:01.208123 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/common/__init__.py
+-rw-r--r--   0        0        0    30693 2024-01-13 04:45:01.209378 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/common/aggregation.py
+-rw-r--r--   0        0        0    16485 2024-01-13 04:45:01.209582 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/common/model.py
+-rw-r--r--   0        0        0     3393 2024-01-13 04:45:01.210249 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/common/parser.py
+-rw-r--r--   0        0        0      948 2024-01-13 04:45:01.210943 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/constants.py
+-rw-r--r--   0        0        0     7395 2024-01-13 04:45:01.212376 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/db/aggregation.py
+-rw-r--r--   0        0        0     1422 2024-01-13 04:45:01.212581 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/db/model.py
+-rw-r--r--   0        0        0      245 2024-01-13 04:45:01.213424 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/db/parser.py
+-rw-r--r--   0        0        0     2977 2024-01-13 04:45:01.213718 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/db/persistence.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:45:01.213788 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/email/__init__.py
+-rw-r--r--   0        0        0     7695 2024-01-13 04:45:01.214305 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/email/config.py
+-rw-r--r--   0        0        0     2106 2024-01-13 04:45:01.215149 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/email/parser.py
+-rw-r--r--   0        0        0     6173 2024-01-13 04:45:01.216112 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/email/processor.py
+-rw-r--r--   0        0        0     3263 2024-01-13 04:45:01.216365 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/gsheet.py
+-rw-r--r--   0        0        0    33662 2024-01-13 04:45:01.216981 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/representation.py
+-rw-r--r--   0        0        0     4787 2024-01-13 04:45:01.217644 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/unit_test_result_aggregator.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/__init__.py
+-rw-r--r--   0        0        0    23770 2024-04-02 21:08:57.503977 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/cache.py
+-rw-r--r--   0        0        0     2235 2024-01-13 04:45:01.218160 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/common.py
+-rw-r--r--   0        0        0     8475 2024-01-13 04:45:01.218450 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/db.py
+-rw-r--r--   0        0        0     4344 2024-01-13 04:45:01.218596 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/email.py
+-rw-r--r--   0        0        0     8528 2024-04-02 21:08:57.504843 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/jenkins.py
+-rw-r--r--   0        0        0     5591 2024-01-13 04:45:01.220507 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/model.py
+-rw-r--r--   0        0        0     6963 2024-04-02 21:08:57.505514 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/parser.py
+-rwxr-xr-x   0        0        0    20125 2024-04-02 21:08:57.506167 yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/unit_test_result_fetcher.py
+-rw-r--r--   0        0        0     5163 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/upstream_jira_patch_differ.py
+-rw-r--r--   0        0        0     4427 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/upstream_pr_fetcher.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:12:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/upstreamumbrellafetcher/__init__.py
+-rw-r--r--   0        0        0     3116 2022-01-06 12:12:39.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/upstreamumbrellafetcher/common.py
+-rw-r--r--   0        0        0    11072 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/upstreamumbrellafetcher/representation.py
+-rw-r--r--   0        0        0    30282 2022-10-07 15:04:28.000000 yarn_dev_tools-2.0.1/yarndevtools/commands/upstreamumbrellafetcher/upstream_jira_umbrella_fetcher.py
+-rw-r--r--   0        0        0     5549 2024-01-13 04:45:01.222034 yarn_dev_tools-2.0.1/yarndevtools/commands/zip_latest_command_data.py
+-rw-r--r--   0        0        0    21980 2024-01-13 04:45:01.226850 yarn_dev_tools-2.0.1/yarndevtools/commands_common.py
+-rw-r--r--   0        0        0        0 2022-01-06 12:10:58.000000 yarn_dev_tools-2.0.1/yarndevtools/common/__init__.py
+-rw-r--r--   0        0        0     9647 2024-01-13 04:45:01.227077 yarn_dev_tools-2.0.1/yarndevtools/common/common_model.py
+-rw-r--r--   0        0        0     7921 2024-04-02 21:08:57.506710 yarn_dev_tools-2.0.1/yarndevtools/common/db.py
+-rw-r--r--   0        0        0    12378 2024-04-03 01:18:31.247244 yarn_dev_tools-2.0.1/yarndevtools/common/shared_command_utils.py
+-rw-r--r--   0        0        0     1518 2022-10-07 15:04:28.000000 yarn_dev_tools-2.0.1/yarndevtools/constants.py
+-rwxr-xr-x   0        0        0     6388 2024-04-02 21:08:57.507266 yarn_dev_tools-2.0.1/yarndevtools/yarn_dev_tools.py
+-rw-r--r--   0        0        0      178 2022-03-25 07:44:59.000000 yarn_dev_tools-2.0.1/yarndevtools/yarn_dev_tools_config.py
+-rw-r--r--   0        0        0     9690 1970-01-01 00:00:00.000000 yarn_dev_tools-2.0.1/PKG-INFO
```

### Comparing `yarn-dev-tools-2.0.0/LICENSE` & `yarn_dev_tools-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/README.md` & `yarn_dev_tools-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/pyproject.toml` & `yarn_dev_tools-2.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "yarn-dev-tools"
-version = "2.0.0"
+version = "2.0.1"
 description = ""
 authors = ["Szilard Nemeth <szilard.nemeth88@gmail.com>"]
 keywords = ["YARN", "development", "dev environment"]
 readme = "README.md"
 homepage = "https://github.com/szilard-nemeth/yarn-dev-tools"
 repository = "https://github.com/szilard-nemeth/yarn-dev-tools"
 packages = [{include = "yarndevtools"}]
@@ -32,16 +32,16 @@
 # TODO Verify if this is required
 [tool.setuptools.package-data]
 yarndevtools = ["cdsw/unit-test-result-aggregator/*.txt", "cdsw/scripts/*.sh"]
 
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
-python-common-lib = "1.0.6"
-google-api-wrapper2 = "1.0.5"
+python-common-lib = "1.0.9"
+google-api-wrapper2 = "1.0.10"
 gitpython = "*"
 humanize = "*"
 bs4 = "*"
 jira = "*"
 dataclasses-json = "*"
 dacite = "*"
 pymongo = "*"
@@ -72,14 +72,15 @@
 
 
 
 
 
 
 
+
 
 
 
 
 
 [tool.poetry.scripts]
 exec-yarndevtools = "yarndevtools.yarn_dev_tools:run"
```

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/argparser.py` & `yarn_dev_tools-2.0.1/yarndevtools/argparser.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/Dockerfile` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/Dockerfile`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_common.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/cdsw_common.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_config.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/cdsw_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/cdsw_runner.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/cdsw_runner.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/constants.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 # TODO Add default value of all env vars to enum
 # TODO Move all EnvVar classes to commands?
 class CdswEnvVar(Enum):
     MAIL_ACC_PASSWORD = "MAIL_ACC_PASSWORD"
     MAIL_ACC_USER = "MAIL_ACC_USER"
     MAIL_RECIPIENTS = "MAIL_RECIPIENTS"
+    # TODO Consider moving these to UnitTestResultFetcherEnvVar
+    JENKINS_USER = "JENKINS_USER"
+    JENKINS_PASSWORD = "JENKINS_PASSWORD"
     CLOUDERA_HADOOP_ROOT = YarnDevToolsEnvVar.ENV_CLOUDERA_HADOOP_ROOT.value
     HADOOP_DEV_DIR = YarnDevToolsEnvVar.ENV_HADOOP_DEV_DIR.value
     PYTHONPATH = "PYTHONPATH"
     TEST_EXECUTION_MODE = "TEST_EXEC_MODE"
     PYTHON_MODULE_MODE = "PYTHON_MODULE_MODE"
     ENABLE_GOOGLE_DRIVE_INTEGRATION = "ENABLE_GOOGLE_DRIVE_INTEGRATION"
     INSTALL_REQUIREMENTS = "INSTALL_REQUIREMENTS"
```

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/branch_comparator_job_config.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/branch_comparator_job_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/jira_umbrella_data_fetcher_job_config.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/jira_umbrella_data_fetcher_job_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/review_sheet_backport_updater_job_config.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/review_sheet_backport_updater_job_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/reviewsync_job_config.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/reviewsync_job_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/unit_test_result_aggregator_email_job_config.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/unit_test_result_aggregator_email_job_config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/job_configs/unit_test_result_fetcher_job_config.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/job_configs/unit_test_result_fetcher_job_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 )
 from yarndevtools.common.shared_command_utils import CommandType
 
 config = {
     "job_name": "Unit test result fetcher",
     "command_type": CommandType.UNIT_TEST_RESULT_FETCHER,
     "env_sanitize_exceptions": [],
-    "mandatory_env_vars": ["MAIL_ACC_USER", "MAIL_ACC_PASSWORD"],
+    "mandatory_env_vars": ["MAIL_ACC_USER", "MAIL_ACC_PASSWORD", "JENKINS_USER", "JENKINS_PASSWORD"],
     "optional_env_vars": ["BUILD_PROCESSING_LIMIT", "FORCE_SENDING_MAIL", "RESET_JOB_BUILD_DATA"],
     "yarn_dev_tools_arguments": [
         lambda conf: f"{Include.when(conf.var('debugMode'), '--debug', '')}",
         f"{CommandType.UNIT_TEST_RESULT_FETCHER.name}",
         lambda conf: f"--smtp_server {conf.var('smtp_server')}",
         lambda conf: f"--smtp_port {conf.var('smtp_port')}",
         lambda conf: f"--account_user {conf.env('MAIL_ACC_USER')}",
         lambda conf: f"--account_password {conf.env('MAIL_ACC_PASSWORD')}",
+        lambda conf: f"--jenkins-user {conf.env('JENKINS_USER')}",
+        lambda conf: f"--jenkins-password {conf.env('JENKINS_PASSWORD')}",
         lambda conf: f"--sender {conf.var('sender')}",
         lambda conf: f"--recipients {conf.var('recipients')}",
         lambda conf: f"--mode {conf.var('mode')}",
         lambda conf: f"--testcase-filter {conf.var('testcase_filters')}",
         lambda conf: f"--request-limit {conf.var('buildProcessingLimit')}",
         lambda conf: f"--num-builds {JENKINS_BUILDS_EXAMINE_UNLIMITIED_VAL}",
         lambda conf: f"{Include.when(conf.var('omitJobSummary'), '--omit-job-summary', '')}",
```

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/libreloader/reload_dependencies.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/libreloader/reload_dependencies.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/resources/cdsw_stacktrace_example.txt` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/resources/cdsw_stacktrace_example.txt`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/restarter.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/restarter.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/clone_downstream_repos.sh` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/clone_downstream_repos.sh`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/clone_upstream_repos.sh` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/clone_upstream_repos.sh`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/clone_repos_python2.sh` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/experiments/clone_repos_python2.sh`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/exit-test.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/experiments/exit-test.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/experiments/exit-test2.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/experiments/exit-test2.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/scripts/initial-cdsw-setup.sh` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/scripts/initial-cdsw-setup.sh`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/start_job.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/start_job.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw/unit-test-result-aggregator/skip_aggregation_defaults.txt` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw/unit-test-result-aggregator/skip_aggregation_defaults.txt`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/cdsw_compat.py` & `yarn_dev_tools-2.0.1/yarndevtools/cdsw_compat.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/backporter.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/backporter.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/branch_comparator.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/branch_comparator.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/common.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/common.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/common_representation.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/common_representation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/group_matching.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/group_matching.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/legacy_script.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/legacy_script.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/branchcomparator/simple_matching.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/branchcomparator/simple_matching.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/format_patch_saver.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/format_patch_saver.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/patch_saver.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/patch_saver.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/review_branch_creator.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/review_branch_creator.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/common.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsheetbackportupdater/common.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/representation.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsheetbackportupdater/representation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsheetbackportupdater/review_sheet_backport_updater.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsheetbackportupdater/review_sheet_backport_updater.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/README.md` & `yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/README.md`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/jira_wrapper.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/jira_wrapper.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/representation.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/representation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/reviewsync/reviewsync.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/reviewsync/reviewsync.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/send_latest_command_data_in_mail.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/send_latest_command_data_in_mail.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/aggregation.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/common/aggregation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/model.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/common/model.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/common/parser.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/common/parser.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/constants.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/constants.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/aggregation.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/db/aggregation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/model.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/db/model.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/db/persistence.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/db/persistence.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/config.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/email/config.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/parser.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/email/parser.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/email/processor.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/email/processor.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/gsheet.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/gsheet.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/representation.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/representation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultaggregator/unit_test_result_aggregator.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultaggregator/unit_test_result_aggregator.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/cache.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,27 +29,28 @@
 from yarndevtools.cdsw.constants import SECRET_PROJECTS_DIR
 from yarndevtools.commands.unittestresultfetcher.common import (
     UnitTestResultFetcherMode,
     CACHED_DATA_DIRNAME,
     JobNameUtils,
 )
 from yarndevtools.commands.unittestresultfetcher.model import CachedBuild, JenkinsJobResult, CachedBuildKey
+from yarndevtools.commands.unittestresultfetcher.unit_test_result_fetcher import UnitTestResultFetcherConfig
 from yarndevtools.common.common_model import FailedJenkinsBuild
 from yarndevtools.common.shared_command_utils import CommandType
 from yarndevtools.constants import YARNDEVTOOLS_MODULE_NAME
 
 LOG = logging.getLogger(__name__)
 
 
 class UnitTestResultFetcherCacheType(Enum):
     FILE = "FILE"
     GOOGLE_DRIVE = "GOOGLE_DRIVE"
 
 
-class Cache(ABC):
+class CacheAbs(ABC):
     @abstractmethod
     def initialize(self) -> Dict[str, JenkinsJobResult]:
         pass
 
     @abstractmethod
     def is_build_data_in_cache(self, key: CachedBuildKey):
         pass
@@ -79,15 +80,91 @@
         pass
 
     @abstractmethod
     def download_reports(self):
         pass
 
 
-class FileCache(Cache):
+class Cache:
+    def __init__(self, config: UnitTestResultFetcherConfig):
+        self.config = config.cache
+        self.file_cache = FileCache(config.cache)
+        # TODO yarndevtoolsv2: Should call self.file_cache.initialize() first?
+        cached_filenames: Dict[CachedBuildKey, str] = self.file_cache.get_cached_filenames()
+        self.google_drive_cache = GoogleDriveCache(config.cache, cached_filenames)
+
+    def initialize(self):
+        self.file_cache.initialize()
+        self.google_drive_cache.initialize()
+
+        if self.config.enable_sync_from_fs_to_drive:
+            self._sync_from_file_cache_to_drive_cache()
+        if self.config.remove_small_reports:
+            cached_build_keys = self.file_cache.small_reports.keys()
+            self.google_drive_cache.remove_small_reports(cached_build_keys)
+
+    def _sync_from_file_cache_to_drive_cache(self):
+        # TODO yarndevtoolsv2 too much of GoogleDriveCache internals shared in this method
+        found_builds: Set[CachedBuildKey] = set()
+        for report_drive_file in self.google_drive_cache.all_report_files:
+            build_key = GoogleDriveCache.create_cached_build_key(report_drive_file)
+            if build_key:
+                found_builds.add(build_key)
+        LOG.debug("Found %d builds from Google Drive: %s", len(found_builds), found_builds)
+        builds_to_check_from_drive = {
+            key: value for (key, value) in self.file_cache.cached_builds.items() if key not in found_builds
+        }
+        LOG.debug("Will check these builds in Google Drive: %s", builds_to_check_from_drive)
+
+        # TODO yarndevtoolsv2 Implement sync from GDrive -> Filesystem (other way around)
+        # TODO yarndevtoolsv2 Create progressTracker object to show current status of Google Drive uploads / queries
+        for key, cached_build in builds_to_check_from_drive.items():
+            drive_report_file_path = self.google_drive_cache.generate_file_name_for_report(key)
+            settings: DriveApiWrapperSingleOperationSettings = DriveApiWrapperSingleOperationSettings(
+                file_find_mode=None,
+                duplicate_file_handling_mode=DuplicateFileWriteResolutionMode.FAIL_FAST,
+                search_result_handling_mode=SearchResultHandlingMode.SINGLE_FILE_PER_SEARCH_RESULT,
+            )
+            exist = self.google_drive_cache.drive_wrapper.does_file_exist(drive_report_file_path, op_settings=settings)
+            if not exist:
+                settings: DriveApiWrapperSingleOperationSettings = DriveApiWrapperSingleOperationSettings(
+                    file_find_mode=None, duplicate_file_handling_mode=DuplicateFileWriteResolutionMode.FAIL_FAST
+                )
+                self.google_drive_cache.drive_wrapper.upload_file(
+                    cached_build.full_report_file_path, drive_report_file_path, op_settings=settings
+                )
+
+    def download_reports(self):
+        reports, remove_fs_reports = self.google_drive_cache.download_reports()
+        for key in remove_fs_reports:
+            self.file_cache.remove_report(key)
+        return reports
+
+    def is_build_data_in_cache(self, key: CachedBuildKey):
+        # TODO yarndevtoolsv2 Check in Drive and if not successful, decide based on local file cache
+        found_in_file_cache = self.file_cache.is_build_data_in_cache(key)
+        return found_in_file_cache
+
+    def load_report(self, key: CachedBuildKey):
+        fs_cache_hit = self.file_cache.is_build_data_in_cache(key)
+        if fs_cache_hit:
+            return self.file_cache.load_report(key)
+        raise NotImplementedError("Fetching Google Drive api file contents is not implemented yet!")
+
+        # TODO yarndevtoolsv2 Load from Drive and if not successful, load from local file cache
+        # TODO yarndevtoolsv2 If report.json is only found in local cache, save it to Drive
+        # loaded_report_from_drive = self.google_drive_cache.load_report(key)
+
+    def save_report(self, data, key: CachedBuildKey):
+        # TODO yarndevtoolsv2 Save to Google Drive cache first?º
+        saved_report_file_path = self.file_cache.save_report(data, key)
+        self.google_drive_cache.save_report(data, key, saved_report_file_path)
+
+
+class FileCache(CacheAbs):
     def __init__(self, config):
         self.config: CacheConfig = config
 
     def get_all_reports(self) -> Dict[CachedBuildKey, CachedBuild]:
         """
         Returns all report file paths
         :return:
@@ -106,17 +183,31 @@
         report_files = FileUtils.find_files(
             self.config.reports_dir,
             find_type=FindResultType.FILES,
             single_level=False,
             full_path_result=True,
             extension="json",
         )
-        self.cached_builds: Dict[CachedBuildKey, CachedBuild] = self._load_cached_builds_from_fs(report_files)
+        small_reports, remaining_reports = self._remove_small_reports(report_files)
+        self.cached_builds: Dict[CachedBuildKey, CachedBuild] = self._load_cached_builds_from_fs(remaining_reports)
+        if self.config.remove_small_reports:
+            self.small_reports: Dict[CachedBuildKey, CachedBuild] = self._load_cached_builds_from_fs(small_reports)
+        else:
+            self.small_reports = {}
         LOG.info("Loaded cached builds: %s", self.cached_builds)
 
+    @staticmethod
+    def _remove_small_reports(report_files):
+        # TODO yarndevtoolsv2: test this manually
+        small_reports = FileUtils.filter_files_less_than_size(10, report_files)
+        for report in small_reports:
+            FileUtils.remove_file(report)
+        remaining_reports = set(report_files).difference(set(small_reports))
+        return small_reports, remaining_reports
+
     def _load_cached_builds_from_fs(self, report_files):
         cached_builds: Dict[CachedBuildKey, CachedBuild] = {}
         for report_file in report_files:
             orig_file_path = report_file
             # Example file name: CDH-7_1-maint-Hadoop-Common-Unit/1-testreport.json
             if report_file.startswith(self.config.reports_dir):
                 report_file = report_file[len(self.config.reports_dir) :]
@@ -160,99 +251,73 @@
         report_file_path = self._generate_file_name_for_report(key)
         LOG.info(f"Removing test report from file cache: {report_file_path}")
         FileUtils.remove_file(report_file_path)
 
     def get_filename_for_report(self, key: CachedBuildKey):
         return self._generate_file_name_for_report(key)
 
+    def get_cached_filenames(self):
+        res: Dict[CachedBuildKey, str] = {}
+        for key, cached_build in self.cached_builds.items():
+            res[key] = self.get_filename_for_report(key)
+        return res
+
 
-class GoogleDriveCache(Cache):
+class GoogleDriveCache(CacheAbs):
     DRIVE_FINAL_CACHE_DIR = CommandType.UNIT_TEST_RESULT_FETCHER.output_dir_name + "_" + CACHED_DATA_DIRNAME
     TEST_REPORT_REGEX = "^[0-9]+-testreport.json$"
     TEST_REPORT_PATTERN = re.compile(TEST_REPORT_REGEX)
     # TODO implement throttling: Too many requests to Google Drive?
 
-    def __init__(self, config):
+    def __init__(self, config, cached_filenames):
         self.config: CacheConfig = config
-        self.file_cache: FileCache = FileCache(config)
         self.authorizer = GoogleApiAuthorizer(
             ServiceType.DRIVE,
             project_name=CommandType.UNIT_TEST_RESULT_FETCHER.output_dir_name,
             secret_basedir=SECRET_PROJECTS_DIR,
             account_email="snemeth@cloudera.com",
             scopes=[DriveApiScope.DRIVE_PER_FILE_ACCESS.value],
         )
         session_settings = DriveApiWrapperSessionSettings(
             FileFindMode.JUST_UNTRASHED, DuplicateFileWriteResolutionMode.ADD_NEW_REVISION, enable_path_cache=True
         )
         self.drive_wrapper = DriveApiWrapper(self.authorizer, session_settings=session_settings)
         self.drive_reports_basedir = FileUtils.join_path(
             PROJECTS_BASEDIR_NAME, YARNDEVTOOLS_MODULE_NAME, self.DRIVE_FINAL_CACHE_DIR, "reports"
         )
-        self.all_report_files = []
-        self.downloader = GoogleFileDownloader(self.drive_wrapper, self.file_cache)
+        self.all_report_files: List[DriveApiFile] = []
+
+        self.downloader = GoogleFileDownloader(self.drive_wrapper, cached_filenames)
 
     def initialize(self):
-        reports = self.file_cache.initialize()
+        # TODO yarndevtoolsv2: Return value of file_cache.initialize is not defined!
         self.all_report_files = self._download_all_reports()
-        if self.config.enable_sync_from_fs_to_drive:
-            self._sync_from_file_cache()
-        return reports
 
     @staticmethod
     def create_cached_build_key(drive_file) -> CachedBuildKey:
         job_name = drive_file._parent.name
         components = drive_file.name.split("-")
         if len(components) != 2:
             LOG.error("Found test report with unexpected name: %s", job_name)
             return None
         return CachedBuildKey(job_name, int(components[0]))
 
-    def _sync_from_file_cache(self):
-        found_builds: Set[CachedBuildKey] = set()
-        for report_drive_file in self.all_report_files:
-            build_key = self.create_cached_build_key(report_drive_file)
-            if build_key:
-                found_builds.add(build_key)
-        LOG.debug("Found %d builds from Google Drive: %s", len(found_builds), found_builds)
-        builds_to_check_from_drive = {
-            key: value for (key, value) in self.file_cache.cached_builds.items() if key not in found_builds
-        }
-        LOG.debug("Will check these builds in Google Drive: %s", builds_to_check_from_drive)
-
-        # TODO yarndevtoolsv2 Implement sync from GDrive -> Filesystem (other way around)
-        # TODO Create progressTracker object to show current status of Google Drive uploads / queries
-        for key, cached_build in builds_to_check_from_drive.items():
-            drive_report_file_path = self._generate_file_name_for_report(key)
-            settings: DriveApiWrapperSingleOperationSettings = DriveApiWrapperSingleOperationSettings(
-                file_find_mode=None,
-                duplicate_file_handling_mode=DuplicateFileWriteResolutionMode.FAIL_FAST,
-                search_result_handling_mode=SearchResultHandlingMode.SINGLE_FILE_PER_SEARCH_RESULT,
-            )
-            exist = self.drive_wrapper.does_file_exist(drive_report_file_path, op_settings=settings)
-            if not exist:
-                settings: DriveApiWrapperSingleOperationSettings = DriveApiWrapperSingleOperationSettings(
-                    file_find_mode=None, duplicate_file_handling_mode=DuplicateFileWriteResolutionMode.FAIL_FAST
-                )
-                self.drive_wrapper.upload_file(
-                    cached_build.full_report_file_path, drive_report_file_path, op_settings=settings
-                )
-
     def get_all_reports(self):
         if not self.all_report_files:
             raise ValueError("Please call initialize on the cache, first!")
         return self.all_report_files
 
     def _download_all_reports(self):
         all_report_files: List[DriveApiFile] = self.drive_wrapper.get_files("*-testreport.json")
         return all_report_files
 
     def download_reports(self) -> Dict[str, FailedJenkinsBuild]:
         drive_api_files = self.get_all_reports()
-        return self.downloader.download_reports(drive_api_files)
+        reports, remove_fs_reports = self.downloader.download_reports(drive_api_files)
+        return reports, remove_fs_reports
 
     def remove_report(self, key: CachedBuildKey):
         raise NotImplementedError("Remove report is not supported by GoogleDriveCache")
 
     @staticmethod
     def determine_creation_date(drive_api_file, file):
         # The only way to tell the timestamp of the build that is in file cache is to use creation date of the file
@@ -282,140 +347,144 @@
         build_url = f"{fetcher_mode.jenkins_base_url}/job/{key.job_name}/{build_number}"
         return FailedJenkinsBuild(
             full_url_of_job=UrlUtils.sanitize_url(build_url),
             timestamp=timestamp,
             job_name=key.job_name,
         )
 
-    def _generate_file_name_for_report(self, key: CachedBuildKey):
+    def generate_file_name_for_report(self, key: CachedBuildKey):
         return FileUtils.join_path(
             self.drive_reports_basedir,
             self.generate_job_dirname(key),
             self.generate_report_filename(key),
         )
 
     def is_build_data_in_cache(self, key: CachedBuildKey):
-        # TODO yarndevtoolsv2 Check in Drive and if not successful, decide based on local file cache
-        return self.file_cache.is_build_data_in_cache(key)
+        # TODO yarndevtoolsv2 implement
+        raise NotImplementedError("not implemented")
 
-    def save_report(self, data, key: CachedBuildKey):
-        saved_report_file_path = self.file_cache.save_report(data, key)
-        drive_path = self._generate_file_name_for_report(key)
+    def save_report(self, data, key: CachedBuildKey, saved_report_file_path):
+        drive_path = self.generate_file_name_for_report(key)
         self.drive_wrapper.upload_file(saved_report_file_path, drive_path)
 
     def load_report(self, key: CachedBuildKey) -> Dict[Any, Any]:
-        cache_hit = self.file_cache.is_build_data_in_cache(key)
-        if cache_hit:
-            return self.file_cache.load_report(key)
-        else:
-            filename = self._generate_file_name_for_report(key)
-            self.drive_wrapper.get_file(filename)
-            # TODO missing return
-        # TODO yarndevtoolsv2 Load from Drive and if not successful, load from local file cache
-        # TODO If report.json is only found in local cache, save it to Drive
+        filename = self.generate_file_name_for_report(key)
+        files = self.drive_wrapper.get_file(filename)
+        # TODO yarndevtoolsv2 What if multiple files found?
+        if len(files) > 1:
+            raise ValueError("Edge case not handled")
+        # TODO yarndevtoolsv2 get json report content from DriveApiFile
+        # return files[0].
+        return {}
+
+    def remove_small_reports(self, cached_build_keys):
+        drive_files_dict: Dict[CachedBuildKey, DriveApiFile] = {}
+        for report_drive_file in self.all_report_files:
+            build_key = self.create_cached_build_key(report_drive_file)
+            if build_key:
+                drive_files_dict[build_key] = report_drive_file
+        LOG.debug("Found builds to remove from Google Drive (small report size): %s", drive_files_dict)
+        for key in cached_build_keys:
+            if key in drive_files_dict:
+                # TODO yarndevtoolsv2 test remove drive file functonality manually
+                drive_api_file = drive_files_dict[key]
+                self.drive_wrapper.remove_file(drive_api_file)
 
 
 class CacheConfig:
     def __init__(self, args, output_dir, force_download_mode=False, load_cached_reports_to_db=False):
-        self.cache_type: UnitTestResultFetcherCacheType = (
-            UnitTestResultFetcherCacheType(args.cache_type.upper())
-            if hasattr(args, "cache_type") and args.cache_type
-            else UnitTestResultFetcherCacheType.FILE
-        )
-        self._explicitly_disable_file_cache = args.disable_file_cache if hasattr(args, "disable_file_cache") else False
-        self.enabled = not self._explicitly_disable_file_cache
-
         self.enable_sync_from_fs_to_drive: bool = (
             not args.disable_sync_from_fs_to_drive if hasattr(args, "disable_sync_from_fs_to_drive") else True
         )
 
-        self.enabled = self._verify_cache_enabled(force_download_mode, load_cached_reports_to_db)
-
+        self.enabled = self._is_caching_enabled(args, force_download_mode, load_cached_reports_to_db)
         self.reports_dir = FileUtils.ensure_dir_created(FileUtils.join_path(output_dir, "reports"))
         self.cached_data_dir = FileUtils.ensure_dir_created(FileUtils.join_path(output_dir, CACHED_DATA_DIRNAME))
         self.download_uncached_job_data: bool = (
             args.download_uncached_job_data if hasattr(args, "download_uncached_job_data") else False
         )
+        self.remove_small_reports: bool = args.remove_small_reports if hasattr(args, "remove_small_reports") else False
 
-    def _verify_cache_enabled(self, force_download_mode, load_cached_reports_to_db):
-        orig_val = self.enabled
+    def _is_caching_enabled(self, args, force_download_mode, load_cached_reports_to_db):
+        disable_cache = args.disable_file_cache if hasattr(args, "disable_file_cache") else False
+        enabled = not disable_cache
+        orig_enabled = enabled
+        new_enabled = enabled
 
         if force_download_mode:
             reason = "force download mode is enabled"
-            new_val = True
-        if self.cache_type:
-            reason = "cache type is set to: " + str(self.cache_type)
-            # TODO do not change because of cache type
-            # new_val = True
-            new_val = orig_val
+            new_enabled = True
         if load_cached_reports_to_db:
             reason = "load cached reports to db is enabled"
-            new_val = True
-            self.cache_type = UnitTestResultFetcherCacheType.GOOGLE_DRIVE
+            new_enabled = True
 
-        if orig_val != new_val:
+        if orig_enabled != new_enabled:
             raise ValueError(
                 "Conflicting cache settings! Original enabled value: {}, new enabled value: {}, reason: {}".format(
-                    orig_val, new_val, reason
+                    orig_enabled, new_enabled, reason
                 )
             )
 
-        return new_val
+        return new_enabled
 
 
 class FileSizeCheckerResult(Enum):
     NORMAL_SIZE = "normal"
     SMALL_SIZE_REDOWNLOAD = "small_size_redownloaded"
     SMALL_SIZE_AFTER_REDOWNLOAD = "small_size_cannot_download"
 
 
 class GoogleFileDownloader:
-    def __init__(self, drive_wrapper, file_cache):
+    def __init__(self, drive_wrapper, cached_fs_filenames: Dict[CachedBuildKey, str]):
+        self.cached_fs_filenames = cached_fs_filenames
         self.drive_wrapper = drive_wrapper
-        self.file_cache = file_cache
         self.file_size_checker = FileSizeChecker()
 
     def download_reports(self, drive_api_files):
         LOG.debug("Found %d reports from Google Drive: %s", len(drive_api_files), drive_api_files)
 
         reports = {}
         # Sum up sizes
         sum_bytes = sum([int(f.size) for f in drive_api_files])
         downloaded_bytes = 0
         LOG.info(
             "Size of %d report files from Google Drive: %s", len(drive_api_files), StringUtils.format_bytes(sum_bytes)
         )
+        remove_fs_reports: Set[CachedBuildKey] = set()
         for idx, drive_api_file in enumerate(drive_api_files):
             LOG.info("Processing file [ %d / %d ]", idx + 1, len(drive_api_files))
             LOG.info("Downloaded bytes [ %d / %d ]", downloaded_bytes, sum_bytes)
             key = GoogleDriveCache.create_cached_build_key(drive_api_file)
             file_name = drive_api_file.name
-            if not self.file_cache.is_build_data_in_cache(key):
+            if key not in self.cached_fs_filenames:
                 LOG.info("Report '%s' is not cached for job '%s', downloading...", file_name, key.job_name)
 
                 creation_date, report_file_path = self.download_and_write_to_file_cache(key, drive_api_file)
             else:
                 LOG.info("Report '%s' for job '%s' found in cache", file_name, key.job_name)
-                report_file_path = self.file_cache.get_filename_for_report(key)
-                report_file_path = self._check_file_size(key, drive_api_file, report_file_path)
+                report_file_path = self.cached_fs_filenames[key]
+                report_file_path, remove_fs_report = self._check_file_size(key, drive_api_file, report_file_path)
                 creation_date = GoogleDriveCache.determine_creation_date(drive_api_file, report_file_path)
+                if remove_fs_report:
+                    remove_fs_reports.add(key)
             file_name = os.path.basename(report_file_path)
             reports[report_file_path] = GoogleDriveCache.create_failed_build(file_name, creation_date, key)
             downloaded_bytes += int(drive_api_file.size)
 
-        return reports
+        return reports, remove_fs_reports
 
     def _check_file_size(self, key: CachedBuildKey, drive_api_file, report_file_path):
+        remove_fs_report = False
         check_result = self.file_size_checker.check_file_size(drive_api_file, key, report_file_path)
         if check_result == FileSizeCheckerResult.SMALL_SIZE_REDOWNLOAD:
             creation_date, report_file_path = self.download_and_write_to_file_cache(key, drive_api_file)
             check_result = self.file_size_checker.check_file_size(drive_api_file, key, report_file_path)
             if check_result == FileSizeCheckerResult.SMALL_SIZE_AFTER_REDOWNLOAD:
-                self.file_cache.remove_report(key)
-        return report_file_path
+                remove_fs_report = True
+        return report_file_path, remove_fs_report
 
     def download_and_write_to_file_cache(self, key, drive_api_file):
         with tempfile.TemporaryDirectory() as tmp:
             downloaded_file = self.drive_wrapper.download_file(drive_api_file.id)
             report_file_tmp_path = os.path.join(tmp, "report.json")
             FileUtils.write_bytesio_to_file(report_file_tmp_path, downloaded_file)
             report_json = JsonFileUtils.load_data_from_json_file(report_file_tmp_path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/common.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/common.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/db.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/db.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/email.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/email.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/jenkins.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/jenkins.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/model.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/model.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/parser.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,21 +41,14 @@
             action="store_true",
             dest="force_download_mode",
             help="Force downloading data from all builds. "
             "If this is set to true, all job data will be downloaded, regardless if they are already in the cache",
         )
 
         parser.add_argument(
-            "--download-uncached-job-data",
-            action="store_true",
-            dest="download_uncached_job_data",
-            help="Download data for all builds that are not in cache yet or was removed from the cache, for any reason.",
-        )
-
-        parser.add_argument(
             "--force-sending-email",
             action="store_true",
             dest="force_send_email",
             help="Force sending email report for all builds.",
         )
 
         parser.add_argument(
@@ -153,41 +146,51 @@
             "--testcase-filter",
             dest="tc_filters",
             nargs="+",
             type=tc_filter_validator,
             help="Testcase filters in format: <project:filter statement>",
         )
 
+        # CACHE RELATED ARGS
+
+        parser.add_argument(
+            "--download-uncached-job-data",
+            action="store_true",
+            dest="download_uncached_job_data",
+            help="Download data for all builds that are not in cache yet or was removed from the cache, for any reason.",
+        )
+
         # TODO change this to disable cache
         parser.add_argument(
             "-d",
             "--disable-file-cache",
             dest="disable_file_cache",
             type=bool,
             help="Whether to disable Jenkins report file cache",
         )
 
         parser.add_argument(
-            "-ct",
-            "--cache-type",
-            type=str,
-            dest="cache_type",
-            choices=[ct.name.lower() for ct in UnitTestResultFetcherCacheType],
-            help="The type of the cache. Either file or google_drive",
-        )
-
-        parser.add_argument(
             "--load-cached-reports-to-db",
             dest="load_cached_reports_to_db",
             action="store_true",
             help="Whether to save all cached reports from Google Drive to MongoDB",
         )
 
         parser.add_argument(
             "--disable-sync-from-fs-to-drive",
             dest="disable_sync_from_fs_to_drive",
             action="store_true",
             default=False,
             help="Whether to sync reports from filesystem to Google Drive",
         )
 
+        parser.add_argument(
+            "--remove-small-reports",
+            dest="remove_small_reports",
+            action="store_true",
+            default=False,
+            help="Whether to remove small reports from FS and Google Drive caches",
+        )
+
+        # END OF CACHE RELATED ARGS
+
         parser.set_defaults(func=func)
```

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/unittestresultfetcher/unit_test_result_fetcher.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/unittestresultfetcher/unit_test_result_fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 from pythoncommons.date_utils import DateUtils
 from pythoncommons.file_utils import JsonFileUtils
 from pythoncommons.logging_setup import SimpleLoggingSetup
 from pythoncommons.os_utils import OsUtils
 from pythoncommons.project_utils import ProjectUtils
 
 from yarndevtools.commands.unittestresultfetcher.cache import (
-    Cache,
-    GoogleDriveCache,
-    FileCache,
-    UnitTestResultFetcherCacheType,
     CacheConfig,
+    Cache,
 )
 from yarndevtools.commands.unittestresultfetcher.common import UnitTestResultFetcherMode, JobNameUtils
 from yarndevtools.commands.unittestresultfetcher.db import (
     JenkinsJobResults,
     UTResultFetcherDatabase,
     MailSendStateForJob,
 )
@@ -168,20 +165,15 @@
         # make CachedBuildKey to follow the dir name pattern, so job_names are always consistent when used in
         # CachedBuildKey.
         job_name = JobNameUtils.escape_job_name(failed_build.job_name)
         return CachedBuildKey(job_name, failed_build.build_number)
 
     @staticmethod
     def _create_cache(config: UnitTestResultFetcherConfig):
-        if config.cache.cache_type == UnitTestResultFetcherCacheType.FILE:
-            LOG.info("Using file cache")
-            return FileCache(config.cache)
-        elif config.cache.cache_type == UnitTestResultFetcherCacheType.GOOGLE_DRIVE:
-            LOG.info("Using Google Drive cache")
-            return GoogleDriveCache(config.cache)
+        return Cache(config)
 
     def run(self):
         LOG.info("Starting Jenkins test reporter. Details: %s", str(self.config))
         SimpleLoggingSetup.init_logger(
             project_name=CommandType.UNIT_TEST_RESULT_FETCHER.output_dir_name,
             logger_name_prefix=YARNDEVTOOLS_MODULE_NAME,
             execution_mode=ExecutionMode.PRODUCTION,
@@ -338,15 +330,15 @@
         if not data or len(data) == 0:
             return JobBuildData(failed_build, None, [], status=JobBuildDataStatus.NO_JSON_DATA_FOUND)
 
         return JenkinsApi.parse_job_data(data, failed_build)
 
     def fetch_raw_data_for_build(self, failed_build: FailedJenkinsBuild):
         if self.config.cache.enabled:
-            cache_build_key = self._convert_to_cache_build_key(failed_build)
+            cache_build_key: CachedBuildKey = self._convert_to_cache_build_key(failed_build)
             cache_hit = self.cache.is_build_data_in_cache(cache_build_key)
             if cache_hit:
                 return self.cache.load_report(cache_build_key)
             else:
                 return self._fetch_build_data(failed_build)
         else:
             return self._fetch_build_data(failed_build)
```

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/upstream_jira_patch_differ.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/upstream_jira_patch_differ.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/upstream_pr_fetcher.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/upstream_pr_fetcher.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/common.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/upstreamumbrellafetcher/common.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/representation.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/upstreamumbrellafetcher/representation.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/upstreamumbrellafetcher/upstream_jira_umbrella_fetcher.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/upstreamumbrellafetcher/upstream_jira_umbrella_fetcher.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands/zip_latest_command_data.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands/zip_latest_command_data.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/commands_common.py` & `yarn_dev_tools-2.0.1/yarndevtools/commands_common.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/common/common_model.py` & `yarn_dev_tools-2.0.1/yarndevtools/common/common_model.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/common/db.py` & `yarn_dev_tools-2.0.1/yarndevtools/common/db.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/common/shared_command_utils.py` & `yarn_dev_tools-2.0.1/yarndevtools/common/shared_command_utils.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/constants.py` & `yarn_dev_tools-2.0.1/yarndevtools/constants.py`

 * *Files identical despite different names*

### Comparing `yarn-dev-tools-2.0.0/yarndevtools/yarn_dev_tools.py` & `yarn_dev_tools-2.0.1/yarndevtools/yarn_dev_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 class YarnDevTools:
     def __init__(self, execution_mode: ExecutionMode = ExecutionMode.PRODUCTION):
         self.env = {}
         self.setup_dirs(execution_mode=execution_mode)
         self.init_repos()
 
+    # TODO move this to pythoncommons?
     def setup_dirs(self, execution_mode: ExecutionMode = ExecutionMode.PRODUCTION):
         strategy = None
         if execution_mode == ExecutionMode.PRODUCTION:
             strategy = ProjectRootDeterminationStrategy.SYS_PATH
         elif execution_mode == ExecutionMode.TEST:
             strategy = ProjectRootDeterminationStrategy.COMMON_FILE
         if YarnDevToolsEnvVar.PROJECT_DETERMINATION_STRATEGY.value in os.environ:
```

### Comparing `yarn-dev-tools-2.0.0/setup.py` & `yarn_dev_tools-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,209 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: yarn-dev-tools
+Version: 2.0.1
+Summary: 
+Home-page: https://github.com/szilard-nemeth/yarn-dev-tools
+Keywords: YARN,development,dev environment
+Author: Szilard Nemeth
+Author-email: szilard.nemeth88@gmail.com
+Requires-Python: >=3.8.12,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bs4
+Requires-Dist: dacite
+Requires-Dist: dataclasses-json
+Requires-Dist: gitpython
+Requires-Dist: google-api-wrapper2 (==1.0.10)
+Requires-Dist: humanize
+Requires-Dist: jira
+Requires-Dist: marshmallow
+Requires-Dist: pymongo
+Requires-Dist: python-common-lib (==1.0.9)
+Project-URL: Repository, https://github.com/szilard-nemeth/yarn-dev-tools
+Description-Content-Type: text/markdown
+
+[![CI for YARN dev tools (pip)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml/badge.svg)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools/branch/master/graph/badge.svg?token=OQD6FIFF7I)](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![GitHub language count](https://img.shields.io/github/languages/count/szilard-nemeth/yarn-dev-tools)
+
+
+# YARN-dev-tools
+
+This project contains various developer helper scripts in order to simplify every day tasks related to Apache Hadoop YARN development.
+
+## Main dependencies
+
+* [gitpython](https://gitpython.readthedocs.io/en/stable/) - GitPython is a python library used to interact with git repositories, high-level like git-porcelain, or low-level like git-plumbing.
+* [tabulate](https://pypi.org/project/tabulate/) - python-tabulate: Pretty-print tabular data in Python, a library and a command-line utility.
+* [bs4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - Beautiful Soup is a Python library for pulling data out of HTML and XML files.
+
+* TODO: Missing dependencies
+
+## Contributing
+
+TODO 
+
+## Authors
+
+* **Szilard Nemeth** - *Initial work* - [Szilard Nemeth](https://github.com/szilard-nemeth)
+
+## License
+
+TODO 
+
+## Acknowledgments
+
+TODO
+
+# Getting started
+
+In order to use this tool, you need to have at least Python 3.8 installed.
+
+## Use yarn-dev-tools from package (Recommended)
+If you don't want to tinker with the source code, you can download [yarn-dev-tools](https://pypi.org/project/yarn-dev-tools/#history) from PyPi as well.
+This is probably the easiest way to use it.
+You don't need to install anything manually as I created a [script](initial_setup.sh) that performs the installation automatically.
+The script has a `setup-vars` function at the beginning that defines some environment variables:
+
+These are the following:
+- `YARNDEVTOOLS_ROOT`: Specifies the directory where the Python virtualenv will be created and yarn-dev-tools will be installed to this virtualenv.
+- `HADOOP_DEV_DIR` Should be set to the upstream Hadoop repository root, e.g.: "~/development/apache/hadoop/"
+- `CLOUDERA_HADOOP_ROOT` Should be set to the downstream Hadoop repository root, e.g.: "~/development/cloudera/hadoop/"
+
+The latter two environment variables is better to be added to your bashrc / zshrc file (depending on what shell you are using) to keep them between the shells.
+
+## Use yarn-dev-tools from source
+If you want to use yarn-dev-tools from source, first you need to install its dependencies.
+The project root contains a pyproject.toml file that has all the dependencies listed.
+The project uses Poetry to resolve the dependencies so you need to [install poetry](https://python-poetry.org/docs/#installation) as well.
+Simply go to the root of this project and execute `poetry install --without localdev`.
+Alternatively, you can run `make` from the root of the project.
+
+## Setting up handy aliases to use yarn-dev-tools
+If you completed the installation (either by source or by package), you may want to define some shell aliases to use the tool more easily.
+In my system, I have [these](
+https://github.com/szilard-nemeth/linux-env/blob/master/workplace-specific/cloudera/scripts/yarn/setup-yarn-dev-tools-aliases.sh).
+Please make sure to source this script so that the command 'yarndevtools' will be available since it's defined as a function.
+It is important to specify `HADOOP_DEV_DIR` and `CLOUDERA_HADOOP_ROOT` as mentioned above, before sourcing the script.
+
+After these steps, you will have a basic set of aliases that is enough to get you started.
+
+
+# Setting up yarn-dev-tools with Cloudera CDSW
+
+## Initial setup
+1. Upload the initial setup scripts to the CDSW files, to the root directory (/home/cdsw)
+- [initial-cdsw-setup.sh](yarndevtools/cdsw/scripts/initial-cdsw-setup.sh)
+- [install-requirements.sh](yarndevtools/cdsw/scripts/install-requirements.sh)
+
+2. Create a new CDSW session.
+Wait for the session to be launched and open up a terminal by Clicking "Terminal access" on the top menu bar.
+
+
+3. Execute this command:
+```
+~/initial-cdsw-setup.sh user cloudera
+```
+
+
+The script performs the following actions: 
+1. Downloads the scripts that are cloning the upstream and downstream Hadoop repositories + installing yarndevtools itself as a python module.
+The download location is: `/home/cdsw/scripts`<br>
+Please note that the files will be downloaded from the GitHub master branch of this repository!
+- [clone_downstream_repos.sh](yarndevtools/cdsw/scripts/clone_downstream_repos.sh)
+- [clone_upstream_repos.sh](yarndevtools/cdsw/scripts/clone_upstream_repos.sh)
+
+2. Executes the script described in step 2. 
+This can take some time, especially cloning Hadoop.
+Note: The individual CDSW jobs should make sure for themselves to clone the repositories.
+
+3. Copies the [python-based job configs](yarndevtools/cdsw/job_configs) for all jobs to `/home/cdsw/jobs`
+
+4. All you have to do in CDSW is to set up the projects and their starter scripts like this:
+
+| Project                                                                | Starter script location         | Arguments for script          |
+|------------------------------------------------------------------------|---------------------------------|-------------------------------|
+| Jira umbrella data fetcher (Formerly: Jira umbrella checker reporting) | scripts/start_job.py            | jira-umbrella-data-fetcher    |
+| Unit test result aggregator                                            | scripts/start_job.py            | unit-test-result-aggregator   |
+| Unit test result fetcher (Formerly: Unit test result reporting)        | scripts/start_job.py            | unit-test-result-fetcher      |
+| Branch comparator (Formerly: Downstream branchdiff reporting)          | scripts/start_job.py            | branch-comparator             |
+| Review sheet backport updater                                          | scripts/start_job.py | review-sheet-backport-updater |
+| Reviewsync                                                             | scripts/start_job.py | reviewsync                    |
+
+# Use-cases
+
+
+### Examples for YARN backporter
+To backport YARN-6221 to 2 branches, run these commands:
+```
+yarn-backport YARN-6221 COMPX-6664 cdpd-master
+yarn-backport YARN-6221 COMPX-6664 CDH-7.1-maint --no-fetch
+```
+The first argument is the upstream Jira ID<br>
+The second argument is the downstream Jira ID.<br>
+The third argument is the downstream branch.<br>
+The `--no-fetch` option is a means to skip git fetch on both repos.
+
+### How to backport to an already existing relation chain?
+1. Go to Gerrit UI and download the patch.
+For example: 
+```
+git fetch "https://gerrit.sjc.cloudera.com/cdh/hadoop" refs/changes/29/156429/5 && git checkout FETCH_HEAD
+```
+2. Checkout a new branch
+```
+git checkout -b my-relation-chain 
+```
+
+3. Run backporter with: 
+```
+yarn-backport YARN-10314 COMPX-7855 CDH-7.1.7.1000 --no-fetch --downstream_base_ref my-relation-chain
+```
+where:<br>
+The first argument is the upstream Jira ID<br>
+The second argument is the downstream Jira ID.<br>
+The third argument is the downstream branch.<br>
+The `--no-fetch` option is a means to skip git fetch on both repos.<br>
+The `--downstream_base_ref <local-branch` is a way to use a local branch to base the backport on so the Git remote name won't be prepended.
+
+
+Finally, I set up two aliases for pushing the changes to the downstream repo:
+```
+alias git-push-to-cdpdmaster="git push <REMOTE> HEAD:refs/for/cdpd-master%<REVIEWER_LIST>"
+alias git-push-to-cdh71maint="git push <REMOTE> HEAD:refs/for/CDH-7.1-maint%<REVIEWER_LIST>"
+```
+where REVIEWER_LIST is in this format: "r=user1,r=user2,r=user3,..."
+
+
+# Contributing
+
+## Setup of pre-commit
+
+Configure precommit as described in [this blogpost](https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/).
+
+Commands:
+1. Install precommit: `pip install pre-commit`
+2. Make sure to add pre-commit to your path. For example, on a Mac system, pre-commit is installed here: 
+   `$HOME/Library/Python/3.8/bin/pre-commit`.
+2. Execute `pre-commit install` to install git hooks in your `.git/` directory.
+
+## Running the tests
+
+TODO
+
+## Troubleshooting
+
+### Installation issues
+In case you're facing a similar issue:
+```
+An error has occurred: InvalidManifestError: 
+=====> /<userhome>/.cache/pre-commit/repoBP08UH/.pre-commit-hooks.yaml does not exist
+Check the log at /<userhome>/.cache/pre-commit/pre-commit.log
+```
+, please run: `pre-commit autoupdate`
 
-packages = \
-['yarndevtools',
- 'yarndevtools.cdsw',
- 'yarndevtools.cdsw.job_configs',
- 'yarndevtools.cdsw.libreloader',
- 'yarndevtools.cdsw.scripts.experiments',
- 'yarndevtools.commands',
- 'yarndevtools.commands.branchcomparator',
- 'yarndevtools.commands.reviewsheetbackportupdater',
- 'yarndevtools.commands.reviewsync',
- 'yarndevtools.commands.unittestresultaggregator',
- 'yarndevtools.commands.unittestresultaggregator.common',
- 'yarndevtools.commands.unittestresultaggregator.db',
- 'yarndevtools.commands.unittestresultaggregator.email',
- 'yarndevtools.commands.unittestresultfetcher',
- 'yarndevtools.commands.upstreamumbrellafetcher',
- 'yarndevtools.common']
-
-package_data = \
-{'': ['*'],
- 'yarndevtools.cdsw': ['resources/*',
-                       'scripts/*',
-                       'unit-test-result-aggregator/*']}
-
-install_requires = \
-['bs4',
- 'dacite',
- 'dataclasses-json',
- 'gitpython',
- 'google-api-wrapper2==1.0.5',
- 'humanize',
- 'jira',
- 'marshmallow',
- 'pymongo',
- 'python-common-lib==1.0.6']
-
-entry_points = \
-{'console_scripts': ['exec-yarndevtools = yarndevtools.yarn_dev_tools:run']}
-
-setup_kwargs = {
-    'name': 'yarn-dev-tools',
-    'version': '2.0.0',
-    'description': '',
-    'long_description': '[![CI for YARN dev tools (pip)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml/badge.svg)](https://github.com/szilard-nemeth/yarn-dev-tools/actions/workflows/ci.yml)\n[![codecov](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools/branch/master/graph/badge.svg?token=OQD6FIFF7I)](https://codecov.io/gh/szilard-nemeth/yarn-dev-tools)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![GitHub language count](https://img.shields.io/github/languages/count/szilard-nemeth/yarn-dev-tools)\n\n\n# YARN-dev-tools\n\nThis project contains various developer helper scripts in order to simplify every day tasks related to Apache Hadoop YARN development.\n\n## Main dependencies\n\n* [gitpython](https://gitpython.readthedocs.io/en/stable/) - GitPython is a python library used to interact with git repositories, high-level like git-porcelain, or low-level like git-plumbing.\n* [tabulate](https://pypi.org/project/tabulate/) - python-tabulate: Pretty-print tabular data in Python, a library and a command-line utility.\n* [bs4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - Beautiful Soup is a Python library for pulling data out of HTML and XML files.\n\n* TODO: Missing dependencies\n\n## Contributing\n\nTODO \n\n## Authors\n\n* **Szilard Nemeth** - *Initial work* - [Szilard Nemeth](https://github.com/szilard-nemeth)\n\n## License\n\nTODO \n\n## Acknowledgments\n\nTODO\n\n# Getting started\n\nIn order to use this tool, you need to have at least Python 3.8 installed.\n\n## Use yarn-dev-tools from package (Recommended)\nIf you don\'t want to tinker with the source code, you can download [yarn-dev-tools](https://pypi.org/project/yarn-dev-tools/#history) from PyPi as well.\nThis is probably the easiest way to use it.\nYou don\'t need to install anything manually as I created a [script](initial_setup.sh) that performs the installation automatically.\nThe script has a `setup-vars` function at the beginning that defines some environment variables:\n\nThese are the following:\n- `YARNDEVTOOLS_ROOT`: Specifies the directory where the Python virtualenv will be created and yarn-dev-tools will be installed to this virtualenv.\n- `HADOOP_DEV_DIR` Should be set to the upstream Hadoop repository root, e.g.: "~/development/apache/hadoop/"\n- `CLOUDERA_HADOOP_ROOT` Should be set to the downstream Hadoop repository root, e.g.: "~/development/cloudera/hadoop/"\n\nThe latter two environment variables is better to be added to your bashrc / zshrc file (depending on what shell you are using) to keep them between the shells.\n\n## Use yarn-dev-tools from source\nIf you want to use yarn-dev-tools from source, first you need to install its dependencies.\nThe project root contains a pyproject.toml file that has all the dependencies listed.\nThe project uses Poetry to resolve the dependencies so you need to [install poetry](https://python-poetry.org/docs/#installation) as well.\nSimply go to the root of this project and execute `poetry install --without localdev`.\nAlternatively, you can run `make` from the root of the project.\n\n## Setting up handy aliases to use yarn-dev-tools\nIf you completed the installation (either by source or by package), you may want to define some shell aliases to use the tool more easily.\nIn my system, I have [these](\nhttps://github.com/szilard-nemeth/linux-env/blob/master/workplace-specific/cloudera/scripts/yarn/setup-yarn-dev-tools-aliases.sh).\nPlease make sure to source this script so that the command \'yarndevtools\' will be available since it\'s defined as a function.\nIt is important to specify `HADOOP_DEV_DIR` and `CLOUDERA_HADOOP_ROOT` as mentioned above, before sourcing the script.\n\nAfter these steps, you will have a basic set of aliases that is enough to get you started.\n\n\n# Setting up yarn-dev-tools with Cloudera CDSW\n\n## Initial setup\n1. Upload the initial setup scripts to the CDSW files, to the root directory (/home/cdsw)\n- [initial-cdsw-setup.sh](yarndevtools/cdsw/scripts/initial-cdsw-setup.sh)\n- [install-requirements.sh](yarndevtools/cdsw/scripts/install-requirements.sh)\n\n2. Create a new CDSW session.\nWait for the session to be launched and open up a terminal by Clicking "Terminal access" on the top menu bar.\n\n\n3. Execute this command:\n```\n~/initial-cdsw-setup.sh user cloudera\n```\n\n\nThe script performs the following actions: \n1. Downloads the scripts that are cloning the upstream and downstream Hadoop repositories + installing yarndevtools itself as a python module.\nThe download location is: `/home/cdsw/scripts`<br>\nPlease note that the files will be downloaded from the GitHub master branch of this repository!\n- [clone_downstream_repos.sh](yarndevtools/cdsw/scripts/clone_downstream_repos.sh)\n- [clone_upstream_repos.sh](yarndevtools/cdsw/scripts/clone_upstream_repos.sh)\n\n2. Executes the script described in step 2. \nThis can take some time, especially cloning Hadoop.\nNote: The individual CDSW jobs should make sure for themselves to clone the repositories.\n\n3. Copies the [python-based job configs](yarndevtools/cdsw/job_configs) for all jobs to `/home/cdsw/jobs`\n\n4. All you have to do in CDSW is to set up the projects and their starter scripts like this:\n\n| Project                                                                | Starter script location         | Arguments for script          |\n|------------------------------------------------------------------------|---------------------------------|-------------------------------|\n| Jira umbrella data fetcher (Formerly: Jira umbrella checker reporting) | scripts/start_job.py            | jira-umbrella-data-fetcher    |\n| Unit test result aggregator                                            | scripts/start_job.py            | unit-test-result-aggregator   |\n| Unit test result fetcher (Formerly: Unit test result reporting)        | scripts/start_job.py            | unit-test-result-fetcher      |\n| Branch comparator (Formerly: Downstream branchdiff reporting)          | scripts/start_job.py            | branch-comparator             |\n| Review sheet backport updater                                          | scripts/start_job.py | review-sheet-backport-updater |\n| Reviewsync                                                             | scripts/start_job.py | reviewsync                    |\n\n# Use-cases\n\n\n### Examples for YARN backporter\nTo backport YARN-6221 to 2 branches, run these commands:\n```\nyarn-backport YARN-6221 COMPX-6664 cdpd-master\nyarn-backport YARN-6221 COMPX-6664 CDH-7.1-maint --no-fetch\n```\nThe first argument is the upstream Jira ID<br>\nThe second argument is the downstream Jira ID.<br>\nThe third argument is the downstream branch.<br>\nThe `--no-fetch` option is a means to skip git fetch on both repos.\n\n### How to backport to an already existing relation chain?\n1. Go to Gerrit UI and download the patch.\nFor example: \n```\ngit fetch "https://gerrit.sjc.cloudera.com/cdh/hadoop" refs/changes/29/156429/5 && git checkout FETCH_HEAD\n```\n2. Checkout a new branch\n```\ngit checkout -b my-relation-chain \n```\n\n3. Run backporter with: \n```\nyarn-backport YARN-10314 COMPX-7855 CDH-7.1.7.1000 --no-fetch --downstream_base_ref my-relation-chain\n```\nwhere:<br>\nThe first argument is the upstream Jira ID<br>\nThe second argument is the downstream Jira ID.<br>\nThe third argument is the downstream branch.<br>\nThe `--no-fetch` option is a means to skip git fetch on both repos.<br>\nThe `--downstream_base_ref <local-branch` is a way to use a local branch to base the backport on so the Git remote name won\'t be prepended.\n\n\nFinally, I set up two aliases for pushing the changes to the downstream repo:\n```\nalias git-push-to-cdpdmaster="git push <REMOTE> HEAD:refs/for/cdpd-master%<REVIEWER_LIST>"\nalias git-push-to-cdh71maint="git push <REMOTE> HEAD:refs/for/CDH-7.1-maint%<REVIEWER_LIST>"\n```\nwhere REVIEWER_LIST is in this format: "r=user1,r=user2,r=user3,..."\n\n\n# Contributing\n\n## Setup of pre-commit\n\nConfigure precommit as described in [this blogpost](https://ljvmiranda921.github.io/notebook/2018/06/21/precommits-using-black-and-flake8/).\n\nCommands:\n1. Install precommit: `pip install pre-commit`\n2. Make sure to add pre-commit to your path. For example, on a Mac system, pre-commit is installed here: \n   `$HOME/Library/Python/3.8/bin/pre-commit`.\n2. Execute `pre-commit install` to install git hooks in your `.git/` directory.\n\n## Running the tests\n\nTODO\n\n## Troubleshooting\n\n### Installation issues\nIn case you\'re facing a similar issue:\n```\nAn error has occurred: InvalidManifestError: \n=====> /<userhome>/.cache/pre-commit/repoBP08UH/.pre-commit-hooks.yaml does not exist\nCheck the log at /<userhome>/.cache/pre-commit/pre-commit.log\n```\n, please run: `pre-commit autoupdate`\n\nMore info can be found [here](https://github.com/pre-commit/pre-commit/issues/577).',
-    'author': 'Szilard Nemeth',
-    'author_email': 'szilard.nemeth88@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/szilard-nemeth/yarn-dev-tools',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.12,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
+More info can be found [here](https://github.com/pre-commit/pre-commit/issues/577).
```

