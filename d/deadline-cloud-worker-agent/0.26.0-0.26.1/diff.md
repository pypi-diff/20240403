# Comparing `tmp/deadline_cloud_worker_agent-0.26.0.tar.gz` & `tmp/deadline_cloud_worker_agent-0.26.1.tar.gz`

## Comparing `deadline_cloud_worker_agent-0.26.0.tar` & `deadline_cloud_worker_agent-0.26.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/_version.py
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/hatch_version_hook.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/__main__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/_version.py
--rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/api_models.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/errors.py
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/file_system_operations.py
--rw-r--r--   0        0        0    19180 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/log_messages.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/metrics.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/progress.py
--rw-r--r--   0        0        0    21274 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/session_events.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/utils.py
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/worker.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws/__init__.py
--rw-r--r--   0        0        0    36140 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws/deadline/__init__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/__init__.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/aws_configs.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/boto3_sessions.py
--rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/credentials_refresher.py
--rw-r--r--   0        0        0    23109 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/temporary_credentials.py
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/boto/__init__.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/boto/config.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/boto/logger.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/boto/retries.py
--rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/boto/shim.py
--rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/installer/__init__.py
--rwxr-xr-x   0        0        0    18766 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/installer/install.sh
--rw-r--r--   0        0        0    36591 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/installer/win_installer.py
--rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/installer/worker.toml.example
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/log_sync/__init__.py
--rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/log_sync/cloudwatch.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/log_sync/loggers.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/log.py
--rw-r--r--   0        0        0    61107 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/scheduler.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/session_action_status.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/session_cleanup.py
--rw-r--r--   0        0        0    19215 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/session_queue.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/active_action.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/errors.py
--rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/log_config.py
--rw-r--r--   0        0        0    53599 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/session.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/__init__.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/action_definition.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/enter_env.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/exit_env.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/openjd_action.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/run_step_task.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/__init__.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/environment_details.py
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py
--rw-r--r--   0        0        0    17689 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/job_details.py
--rw-r--r--   0        0        0    15220 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/job_entities.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/job_entity_type.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/step_details.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/validation.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/__init__.py
--rw-r--r--   0        0        0    20997 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/bootstrap.py
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/capabilities.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/cli_args.py
--rw-r--r--   0        0        0    10967 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/config.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/config_file.py
--rw-r--r--   0        0        0    16187 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/entrypoint.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/host_properties.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/settings.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/windows/__init__.py
--rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/windows/win_credentials_resolver.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/windows/win_service.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/NOTICE
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/README.md
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/hatch.toml
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/pyproject.toml
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.0/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/_version.py
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/hatch_version_hook.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/__main__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/_version.py
+-rw-r--r--   0        0        0    11897 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/api_models.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/errors.py
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/file_system_operations.py
+-rw-r--r--   0        0        0    19180 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_messages.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/metrics.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/progress.py
+-rw-r--r--   0        0        0    21274 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/session_events.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/utils.py
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/worker.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws/__init__.py
+-rw-r--r--   0        0        0    36140 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws/deadline/__init__.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/__init__.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/aws_configs.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/boto3_sessions.py
+-rw-r--r--   0        0        0     8937 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/credentials_refresher.py
+-rw-r--r--   0        0        0    23258 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/temporary_credentials.py
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/__init__.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/config.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/logger.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/retries.py
+-rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/shim.py
+-rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/__init__.py
+-rwxr-xr-x   0        0        0    18766 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/install.sh
+-rw-r--r--   0        0        0    38437 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/win_installer.py
+-rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/worker.toml.example
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_sync/__init__.py
+-rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_sync/cloudwatch.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_sync/loggers.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/log.py
+-rw-r--r--   0        0        0    61170 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/scheduler.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_action_status.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_cleanup.py
+-rw-r--r--   0        0        0    19215 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_queue.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/active_action.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/errors.py
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/log_config.py
+-rw-r--r--   0        0        0    53599 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/session.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/__init__.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/action_definition.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/enter_env.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/exit_env.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/openjd_action.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/run_step_task.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/__init__.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/environment_details.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py
+-rw-r--r--   0        0        0    17689 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_details.py
+-rw-r--r--   0        0        0    15220 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_entities.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_entity_type.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/step_details.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/validation.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/__init__.py
+-rw-r--r--   0        0        0    20997 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/bootstrap.py
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/capabilities.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/cli_args.py
+-rw-r--r--   0        0        0    10967 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/config.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/config_file.py
+-rw-r--r--   0        0        0    16187 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/entrypoint.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/host_properties.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/settings.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/__init__.py
+-rw-r--r--   0        0        0    12818 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/win_credentials_resolver.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/win_service.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/NOTICE
+-rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/README.md
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/hatch.toml
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/pyproject.toml
+-rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 deadline_cloud_worker_agent-0.26.1/PKG-INFO
```

### Comparing `deadline_cloud_worker_agent-0.26.0/hatch_version_hook.py` & `deadline_cloud_worker_agent-0.26.1/hatch_version_hook.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/api_models.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/api_models.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/file_system_operations.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/file_system_operations.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/log_messages.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_messages.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/metrics.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/metrics.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/progress.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/progress.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/session_events.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/session_events.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/utils.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/utils.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/worker.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/worker.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws/deadline/__init__.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws/deadline/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/aws_configs.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/aws_configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -103,24 +103,28 @@
             file_path=self.path,
             owner=os_user,
         )
 
         # finally, read the config
         self._config_parser.read(self.path)
 
-    def install_credential_process(self, profile_name: str, script_path: Path) -> None:
+    def install_credential_process(
+        self,
+        profile_name: str,
+        script_path: Path,
+    ) -> None:
         """
         Installs a credential process given the profile name and script path
 
         Args:
             profile_name (str): The profile name to install under
             script_path (Path): The script to call in the process
         """
         self._config_parser[self._get_profile_name(profile_name)] = {
-            "credential_process": str(script_path.absolute())
+            "credential_process": str(script_path.absolute()),
         }
         self._write()
 
     def uninstall_credential_process(self, profile_name: str) -> None:
         """
         Uninstalls a credential process given the profile name
 
@@ -169,21 +173,65 @@
 
 
 class AWSConfig(_AWSConfigBase):
     """
     Implementation of _AWSConfigBase to represent the ~/.aws/config file
     """
 
+    _region: str
+
+    def __init__(
+        self,
+        *,
+        os_user: Optional[SessionUser],
+        parent_dir: Path,
+        region: str,
+    ) -> None:
+        """
+        Constructor for the AWSConfigBase class
+
+        Args:
+            os_user (Optional[SessionUser]): If non-None, then this is the os user to add read
+                permissions for. If None, then the only the process user will be able to read
+                the credentials files.
+            parent_dir (Path): The directory where the AWS config and credentials files will be
+                written to.
+            region (str): The target region where the credentials are for
+        """
+        super(AWSConfig, self).__init__(
+            os_user=os_user,
+            parent_dir=parent_dir,
+        )
+        self._region = region
+
     def _get_profile_name(self, profile_name: str) -> str:
         return f"profile {profile_name}"
 
     @property
     def path(self) -> Path:
         return self._parent_dir / "config"
 
+    def install_credential_process(
+        self,
+        profile_name: str,
+        script_path: Path,
+    ) -> None:
+        """
+        Installs a credential process given the profile name and script path
+
+        Args:
+            profile_name (str): The profile name to install under
+            script_path (Path): The script to call in the process
+        """
+        self._config_parser[self._get_profile_name(profile_name)] = {
+            "credential_process": str(script_path.absolute()),
+            "region": self._region,
+        }
+        self._write()
+
 
 class AWSCredentials(_AWSConfigBase):
     """
     Implementation of _AWSConfigBase to represent the ~/.aws/credentials file
     """
 
     def _get_profile_name(self, profile_name: str) -> str:
```

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/boto3_sessions.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/boto3_sessions.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/credentials_refresher.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/credentials_refresher.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/queue_boto3_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     _farm_id: str
     _fleet_id: str
     _queue_id: str
     _worker_id: str
     _role_arn: str
     _os_user: Optional[SessionUser]
     _interrupt_event: Event
+    _region: str
 
     # Name of the profile written to the user's AWS configuration for the
     # credentials process
     _profile_name: str
 
     # Directory where the credentials file & credentials process script are
     # written.
@@ -131,25 +132,27 @@
         fleet_id: str,
         worker_id: str,
         queue_id: str,
         role_arn: str,
         os_user: Optional[SessionUser] = None,
         interrupt_event: Event,
         worker_persistence_dir: Path,
+        region: str,
     ) -> None:
         super().__init__()
 
         self._deadline_client = deadline_client
         self._farm_id = farm_id
         self._fleet_id = fleet_id
         self._worker_id = worker_id
         self._queue_id = queue_id
         self._role_arn = role_arn
         self._os_user = os_user
         self._interrupt_event = interrupt_event
+        self._region = region
 
         self._profile_name = f"deadline-{self._queue_id}"
 
         self._credential_dir = self._get_credentials_dir(worker_persistence_dir, queue_id)
         self._file_cache = JSONFileCache(working_dir=self._credential_dir)
         self._credentials_filename_no_ext = (
             "aws_credentials"  # note: .json extension added by JSONFileCache
@@ -158,17 +161,22 @@
         if os.name == "posix":
             self._credentials_process_script_path = self._credential_dir / "get_aws_credentials.sh"
         else:
             self._credentials_process_script_path = self._credential_dir / "get_aws_credentials.cmd"
 
         self._create_credentials_directory(os_user)
 
-        self._aws_config = AWSConfig(os_user=self._os_user, parent_dir=self._credential_dir)
+        self._aws_config = AWSConfig(
+            os_user=self._os_user,
+            parent_dir=self._credential_dir,
+            region=self._region,
+        )
         self._aws_credentials = AWSCredentials(
-            os_user=self._os_user, parent_dir=self._credential_dir
+            os_user=self._os_user,
+            parent_dir=self._credential_dir,
         )
 
         self._install_credential_process()
 
         # Output at debug level queue credential file ownership and permissions
         self._debug_path_permissions(self._credential_dir)
         self._debug_path_permissions(self._aws_config.path)
```

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/temporary_credentials.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/temporary_credentials.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/aws_credentials/worker_boto3_session.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/boto/config.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/config.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/boto/retries.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/retries.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/boto/shim.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/boto/shim.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/installer/__init__.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/installer/install.sh` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/install.sh`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/installer/win_installer.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/win_installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import os
 import re
 import secrets
 import shutil
 import string
 import sys
+import time
 from argparse import ArgumentParser
 from getpass import getpass
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import deadline.client.config.config_file
 import pywintypes
@@ -29,15 +30,14 @@
 
 from ..file_system_operations import (
     _set_windows_permissions,
     FileSystemPermissionEnum,
 )
 from ..windows.win_service import WorkerAgentWindowsService
 
-
 # Defaults
 DEFAULT_WA_USER = "deadline-worker"
 DEFAULT_JOB_GROUP = "deadline-job-users"
 DEFAULT_PASSWORD_LENGTH = 32
 
 # Environment variable that overrides the config path used by the Deadline client
 DEADLINE_CLIENT_CONFIG_PATH_OVERRIDE_ENV_VAR = "DEADLINE_CONFIG_FILE_PATH"
@@ -502,14 +502,53 @@
         logging.error(f"Failed to update Deadline Client configuration for user '{user}': {e}")
         raise
     finally:
         os.environ.clear()
         os.environ.update(old_environ)
 
 
+def _check_and_stop_service(service_name: str):
+    """
+    Checks the status of a Windows service and stops it if running.
+
+    Parameters:
+        service_name (str): The name of the Windows service to check and stop
+    """
+    try:
+        # Check if the service is installed.
+        # It will return the SERVICE_STATUS objece
+        # https://learn.microsoft.com/en-us/windows/win32/api/winsvc/ns-winsvc-service_status
+        status = win32serviceutil.QueryServiceStatus(service_name)
+        # The service is installed, now check its state
+        if status[1] == win32service.SERVICE_RUNNING:
+            logging.info(f"Service '{service_name}' is installed and running.")
+            logging.info(f"Before installation, attempting to stop '{service_name}'...")
+            win32serviceutil.StopService(service_name)
+            service_stop_time_out_in_seconds = 300
+            for seconds in range(service_stop_time_out_in_seconds):
+                time.sleep(1)
+                status = win32serviceutil.QueryServiceStatus(service_name)
+                if status[1] == win32service.SERVICE_STOPPED:
+                    logging.info(f"Service '{service_name}' has been stopped successfully.")
+                    break
+            else:
+                logging.error(
+                    f"Service '{service_name}' could not be stopped within {service_stop_time_out_in_seconds}."
+                )
+                exit(1)
+    except pywintypes.error as e:
+        if e.winerror == winerror.ERROR_SERVICE_DOES_NOT_EXIST:
+            pass
+        else:
+            logging.error(
+                f"Service '{service_name}' could not be stopped due to the exception: {e}."
+            )
+            exit(e.winerror)
+
+
 def _install_service(
     *,
     agent_user_name: str,
     password: str,
 ) -> None:
     """Installs the Windows Service that hosts the Worker Agent
 
@@ -531,14 +570,17 @@
     service_class_str = win32serviceutil.GetServiceClassString(WorkerAgentWindowsService)
     service_name = WorkerAgentWindowsService._svc_name_
     service_display_name = WorkerAgentWindowsService._svc_display_name_
     service_description = getattr(WorkerAgentWindowsService, "_svc_description_", None)
     exe_name = getattr(WorkerAgentWindowsService, "_exe_name_", None)
     exe_args = getattr(WorkerAgentWindowsService, "_exe_args_", None)
 
+    # Check if the service is installed and stop it if running.
+    _check_and_stop_service(service_name)
+
     # Configure the service to start on boot
     startup = win32service.SERVICE_AUTO_START
 
     logging.info(f'Configuring Windows Service "{service_display_name}"...')
     try:
         win32serviceutil.InstallService(
             service_class_str,
```

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/installer/worker.toml.example` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/installer/worker.toml.example`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/log_sync/cloudwatch.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/log_sync/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/scheduler.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1147,14 +1147,15 @@
                         fleet_id=self._fleet_id,
                         worker_id=self._worker_id,
                         queue_id=queue_id,
                         role_arn=queue_role_arn,
                         os_user=os_user,
                         interrupt_event=self._shutdown,
                         worker_persistence_dir=self._worker_persistence_dir,
+                        region=self._boto_session.region_name,
                     )
                 except (DeadlineRequestWorkerOfflineError, DeadlineRequestUnrecoverableError):
                     # These are terminal errors for the Session. We need to fail it, without attempting,
                     # if we have a terminal error.
                     # The caller will log a message.
                     raise
                 except (DeadlineRequestError, DeadlineRequestInterrupted):
```

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/session_action_status.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_action_status.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/session_cleanup.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_cleanup.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/scheduler/session_queue.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/scheduler/session_queue.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/errors.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/errors.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/log_config.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/log_config.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/session.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/session.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/__init__.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/action_definition.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/action_definition.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/enter_env.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/enter_env.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/exit_env.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/exit_env.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/openjd_action.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/openjd_action.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/run_step_task.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/run_step_task.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/actions/sync_input_job_attachments.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/environment_details.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/environment_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_attachment_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/job_details.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/job_entities.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/job_entities.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/step_details.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/step_details.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/sessions/job_entities/validation.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/sessions/job_entities/validation.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/bootstrap.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/bootstrap.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/capabilities.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/capabilities.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/cli_args.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/cli_args.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/config.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/config.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/config_file.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/config_file.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/entrypoint.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/entrypoint.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/host_properties.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/host_properties.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/startup/settings.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/startup/settings.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/windows/win_credentials_resolver.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/win_credentials_resolver.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/src/deadline_worker_agent/windows/win_service.py` & `deadline_cloud_worker_agent-0.26.1/src/deadline_worker_agent/windows/win_service.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/LICENSE` & `deadline_cloud_worker_agent-0.26.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/README.md` & `deadline_cloud_worker_agent-0.26.1/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/hatch.toml` & `deadline_cloud_worker_agent-0.26.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/pyproject.toml` & `deadline_cloud_worker_agent-0.26.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_worker_agent-0.26.0/PKG-INFO` & `deadline_cloud_worker_agent-0.26.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-worker-agent
-Version: 0.26.0
+Version: 0.26.1
 Summary: The AWS Deadline Cloud worker agent can be used to run a worker in an AWS Deadline Cloud fleet
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-worker-agent
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-worker-agent
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

