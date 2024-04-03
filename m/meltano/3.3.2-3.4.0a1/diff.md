# Comparing `tmp/meltano-3.3.2.tar.gz` & `tmp/meltano-3.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltano-3.3.2.tar", max compression
+gzip compressed data, was "meltano-3.4.0a1.tar", max compression
```

## Comparing `meltano-3.3.2.tar` & `meltano-3.4.0a1.tar`

### file list

```diff
@@ -1,298 +1,298 @@
--rw-r--r--   0        0        0     1048 2024-03-06 19:15:05.471450 meltano-3.3.2/LICENSE
--rw-r--r--   0        0        0     5237 2024-03-06 19:15:05.471450 meltano-3.3.2/README.md
--rw-r--r--   0        0        0    19166 2024-03-06 19:15:05.603453 meltano-3.3.2/pyproject.toml
--rw-r--r--   0        0        0       98 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/__init__.py
--rw-r--r--   0        0        0     3601 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/__init__.py
--rw-r--r--   0        0        0       73 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/__main__.py
--rw-r--r--   0        0        0     6712 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/add.py
--rw-r--r--   0        0        0     5991 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/cli.py
--rw-r--r--   0        0        0     3776 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/compile.py
--rw-r--r--   0        0        0    14429 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/config.py
--rw-r--r--   0        0        0      405 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/docs.py
--rw-r--r--   0        0        0      506 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/dragon.py
--rw-r--r--   0        0        0    17169 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/elt.py
--rw-r--r--   0        0        0     2548 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/environment.py
--rw-r--r--   0        0        0     1656 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/hub.py
--rw-r--r--   0        0        0     2221 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/initialize.py
--rw-r--r--   0        0        0     4050 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/install.py
--rw-r--r--   0        0        0      180 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/interactive/__init__.py
--rw-r--r--   0        0        0    16360 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/interactive/config.py
--rw-r--r--   0        0        0      240 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/interactive/utils.py
--rw-r--r--   0        0        0     6239 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/invoke.py
--rw-r--r--   0        0        0    10045 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/job.py
--rw-r--r--   0        0        0     3789 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/lock.py
--rw-r--r--   0        0        0     2227 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/params.py
--rw-r--r--   0        0        0     2788 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/remove.py
--rw-r--r--   0        0        0     7269 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/run.py
--rw-r--r--   0        0        0    12888 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/schedule.py
--rw-r--r--   0        0        0      770 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/schema.py
--rw-r--r--   0        0        0     4418 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/select.py
--rw-r--r--   0        0        0    10594 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/state.py
--rw-r--r--   0        0        0     4344 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/upgrade.py
--rw-r--r--   0        0        0    23951 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/utils.py
--rw-r--r--   0        0        0     4210 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/cli/validate.py
--rw-r--r--   0        0        0        0 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/core/__init__.py
--rw-r--r--   0        0        0       64 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/core/behavior/__init__.py
--rw-r--r--   0        0        0    13060 2024-03-06 19:15:05.603453 meltano-3.3.2/src/meltano/core/behavior/canonical.py
--rw-r--r--   0        0        0     3961 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/behavior/hookable.py
--rw-r--r--   0        0        0      192 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/behavior/name_eq.py
--rw-r--r--   0        0        0     1172 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/behavior/versioned.py
--rw-r--r--   0        0        0      406 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/behavior/visitor.py
--rw-r--r--   0        0        0      117 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/block/__init__.py
--rw-r--r--   0        0        0     1582 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/block/blockset.py
--rw-r--r--   0        0        0    29312 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/block/extract_load.py
--rw-r--r--   0        0        0     2674 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/block/future_utils.py
--rw-r--r--   0        0        0     3946 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/block/ioblock.py
--rw-r--r--   0        0        0    11166 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/block/parser.py
--rw-r--r--   0        0        0     5730 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/block/plugin_command.py
--rw-r--r--   0        0        0    12162 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/block/singer.py
--rw-r--r--   0        0        0      128 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/bundle/__init__.py
--rw-r--r--   0        0        0      460 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/bundle/initialize.yml
--rw-r--r--   0        0        0     2625 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/bundle/settings.yml
--rw-r--r--   0        0        0    10326 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/cli_messages.py
--rw-r--r--   0        0        0     3094 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/config_service.py
--rw-r--r--   0        0        0       81 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/container/__init__.py
--rw-r--r--   0        0        0     2130 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/container/container_service.py
--rw-r--r--   0        0        0     2997 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/container/container_spec.py
--rw-r--r--   0        0        0     7376 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/db.py
--rw-r--r--   0        0        0    14899 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/elt_context.py
--rw-r--r--   0        0        0     6924 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/environment.py
--rw-r--r--   0        0        0     2797 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/environment_service.py
--rw-r--r--   0        0        0     3749 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/error.py
--rw-r--r--   0        0        0      181 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/hub/__init__.py
--rw-r--r--   0        0        0    11070 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/hub/client.py
--rw-r--r--   0        0        0      896 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/hub/schema.py
--rw-r--r--   0        0        0      103 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/job/__init__.py
--rw-r--r--   0        0        0     5940 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/job/finder.py
--rw-r--r--   0        0        0    11543 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/job/job.py
--rw-r--r--   0        0        0     1036 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/job/stale_job_failer.py
--rw-r--r--   0        0        0     6014 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/job_state.py
--rw-r--r--   0        0        0     2914 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/locked_definition_service.py
--rw-r--r--   0        0        0      698 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/logging/__init__.py
--rw-r--r--   0        0        0     4530 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/logging/formatters.py
--rw-r--r--   0        0        0     4826 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/logging/job_logging_service.py
--rw-r--r--   0        0        0     7366 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/logging/output_logger.py
--rw-r--r--   0        0        0     7361 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/logging/utils.py
--rw-r--r--   0        0        0     3453 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/manifest/__init__.py
--rw-r--r--   0        0        0      365 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/manifest/cache.py
--rw-r--r--   0        0        0     4775 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/manifest/contexts.py
--rw-r--r--   0        0        0     4822 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/manifest/jsonschema.py
--rw-r--r--   0        0        0    18144 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/manifest/manifest.py
--rw-r--r--   0        0        0     5137 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/meltano_file.py
--rw-r--r--   0        0        0     2679 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/meltano_invoker.py
--rw-r--r--   0        0        0     3635 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/migration_service.py
--rw-r--r--   0        0        0      481 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/models.py
--rw-r--r--   0        0        0      188 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/__init__.py
--rw-r--r--   0        0        0     5661 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/airflow.py
--rw-r--r--   0        0        0    27329 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/base.py
--rw-r--r--   0        0        0     3638 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/command.py
--rw-r--r--   0        0        0     1422 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/config_service.py
--rw-r--r--   0        0        0      139 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/dbt/__init__.py
--rw-r--r--   0        0        0     4041 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/dbt/base.py
--rw-r--r--   0        0        0     2703 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/error.py
--rw-r--r--   0        0        0     1848 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/factory.py
--rw-r--r--   0        0        0     9890 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/file.py
--rw-r--r--   0        0        0     2708 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/meltano_file.py
--rw-r--r--   0        0        0    14822 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/project_plugin.py
--rw-r--r--   0        0        0     1135 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/requirements.py
--rw-r--r--   0        0        0     7651 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/settings_service.py
--rw-r--r--   0        0        0      282 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/singer/__init__.py
--rw-r--r--   0        0        0     2552 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/singer/base.py
--rw-r--r--   0        0        0    19585 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/singer/catalog.py
--rw-r--r--   0        0        0     2346 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/singer/mapper.py
--rw-r--r--   0        0        0    23401 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/singer/tap.py
--rw-r--r--   0        0        0     5573 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/singer/target.py
--rw-r--r--   0        0        0     5804 2024-03-06 19:15:05.607452 meltano-3.3.2/src/meltano/core/plugin/superset.py
--rw-r--r--   0        0        0      269 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/plugin/utility.py
--rw-r--r--   0        0        0    16702 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/plugin_install_service.py
--rw-r--r--   0        0        0    17137 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/plugin_invoker.py
--rw-r--r--   0        0        0     6473 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/plugin_location_remove.py
--rw-r--r--   0        0        0     3916 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/plugin_lock_service.py
--rw-r--r--   0        0        0     2817 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/plugin_remove_service.py
--rw-r--r--   0        0        0     2180 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/plugin_repository.py
--rw-r--r--   0        0        0     3289 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/plugin_test_service.py
--rw-r--r--   0        0        0    18073 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/project.py
--rw-r--r--   0        0        0     3999 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/project_add_service.py
--rw-r--r--   0        0        0    14167 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/project_files.py
--rw-r--r--   0        0        0     6551 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/project_init_service.py
--rw-r--r--   0        0        0    18296 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/project_plugins_service.py
--rw-r--r--   0        0        0     5118 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/project_settings_service.py
--rw-r--r--   0        0        0      262 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/runner/__init__.py
--rw-r--r--   0        0        0     2119 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/runner/dbt.py
--rw-r--r--   0        0        0    10084 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/runner/singer.py
--rw-r--r--   0        0        0     3754 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/schedule.py
--rw-r--r--   0        0        0    10918 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/schedule_service.py
--rw-r--r--   0        0        0     3369 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/select_service.py
--rw-r--r--   0        0        0      926 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/setting.py
--rw-r--r--   0        0        0    15085 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/setting_definition.py
--rw-r--r--   0        0        0    21237 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/settings_service.py
--rw-r--r--   0        0        0    46326 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/settings_store.py
--rw-r--r--   0        0        0     2575 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/sqlalchemy.py
--rw-r--r--   0        0        0     7253 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/state_service.py
--rw-r--r--   0        0        0     3727 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/state_store/__init__.py
--rw-r--r--   0        0        0     5451 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/state_store/azure.py
--rw-r--r--   0        0        0     2133 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/state_store/base.py
--rw-r--r--   0        0        0     3840 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/state_store/db.py
--rw-r--r--   0        0        0    17943 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/state_store/filesystem.py
--rw-r--r--   0        0        0     4169 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/state_store/google.py
--rw-r--r--   0        0        0     4833 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/state_store/s3.py
--rw-r--r--   0        0        0     4460 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/task_sets.py
--rw-r--r--   0        0        0     3992 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/task_sets_service.py
--rw-r--r--   0        0        0        0 2024-03-06 19:15:26.915780 meltano-3.3.2/src/meltano/core/tracking/.release_marker
--rw-r--r--   0        0        0     3614 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/README.md
--rw-r--r--   0        0        0      125 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/__init__.py
--rw-r--r--   0        0        0      470 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/contexts/__init__.py
--rw-r--r--   0        0        0     2514 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/contexts/cli.py
--rw-r--r--   0        0        0     6044 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/contexts/environment.py
--rw-r--r--   0        0        0     3790 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/contexts/exception.py
--rw-r--r--   0        0        0     4933 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/contexts/plugins.py
--rw-r--r--   0        0        0     4128 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/contexts/project.py
--rw-r--r--   0        0        0      918 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1051 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1194 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
--rw-r--r--   0        0        0      720 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      748 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     6002 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     6501 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     6963 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
--rw-r--r--   0        0        0     7408 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
--rw-r--r--   0        0        0     4449 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1403 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1462 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     3920 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2109 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2812 2024-03-06 19:15:05.611453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     1202 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      404 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/tracking/iglu.json
--rw-r--r--   0        0        0     9688 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/tracking/micro.conf
--rw-r--r--   0        0        0     1112 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/tracking/schemas.py
--rw-r--r--   0        0        0    18604 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/tracking/tracker.py
--rw-r--r--   0        0        0     3547 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/transform_add_service.py
--rw-r--r--   0        0        0     7678 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/upgrade_service.py
--rw-r--r--   0        0        0    25128 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/utils/__init__.py
--rw-r--r--   0        0        0     1451 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/utils/pidfile.py
--rw-r--r--   0        0        0     4090 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/validation_service.py
--rw-r--r--   0        0        0    15525 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/venv_service.py
--rw-r--r--   0        0        0     1521 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/core/yaml.py
--rw-r--r--   0        0        0      508 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/__init__.py
--rw-r--r--   0        0        0       12 2024-03-06 19:15:26.839779 meltano-3.3.2/src/meltano/migrations/db.lock
--rw-r--r--   0        0        0     1490 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/env.py
--rw-r--r--   0        0        0      495 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/script.py.mako
--rw-r--r--   0        0        0       67 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/utils/__init__.py
--rw-r--r--   0        0        0     1261 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/utils/dialect_typing.py
--rw-r--r--   0        0        0     1814 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
--rw-r--r--   0        0        0      972 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
--rw-r--r--   0        0        0      674 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
--rw-r--r--   0        0        0      802 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
--rw-r--r--   0        0        0      563 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
--rw-r--r--   0        0        0    11827 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
--rw-r--r--   0        0        0     2877 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/6ef30ab7b8e5_.py
--rw-r--r--   0        0        0     1095 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
--rw-r--r--   0        0        0      643 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
--rw-r--r--   0        0        0      786 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
--rw-r--r--   0        0        0     2026 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/b4c05e463b53_.py
--rw-r--r--   0        0        0      972 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
--rw-r--r--   0        0        0      699 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
--rw-r--r--   0        0        0      679 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
--rw-r--r--   0        0        0      486 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
--rw-r--r--   0        0        0    37186 2024-03-06 19:15:05.615453 meltano-3.3.2/src/meltano/schemas/meltano.schema.json
--rw-r--r--   0        0        0      438 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/asserts.py
--rw-r--r--   0        0        0     7462 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/conftest.py
--rw-r--r--   0        0        0     2174 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/cli.py
--rw-r--r--   0        0        0   125876 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/core.py
--rw-r--r--   0        0        0     2829 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/db/__init__.py
--rw-r--r--   0        0        0     2510 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/db/mssql.py
--rw-r--r--   0        0        0     1227 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/db/postgresql.py
--rw-r--r--   0        0        0     1222 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/db/postgresql_psycopg3.py
--rw-r--r--   0        0        0      328 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/db/sqlite.py
--rw-r--r--   0        0        0      752 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/docker/__init__.py
--rw-r--r--   0        0        0      276 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/docker/docker-compose.yml
--rw-r--r--   0        0        0     4132 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/docker/snowplow.py
--rw-r--r--   0        0        0     1535 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/fs.py
--rw-r--r--   0        0        0     3135 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/large_config_project/meltano.yml
--rw-r--r--   0        0        0    30013 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/large_config_project/schedule.yml
--rw-r--r--   0        0        0     1086 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/multifile_project/meltano.yml
--rw-r--r--   0        0        0      469 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/multifile_project/subconfig_2.yml
--rw-r--r--   0        0        0      394 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
--rw-r--r--   0        0        0      631 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/plugins/extractors/tap-custom/test.yml
--rw-r--r--   0        0        0     1136 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/fixtures/utils.py
--rw-r--r--   0        0        0    31067 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/meltano/cli/test_add.py
--rw-r--r--   0        0        0    15154 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/meltano/cli/test_cli.py
--rw-r--r--   0        0        0     5174 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/meltano/cli/test_compile.py
--rw-r--r--   0        0        0     8595 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/meltano/cli/test_config.py
--rw-r--r--   0        0        0    41995 2024-03-06 19:15:05.615453 meltano-3.3.2/tests/meltano/cli/test_elt.py
--rw-r--r--   0        0        0     1585 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_hub.py
--rw-r--r--   0        0        0     3577 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_initialize.py
--rw-r--r--   0        0        0    11520 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_install.py
--rw-r--r--   0        0        0     9285 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_invoke.py
--rw-r--r--   0        0        0     6777 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_job_cmd.py
--rw-r--r--   0        0        0     3771 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_lock.py
--rw-r--r--   0        0        0     1864 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_remove.py
--rw-r--r--   0        0        0    47425 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_run.py
--rw-r--r--   0        0        0     8502 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_schedule.py
--rw-r--r--   0        0        0     1140 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_select.py
--rw-r--r--   0        0        0    11532 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_state.py
--rw-r--r--   0        0        0     8268 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/cli/test_upgrade.py
--rw-r--r--   0        0        0     5381 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/behavior/test_canonical.py
--rw-r--r--   0        0        0     2155 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/behavior/test_hookable.py
--rw-r--r--   0        0        0    21766 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/block/test_extract_load.py
--rw-r--r--   0        0        0      241 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/block/test_parser.py
--rw-r--r--   0        0        0      933 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/block/test_plugin_command.py
--rw-r--r--   0        0        0     7736 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/block/test_singer.py
--rw-r--r--   0        0        0     2302 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/container/test_container_spec.py
--rw-r--r--   0        0        0     6783 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/hub/test_meltano_hub_service.py
--rw-r--r--   0        0        0     2076 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/job/test_finder.py
--rw-r--r--   0        0        0     6243 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/job/test_job.py
--rw-r--r--   0        0        0     2579 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/job/test_stale_job_failer.py
--rw-r--r--   0        0        0     3326 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/logging/test_formatters.py
--rw-r--r--   0        0        0      806 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/logging/test_logging_utils.py
--rw-r--r--   0        0        0     7386 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/logging/test_output_logger.py
--rw-r--r--   0        0        0    32051 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/singer/test_catalog.py
--rw-r--r--   0        0        0      562 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/singer/test_mapper.py
--rw-r--r--   0        0        0    37590 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/singer/test_tap.py
--rw-r--r--   0        0        0     3690 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/singer/test_target.py
--rw-r--r--   0        0        0     3921 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/test_airflow.py
--rw-r--r--   0        0        0     2396 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/test_command.py
--rw-r--r--   0        0        0    22146 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/test_plugin.py
--rw-r--r--   0        0        0      174 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/test_plugin_config_service.py
--rw-r--r--   0        0        0    35208 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/test_plugin_settings.py
--rw-r--r--   0        0        0     5963 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/plugin/test_superset.py
--rw-r--r--   0        0        0     7999 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/runner/test_runner.py
--rw-r--r--   0        0        0     2807 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/state_store/test_db.py
--rw-r--r--   0        0        0    21750 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/state_store/test_filesystem.py
--rw-r--r--   0        0        0     6765 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/state_store/test_state_store.py
--rw-r--r--   0        0        0     1558 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_db_compat.py
--rw-r--r--   0        0        0     1813 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_db_connection.py
--rw-r--r--   0        0        0     5217 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_elt_context.py
--rw-r--r--   0        0        0     2610 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_environment_service.py
--rw-r--r--   0        0        0    13772 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_environment_variables.py
--rw-r--r--   0        0        0     2261 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_locked_definition_service.py
--rw-r--r--   0        0        0     2108 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_meltano_file.py
--rw-r--r--   0        0        0     3128 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_meltano_invoker.py
--rw-r--r--   0        0        0     4094 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_plugin_install_service.py
--rw-r--r--   0        0        0     6101 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_plugin_invoker.py
--rw-r--r--   0        0        0     3127 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_plugin_lock_service.py
--rw-r--r--   0        0        0     5723 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_plugin_remove_service.py
--rw-r--r--   0        0        0     5776 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_plugin_test_service.py
--rw-r--r--   0        0        0     4319 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_project.py
--rw-r--r--   0        0        0     8866 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_project_add_service.py
--rw-r--r--   0        0        0    16322 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_project_files.py
--rw-r--r--   0        0        0     3281 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_project_init_service.py
--rw-r--r--   0        0        0     8071 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_project_plugins_service.py
--rw-r--r--   0        0        0     7238 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_project_settings_service.py
--rw-r--r--   0        0        0     9759 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_schedule_service.py
--rw-r--r--   0        0        0     2766 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_setting_definition.py
--rw-r--r--   0        0        0    22226 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_settings_store.py
--rw-r--r--   0        0        0     3665 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_state_service.py
--rw-r--r--   0        0        0     2430 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_task_sets.py
--rw-r--r--   0        0        0     2645 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_task_sets_service.py
--rw-r--r--   0        0        0     6583 2024-03-06 19:15:05.619453 meltano-3.3.2/tests/meltano/core/test_utils.py
--rw-r--r--   0        0        0     1813 2024-03-06 19:15:05.623453 meltano-3.3.2/tests/meltano/core/test_validation_service.py
--rw-r--r--   0        0        0    10040 2024-03-06 19:15:05.623453 meltano-3.3.2/tests/meltano/core/test_venv_service.py
--rw-r--r--   0        0        0     1980 2024-03-06 19:15:05.623453 meltano-3.3.2/tests/meltano/core/tracking/test_environment_context.py
--rw-r--r--   0        0        0     5693 2024-03-06 19:15:05.623453 meltano-3.3.2/tests/meltano/core/tracking/test_exception.py
--rw-r--r--   0        0        0     3061 2024-03-06 19:15:05.623453 meltano-3.3.2/tests/meltano/core/tracking/test_plugins.py
--rw-r--r--   0        0        0     1271 2024-03-06 19:15:05.623453 meltano-3.3.2/tests/meltano/core/tracking/test_project_context.py
--rw-r--r--   0        0        0      684 2024-03-06 19:15:05.623453 meltano-3.3.2/tests/meltano/core/tracking/test_schemas.py
--rw-r--r--   0        0        0    19704 2024-03-06 19:15:05.623453 meltano-3.3.2/tests/meltano/core/tracking/test_tracker.py
--rw-r--r--   0        0        0     8962 1970-01-01 00:00:00.000000 meltano-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1048 2024-04-03 20:47:33.568166 meltano-3.4.0a1/LICENSE
+-rw-r--r--   0        0        0     5237 2024-04-03 20:47:33.568166 meltano-3.4.0a1/README.md
+-rw-r--r--   0        0        0    19356 2024-04-03 20:47:33.704166 meltano-3.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/__init__.py
+-rw-r--r--   0        0        0     3631 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/__main__.py
+-rw-r--r--   0        0        0     6770 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/add.py
+-rw-r--r--   0        0        0     6006 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/cli.py
+-rw-r--r--   0        0        0     3806 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/compile.py
+-rw-r--r--   0        0        0    14489 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/config.py
+-rw-r--r--   0        0        0      406 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/docs.py
+-rw-r--r--   0        0        0      507 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/dragon.py
+-rw-r--r--   0        0        0    17244 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/elt.py
+-rw-r--r--   0        0        0     2548 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/environment.py
+-rw-r--r--   0        0        0     1671 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/hub.py
+-rw-r--r--   0        0        0     2221 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/initialize.py
+-rw-r--r--   0        0        0     4100 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/install.py
+-rw-r--r--   0        0        0      181 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/interactive/__init__.py
+-rw-r--r--   0        0        0    16395 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/interactive/config.py
+-rw-r--r--   0        0        0      241 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/interactive/utils.py
+-rw-r--r--   0        0        0     6275 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/invoke.py
+-rw-r--r--   0        0        0    10060 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/job.py
+-rw-r--r--   0        0        0     3804 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/lock.py
+-rw-r--r--   0        0        0     2242 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/params.py
+-rw-r--r--   0        0        0     2789 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/remove.py
+-rw-r--r--   0        0        0     7299 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/run.py
+-rw-r--r--   0        0        0    12993 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/schedule.py
+-rw-r--r--   0        0        0      770 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/schema.py
+-rw-r--r--   0        0        0     4446 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/select.py
+-rw-r--r--   0        0        0    10590 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/state.py
+-rw-r--r--   0        0        0     4344 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/upgrade.py
+-rw-r--r--   0        0        0    23965 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/utils.py
+-rw-r--r--   0        0        0     4185 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/validate.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/__init__.py
+-rw-r--r--   0        0        0    13060 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/canonical.py
+-rw-r--r--   0        0        0     3962 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/hookable.py
+-rw-r--r--   0        0        0      192 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/name_eq.py
+-rw-r--r--   0        0        0     1187 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/versioned.py
+-rw-r--r--   0        0        0      406 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/visitor.py
+-rw-r--r--   0        0        0      117 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/__init__.py
+-rw-r--r--   0        0        0     1582 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/blockset.py
+-rw-r--r--   0        0        0    29706 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/extract_load.py
+-rw-r--r--   0        0        0     2705 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/future_utils.py
+-rw-r--r--   0        0        0     3946 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/ioblock.py
+-rw-r--r--   0        0        0    11236 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/parser.py
+-rw-r--r--   0        0        0     5745 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/plugin_command.py
+-rw-r--r--   0        0        0    12176 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/singer.py
+-rw-r--r--   0        0        0      128 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/bundle/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/bundle/initialize.yml
+-rw-r--r--   0        0        0     2625 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/bundle/settings.yml
+-rw-r--r--   0        0        0    10326 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/cli_messages.py
+-rw-r--r--   0        0        0     3094 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/config_service.py
+-rw-r--r--   0        0        0       81 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/container/__init__.py
+-rw-r--r--   0        0        0     2130 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/container/container_service.py
+-rw-r--r--   0        0        0     2997 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/container/container_spec.py
+-rw-r--r--   0        0        0     7391 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/db.py
+-rw-r--r--   0        0        0    14930 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/elt_context.py
+-rw-r--r--   0        0        0     6924 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/environment.py
+-rw-r--r--   0        0        0     2797 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/environment_service.py
+-rw-r--r--   0        0        0     3747 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/error.py
+-rw-r--r--   0        0        0      181 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/hub/__init__.py
+-rw-r--r--   0        0        0    11085 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/hub/client.py
+-rw-r--r--   0        0        0      896 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/hub/schema.py
+-rw-r--r--   0        0        0      103 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job/__init__.py
+-rw-r--r--   0        0        0     5940 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job/finder.py
+-rw-r--r--   0        0        0    11544 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job/job.py
+-rw-r--r--   0        0        0     1036 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job/stale_job_failer.py
+-rw-r--r--   0        0        0     6015 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job_state.py
+-rw-r--r--   0        0        0     2974 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/locked_definition_service.py
+-rw-r--r--   0        0        0      699 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/__init__.py
+-rw-r--r--   0        0        0     4530 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/formatters.py
+-rw-r--r--   0        0        0     5573 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/job_logging_service.py
+-rw-r--r--   0        0        0     7367 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/output_logger.py
+-rw-r--r--   0        0        0     7084 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/utils.py
+-rw-r--r--   0        0        0     3453 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/__init__.py
+-rw-r--r--   0        0        0      365 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/cache.py
+-rw-r--r--   0        0        0     4835 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/contexts.py
+-rw-r--r--   0        0        0     4867 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/jsonschema.py
+-rw-r--r--   0        0        0    18190 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/manifest.py
+-rw-r--r--   0        0        0     5137 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/meltano_file.py
+-rw-r--r--   0        0        0     2679 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/meltano_invoker.py
+-rw-r--r--   0        0        0     3665 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/migration_service.py
+-rw-r--r--   0        0        0      481 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/models.py
+-rw-r--r--   0        0        0      188 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/plugin/__init__.py
+-rw-r--r--   0        0        0     5707 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/plugin/airflow.py
+-rw-r--r--   0        0        0    27344 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/plugin/base.py
+-rw-r--r--   0        0        0     3638 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/command.py
+-rw-r--r--   0        0        0     1422 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/config_service.py
+-rw-r--r--   0        0        0      139 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/dbt/__init__.py
+-rw-r--r--   0        0        0     4072 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/dbt/base.py
+-rw-r--r--   0        0        0     2703 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/error.py
+-rw-r--r--   0        0        0     1849 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/factory.py
+-rw-r--r--   0        0        0     9890 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/file.py
+-rw-r--r--   0        0        0     2708 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/meltano_file.py
+-rw-r--r--   0        0        0    14822 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/project_plugin.py
+-rw-r--r--   0        0        0     1135 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/requirements.py
+-rw-r--r--   0        0        0     7651 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/settings_service.py
+-rw-r--r--   0        0        0      282 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/__init__.py
+-rw-r--r--   0        0        0     2552 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/base.py
+-rw-r--r--   0        0        0    19585 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/catalog.py
+-rw-r--r--   0        0        0     2362 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/mapper.py
+-rw-r--r--   0        0        0    23536 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/tap.py
+-rw-r--r--   0        0        0     5573 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/target.py
+-rw-r--r--   0        0        0     5850 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/superset.py
+-rw-r--r--   0        0        0      269 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/utility.py
+-rw-r--r--   0        0        0    16700 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_install_service.py
+-rw-r--r--   0        0        0    17248 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_invoker.py
+-rw-r--r--   0        0        0     6473 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_location_remove.py
+-rw-r--r--   0        0        0     3931 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_lock_service.py
+-rw-r--r--   0        0        0     2817 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_remove_service.py
+-rw-r--r--   0        0        0     2180 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_repository.py
+-rw-r--r--   0        0        0     3289 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_test_service.py
+-rw-r--r--   0        0        0    20306 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project.py
+-rw-r--r--   0        0        0     3999 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_add_service.py
+-rw-r--r--   0        0        0    14180 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_files.py
+-rw-r--r--   0        0        0     6581 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_init_service.py
+-rw-r--r--   0        0        0    18330 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_plugins_service.py
+-rw-r--r--   0        0        0     5118 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_settings_service.py
+-rw-r--r--   0        0        0      262 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/runner/__init__.py
+-rw-r--r--   0        0        0     2149 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/runner/dbt.py
+-rw-r--r--   0        0        0    10141 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/runner/singer.py
+-rw-r--r--   0        0        0     3769 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/schedule.py
+-rw-r--r--   0        0        0    10918 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/schedule_service.py
+-rw-r--r--   0        0        0     3384 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/select_service.py
+-rw-r--r--   0        0        0      926 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/setting.py
+-rw-r--r--   0        0        0    15081 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/setting_definition.py
+-rw-r--r--   0        0        0    21245 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/settings_service.py
+-rw-r--r--   0        0        0    46397 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/settings_store.py
+-rw-r--r--   0        0        0     2573 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/sqlalchemy.py
+-rw-r--r--   0        0        0     7282 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_service.py
+-rw-r--r--   0        0        0     3728 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/__init__.py
+-rw-r--r--   0        0        0     5482 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/azure.py
+-rw-r--r--   0        0        0     2134 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/base.py
+-rw-r--r--   0        0        0     3831 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/db.py
+-rw-r--r--   0        0        0    17948 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/filesystem.py
+-rw-r--r--   0        0        0     4170 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/google.py
+-rw-r--r--   0        0        0     4860 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/s3.py
+-rw-r--r--   0        0        0     4461 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/task_sets.py
+-rw-r--r--   0        0        0     3993 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/task_sets_service.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:47:55.036203 meltano-3.4.0a1/src/meltano/core/tracking/.release_marker
+-rw-r--r--   0        0        0     3614 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/README.md
+-rw-r--r--   0        0        0      125 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/__init__.py
+-rw-r--r--   0        0        0      470 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/cli.py
+-rw-r--r--   0        0        0     6044 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/environment.py
+-rw-r--r--   0        0        0     3790 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/exception.py
+-rw-r--r--   0        0        0     4948 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/plugins.py
+-rw-r--r--   0        0        0     4128 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/project.py
+-rw-r--r--   0        0        0      918 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1051 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1194 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0      720 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      748 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     6002 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     6501 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     6963 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
+-rw-r--r--   0        0        0     7408 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
+-rw-r--r--   0        0        0     4449 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1403 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1462 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     3920 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2109 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2812 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     1202 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      404 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu.json
+-rw-r--r--   0        0        0     9688 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/micro.conf
+-rw-r--r--   0        0        0     1112 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/schemas.py
+-rw-r--r--   0        0        0    18604 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/tracker.py
+-rw-r--r--   0        0        0     3562 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/transform_add_service.py
+-rw-r--r--   0        0        0     7708 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/upgrade_service.py
+-rw-r--r--   0        0        0    25155 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/utils/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/utils/pidfile.py
+-rw-r--r--   0        0        0     4105 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/validation_service.py
+-rw-r--r--   0        0        0    15701 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/venv_service.py
+-rw-r--r--   0        0        0     1521 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/yaml.py
+-rw-r--r--   0        0        0      508 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/__init__.py
+-rw-r--r--   0        0        0       12 2024-04-03 20:47:54.964203 meltano-3.4.0a1/src/meltano/migrations/db.lock
+-rw-r--r--   0        0        0     1490 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/env.py
+-rw-r--r--   0        0        0      495 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/script.py.mako
+-rw-r--r--   0        0        0       67 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/utils/__init__.py
+-rw-r--r--   0        0        0     1261 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/utils/dialect_typing.py
+-rw-r--r--   0        0        0     1814 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
+-rw-r--r--   0        0        0      972 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
+-rw-r--r--   0        0        0      674 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
+-rw-r--r--   0        0        0      802 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
+-rw-r--r--   0        0        0      563 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
+-rw-r--r--   0        0        0    11827 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
+-rw-r--r--   0        0        0     2877 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/6ef30ab7b8e5_.py
+-rw-r--r--   0        0        0     1095 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
+-rw-r--r--   0        0        0      643 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
+-rw-r--r--   0        0        0      786 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
+-rw-r--r--   0        0        0     2026 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/b4c05e463b53_.py
+-rw-r--r--   0        0        0      972 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
+-rw-r--r--   0        0        0      699 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
+-rw-r--r--   0        0        0      679 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
+-rw-r--r--   0        0        0      486 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
+-rw-r--r--   0        0        0    37186 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/schemas/meltano.schema.json
+-rw-r--r--   0        0        0      438 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/asserts.py
+-rw-r--r--   0        0        0     7479 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/conftest.py
+-rw-r--r--   0        0        0     2174 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/cli.py
+-rw-r--r--   0        0        0   125876 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/core.py
+-rw-r--r--   0        0        0     2829 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/__init__.py
+-rw-r--r--   0        0        0     2510 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/mssql.py
+-rw-r--r--   0        0        0     1227 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/postgresql.py
+-rw-r--r--   0        0        0     1222 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/postgresql_psycopg3.py
+-rw-r--r--   0        0        0      328 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/sqlite.py
+-rw-r--r--   0        0        0      752 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/docker/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/docker/docker-compose.yml
+-rw-r--r--   0        0        0     4132 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/docker/snowplow.py
+-rw-r--r--   0        0        0     1535 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/fs.py
+-rw-r--r--   0        0        0     3135 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/large_config_project/meltano.yml
+-rw-r--r--   0        0        0    30013 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/large_config_project/schedule.yml
+-rw-r--r--   0        0        0     1086 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/multifile_project/meltano.yml
+-rw-r--r--   0        0        0      469 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/multifile_project/subconfig_2.yml
+-rw-r--r--   0        0        0      394 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
+-rw-r--r--   0        0        0      631 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/plugins/extractors/tap-custom/test.yml
+-rw-r--r--   0        0        0     1136 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/utils.py
+-rw-r--r--   0        0        0    31067 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_add.py
+-rw-r--r--   0        0        0    15154 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_cli.py
+-rw-r--r--   0        0        0     5174 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_compile.py
+-rw-r--r--   0        0        0     8595 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_config.py
+-rw-r--r--   0        0        0    42025 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_elt.py
+-rw-r--r--   0        0        0     1585 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_hub.py
+-rw-r--r--   0        0        0     3577 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_initialize.py
+-rw-r--r--   0        0        0    12665 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_install.py
+-rw-r--r--   0        0        0     9285 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_invoke.py
+-rw-r--r--   0        0        0     6777 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_job_cmd.py
+-rw-r--r--   0        0        0     3771 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_lock.py
+-rw-r--r--   0        0        0     1864 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_remove.py
+-rw-r--r--   0        0        0    47456 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_run.py
+-rw-r--r--   0        0        0     8502 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_schedule.py
+-rw-r--r--   0        0        0     1140 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_select.py
+-rw-r--r--   0        0        0    11532 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_state.py
+-rw-r--r--   0        0        0     8268 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_upgrade.py
+-rw-r--r--   0        0        0     5381 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/behavior/test_canonical.py
+-rw-r--r--   0        0        0     2155 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/behavior/test_hookable.py
+-rw-r--r--   0        0        0    21766 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/block/test_extract_load.py
+-rw-r--r--   0        0        0      241 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/block/test_parser.py
+-rw-r--r--   0        0        0      933 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/block/test_plugin_command.py
+-rw-r--r--   0        0        0     7736 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/block/test_singer.py
+-rw-r--r--   0        0        0     2302 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/container/test_container_spec.py
+-rw-r--r--   0        0        0     6783 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/hub/test_meltano_hub_service.py
+-rw-r--r--   0        0        0     2076 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/job/test_finder.py
+-rw-r--r--   0        0        0     6240 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/job/test_job.py
+-rw-r--r--   0        0        0     2579 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/job/test_stale_job_failer.py
+-rw-r--r--   0        0        0     3357 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/logging/test_formatters.py
+-rw-r--r--   0        0        0      806 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/logging/test_logging_utils.py
+-rw-r--r--   0        0        0     7398 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/logging/test_output_logger.py
+-rw-r--r--   0        0        0    32051 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_catalog.py
+-rw-r--r--   0        0        0      562 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_mapper.py
+-rw-r--r--   0        0        0    37590 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_tap.py
+-rw-r--r--   0        0        0     3690 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_target.py
+-rw-r--r--   0        0        0     3921 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_airflow.py
+-rw-r--r--   0        0        0     2396 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_command.py
+-rw-r--r--   0        0        0    22146 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin.py
+-rw-r--r--   0        0        0      174 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin_config_service.py
+-rw-r--r--   0        0        0    35208 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin_settings.py
+-rw-r--r--   0        0        0     5963 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_superset.py
+-rw-r--r--   0        0        0     7999 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/runner/test_runner.py
+-rw-r--r--   0        0        0     2807 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/state_store/test_db.py
+-rw-r--r--   0        0        0    21574 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/state_store/test_filesystem.py
+-rw-r--r--   0        0        0     6765 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/state_store/test_state_store.py
+-rw-r--r--   0        0        0     1558 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_db_compat.py
+-rw-r--r--   0        0        0     1813 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_db_connection.py
+-rw-r--r--   0        0        0     5217 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_elt_context.py
+-rw-r--r--   0        0        0     2610 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_environment_service.py
+-rw-r--r--   0        0        0    13772 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_environment_variables.py
+-rw-r--r--   0        0        0     2274 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_locked_definition_service.py
+-rw-r--r--   0        0        0     2108 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_meltano_file.py
+-rw-r--r--   0        0        0     3128 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_meltano_invoker.py
+-rw-r--r--   0        0        0     4094 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_plugin_install_service.py
+-rw-r--r--   0        0        0     6101 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_plugin_invoker.py
+-rw-r--r--   0        0        0     3127 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_plugin_lock_service.py
+-rw-r--r--   0        0        0     5749 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_plugin_remove_service.py
+-rw-r--r--   0        0        0     5776 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_plugin_test_service.py
+-rw-r--r--   0        0        0     4319 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project.py
+-rw-r--r--   0        0        0     8892 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_add_service.py
+-rw-r--r--   0        0        0    16326 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_files.py
+-rw-r--r--   0        0        0     3281 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_init_service.py
+-rw-r--r--   0        0        0     8071 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_plugins_service.py
+-rw-r--r--   0        0        0     7238 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_settings_service.py
+-rw-r--r--   0        0        0     9759 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_schedule_service.py
+-rw-r--r--   0        0        0     2766 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_setting_definition.py
+-rw-r--r--   0        0        0    22226 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_settings_store.py
+-rw-r--r--   0        0        0     3665 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_state_service.py
+-rw-r--r--   0        0        0     2430 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_task_sets.py
+-rw-r--r--   0        0        0     2645 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_task_sets_service.py
+-rw-r--r--   0        0        0     7126 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_utils.py
+-rw-r--r--   0        0        0     1813 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_validation_service.py
+-rw-r--r--   0        0        0    10040 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_venv_service.py
+-rw-r--r--   0        0        0     1980 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_environment_context.py
+-rw-r--r--   0        0        0     5708 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_exception.py
+-rw-r--r--   0        0        0     3061 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_plugins.py
+-rw-r--r--   0        0        0     1271 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_project_context.py
+-rw-r--r--   0        0        0      684 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_schemas.py
+-rw-r--r--   0        0        0    19704 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_tracker.py
+-rw-r--r--   0        0        0     8964 1970-01-01 00:00:00.000000 meltano-3.4.0a1/PKG-INFO
```

### Comparing `meltano-3.3.2/LICENSE` & `meltano-3.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/README.md` & `meltano-3.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/pyproject.toml` & `meltano-3.4.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltano"
-version = "3.3.2"
+version = "3.4.0a1"
 description = "Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love."
 authors = ["Meltano <hello@meltano.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/meltano/meltano"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -40,50 +40,50 @@
 "Youtube" = "https://www.youtube.com/meltano"
 
 [tool.poetry.dependencies]
 aiodocker = "^0.21.0"
 alembic = "^1.13.1"
 atomicwrites = "^1.2.1"
 azure-common = {version = "^1.1.28", optional = true}
-azure-core = {version = "^1.30.0", optional = true}
+azure-core = {version = "^1.30.1", optional = true}
 azure-identity = {version = "^1.15.0", optional = true}
-azure-storage-blob = {version = "^12.19.0", optional = true}
-boto3 = {version = "^1.34.49", optional = true}
-check-jsonschema = "^0.28.0"
+azure-storage-blob = {version = "^12.19.1", optional = true}
+boto3 = {version = "^1.34.74", optional = true}
+check-jsonschema = "^0.28.1"
 click = "^8.1"
 click-default-group = "^1.2.4"
-click-didyoumean = "^0.3.0"
-croniter = "^2.0.1"
+click-didyoumean = "^0.3.1"
+croniter = "^2.0.3"
 fasteners = "^0.19"
 flatten-dict = "^0"
 google-cloud-storage = {version = ">=1.31.0", optional = true}
-importlib-resources = "^6.1.2"
+importlib-resources = "^6.4.0"
 jinja2 = "^3.1.3"
 jsonschema = "^4.21"
-packaging = "^23.2"
+packaging = "^24.0"
 platformdirs = "^4.2.0"
 psutil = "^5.9.8"
 psycopg = {version = "^3.1.18", extras = ["binary"], optional = true}
 psycopg2-binary = {version="^2.9.9", optional=true}
 pyjwt = "^2.6.0"
 pymssql = {version = "^2.2.11", optional = true}
 python = ">=3.8,<3.13"
-python-dateutil = "^2.8.2"
+python-dateutil = "^2.9.0"
 python-dotenv = "^1.0.1"
 python-slugify = "^8.0.4"
 python-ulid = "^1.1.0"
 pyyaml = "^6.0.1"
 questionary = "^2.0.1"
 requests = "^2.31.0"
-rich = "^13.7.0"
-"ruamel.yaml" = "^0.18.5"
-setuptools = {version = "^69.1.1", python = ">=3.12"}
-smart-open = "^7.0.1"
-snowplow-tracker = "^1.0.1"
-sqlalchemy = "^2.0.27"
+rich = "^13.7.1"
+"ruamel.yaml" = "^0.18.6"
+setuptools = {version = "^69.2.0", python = ">=3.12"}
+smart-open = "^7.0.4"
+snowplow-tracker = "^1.0.2"
+sqlalchemy = "^2.0.29"
 structlog = "^24.1.0"
 tabulate = "^0.9.0"
 typing-extensions = "^4.10.0"
 tzlocal = "^5.2"
 # Compatibility issues with boto: https://github.com/boto/botocore/pull/3034
 urllib3 = "<2"
 virtualenv = "^20.25.1"
@@ -95,43 +95,43 @@
 mssql = ["pymssql"]
 postgres = ["psycopg"]
 psycopg2 = ["psycopg2-binary"]
 s3 = ["boto3"]
 
 [tool.poetry.group.dev.dependencies]
 backoff = "^2.1.2"
-black = "^24.2.0"
-boto3-stubs = {extras = ["essential"], version = "1.34.54"}
+black = "^24.3.0"
+boto3-stubs = {extras = ["essential"], version = "1.34.74"}
 bumpversion = "^0.6.0"
 colorama = "^0.4.4"
 coverage = {extras = ["toml"], version = ">=7.3.2,!=7.3.3"}
 freezegun = "^1.4.0"
-hypothesis = "^6.98.17"
+hypothesis = "^6.100.0"
 mock = "^5.0.2"
-moto = "^5.0.2"
-mypy = "^1.8.0"
+moto = "^5.0.4"
+mypy = "^1.9.0"
 pre-commit = "^3.5.0"
-pytest = "^8.1.0"
-pytest-asyncio = "^0.23.4"
-pytest-cov = "^4.1.0"
+pytest = "^8.1.1"
+pytest-asyncio = "^0.23.6"
+pytest-cov = "^5.0.0"
 pytest-docker = "^3.1"
 pytest-httpserver = "^1.0.10"
 pytest-order = "^1.2"
 pytest-randomly = "^3.12"
-pytest-rerunfailures = "^13.0"
-pytest-structlog = "^0.7"
+pytest-rerunfailures = "^14.0"
+pytest-structlog = "^0.8"
 pytest-xdist = "^3.5"
-requests-mock = "^1.11.0"
+requests-mock = "^1.12.1"
 setproctitle = "^1.3" # Used by pytest-xdist to aid with handling resource intensive processes.
 types-croniter = "^2.0.0"
-types-jsonschema = "^4.21.0.20240118"
-types-psutil = "^5.9.5.20240205"
-types-python-dateutil = "^2.8.19.20240106"
-types-python-slugify = "^8.0.2.20240127"
-types-pyyaml = "^6.0.12.12"
+types-jsonschema = "^4.21.0.20240331"
+types-psutil = "^5.9.5.20240316"
+types-python-dateutil = "^2.9.0.20240316"
+types-python-slugify = "^8.0.2.20240310"
+types-pyyaml = "^6.0.12.20240311"
 types-requests = "^2.31.0"
 types-tabulate = "^0.9.0.20240106"
 
 [tool.poetry.scripts]
 meltano = "meltano.cli:main"
 
 [tool.black]
@@ -442,38 +442,41 @@
 ]
 parallel = true
 relative_files = true  # This allows coverage to be measured in Windows
 source = [
   "meltano",
   "tests",
 ]
+omit = [
+  "src/meltano/migrations/env.py",
+  "src/meltano/cli/interactive/*",
+]
 
 [tool.coverage.paths]
 source = [
   "src/meltano/",
   "**/site-packages/meltano/",
   "**/site-packages/meltano*/meltano/",
 ]
 
 [tool.coverage.report]
-exclude_lines = [
-  "pragma: no cover",
+exclude_also = [
   '''if (t\.)?TYPE_CHECKING:''',
   "\\.\\.\\.",
 ]
 precision = 2
 show_missing = true
 skip_covered = true
 
 [tool.commitizen]
 name = "cz_version_bump"
 prerelease_offset = 1
 tag_format = "v$major.$minor.$patch$prerelease"
 changelog_merge_prerelease = true
-version = "3.3.2"
+version = "3.4.0a1"
 version_files = [
   "pyproject.toml:^version =",
   "src/meltano/__init__.py:^__version__ =",
   'docs/package.json:^  "version":',
 ]
 
 [tool.mypy]
@@ -523,15 +526,14 @@
   "meltano.core.elt_context",
   "meltano.core.meltano_invoker",
   "meltano.core.migration_service",
   "meltano.core.models",
   "meltano.core.plugin_install_service",
   "meltano.core.plugin_invoker",
   "meltano.core.plugin_test_service",
-  "meltano.core.project",
   "meltano.core.project_add_service",
   "meltano.core.project_files",
   "meltano.core.project_plugins_service",
   "meltano.core.project_settings_service",
   "meltano.core.select_service",
   "meltano.core.settings_service",
   "meltano.core.settings_store",
@@ -589,24 +591,30 @@
 ]
 select = [
   "ARG", # flake8-unused-arguments
   "B",   # flake8-bugbear
   "C4",  # flake8-comprehensions
   "COM", # flake8-commas
   "E",   # pycodestyle (error)
+  "EM",   # flake8-errmsg
   "ERA", # flake8-eradicate
   "F",   # pyflakes
   "G",   # flake8-logging-format
   "I",   # isort
   "ISC", # flake8-implicit-str-concat
   "N",   # pep8-naming
+  "PIE", # flake8-pie
   "PT",  # flake8-pytest-style
+  "Q",   # flake8-quotes
+  "RET", # flake8-return
   "RSE", # flake8-raise
   "S",   # flake8-bandit
   "SIM", # flake8-simplify
+  "T10", # flake8-debugger
+  "T20", # flake8-print
   "TID", # flake8-tidy-imports
   "UP",  # pyupgrade
   "W",   # pycodestyle (warning)
   "TID", # flake8-tidy-imports
   "TCH", # flake8-type-checking
 ]
 unfixable = [
```

### Comparing `meltano-3.3.2/src/meltano/cli/__init__.py` & `meltano-3.4.0a1/src/meltano/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,22 +98,22 @@
         KeyboardInterrupt: if caught.
     """
     try:
         try:  # noqa: WPS225, WPS505
             cli(obj={"project": None})
         except ProjectReadonly as err:
             raise CliError(
-                f"The requested action could not be completed: {err}",
+                f"The requested action could not be completed: {err}",  # noqa: EM102
             ) from err
         except KeyboardInterrupt:  # noqa: WPS329
             raise
         except MeltanoError as err:
             handle_meltano_error(err)
         except Exception as err:
-            raise CliError(f"{troubleshooting_message}\n{err}") from err
+            raise CliError(f"{troubleshooting_message}\n{err}") from err  # noqa: EM102
     except CliError as cli_error:
         cli_error.print()
         sys.exit(1)
 
 
 def main():
     """Entry point for the meltano CLI."""
```

### Comparing `meltano-3.3.2/src/meltano/cli/add.py` & `meltano-3.4.0a1/src/meltano/cli/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 if t.TYPE_CHECKING:
     from meltano.core.plugin.project_plugin import ProjectPlugin
     from meltano.core.project import Project
     from meltano.core.tracking import Tracker
 
 
-def _load_yaml_from_ref(_ctx, _param, value: str | None) -> dict:
+def _load_yaml_from_ref(_ctx, _param, value: str | None) -> dict | None:
     if not value:
-        return
+        return None
 
     try:
         url = urlparse(value)
         if url.scheme and url.netloc:
             response = requests.get(value, timeout=10)
             response.raise_for_status()
             content = response.text
@@ -75,15 +75,15 @@
         "Usage:\b\n\nadd <type> <inherit-from> --as <name>"
     ),
 )
 @click.option(
     "--from-ref",
     "plugin_yaml",
     callback=_load_yaml_from_ref,
-    help="Reference a plugin defintion to add from.",
+    help="Reference a plugin definition to add from.",
 )
 @click.option(
     "--python",
     help=(
         "The Python version to use for the plugin. Only applies to base plugins which "
         "have Python virtual environments, rather than inherited plugins which use the "
         "virtual environment of their base plugin, or plugins that run in a container."
@@ -144,26 +144,26 @@
         plugin_names = [as_name]
 
     if flags["custom"] and plugin_type in {
         PluginType.TRANSFORMS,
         PluginType.ORCHESTRATORS,
     }:
         tracker.track_command_event(CliEvent.aborted)
-        raise CliError(f"--custom is not supported for {plugin_type}")
+        raise CliError(f"--custom is not supported for {plugin_type}")  # noqa: EM102
 
     plugin_refs = [
         PluginRef(plugin_type=plugin_type, name=name) for name in plugin_names
     ]
     dependencies_met, err = check_dependencies_met(
         plugin_refs=plugin_refs,
         plugins_service=project.plugins,
     )
     if not dependencies_met:
         tracker.track_command_event(CliEvent.aborted)
-        raise CliError(f"Failed to install plugin(s): {err}")
+        raise CliError(f"Failed to install plugin(s): {err}")  # noqa: EM102
 
     add_service = ProjectAddService(project)
 
     plugins: list[ProjectPlugin] = []
     for plugin in plugin_names:
         try:
             plugins.append(
@@ -203,15 +203,15 @@
             plugins,
             reason=PluginInstallReason.ADD,
             force=flags.get("force_install", False),
         )
 
         if not success:
             tracker.track_command_event(CliEvent.failed)
-            raise CliError("Failed to install plugin(s)")
+            raise CliError("Failed to install plugin(s)")  # noqa: EM101
 
     _print_plugins(plugins)
     tracker.track_command_event(CliEvent.completed)
 
 
 def _print_plugins(plugins):
     printed_empty_line = False
```

### Comparing `meltano-3.3.2/src/meltano/cli/cli.py` & `meltano-3.4.0a1/src/meltano/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     if no_color:
         ctx.color = False
 
     if cwd:
         try:
             os.chdir(cwd)
         except OSError as ex:
-            raise Exception(f"Unable to run Meltano from {cwd!r}") from ex
+            raise Exception(f"Unable to run Meltano from {cwd!r}") from ex  # noqa: EM102
 
     try:
         project = Project.find()
         setup_logging(project)
         logger.debug("meltano %s, %s", __version__, platform.system())  # noqa: WPS323
         if project.readonly:
             logger.debug("Project is read-only.")
```

### Comparing `meltano-3.3.2/src/meltano/cli/compile.py` & `meltano-3.4.0a1/src/meltano/cli/compile.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     """  # noqa: E501
     tracker: Tracker = ctx.obj["tracker"]
 
     try:
         directory.mkdir(parents=True, exist_ok=True)
     except OSError as ex:
         raise CliError(
-            f"Unable to create directory for Meltano manifests {directory}: {ex}",
+            f"Unable to create directory for Meltano manifests {directory}: {ex}",  # noqa: EM102
         ) from ex
 
     environments = _environments(ctx, project)
 
     click.echo(
         "Compiling Meltano manifest for environments: "
         + ", ".join("no environment" if x is None else x.name for x in environments),
@@ -95,15 +95,15 @@
                     manifest.data,
                     manifest_file,
                     indent=indent if indent > 0 else None,
                     sort_keys=True,
                 )
         except OSError as ex:
             raise CliError(
-                f"Unable to write Meltano manifest {str(path)!r}: {ex}",
+                f"Unable to write Meltano manifest {str(path)!r}: {ex}",  # noqa: EM102
             ) from ex
 
         click.echo(f"Compiled {path}")
         tracker.track_command_event(CliEvent.inflight)
 
 
 def _environments(
```

### Comparing `meltano-3.3.2/src/meltano/cli/config.py` & `meltano-3.4.0a1/src/meltano/cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     Raises:
         ValueError: if there is no click.core.Context in the given args.
     """
     for arg in args:
         if isinstance(arg, click.core.Context):
             return arg
-    raise ValueError("No click.core.Context provided in *args")
+    raise ValueError("No click.core.Context provided in *args")  # noqa: EM101
 
 
 def _get_store_choices() -> list[SettingValueStore]:
     """Get a list of valid choices for the --store flag.
 
     Returns:
         SettingValueStore.writables(), without meltano_env
@@ -339,15 +339,15 @@
     tracker = ctx.obj["tracker"]
 
     try:
         metadata = settings.reset(store=store, session=session)
     except StoreNotSupportedError as err:
         tracker.track_command_event(CliEvent.aborted)
         raise CliError(
-            f"{settings.label.capitalize()} settings in {store.label} could "
+            f"{settings.label.capitalize()} settings in {store.label} could "  # noqa: EM102
             f"not be reset: {err}",
         ) from err
 
     store = metadata["store"]
     click.secho(
         f"{settings.label.capitalize()} settings in {store.label} were reset",
         fg="green",
@@ -396,15 +396,15 @@
 @click.pass_context
 def test(ctx):
     """Test the configuration of a plugin."""
     invoker = ctx.obj["invoker"]
     tracker = ctx.obj["tracker"]
     if not invoker:
         tracker.track_command_event(CliEvent.aborted)
-        raise CliError("Testing of the Meltano project configuration is not supported")
+        raise CliError("Testing of the Meltano project configuration is not supported")  # noqa: EM101
 
     session = ctx.obj["session"]
 
     async def _validate():  # noqa: WPS430
         plugin_test_service = PluginTestServiceFactory(invoker).get_test_service()
         async with plugin_test_service.plugin_invoker.prepared(session):
             return await plugin_test_service.validate()
@@ -442,15 +442,15 @@
 
     path = list(setting_name)
     try:
         metadata = settings.unset(path, store=store, session=session)
     except StoreNotSupportedError as err:
         tracker.track_command_event(CliEvent.aborted)
         raise CliError(
-            f"{settings.label.capitalize()} setting '{path}' in {store.label} "
+            f"{settings.label.capitalize()} setting '{path}' in {store.label} "  # noqa: EM102
             f"could not be unset: {err}",
         ) from err
 
     name = metadata["name"]
     store = metadata["store"]
     click.secho(
         f"{settings.label.capitalize()} setting '{name}' in {store.label} was unset",
```

### Comparing `meltano-3.3.2/src/meltano/cli/elt.py` & `meltano-3.4.0a1/src/meltano/cli/elt.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     dump: str,
     state_id: str,
     force: bool,
     merge_state: bool,
 ):
     if platform.system() == "Windows":
         raise CliError(
-            "ELT command not supported on Windows. Please use the run command "
+            "ELT command not supported on Windows. Please use the run command "  # noqa: EM101
             "as documented here: "
             "https://docs.meltano.com/reference/command-line-interface#run",
         )
 
     tracker: Tracker = ctx.obj["tracker"]
 
     # We no longer set a default choice for transform, so that we can detect
@@ -349,25 +349,25 @@
         invoker = elt_context.invoker_for(plugin_type)
 
         async with invoker.prepared(elt_context.session):
             content = await invoker.dump(file_id)
 
         click.echo(content)
     except FileNotFoundError as err:
-        raise CliError(f"Could not find {dumpable} file for this pipeline") from err
+        raise CliError(f"Could not find {dumpable} file for this pipeline") from err  # noqa: EM102
     except Exception as err:
-        raise CliError(f"Could not dump {dumpable}: {err}") from err
+        raise CliError(f"Could not dump {dumpable}: {err}") from err  # noqa: EM102
 
 
 async def _run_job(tracker, project, job, session, context_builder, force=False):
     fail_stale_jobs(session, job.job_name)
 
     if not force and (existing := JobFinder(job.job_name).latest_running(session)):
         raise CliError(
-            f"Another '{job.job_name}' pipeline is already running which "
+            f"Another '{job.job_name}' pipeline is already running which "  # noqa: EM102
             f"started at {existing.started_at}. To ignore this check use "
             "the '--force' option.",
         )
 
     async with job.run(session):
         job_logging_service = JobLoggingService(project)
         log_file = job_logging_service.generate_log_name(job.job_name, job.run_id)
@@ -423,15 +423,15 @@
                     "removed in a future version.",
                 )
                 await _run_transform(log, elt_context, output_logger)
             else:
                 log.info("Transformation skipped.")
         except RunnerError as err:
             raise CliError(
-                f"ELT could not be completed: {err}.\nFor more detailed log "
+                f"ELT could not be completed: {err}.\nFor more detailed log "  # noqa: EM102
                 "messages re-run the command using 'meltano "
                 "--log-level=debug ...' CLI flag.\nNote that you can also "
                 f"check the generated log file at '{output_logger.file}'.\n"
                 "For more information on debugging and logging: "
                 "https://docs.meltano.com/reference/command-line-interface#debugging",
             ) from err
```

### Comparing `meltano-3.3.2/src/meltano/cli/environment.py` & `meltano-3.4.0a1/src/meltano/cli/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/cli/hub.py` & `meltano-3.4.0a1/src/meltano/cli/hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,14 @@
         # We want to ensure that we can actually communicate with the Hub.
         # Requesting a list of plugins is a good way to do that, but we don't
         # want to waste bandwidth, so we request the list of orchestrators,
         # which is currently very small.
         project.hub_service.get_plugins_of_type(PluginType.ORCHESTRATORS)
     except Exception as ex:
         raise click.ClickException(
-            f"Failed to connect to the Hub at {project.hub_service.hub_api_url!r}",
+            f"Failed to connect to the Hub at {project.hub_service.hub_api_url!r}",  # noqa: EM102
         ) from ex
     else:
         click.secho(
             f"Successfully connected to the Hub at {project.hub_service.hub_api_url!r}",
             fg="green",
         )
```

### Comparing `meltano-3.3.2/src/meltano/cli/initialize.py` & `meltano-3.4.0a1/src/meltano/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/cli/install.py` & `meltano-3.4.0a1/src/meltano/cli/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 from meltano.core.schedule_service import ScheduleService
 from meltano.core.tracking.contexts import CliEvent, PluginsTrackingContext
 
 if t.TYPE_CHECKING:
     from meltano.core.project import Project
     from meltano.core.tracking import Tracker
 
+ANY = "-"
+
 logger = structlog.getLogger(__name__)
 
 
 @click.command(cls=PartialInstrumentedCmd, short_help="Install project dependencies.")
 @click.argument(
     "plugin_type",
-    type=click.Choice(PluginType.cli_arguments()),
+    type=click.Choice((*PluginType.cli_arguments(), ANY)),
     required=False,
 )
 @click.argument("plugin_name", nargs=-1, required=False)
 @click.option(
     "--clean",
     is_flag=True,
     help="Completely reinstall a plugin rather than simply upgrading if necessary.",
@@ -70,22 +72,23 @@
     """
     Install all the dependencies of your project based on the meltano.yml file.
 
     \b\nRead more at https://docs.meltano.com/reference/command-line-interface#install
     """
     tracker: Tracker = ctx.obj["tracker"]
     try:
-        if plugin_type:
+        if plugin_type and plugin_type != ANY:
             plugin_type = PluginType.from_cli_argument(plugin_type)
             plugins = project.plugins.get_plugins_of_type(plugin_type)
-            if plugin_name:
-                plugins = [plugin for plugin in plugins if plugin.name in plugin_name]
         else:
             plugins = list(project.plugins.plugins())
 
+        if plugin_name:
+            plugins = [plugin for plugin in plugins if plugin.name in plugin_name]
+
         if schedule_name:
             schedule_plugins = _get_schedule_plugins(
                 ctx.obj["project"],
                 schedule_name,
             )
             plugins = list(set(plugins) & set(schedule_plugins))
     except Exception:
@@ -103,15 +106,15 @@
         plugins,
         parallelism=parallelism,
         clean=clean,
         force=force,
     )
     if not success:
         tracker.track_command_event(CliEvent.failed)
-        raise CliError("Failed to install plugin(s)")
+        raise CliError("Failed to install plugin(s)")  # noqa: EM101
     tracker.track_command_event(CliEvent.completed)
 
 
 def _get_schedule_plugins(project: Project, schedule_name: str):
     schedule_service = ScheduleService(project)
     schedule_obj = schedule_service.find_schedule(schedule_name)
     schedule_plugins = set()
```

### Comparing `meltano-3.3.2/src/meltano/cli/interactive/config.py` & `meltano-3.4.0a1/src/meltano/cli/interactive/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,14 +327,15 @@
                     click.secho(f"Failed to set value: {e}", fg="red")
 
         elif action.lower() == "n":
             return InteractionStatus.SKIP
 
         elif action.lower() == "e":
             return InteractionStatus.EXIT
+        return None
 
     def configure_all(self):
         """Configure all settings."""
         numeric_choices = [idx for idx, _, _ in self.setting_choices]
         if not numeric_choices:
             click.secho(
                 "There are no settings to configure. "
@@ -408,15 +409,15 @@
             )
         except StoreNotSupportedError as err:
             if interactive:
                 self.tracker.track_command_event(CliEvent.inflight)
             else:
                 self.tracker.track_command_event(CliEvent.aborted)
             raise CliError(
-                f"{settings.label.capitalize()} setting '{path}' could not be "
+                f"{settings.label.capitalize()} setting '{path}' could not be "  # noqa: EM102
                 f"set in {store.label}: {err}",
             ) from err
 
         name = metadata["name"]
         store = metadata["store"]
         setting = metadata["setting"]
         is_redacted = self.safe and setting and setting.is_redacted
```

### Comparing `meltano-3.3.2/src/meltano/cli/invoke.py` & `meltano-3.4.0a1/src/meltano/cli/invoke.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,11 +209,11 @@
 
 
 async def dump_file(invoker: PluginInvoker, file_id: str):
     """Dump file."""
     try:
         content = await invoker.dump(file_id)
     except FileNotFoundError as err:
-        raise CliError(f"Could not find {file_id}") from err
+        raise CliError(f"Could not find {file_id}") from err  # noqa: EM102
     except Exception as err:
-        raise CliError(f"Could not dump {file_id}: {err}") from err
-    print(content)  # noqa: WPS421
+        raise CliError(f"Could not dump {file_id}: {err}") from err  # noqa: EM102
+    print(content)  # noqa: T201, WPS421
```

### Comparing `meltano-3.3.2/src/meltano/cli/job.py` & `meltano-3.4.0a1/src/meltano/cli/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         tracker.track_command_event(CliEvent.aborted)
         raise CliError(err) from err
 
     try:
         task_sets_service.add(task_sets)
     except JobAlreadyExistsError as serr:
         tracker.track_command_event(CliEvent.failed)
-        raise CliError(f"Job '{task_sets.name}' already exists.") from serr
+        raise CliError(f"Job '{task_sets.name}' already exists.") from serr  # noqa: EM102
 
     click.echo(f"Added job {task_sets.name}: {task_sets.tasks}")
 
     tracker.track_command_event(CliEvent.completed)
 
 
 @job.command(
```

### Comparing `meltano-3.3.2/src/meltano/cli/lock.py` & `meltano-3.4.0a1/src/meltano/cli/lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     \b\nRead more at https://docs.meltano.com/reference/command-line-interface#lock
     """
     tracker: Tracker = ctx.obj["tracker"]
 
     lock_service = PluginLockService(project)
     if (all_plugins and plugin_name) or not (all_plugins or plugin_name):
         tracker.track_command_event(CliEvent.aborted)
-        raise CliError("Exactly one of --all or plugin name must be specified.")
+        raise CliError("Exactly one of --all or plugin name must be specified.")  # noqa: EM101
 
     try:
         with project.plugins.use_preferred_source(DefinitionSource.ANY):
             # Make it a list so source preference is not lazily evaluated.
             plugins = list(project.plugins.plugins())
     except Exception:
         tracker.track_command_event(CliEvent.aborted)
```

### Comparing `meltano-3.3.2/src/meltano/cli/params.py` & `meltano-3.4.0a1/src/meltano/cli/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         @database_uri_option
         def decorate(*args, **kwargs):
             ctx = click.get_current_context()
 
             project = ctx.obj["project"]
             if not project:
                 raise CliError(
-                    f"`{ctx.command_path}` must be run inside a Meltano project.\n"
+                    f"`{ctx.command_path}` must be run inside a Meltano project.\n"  # noqa: EM102
                     "Use `meltano init <project_directory>` to create one.",
                 )
 
             # register the system database connection
             engine, _ = project_engine(project, default=True)
 
             if self.migrate:
```

### Comparing `meltano-3.3.2/src/meltano/cli/remove.py` & `meltano-3.4.0a1/src/meltano/cli/remove.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defines `meltano remove` command."""
+
 from __future__ import annotations
 
 import click
 
 from meltano.cli.params import pass_project
 from meltano.cli.utils import InstrumentedCmd
 from meltano.core.plugin import PluginType
```

### Comparing `meltano-3.3.2/src/meltano/cli/run.py` & `meltano-3.4.0a1/src/meltano/cli/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         tracker.track_command_event(CliEvent.aborted)
         raise parser_err
 
     if validate_block_sets(logger, parsed_blocks):
         logger.debug("All ExtractLoadBlocks validated, starting execution.")
     else:
         tracker.track_command_event(CliEvent.aborted)
-        raise CliError("Some ExtractLoadBlocks set failed validation.")
+        raise CliError("Some ExtractLoadBlocks set failed validation.")  # noqa: EM101
     try:
         await _run_blocks(tracker, parsed_blocks, dry_run=dry_run)
     except Exception as err:
         tracker.track_command_event(CliEvent.failed)
         raise err
     tracker.track_command_event(CliEvent.completed)
 
@@ -186,15 +186,15 @@
                 success=False,
                 err=err,
                 exit_codes=err.exitcodes,
             )
             with tracker.with_contexts(tracking_ctx):
                 tracker.track_block_event(blk_name, BlockEvents.failed)
             raise CliError(
-                f"Run invocation could not be completed as block failed: {err}",
+                f"Run invocation could not be completed as block failed: {err}",  # noqa: EM102
             ) from err
         except Exception as bare_err:
             # make sure we also fire block failed events for all other exceptions
             with tracker.with_contexts(tracking_ctx):
                 tracker.track_block_event(blk_name, BlockEvents.failed)
             raise bare_err
```

### Comparing `meltano-3.3.2/src/meltano/cli/schedule.py` & `meltano-3.4.0a1/src/meltano/cli/schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,22 +136,22 @@
 
     \b\nNote that the --job option and --extractor/--loader options are mutually exclusive.
 
     \b\nRead more at https://docs.meltano.com/reference/command-line-interface#schedule
     """  # noqa: E501
     if job and (extractor or loader):
         raise click.ClickException(
-            "Cannot mix --job with --extractor/--loader/--transform",
+            "Cannot mix --job with --extractor/--loader/--transform",  # noqa: EM101
         )
 
     if not job:
         if not extractor:
-            raise click.ClickException("Missing --extractor")
+            raise click.ClickException("Missing --extractor")  # noqa: EM101
         if not loader:
-            raise click.ClickException("Missing --loader")
+            raise click.ClickException("Missing --loader")  # noqa: EM101
 
         _add_elt(ctx, name, extractor, loader, transform, interval, start_date)
         return
     _add_job(ctx, name, job, interval)
 
 
 def _format_job_list_output(entry: Schedule, job: TaskSets) -> dict:
@@ -303,15 +303,15 @@
         click.ClickException: If the schedule is not a scheduled job.
 
     Returns:
         The updated schedule.
     """
     if not candidate.job:
         raise click.ClickException(
-            f"Cannot update schedule {candidate.name} with job only flags as "
+            f"Cannot update schedule {candidate.name} with job only flags as "  # noqa: EM102
             "its a elt schedule",
         )
     if job:
         candidate.job = job
     if interval:
         candidate.interval = interval
     return candidate
@@ -337,15 +337,15 @@
         click.ClickException: If the schedule is not a scheduled elt task.
 
     Returns:
         The updated schedule.
     """
     if candidate.job:
         raise click.ClickException(
-            f"Cannot update schedule {candidate.name} with elt only flags as "
+            f"Cannot update schedule {candidate.name} with elt only flags as "  # noqa: EM102
             "its a scheduled job",
         )
 
     if extractor:
         candidate.extractor = extractor
     if loader:
         candidate.loader = loader
@@ -398,21 +398,21 @@
     """  # noqa: E501
     schedule_service: ScheduleService = ctx.obj["schedule_service"]
     candidate = schedule_service.find_schedule(name)
 
     if candidate.job:
         if extractor or loader or transform:
             raise click.ClickException(
-                "Cannot mix --job with --extractor/--loader/--transform",
+                "Cannot mix --job with --extractor/--loader/--transform",  # noqa: EM101
             )
         updated = _update_job_schedule(candidate, job, interval)
     else:
         if job:
             raise click.ClickException(
-                "Cannot mix --job with --extractor/--loader/--transform",
+                "Cannot mix --job with --extractor/--loader/--transform",  # noqa: EM101
             )
         updated = _update_elt_schedule(
             candidate,
             extractor,
             loader,
             transform,
             interval,
```

### Comparing `meltano-3.3.2/src/meltano/cli/schema.py` & `meltano-3.4.0a1/src/meltano/cli/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/cli/select.py` & `meltano-3.4.0a1/src/meltano/cli/select.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Extractor selection management CLI."""
+
 from __future__ import annotations
 
 import typing as t
 from contextlib import closing
 
 import click
 
@@ -18,18 +19,19 @@
     from meltano.core.project import Project
 
 
 def selection_color(selection):
     """Return the appropriate colour for given SelectionType."""
     if selection is SelectionType.SELECTED:
         return "bright_green"
-    elif selection is SelectionType.AUTOMATIC:
+    if selection is SelectionType.AUTOMATIC:
         return "bright_white"
-    elif selection is SelectionType.EXCLUDED:
+    if selection is SelectionType.EXCLUDED:
         return "red"
+    return None
 
 
 def selection_mark(selection):
     """
     Return the mark to indicate the selection type of an attribute.
 
     Examples:
@@ -90,15 +92,15 @@
                 extractor,
                 entities_filter,
                 attributes_filter,
                 exclude=flags["exclude"],
                 remove=flags["remove"],
             )
     except PluginExecutionError as err:
-        raise CliError(f"Cannot list the selected attributes: {err}") from err
+        raise CliError(f"Cannot list the selected attributes: {err}") from err  # noqa: EM102
 
 
 def update(
     project,
     extractor,
     entities_filter,
     attributes_filter,
```

### Comparing `meltano-3.3.2/src/meltano/cli/state.py` & `meltano-3.4.0a1/src/meltano/cli/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     mutually_exclusive_options = {
         "--input-file": input_file,
         "STATE": state,
         "--from-state-id": from_state_id,
     }
     if not reduce(xor, (bool(x) for x in mutually_exclusive_options.values())):
         raise MutuallyExclusiveOptionsError(*mutually_exclusive_options)
-    elif input_file:
+    if input_file:
         with open(input_file) as state_f:
             state_service.add_state(
                 state_id,
                 state_f.read(),
                 payload_flags=Payload.INCOMPLETE_STATE,
             )
     elif state:
@@ -278,15 +278,15 @@
     )
     mutually_exclusive_options = {
         "--input-file": input_file,
         "STATE": state,
     }
     if not reduce(xor, (bool(x) for x in mutually_exclusive_options.values())):
         raise MutuallyExclusiveOptionsError(*mutually_exclusive_options)
-    elif input_file:
+    if input_file:
         with open(input_file) as state_f:
             state_service.set_state(state_id, state_f.read())
     elif state:
         state_service.set_state(state_id, state)
     logger.info(
         f"State for {state_id} was successfully set "  # noqa: G004
         f"at {dt.utcnow():%Y-%m-%d %H:%M:%S}.",  # noqa: WPS323
```

### Comparing `meltano-3.3.2/src/meltano/cli/upgrade.py` & `meltano-3.4.0a1/src/meltano/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/cli/utils.py` & `meltano-3.4.0a1/src/meltano/cli/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def __init__(self, *args, **kwargs):
         """Instantiate custom CLI Error exception."""
         super().__init__(*args, **kwargs)
 
         self.printed = False
 
-    def print(self):
+    def print(self):  # noqa: T202
         """Print CLI error."""
         if self.printed:
             return
 
         logger.debug(str(self), exc_info=True)
         click.secho(str(self), fg="red", err=True)
```

### Comparing `meltano-3.3.2/src/meltano/cli/validate.py` & `meltano-3.4.0a1/src/meltano/cli/validate.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,16 +59,15 @@
 
         Returns:
             Exit code for the plugin invocation.
         """
         write_sep_line(f"{self.plugin_name}:{name}", "=", bold=True)
         handle = await self.invoker.invoke_async(command=name)
         with propagate_stop_signals(handle):
-            exit_code = await handle.wait()
-        return exit_code
+            return await handle.wait()
 
 
 @click.command(
     cls=InstrumentedCmd,
     short_help="Run validations using plugins' tests.",
     environment_behavior=CliEnvironmentBehavior.environment_optional_use_default,
 )
@@ -84,15 +83,15 @@
     required=False,
     nargs=-1,
 )
 @pass_project(migrate=True)
 def test(
     project: Project,
     all_tests: bool,
-    plugin_tests: tuple[str] = (),
+    plugin_tests: tuple[str, ...] = (),
 ):
     """
     Run validations using plugins' tests.
 
     \b\nRead more at https://docs.meltano.com/reference/command-line-interface#test
     """
     _, session_maker = project_engine(project)
```

### Comparing `meltano-3.3.2/src/meltano/core/behavior/canonical.py` & `meltano-3.4.0a1/src/meltano/core/behavior/canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/behavior/hookable.py` & `meltano-3.4.0a1/src/meltano/core/behavior/hookable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Hookable class and supporting functions, classes, and decorators.
 
 This module contains the Hookable class which allows for implementation of a
 classic before/after hook pattern. Allowing you to register functions to be
 called before or after given trigger.
 """
+
 from __future__ import annotations
 
 import logging
 from collections import OrderedDict
 from contextlib import asynccontextmanager
 
 logger = logging.getLogger(__name__)
```

### Comparing `meltano-3.3.2/src/meltano/core/behavior/versioned.py` & `meltano-3.4.0a1/src/meltano/core/behavior/versioned.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,11 +30,11 @@
 
     def ensure_compatible(self, version: int | None = None):
         version = self.__class__.__version__ if version is None else version
         file_version = self.file_version
 
         if file_version != version:
             raise IncompatibleVersionError(
-                f"Version {version} required, currently at {self.file_version}",
+                f"Version {version} required, currently at {self.file_version}",  # noqa: EM102
                 file_version,
                 version,
             )
```

### Comparing `meltano-3.3.2/src/meltano/core/block/blockset.py` & `meltano-3.4.0a1/src/meltano/core/block/blockset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/block/extract_load.py` & `meltano-3.4.0a1/src/meltano/core/block/extract_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     @property
     def elt_run_dir(self) -> Path | None:
         """Obtain the run directory for the current job.
 
         Returns:
             The run directory for the current job.
         """
-        if self.job:
+        if self.job:  # noqa: RET503
             return self.project.job_dir(self.job.job_name, str(self.job.run_id))
 
 
 class ELBContextBuilder:  # noqa: WPS214
     """Build up ELBContexts for ExtractLoadBlocks."""
 
     def __init__(self, project: Project):
@@ -274,15 +274,15 @@
     @property
     def elt_run_dir(self) -> Path | None:
         """Get the run directory for the current job.
 
         Returns:
             The run directory for the current job.
         """
-        if self._job:
+        if self._job:  # noqa: RET503
             return self.project.job_dir(self._job.job_name, str(self._job.run_id))
 
     def context(self) -> ELBContext:
         """Create an ELBContext object from the current builder state.
 
         Returns:
             A new `ELBContext` object.
@@ -373,28 +373,28 @@
 
     def index_last_input_done(self) -> int | None:
         """Return index of the block furthest from the start that has exited and required input.
 
         Returns:
             The index of the block furthest from the start that has exited and required input.
         """  # noqa: E501
-        for idx, block in reversed(list(enumerate(self.blocks))):
+        for idx, block in reversed(list(enumerate(self.blocks))):  # noqa: RET503
             if block.requires_input and block.proxy_stderr.done():
                 return idx
 
     def upstream_complete(self, index: int) -> bool | None:
         """Return whether blocks upstream from a given block index are already done.
 
         Args:
             index: The index of the block to check upstream from.
 
         Returns:
             True if all upstream blocks are done, False otherwise.
         """
-        for idx, block in enumerate(self.blocks):
+        for idx, block in enumerate(self.blocks):  # noqa: RET503
             if idx >= index:
                 return True
             if block.process_future.done():
                 continue
             return False
 
     async def upstream_stop(self, index) -> None:
@@ -433,26 +433,26 @@
     def validate_set(self) -> None:  # noqa: WPS231, WPS238
         """Validate a ExtractLoad block set to ensure its valid and runnable.
 
         Raises:
             BlockSetValidationError: if the block set is not valid.
         """
         if not self.blocks:
-            raise BlockSetValidationError("No blocks in set.")
+            raise BlockSetValidationError("No blocks in set.")  # noqa: EM101
 
         if self.head.consumer:
-            raise BlockSetValidationError("first block in set should not be consumer")
+            raise BlockSetValidationError("first block in set should not be consumer")  # noqa: EM101
 
         if self.tail.producer:
-            raise BlockSetValidationError("last block in set should not be a producer")
+            raise BlockSetValidationError("last block in set should not be a producer")  # noqa: EM101
 
         for block in self.intermediate:
             if not block.consumer or not block.producer:
                 raise BlockSetValidationError(
-                    "intermediate blocks must be producers AND consumers",
+                    "intermediate blocks must be producers AND consumers",  # noqa: EM101
                 )
 
     async def execute(self) -> None:
         """Build the IO chain and execute the actual ELT task."""
         async with self._start_blocks():
             await self._link_io()
             manager = ELBExecutionManager(self)
@@ -485,15 +485,15 @@
         fail_stale_jobs(self.context.session, job.job_name)
         if not self.context.force and (
             existing := JobFinder(job.job_name).latest_running(
                 self.context.session,
             )
         ):
             raise RunnerError(
-                f"Another '{job.job_name}' pipeline is already running "
+                f"Another '{job.job_name}' pipeline is already running "  # noqa: EM102
                 f"which started at {existing.started_at}. To ignore this "
                 "check use the '--force' option.",
             )
 
         with closing(self.context.session) as session:
             async with job.run(session):
                 await self.execute()
@@ -605,14 +605,16 @@
         """
         for idx, block in enumerate(self.blocks):
             logger_base = logger.bind(
                 consumer=block.consumer,
                 producer=block.producer,
                 string_id=block.string_id,
                 cmd_type="elb",
+                run_id=str(self.context.job.run_id) if self.context.job else None,
+                job_name=self.context.job.job_name if self.context.job else None,
             )
             if logger.isEnabledFor(logging.DEBUG):
                 block.stdout_link(
                     self.output_logger.out(
                         block.string_id,
                         logger_base.bind(stdio="stdout"),
                     ),
@@ -626,15 +628,15 @@
             if block.consumer:
                 if idx != 0 and self.blocks[idx - 1].producer:
                     self.blocks[idx - 1].stdout_link(
                         block.stdin,
                     )  # link previous blocks stdout with current blocks stdin
                 else:
                     raise BlockSetValidationError(
-                        "run step requires input but has no upstream",
+                        "run step requires input but has no upstream",  # noqa: EM101
                     )
 
 
 class ELBExecutionManager:
     """Execution manager for ExtractLoadBlock sets."""
 
     def __init__(self, elb: ExtractLoadBlocks) -> None:
@@ -731,20 +733,21 @@
             if self.elb.head.proxy_stdout() == output_futures_failed:
                 handle_producer_line_length_limit_error(
                     output_futures_failed.exception(),
                     line_length_limit=self.line_length_limit,
                     stream_buffer_size=self.stream_buffer_size,
                 )
             raise output_futures_failed.exception()  # noqa: RSE102
-        else:
-            # If all the output handlers completed without raising an
-            # exception, we still need to wait for all the underlying block
-            # processes to complete. Note that since all output handlers
-            # completed we DO NOT need to wait for any output futures!
-            done = await self.elb.process_wait(None, start_idx)
+
+        # If all the output handlers completed without raising an
+        # exception, we still need to wait for all the underlying block
+        # processes to complete. Note that since all output handlers
+        # completed we DO NOT need to wait for any output futures!
+        done = await self.elb.process_wait(None, start_idx)
+
         if self.elb.tail.process_future.done():
             logger.debug("tail consumer completed first")
             self._consumer_code = self.elb.tail.process_future.result()
             await self._complete_upstream()
         elif current_head.process_future.done():
             logger.debug(
                 "head producer completed first as expected",
@@ -752,15 +755,15 @@
             )
             await self._handle_head_completed(current_head, start_idx)
         else:
             logger.warning("Intermediate block in sequence failed.")
             await self._stop_all_blocks(start_idx)
             raise RunnerError(
                 (
-                    "Unexpected completion sequence in ExtractLoadBlock set. "
+                    "Unexpected completion sequence in ExtractLoadBlock set. "  # noqa: EM101
                     "Intermediate block (likely a mapper) failed."
                 ),
                 {
                     PluginType.EXTRACTORS: 1,
                     PluginType.LOADERS: 1,
                 },
             )
@@ -771,17 +774,17 @@
         start_idx: int,
     ) -> None:
         next_head: IOBlock = self.elb.blocks[start_idx + 1]
 
         if current_head is self.elb.head:
             self._producer_code = current_head.process_future.result()
         else:
-            self._intermediate_codes[
-                current_head.string_id
-            ] = current_head.process_future.result()
+            self._intermediate_codes[current_head.string_id] = (
+                current_head.process_future.result()
+            )
 
         await asyncio.wait([current_head.proxy_stdout(), current_head.proxy_stderr()])
         # Close next inline stdin so downstream can cascade and complete naturally
         await next_head.close_stdin()
 
         if next_head is self.elb.tail:
             logger.debug("tail consumer is next block, wrapping up")
@@ -820,31 +823,31 @@
 
     Raises:
         RunnerError: if the producer, consumer, or mapper exit codes are non-zero
     """
     if producer_code:
         if consumer_code:
             raise RunnerError(
-                "Extractor and loader failed",
+                "Extractor and loader failed",  # noqa: EM101
                 {
                     PluginType.EXTRACTORS: producer_code,
                     PluginType.LOADERS: consumer_code,
                 },
             )
-        raise RunnerError("Extractor failed", {PluginType.EXTRACTORS: producer_code})
+        raise RunnerError("Extractor failed", {PluginType.EXTRACTORS: producer_code})  # noqa: EM101
 
     if consumer_code:
-        raise RunnerError("Loader failed", {PluginType.LOADERS: consumer_code})
+        raise RunnerError("Loader failed", {PluginType.LOADERS: consumer_code})  # noqa: EM101
 
     if failed_mappers := [
         {mapper_id: exit_code}
         for mapper_id, exit_code in intermediate_codes.items()
         if exit_code
     ]:
-        raise RunnerError("Mappers failed", failed_mappers)
+        raise RunnerError("Mappers failed", failed_mappers)  # noqa: EM101
 
 
 def generate_state_id(
     project: Project,
     state_id_suffix: str | None,
     consumer: IOBlock,
     producer: IOBlock,
@@ -861,23 +864,23 @@
         State id string.
 
     Raises:
         RunnerError: if the project does not have an active environment.
     """
     if not project.environment:
         raise RunnerError(
-            "No active environment for invocation, but requested state ID",
+            "No active environment for invocation, but requested state ID",  # noqa: EM101
         )
 
     state_id_components = [
         project.environment.name,
         f"{consumer.string_id}-to-{producer.string_id}",
         state_id_suffix or project.environment.state_id_suffix,
     ]
 
     if any(c for c in state_id_components if c and STATE_ID_COMPONENT_DELIMITER in c):
         raise RunnerError(
-            "Cannot generate a state ID from components containing the "
+            "Cannot generate a state ID from components containing the "  # noqa: EM102
             f"delimiter string '{STATE_ID_COMPONENT_DELIMITER}'",
         )
 
     return STATE_ID_COMPONENT_DELIMITER.join(c for c in state_id_components if c)
```

### Comparing `meltano-3.3.2/src/meltano/core/block/future_utils.py` & `meltano-3.4.0a1/src/meltano/core/block/future_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
     if exception_future in done:
         futures_done, _ = exception_future.result()
         if futures_failed := [
             future for future in futures_done if future.exception() is not None
         ]:
             return futures_failed.pop()
+    return None
 
 
 def handle_producer_line_length_limit_error(
     exception: Exception,
     line_length_limit: int,
     stream_buffer_size: int,
 ):
@@ -70,8 +71,8 @@
         "setting to at least double the size of the largest expected message, "
         "and try again.",
     )
     logging.error(
         "To learn more, visit "
         "https://docs.meltano.com/reference/settings#eltbuffer_size",
     )
-    raise RunnerError("Output line length limit exceeded") from exception
+    raise RunnerError("Output line length limit exceeded") from exception  # noqa: EM101
```

### Comparing `meltano-3.3.2/src/meltano/core/block/ioblock.py` & `meltano-3.4.0a1/src/meltano/core/block/ioblock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/block/parser.py` & `meltano-3.4.0a1/src/meltano/core/block/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,19 +115,19 @@
             except ValueError:
                 parsed_name = name
                 command_name = None
 
             try:
                 plugin = self.project.plugins.find_plugin(parsed_name)
             except PluginNotFoundError as e:
-                raise click.ClickException(f"Block {name} not found") from e
+                raise click.ClickException(f"Block {name} not found") from e  # noqa: EM102
 
             if plugin and task_sets_service.exists(name):
                 raise click.ClickException(
-                    f"Ambiguous reference to '{name}' which matches a job "
+                    f"Ambiguous reference to '{name}' which matches a job "  # noqa: EM102
                     "name AND a plugin name.",
                 )
 
             if plugin.type == PluginType.MAPPERS:
                 self._mappings_ref[idx] = parsed_name
 
             self._plugins.append(plugin)
@@ -212,15 +212,15 @@
                     self._plugins[cur],
                     self.project,
                     command=self._commands.get(cur),
                 )
                 cur += 1
             else:
                 raise BlockSetValidationError(
-                    "Unknown command type or bad block sequence at index "
+                    "Unknown command type or bad block sequence at index "  # noqa: EM102
                     f"{cur + 1}, starting block '{plugin.name}'",  # noqa: WPS237
                 )
 
     def _find_next_elb_set(  # noqa: WPS231, WPS213
         self,
         offset: int = 0,
     ) -> tuple[ExtractLoadBlocks | None, int]:  # noqa: WPS231, WPS213
@@ -252,15 +252,15 @@
                 offset=offset,
                 plugin_type=self._plugins[offset].type,
             )
             return None, offset
 
         self.log.debug(
             "head of set is extractor as expected",
-            block=self._plugins[offset],
+            block=self._plugins[offset].name,
         )
 
         blocks.append(builder.make_block(self._plugins[offset]))
 
         for idx, plugin in enumerate(self._plugins[offset + 1 :]):  # noqa: E203
             next_block = idx + 1
 
@@ -290,27 +290,27 @@
                 # to stop errors due to ambiguous commands.
                 if plugin.name == self._mappings_ref.get(next_block):
                     self.log.warning(
                         "Found unexpected mapper plugin name. ",
                         plugin_name=plugin.name,
                     )
                     raise BlockSetValidationError(
-                        f"Expected unique mappings name not the mapper plugin "
+                        f"Expected unique mappings name not the mapper plugin "  # noqa: EM102
                         f"name: {plugin.name}.",
                     )
-                else:
-                    blocks.append(builder.make_block(plugin))
+                blocks.append(builder.make_block(plugin))
+
             elif plugin.type == PluginType.LOADERS:
                 self.log.debug("blocks", offset=offset, idx=next_block)
                 blocks.append(builder.make_block(plugin))
                 elb = ExtractLoadBlocks(builder.context(), blocks)
                 return elb, idx + 2
             else:
                 self.log.warning(
                     "Found unexpected plugin type for block in middle of block set.",
                     plugin_type=plugin.type,
                     plugin_name=plugin.name,
                 )
                 raise BlockSetValidationError(
-                    f"Expected {PluginType.MAPPERS} or {PluginType.LOADERS}.",
+                    f"Expected {PluginType.MAPPERS} or {PluginType.LOADERS}.",  # noqa: EM102
                 )
-        raise BlockSetValidationError("Found no end in block set!")
+        raise BlockSetValidationError("Found no end in block set!")  # noqa: EM101
```

### Comparing `meltano-3.3.2/src/meltano/core/block/plugin_command.py` & `meltano-3.4.0a1/src/meltano/core/block/plugin_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                     return_when=asyncio.ALL_COMPLETED,
                 )
         finally:
             self.context.session.close()
         if exitcode := self.process_future.result():
             command = self.command or self.command_args[0]
             raise RunnerError(
-                f"`{self.name} {command}` failed with exit code: {exitcode}",
+                f"`{self.name} {command}` failed with exit code: {exitcode}",  # noqa: EM102
             )
 
 
 def plugin_command_invoker(
     plugin: ProjectPlugin,
     project: Project,
     command: str | None,
```

### Comparing `meltano-3.3.2/src/meltano/core/block/singer.py` & `meltano-3.4.0a1/src/meltano/core/block/singer.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 *args,
                 command=self.command,
                 **kwargs,
                 stdout=asyncio.subprocess.PIPE,
                 stderr=asyncio.subprocess.PIPE,
             )
         except Exception as err:
-            raise RunnerError(f"Cannot start plugin: {err}") from err
+            raise RunnerError(f"Cannot start plugin: {err}") from err  # noqa: EM102
 
     async def stop(self, kill: bool = True):
         """Stop (kill) the underlying process and cancel output proxying.
 
         Args:
             kill: whether to send a SIGKILL. If false, a SIGTERM is sent.
         """
@@ -129,15 +129,15 @@
             The stdout proxy future.
 
         Raises:
             IOLinkError: If the processes is not running and so there is no IO
                 to proxy.
         """
         if self.process_handle is None:
-            raise IOLinkError("No IO to proxy, process not running")
+            raise IOLinkError("No IO to proxy, process not running")  # noqa: EM101
 
         if self._stdout_future is None:
             outputs = self._merge_outputs(self.invoker.StdioSource.STDOUT, self.outputs)
             self._stdout_future = asyncio.ensure_future(
                 # forward subproc stdout to downstream (i.e. targets stdin, loggers)
                 capture_subprocess_output(self.process_handle.stdout, *outputs),
             )
@@ -150,15 +150,15 @@
             The stderr proxy future.
 
         Raises:
             IOLinkError: If the processes is not running and so there is no IO
                 to proxy.
         """
         if self.process_handle is None:
-            raise IOLinkError("No IO to proxy, process not running")
+            raise IOLinkError("No IO to proxy, process not running")  # noqa: EM101
 
         if self._stderr_future is None:
             err_outputs = self._merge_outputs(
                 self.invoker.StdioSource.STDERR,
                 self.err_outputs,
             )
             self._stderr_future = asyncio.ensure_future(
@@ -183,15 +183,15 @@
 
         Raises:
             ProcessWaitError: If the process is not running.
         """
         if self._process_future is None:
             if self.process_handle is None:
                 raise ProcessWaitError(
-                    "No process to wait, process not running running",
+                    "No process to wait, process not running running",  # noqa: EM101
                 )
             self._process_future = asyncio.ensure_future(self.process_handle.wait())
         return self._process_future
 
     @property
     def stdin(self) -> asyncio.StreamWriter | None:
         """Return stdin of the underlying process.
@@ -201,44 +201,43 @@
         """
         return None if self.process_handle is None else self.process_handle.stdin
 
     async def close_stdin(self) -> None:
         """Close the underlying process stdin if the block is a consumer."""
         if self.consumer:
             self.process_handle.stdin.close()
-            with suppress(AttributeError):  # `wait_closed` is Python 3.8+ (see #3347)
-                await self.process_handle.stdin.wait_closed()
+            await self.process_handle.stdin.wait_closed()
 
     def stdout_link(self, dst: SubprocessOutputWriter) -> None:
         """Use stdout_link to instruct block to link/write stdout content to dst.
 
         Args:
             dst:  The destination stdout output should be written too.
 
         Raises:
             IOLinkError: If the IO is already in flight.
         """
         if self._stdout_future is None:
             self.outputs.append(dst)
         else:
-            raise IOLinkError("IO capture already in flight")
+            raise IOLinkError("IO capture already in flight")  # noqa: EM101
 
     def stderr_link(self, dst: SubprocessOutputWriter):
         """Use stderr_link to instruct block to link/write stderr content to dst.
 
         Args:
             dst:  The destination stderr output should be written too.
 
         Raises:
             IOLinkError: If the IO is already in flight.
         """
         if self._stderr_future is None:
             self.err_outputs.append(dst)
         else:
-            raise IOLinkError("IO capture already in flight")
+            raise IOLinkError("IO capture already in flight")  # noqa: EM101
 
     async def pre(self, context) -> None:
         """Pre triggers preparation of the underlying plugin.
 
         Args:
             context: The context with which to update the invoker
         """
@@ -332,15 +331,15 @@
             self.process_handle = await self.invoker.invoke_async(
                 limit=line_length_limit,
                 stdin=stdin,  # Singer messages
                 stdout=asyncio.subprocess.PIPE,  # Singer state
                 stderr=asyncio.subprocess.PIPE,  # Log
             )
         except Exception as err:
-            raise RunnerError(f"Cannot start plugin {self.string_id}: {err}") from err
+            raise RunnerError(f"Cannot start plugin {self.string_id}: {err}") from err  # noqa: EM102
 
     async def stop(self, kill: bool = True):
         """Stop (kill) the underlying process and cancel output proxying.
 
         Args:
             kill: Whether to send a SIGKILL. If false, a SIGTERM is sent.
         """
```

### Comparing `meltano-3.3.2/src/meltano/core/bundle/settings.yml` & `meltano-3.4.0a1/src/meltano/core/bundle/settings.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/cli_messages.py` & `meltano-3.4.0a1/src/meltano/core/cli_messages.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/config_service.py` & `meltano-3.4.0a1/src/meltano/core/config_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/container/container_service.py` & `meltano-3.4.0a1/src/meltano/core/container/container_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/container/container_spec.py` & `meltano-3.4.0a1/src/meltano/core/container/container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/db.py` & `meltano-3.4.0a1/src/meltano/core/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         Exception: The init hook raised an exception.
     """
     if hook := init_hooks.get(engine.dialect.name):
         with engine.connect() as conn:
             try:
                 hook(conn)
             except Exception as ex:
-                raise Exception(f"Failed to initialize database: {ex!s}") from ex
+                raise Exception(f"Failed to initialize database: {ex!s}") from ex  # noqa: EM102
 
 
 def ensure_schema_exists(
     engine: Engine,
     schema_name: str,
     grant_roles: tuple[str] = (),
 ) -> None:
```

### Comparing `meltano-3.3.2/src/meltano/core/elt_context.py` & `meltano-3.4.0a1/src/meltano/core/elt_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     @property
     def elt_run_dir(self):
         """Get the ELT run directory.
 
         Returns:
             The job dir, if a Job is provided, else None.
         """
-        if self.job:
+        if self.job:  # noqa: RET503
             return self.project.job_dir(self.job.job_name, str(self.job.run_id))
 
     def invoker_for(self, plugin_type: PluginType) -> PluginInvoker:
         """Get invoker for given plugin type.
 
         Args:
             plugin_type: Plugin type to get invoker for.
@@ -414,15 +414,15 @@
             PluginNotFoundError: if a plugin specified cannot be found.
         """
         try:
             plugin = self.project.plugins.get_plugin(plugin_ref)
         except PluginNotFoundError as err:
             if plugin_ref.name == "dbt":
                 raise PluginNotFoundError(
-                    "Transformer 'dbt' not found.\n"
+                    "Transformer 'dbt' not found.\n"  # noqa: EM101
                     "Use of the legacy 'dbt' Transformer is deprecated in favor of "
                     "new adapter specific implementations (e.g. 'dbt-snowflake') "
                     "compatible with the 'meltano run ...' command.\n"
                     "https://docs.meltano.com/guide/transformation\n"
                     "To continue using the legacy 'dbt' Transformer, "
                     "add it to your Project using 'meltano add transformer dbt'.",
                 ) from err
```

### Comparing `meltano-3.3.2/src/meltano/core/environment.py` & `meltano-3.4.0a1/src/meltano/core/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/environment_service.py` & `meltano-3.4.0a1/src/meltano/core/environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/error.py` & `meltano-3.4.0a1/src/meltano/core/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         super().__init__(message)
 
     @property
     async def stderr(self) -> str | None:
         """Return the output of the process to stderr."""
         if not self._stderr:  # noqa: DAR201
             return None
-        elif not isinstance(self._stderr, str):
+        if not isinstance(self._stderr, str):
             stream = await self._stderr.read()
             self._stderr = stream.decode("utf-8")
 
         return self._stderr
 
 
 class PluginInstallError(Exception):
@@ -108,15 +108,15 @@
         """Instantiate the error."""
         reason = "Your meltano.yml file is empty"
         instruction = "Please update your meltano file with a valid configuration"
         super().__init__(reason, instruction)
 
 
 class MeltanoConfigurationError(MeltanoError):
-    """Exception for when Meltano is inproperly configured."""
+    """Exception for when Meltano is improperly configured."""
 
 
 class ProjectNotFound(Error):
     """A Project is instantiated outside of a meltano project structure."""
 
     def __init__(self, project: Project):
         """Instantiate the error.
```

### Comparing `meltano-3.3.2/src/meltano/core/hub/client.py` & `meltano-3.4.0a1/src/meltano/core/hub/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
             None,
             None,
         )
 
         try:
             return self.session.send(prep, **settings)
         except requests.exceptions.ConnectionError as connection_err:
-            raise HubConnectionError("Could not reach Meltano Hub.") from connection_err
+            raise HubConnectionError("Could not reach Meltano Hub.") from connection_err  # noqa: EM101
 
     def find_definition(
         self,
         plugin_type: PluginType,
         plugin_name: str,
         variant_name: str | None = None,
     ) -> PluginDefinition:
```

### Comparing `meltano-3.3.2/src/meltano/core/hub/schema.py` & `meltano-3.4.0a1/src/meltano/core/hub/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/job/finder.py` & `meltano-3.4.0a1/src/meltano/core/job/finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/job/job.py` & `meltano-3.4.0a1/src/meltano/core/job/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defines Job model class."""
+
 from __future__ import annotations
 
 import asyncio
 import os
 import signal
 import typing as t
 import uuid
```

### Comparing `meltano-3.3.2/src/meltano/core/job/stale_job_failer.py` & `meltano-3.4.0a1/src/meltano/core/job/stale_job_failer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/job_state.py` & `meltano-3.4.0a1/src/meltano/core/job_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defines JobState model class."""
+
 from __future__ import annotations
 
 import json
 import typing as t
 from datetime import datetime
 
 from sqlalchemy.orm import Mapped, Session, mapped_column
```

### Comparing `meltano-3.3.2/src/meltano/core/locked_definition_service.py` & `meltano-3.4.0a1/src/meltano/core/locked_definition_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,19 @@
 
         Returns:
             The plugin definition.
 
         Raises:
             PluginNotFoundError: If the plugin definition could not be found.
         """
-        path = self.project.plugin_lock_path(plugin_type, plugin_name, variant_name)
+        path = self.project.plugin_lock_path(
+            plugin_type,
+            plugin_name,
+            variant_name=variant_name,
+        )
         try:
             standalone = StandalonePlugin.parse_json_file(path)
         except FileNotFoundError as err:
             raise PluginNotFoundError(PluginRef(plugin_type, plugin_name)) from err
         return PluginDefinition.from_standalone(standalone)
 
     def find_base_plugin(
```

### Comparing `meltano-3.3.2/src/meltano/core/logging/__init__.py` & `meltano-3.4.0a1/src/meltano/core/logging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Logging and log related utilities."""
+
 from __future__ import annotations
 
 from .formatters import console_log_formatter, json_formatter, key_value_formatter
 from .job_logging_service import (
     JobLoggingService,
     MissingJobLogException,
     SizeThresholdJobLogException,
```

### Comparing `meltano-3.3.2/src/meltano/core/logging/formatters.py` & `meltano-3.4.0a1/src/meltano/core/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/logging/job_logging_service.py` & `meltano-3.4.0a1/src/meltano/core/logging/job_logging_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os
 import typing as t
 from contextlib import contextmanager
 
 from meltano.core.utils import makedirs, slugify
 
 if t.TYPE_CHECKING:
+    from pathlib import Path
+
     from meltano.core.project import Project
 
 MAX_FILE_SIZE = 2097152  # 2MB max
 
 
 class MissingJobLogException(Exception):
     """Occurs when `JobLoggingService` can not find a requested log."""
@@ -22,24 +24,43 @@
 
 
 class JobLoggingService:
     def __init__(self, project: Project):
         self.project = project
 
     @makedirs
-    def logs_dir(self, state_id, *joinpaths):
-        return self.project.job_logs_dir(state_id, *joinpaths)
+    def logs_dir(self, state_id, *joinpaths, make_dirs: bool = True):  # noqa: ARG002
+        """Return the logs directory for a given state_id.
+
+        Args:
+            state_id: The state ID for the logs.
+            joinpaths: Additional paths to join to the logs directory.
+            make_dirs: Whether to create the directory if it does not exist.
+
+        Returns:
+            The logs directory for the given state ID.
+        """
+        return self.project.job_logs_dir(state_id, *joinpaths, make_dirs=make_dirs)
 
     def generate_log_name(
         self,
         state_id: str,
         run_id: str,
         file_name: str = "elt.log",
-    ) -> str:
-        """Generate an internal etl log path and name."""
+    ) -> Path:
+        """Generate an internal etl log path and name.
+
+        Args:
+            state_id: The state ID for the log.
+            run_id: The run ID for the log.
+            file_name: The name of the log file.
+
+        Returns:
+            The full path to the log file.
+        """
         return self.logs_dir(state_id, str(run_id), file_name)
 
     @contextmanager
     def create_log(self, state_id, run_id, file_name="elt.log"):
         """Open a new log file for logging and yield it.
 
         Log will be created inside the logs_dir, which is
@@ -48,17 +69,17 @@
         log_file_name = self.generate_log_name(state_id, run_id, file_name)
 
         try:
             with open(log_file_name, "w") as log_file:
                 yield log_file
         except OSError:
             # Don't stop the Job running if you can not open the log file
-            # for writting: just return /dev/null
+            # for writing: just return /dev/null
             logging.error(
-                f"Could open log file {log_file_name!r} for writting. "  # noqa: G004
+                f"Could open log file {log_file_name!r} for writing. "  # noqa: G004
                 "Using `/dev/null`",
             )
             with open(os.devnull, "w") as log_file:
                 yield log_file
 
     def get_latest_log(self, state_id) -> str:
         """Get the latest log.
@@ -71,40 +92,40 @@
             the provided `state_id`.
         """  # noqa: DAR301, DAR401
         try:
             latest_log = next(iter(self.get_all_logs(state_id)))
 
             if latest_log.stat().st_size > MAX_FILE_SIZE:
                 raise SizeThresholdJobLogException(
-                    f"The log file size exceeds '{MAX_FILE_SIZE}'",
+                    f"The log file size exceeds '{MAX_FILE_SIZE}'",  # noqa: EM102
                 )
 
             with latest_log.open() as f:
                 return f.read()
         except StopIteration:
             raise MissingJobLogException(
-                f"Could not find any log for job with ID '{state_id}'",
+                f"Could not find any log for job with ID '{state_id}'",  # noqa: EM102
             ) from None
         except FileNotFoundError as ex:
             raise MissingJobLogException(
-                f"Cannot log for job with ID '{state_id}': '{latest_log}' is missing.",
+                f"Cannot log for job with ID '{state_id}': '{latest_log}' is missing.",  # noqa: EM102
             ) from ex
 
     def get_downloadable_log(self, state_id):
         """Get the `*.log` file of the most recent log for any ELT job that ran with the provided `state_id`."""  # noqa: E501, DAR101, DAR201, DAR401
         try:
             latest_log = next(iter(self.get_all_logs(state_id)))
             return str(latest_log.resolve())
         except StopIteration:
             raise MissingJobLogException(
-                f"Could not find any log for job with ID '{state_id}'",
+                f"Could not find any log for job with ID '{state_id}'",  # noqa: EM102
             ) from None
         except FileNotFoundError as ex:
             raise MissingJobLogException(
-                f"Cannot log for job with ID '{state_id}': '{latest_log}' is missing.",
+                f"Cannot log for job with ID '{state_id}': '{latest_log}' is missing.",  # noqa: EM102
             ) from ex
 
     def get_all_logs(self, state_id):
         """Get all the log files for any ELT job that ran with the provided `state_id`.
 
         The result is ordered so that the most recent is first on the list.
         """
```

### Comparing `meltano-3.3.2/src/meltano/core/logging/output_logger.py` & `meltano-3.4.0a1/src/meltano/core/logging/output_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Output Logger."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import os
 import sys
 from contextlib import (
```

### Comparing `meltano-3.3.2/src/meltano/core/logging/utils.py` & `meltano-3.4.0a1/src/meltano/core/logging/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,22 +131,15 @@
     """Configure logging for a meltano project.
 
     Args:
         project: the meltano project
         log_level: set log levels to provided level.
         log_config: a logging config suitable for use with `logging.config.dictConfig`.
     """
-    # Mimick Python 3.8's `force=True` kwarg to override any
-    # existing logger handlers
-    # See https://github.com/python/cpython/commit/cf67d6a934b51b1f97e72945b596477b271f70b8
-    root = logging.getLogger()
-    for handler in root.handlers[:]:
-        root.removeHandler(handler)
-        handler.close()
-
+    logging.basicConfig(force=True)
     log_level = log_level.upper()
 
     if project:
         log_config = log_config or project.settings.get("cli.log_config")
         log_level = project.settings.get("cli.log_level")
 
     config = read_config(log_config) or default_config(log_level)
```

### Comparing `meltano-3.3.2/src/meltano/core/manifest/__init__.py` & `meltano-3.4.0a1/src/meltano/core/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/manifest/contexts.py` & `meltano-3.4.0a1/src/meltano/core/manifest/contexts.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 _active_manifest: list[Manifest] = []
 
 
 def _get_active_manifest() -> Manifest:
     try:
         return _active_manifest[-1]
     except IndexError:
-        raise Exception("No manifest has been activated") from None
+        raise Exception("No manifest has been activated") from None  # noqa: EM101
 
 
 @contextmanager
 def _manifest_context(manifest: Manifest) -> t.Iterator[None]:
     _active_manifest.append(manifest)
     try:
         yield
@@ -96,15 +96,15 @@
         plugin = next(
             x
             for v in manifest.data["plugins"].values()
             for x in v
             if x["name"] == plugin_name
         )
     except StopIteration:
-        raise ValueError(f"Plugin {plugin_name!r} not found in manifest") from None
+        raise ValueError(f"Plugin {plugin_name!r} not found in manifest") from None  # noqa: EM102
 
     with _env_context(plugin["env"]):
         yield
 
 
 @contextmanager
 def schedule_context(schedule_name: str) -> t.Iterator[None]:
@@ -124,15 +124,15 @@
         `None`.
     """
     schedules = _get_active_manifest().data["schedules"]
 
     try:
         schedule = next(x for x in schedules if x["name"] == schedule_name)
     except StopIteration:
-        raise ValueError(f"Schedule {schedule!r} not found in manifest") from None
+        raise ValueError(f"Schedule {schedule!r} not found in manifest") from None  # noqa: EM102
 
     with _env_context(schedule["env"]):
         yield
 
 
 @contextmanager
 def job_context(job_name: str) -> t.Iterator[None]:
@@ -152,15 +152,15 @@
         `None`.
     """
     jobs = _get_active_manifest().data["jobs"]
 
     try:
         job = next(x for x in jobs if x["name"] == job_name)
     except StopIteration:
-        raise ValueError(f"Job {job!r} not found in manifest") from None
+        raise ValueError(f"Job {job!r} not found in manifest") from None  # noqa: EM102
 
     with _env_context(job["env"]):
         yield
 
 
 # TODO: Provide a function which returns `_get_active_manifest().data` with
 # env vars injected into each of its string fields, taking only from
```

### Comparing `meltano-3.3.2/src/meltano/core/manifest/jsonschema.py` & `meltano-3.4.0a1/src/meltano/core/manifest/jsonschema.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,30 +95,30 @@
         """
         with suppress(KeyError):
             return self._resolved_refs[ref]
 
         location_as_ref = self.path_to_ref(path)
         if location_as_ref.startswith(ref):
             raise RecursionError(
-                "Cannot resolve recursive jsonschema "
+                "Cannot resolve recursive jsonschema "  # noqa: EM102
                 f"ref {ref!r} at {location_as_ref!r}",
             )
 
         current_schema = self.root_schema
         parts = ref.split("/")
 
         if parts[0] != "#":
-            raise ValueError("Cannot resolve non-local jsonschema ref")
+            raise ValueError("Cannot resolve non-local jsonschema ref")  # noqa: EM101
 
         for key in parts[1:]:
             try:
                 current_schema = current_schema[key]
             except KeyError as ex:
                 raise KeyError(
-                    f"Unable to resolve local jsonschema ref {ref!r} at level {key!r}",
+                    f"Unable to resolve local jsonschema ref {ref!r} at level {key!r}",  # noqa: EM102
                 ) from ex
         return current_schema
 
     @staticmethod
     def path_to_ref(path: tuple[str, ...]) -> str:
         """Convert a sequence of jq filters into a jsonschema ref.
```

### Comparing `meltano-3.3.2/src/meltano/core/manifest/manifest.py` & `meltano-3.4.0a1/src/meltano/core/manifest/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Compile a Meltano manifest."""
 
-
 from __future__ import annotations
 
 import json
 import re
 import subprocess
 import typing as t
 from collections import defaultdict
@@ -231,15 +230,15 @@
             _plugins_by_name_by_type(manifest["plugins"]),
             _plugins_by_name_by_type(locked_plugins),
         )
 
     def sanitize_env_vars(self, env: t.Mapping[str, str]) -> dict[str, str]:
         """Sanitize environment variables.
 
-        Sanitization is perfomed by:
+        Sanitization is performed by:
         - Replacing the project root as an absolute path in values with
             '${MELTANO_PROJECT_ROOT}'
 
         Args:
             env: A mapping of environment variables.
 
         Returns:
@@ -267,15 +266,15 @@
             _: Merge strategies - unused argument.
 
         Returns:
             `NotImplemented` if the key is not "env"; `None` otherwise.
         """
         if key != "env":
             return NotImplemented  # type: ignore
-        data[key] = self.sanitize_env_vars(
+        data[key] = self.sanitize_env_vars(  # noqa: RET503
             {
                 **expand_env_vars(
                     data[key],
                     value,
                     if_missing=EnvVarMissingBehavior.ignore,
                 ),
                 **expand_env_vars(
@@ -452,27 +451,27 @@
     trie: Trie,
     manifest_component: dict[str, t.Any] | list[t.Any],
 ) -> None:
     for key, sub_trie in trie.items():
         if key == "[]":
             if not isinstance(manifest_component, list):
                 raise TypeError(
-                    "Expected list during manifest scaffolding, "
+                    "Expected list during manifest scaffolding, "  # noqa: EM102
                     f"got {type(manifest_component)}",
                 )
             for element in manifest_component:
                 _apply_scaffold(sub_trie, element)
         elif isinstance(manifest_component, dict):
             _apply_scaffold(
                 sub_trie,
                 manifest_component.setdefault(key, [] if "[]" in sub_trie else {}),
             )
         else:
             raise TypeError(
-                "Expected dict during manifest scaffolding, "
+                "Expected dict during manifest scaffolding, "  # noqa: EM102
                 f"got {type(manifest_component)}",
             )
 
 
 def apply_scaffold(manifest: dict[str, t.Any], locations: Iterable[str]) -> None:
     """Update the provided manifest dict with dicts/lists at the provided locations.
```

### Comparing `meltano-3.3.2/src/meltano/core/meltano_file.py` & `meltano-3.4.0a1/src/meltano/core/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/meltano_invoker.py` & `meltano-3.4.0a1/src/meltano/core/meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/migration_service.py` & `meltano-3.4.0a1/src/meltano/core/migration_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,18 +97,18 @@
                     click.secho(f"Upgrading database to {head}")
                 command.upgrade(cfg, head)
 
                 if silent:
                     migration_logger.setLevel(original_log_level)
             except FileNotFoundError as ex:
                 raise MigrationError(
-                    "Cannot upgrade the system database, revision lock not found.",
+                    "Cannot upgrade the system database, revision lock not found.",  # noqa: EM101
                 ) from ex
             except MigrationUneededException:
                 if not silent:
                     click.secho("System database up-to-date.")
             except Exception as ex:
                 logging.exception(str(ex))
                 raise MigrationError(
-                    "Cannot upgrade the system database. It might be corrupted or "
+                    "Cannot upgrade the system database. It might be corrupted or "  # noqa: EM101
                     "was created before database migrations where introduced (v0.34.0)",
                 ) from ex
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin/airflow.py` & `meltano-3.4.0a1/src/meltano/core/plugin/airflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Plugin glue code for Airflow."""
+
 from __future__ import annotations
 
 import configparser
 import logging
 import os
 import subprocess
 from contextlib import suppress
@@ -118,15 +119,15 @@
             stdout=subprocess.DEVNULL,
             stderr=subprocess.PIPE,
         )
         exit_code = await handle.wait()
 
         if exit_code:
             raise AsyncSubprocessError(
-                "Command `airflow --help` failed",
+                "Command `airflow --help` failed",  # noqa: EM101
                 process=handle,
             )
 
         # Read and update airflow.cfg
         self.update_config_file(invoker)
 
         # we've changed the configuration here, so we need to call
@@ -141,15 +142,15 @@
             stderr=subprocess.PIPE,
         )
 
         stdout, stderr = await handle.communicate()
 
         if handle.returncode:
             raise AsyncSubprocessError(
-                "Command `airflow version` failed",
+                "Command `airflow version` failed",  # noqa: EM101
                 process=handle,
             )
 
         version = stdout.decode()
         init_db_cmd = (
             ["initdb"] if Version(version) < Version("2.0.0") else ["db", "init"]
         )
@@ -160,15 +161,15 @@
             stderr=subprocess.PIPE,
         )
         exit_code = await handle.wait()
 
         if exit_code:
             raise AsyncSubprocessError(
                 (
-                    "Airflow metadata database could not be initialized: "
+                    "Airflow metadata database could not be initialized: "  # noqa: EM101
                     "`airflow initdb` failed"
                 ),
                 handle,
             )
 
         logging.debug("Completed `airflow initdb`")
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin/base.py` & `meltano-3.4.0a1/src/meltano/core/plugin/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         Raises:
             ValueError: If the plugin type does not exist.
         """
         for plugin_type in cls:
             if value in {plugin_type.value, plugin_type.singular}:
                 return plugin_type
 
-        raise ValueError(f"{value!r} is not a valid {cls.__name__}")
+        raise ValueError(f"{value!r} is not a valid {cls.__name__}")  # noqa: EM102
 
     @classmethod
     def plurals(cls) -> list[str]:
         """Return the list of plugin plural names.
 
         Returns:
             The list of plugin plurals.
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin/command.py` & `meltano-3.4.0a1/src/meltano/core/plugin/command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/config_service.py` & `meltano-3.4.0a1/src/meltano/core/plugin/config_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/dbt/base.py` & `meltano-3.4.0a1/src/meltano/core/plugin/dbt/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Defines DBT-specific plugins."""
+
 from __future__ import annotations
 
 import logging
 import typing as t
 from pathlib import Path
 
 from meltano.core.error import PluginInstallError
@@ -77,21 +78,21 @@
         dbt_project_path = transform_add_service.dbt_project_file.relative_to(
             project.root,
         )
         logger.info(f"Adding dbt model to '{dbt_project_path}'...")  # noqa: G004
         transform_add_service.update_dbt_project(plugin)
     except PluginNotFoundError as ex:
         raise PluginInstallError(
-            "Transformer 'dbt' is not installed. "
+            "Transformer 'dbt' is not installed. "  # noqa: EM101
             "Run `meltano add transformer dbt` to add it to your project.",
         ) from ex
     except FileNotFoundError as ex:
         relative_path = Path(ex.filename).relative_to(project.root)
         raise PluginInstallError(
-            f"File '{relative_path}' could not be found. "
+            f"File '{relative_path}' could not be found. "  # noqa: EM102
             "Run `meltano add files files-dbt` to set up a dbt project.",
         ) from ex
 
 
 class DbtTransformPlugin(BasePlugin):
     """Plugin type for dbt transforms."""
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin/error.py` & `meltano-3.4.0a1/src/meltano/core/plugin/error.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/factory.py` & `meltano-3.4.0a1/src/meltano/core/plugin/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Factory for creating plugins."""
+
 from __future__ import annotations
 
 import importlib
 
 from . import BasePlugin, PluginDefinition, PluginType, Variant
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin/file.py` & `meltano-3.4.0a1/src/meltano/core/plugin/file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/meltano_file.py` & `meltano-3.4.0a1/src/meltano/core/plugin/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/project_plugin.py` & `meltano-3.4.0a1/src/meltano/core/plugin/project_plugin.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/requirements.py` & `meltano-3.4.0a1/src/meltano/core/plugin/requirements.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/settings_service.py` & `meltano-3.4.0a1/src/meltano/core/plugin/settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/singer/base.py` & `meltano-3.4.0a1/src/meltano/core/plugin/singer/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/singer/catalog.py` & `meltano-3.4.0a1/src/meltano/core/plugin/singer/catalog.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/singer/mapper.py` & `meltano-3.4.0a1/src/meltano/core/plugin/singer/mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,10 +67,10 @@
             plugin_name=invoker.plugin.name,
             mapping_name=invoker.plugin_config_extras["_mapping_name"],
             mapping_config=config_payload,
         )
 
     @staticmethod
     def _get_mapping_config(extra_config: dict) -> dict | None:
-        for mapping in extra_config.get("_mappings", []):
+        for mapping in extra_config.get("_mappings", []):  # noqa: RET503
             if mapping.get("name") == extra_config.get("_mapping_name"):
                 return mapping["config"]
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin/singer/tap.py` & `meltano-3.4.0a1/src/meltano/core/plugin/singer/tap.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,15 @@
         Raises:
             PluginExecutionError: if state could not be found for this plugin
             PluginLacksCapabilityError: if this plugin does not support
                 incremental state
         """
         if "state" not in plugin_invoker.capabilities:
             raise PluginLacksCapabilityError(
-                f"Extractor '{self.name}' does not support incremental state",
+                f"Extractor '{self.name}' does not support incremental state",  # noqa: EM102
             )
 
         state_path = plugin_invoker.files["state"]
 
         with suppress(FileNotFoundError):
             # Delete state left over from different pipeline run for same extractor
             state_path.unlink()
@@ -305,15 +305,15 @@
             )
 
             try:
                 shutil.copy(custom_state_path, state_path)
                 logger.info(f"Found state in {custom_state_filename}")  # noqa: G004
             except FileNotFoundError as err:
                 raise PluginExecutionError(
-                    f"Could not find state file {custom_state_path}",
+                    f"Could not find state file {custom_state_path}",  # noqa: EM102
                 ) from err
 
             return
         # the `state.json` is stored in the database
         if state := StateService(
             project=elt_context.project,
             session=elt_context.session,
@@ -383,28 +383,28 @@
             )
 
             try:
                 shutil.copy(custom_catalog_path, catalog_path)
                 logger.info(f"Found catalog in {custom_catalog_path}")  # noqa: G004
             except FileNotFoundError as err:
                 raise PluginExecutionError(
-                    f"Could not find catalog file {custom_catalog_path}",
+                    f"Could not find catalog file {custom_catalog_path}",  # noqa: EM102
                 ) from err
         else:
             await self.run_discovery(plugin_invoker, catalog_path)
 
         # test for the result to be a valid catalog
         try:
             with catalog_path.open("r") as catalog_file:
                 catalog = json.load(catalog_file)
                 Draft4Validator.check_schema(catalog)
         except Exception as err:
             catalog_path.unlink()
             raise PluginExecutionError(
-                f"Catalog discovery failed: invalid catalog: {err}",
+                f"Catalog discovery failed: invalid catalog: {err}",  # noqa: EM102
             ) from err
 
     async def run_discovery(  # noqa: WPS238, WPS210
         self,
         plugin_invoker: PluginInvoker,
         catalog_path: Path,
     ):  # noqa: DAR401
@@ -418,15 +418,15 @@
             PluginExecutionError: if state could not be found for this plugin.
             PluginLacksCapabilityError: if this plugin does not support
                 incremental state.
             Exception: if any other exception occurs.
         """
         if "discover" not in plugin_invoker.capabilities:
             raise PluginLacksCapabilityError(
-                f"Extractor '{self.name}' does not support catalog discovery "
+                f"Extractor '{self.name}' does not support catalog discovery "  # noqa: EM102
                 "(the `discover` capability is not advertised)",
             )
         with StringIO("") as stderr_buff:
             try:
                 with catalog_path.open(mode="wb") as catalog:
                     handle = await plugin_invoker.invoke_async(
                         "--discover",
@@ -472,15 +472,15 @@
                 catalog_path.unlink()
                 raise
 
             if exit_code != 0:
                 catalog_path.unlink()
                 stderr_buff.seek(0)
                 raise PluginExecutionError(
-                    "Catalog discovery failed: command "
+                    "Catalog discovery failed: command "  # noqa: EM102
                     f"{plugin_invoker.exec_args('--discover')} returned "
                     f"{exit_code} with stderr:\n {stderr_buff.read()}",
                 )
 
     @hook("before_invoke")
     async def apply_catalog_rules_hook(
         self,
@@ -522,15 +522,15 @@
             PluginExecutionError: if catalog rules could not be applied
         """
         if (
             "catalog" not in plugin_invoker.capabilities
             and "properties" not in plugin_invoker.capabilities
         ):
             raise PluginLacksCapabilityError(
-                f"Extractor '{self.name}' does not support entity selection "
+                f"Extractor '{self.name}' does not support entity selection "  # noqa: EM102
                 "or catalog metadata and schema rules",
             )
 
         config = plugin_invoker.plugin_config_extras
 
         schema_rules = []
         metadata_rules = []
@@ -569,20 +569,20 @@
             if cache_key := self.catalog_cache_key(plugin_invoker):
                 catalog_cache_key_path.write_text(cache_key)
             else:
                 with suppress(FileNotFoundError):
                     catalog_cache_key_path.unlink()
         except FileNotFoundError as err:
             raise PluginExecutionError(
-                "Applying catalog rules failed: catalog file is missing.",
+                "Applying catalog rules failed: catalog file is missing.",  # noqa: EM101
             ) from err
         except Exception as err:
             catalog_path.unlink()
             raise PluginExecutionError(
-                f"Applying catalog rules failed: catalog file is invalid: {err}",
+                f"Applying catalog rules failed: catalog file is invalid: {err}",  # noqa: EM102
             ) from err
 
     def catalog_cache_key(self, plugin_invoker):
         """Get a cache key for the catalog.
 
         Args:
             plugin_invoker: the plugin invoker running
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin/singer/target.py` & `meltano-3.4.0a1/src/meltano/core/plugin/singer/target.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin/superset.py` & `meltano-3.4.0a1/src/meltano/core/plugin/superset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Plugin glue code for Superset."""
+
 from __future__ import annotations
 
 import logging
 import subprocess
 from contextlib import suppress
 
 import structlog
@@ -81,15 +82,15 @@
         ]
 
         if custom_config_filename := invoker.plugin_config_extras["_config_path"]:
             custom_config_path = invoker.project.root.joinpath(custom_config_filename)
 
             if not custom_config_path.exists():
                 raise PluginExecutionError(
-                    f"Could not find config file {custom_config_path}",
+                    f"Could not find config file {custom_config_path}",  # noqa: EM102
                 )
 
             config_script_lines.extend(
                 [
                     "from importlib.util import module_from_spec, spec_from_file_location",  # noqa: E501
                     f'spec = spec_from_file_location("superset_config", {str(custom_config_path)!r})',  # noqa: E501
                     "custom_config = module_from_spec(spec)",
@@ -129,15 +130,15 @@
             stderr=subprocess.PIPE,
         )
         exit_code = await handle.wait()
 
         if exit_code:
             raise AsyncSubprocessError(
                 (
-                    "Superset metadata database could not be initialized: "
+                    "Superset metadata database could not be initialized: "  # noqa: EM101
                     "`superset db upgrade` failed"
                 ),
                 handle,
             )
 
         logging.debug("Completed `superset db upgrade`")
 
@@ -162,15 +163,15 @@
             stderr=subprocess.PIPE,
         )
         exit_code = await handle.wait()
 
         if exit_code:
             raise AsyncSubprocessError(
                 (
-                    "Superset default roles and permissions could not be "
+                    "Superset default roles and permissions could not be "  # noqa: EM101
                     "created: `superset init` failed"
                 ),
                 handle,
             )
 
         logging.debug("Completed `superset init`")
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin_install_service.py` & `meltano-3.4.0a1/src/meltano/core/plugin_install_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         """Return the number of parallel installation processes to use.
 
         Returns:
             The number of parallel installation processes to use.
         """
         if self._parallelism is None:
             return cpu_count()
-        elif self._parallelism < 1:
+        if self._parallelism < 1:
             return sys.maxsize
         return self._parallelism
 
     @cached_property
     def semaphore(self):
         """An asyncio semaphore with a counter starting at `self.parallelism`.
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin_invoker.py` & `meltano-3.4.0a1/src/meltano/core/plugin_invoker.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,19 @@
 
         # Ensure Meltano venv is not inherited
         env.pop("VIRTUAL_ENV", None)
         env.pop("PYTHONPATH", None)
         if self.venv_service:
             # Switch to plugin-specific venv
             venv = VirtualEnv(
-                self.project.venvs_dir(self.plugin.type, self.plugin.name),
+                self.project.venvs_dir(
+                    self.plugin.type,
+                    self.plugin.name,
+                    make_dirs=False,
+                ),
             )
             venv_dir = str(venv.bin_dir)
             env["VIRTUAL_ENV"] = str(venv.root)
             env["PATH"] = os.pathsep.join([venv_dir, env["PATH"]])
 
         return env
 
@@ -473,15 +477,15 @@
 
         Returns:
             The container run exit code.
         """
         command_config = self.find_command(plugin_command)
 
         if not command_config.container_spec:
-            raise ValueError("Command is missing a container spec")
+            raise ValueError("Command is missing a container spec")  # noqa: EM101
 
         spec = command_config.container_spec
         service = ContainerService()
 
         logger.debug("Running containerized command", command=plugin_command)
         async with self._invoke(*args, **kwargs) as (_proc_args, _, proc_env):
             plugin_name = self.plugin.name
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin_location_remove.py` & `meltano-3.4.0a1/src/meltano/core/plugin_location_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin_lock_service.py` & `meltano-3.4.0a1/src/meltano/core/plugin_lock_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             LockfileAlreadyExistsError: If the lockfile already exists and is not
                 flagged for overwriting.
         """
         plugin_lock = PluginLock(self.project, plugin)
 
         if plugin_lock.path.exists() and not exists_ok:
             raise LockfileAlreadyExistsError(
-                f"Lockfile already exists: {plugin_lock.path}",
+                f"Lockfile already exists: {plugin_lock.path}",  # noqa: EM102
                 plugin_lock.path,
                 plugin,
             )
 
         plugin_lock.save()
 
         logger.debug("Locked plugin definition", path=plugin_lock.path)
```

### Comparing `meltano-3.3.2/src/meltano/core/plugin_remove_service.py` & `meltano-3.4.0a1/src/meltano/core/plugin_remove_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin_repository.py` & `meltano-3.4.0a1/src/meltano/core/plugin_repository.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/plugin_test_service.py` & `meltano-3.4.0a1/src/meltano/core/plugin_test_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/project.py` & `meltano-3.4.0a1/src/meltano/core/project.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Meltano Projects."""
 
-
 from __future__ import annotations
 
 import errno
 import logging
 import os
 import sys
 import threading
 import typing as t
 from contextlib import contextmanager
 from functools import cached_property
 from pathlib import Path
 
-import fasteners
+import fasteners  # type: ignore[import-untyped]
 from dotenv import dotenv_values
 
 from meltano.core import yaml
 from meltano.core.behavior.versioned import Versioned
 from meltano.core.config_service import ConfigService
 from meltano.core.environment import Environment
 from meltano.core.error import (
@@ -31,14 +30,21 @@
 from meltano.core.project_settings_service import ProjectSettingsService
 from meltano.core.utils import makedirs, sanitize_filename, truthy
 
 if t.TYPE_CHECKING:
     from meltano.core.meltano_file import MeltanoFile as MeltanoFileTypeHint
     from meltano.core.plugin.base import PluginRef
 
+    if sys.version_info < (3, 10):
+        from typing import TypeAlias
+    else:
+        from typing_extensions import TypeAlias
+
+
+StrPath: TypeAlias = t.Union[str, os.PathLike]
 
 logger = logging.getLogger(__name__)
 
 
 PROJECT_ROOT_ENV = "MELTANO_PROJECT_ROOT"
 PROJECT_ENVIRONMENT_ENV = "MELTANO_ENVIRONMENT"
 PROJECT_READONLY_ENV = "MELTANO_PROJECT_READONLY"
@@ -68,15 +74,15 @@
     _activate_lock = threading.Lock()
     _find_lock = threading.Lock()
     _meltano_rw_lock = fasteners.ReaderWriterLock()
     _default = None
 
     def __init__(
         self,
-        root: os.PathLike,
+        root: StrPath,
         environment: Environment | None = None,
         readonly: bool = False,
     ):
         """Initialize a `Project` instance.
 
         Args:
             root: The root directory of the project.
@@ -198,15 +204,15 @@
 
         # create a symlink to our current binary
         try:
             # check if running on Windows
             if os.name == "nt":
                 executable = Path(sys.executable).parent / "meltano.exe"
                 # Admin privileges are required to create symlinks on Windows
-                if ctypes.windll.shell32.IsUserAnAdmin():
+                if ctypes.windll.shell32.IsUserAnAdmin():  # type: ignore[attr-defined]
                     if executable.is_file():
                         project.run_dir().joinpath("bin").symlink_to(executable)
                     else:
                         logger.warning(
                             "Could not create symlink: meltano.exe not "  # noqa: G004
                             f"present in {str(Path(sys.executable).parent)}",
                         )
@@ -339,45 +345,45 @@
                 self.project_files.update(meltano_config.canonical())
             except Exception as err:
                 logger.critical("Could not update meltano.yml: %s", err)  # noqa: WPS323
                 raise
 
         self.refresh()
 
-    def root_dir(self, *joinpaths):
+    def root_dir(self, *joinpaths: StrPath) -> Path:  # noqa: ARG002
         """Return the root directory of this project, optionally joined with path.
 
         Args:
             joinpaths: list of subdirs and/or file to join to project root.
 
         Returns:
             project root joined with provided subdirs and/or file
         """
         return self.root.joinpath(*joinpaths)
 
     @property
-    def meltanofile(self):
+    def meltanofile(self) -> Path:
         """Get the path to this project's meltano.yml.
 
         Returns:
             the path to this project meltano.yml
         """
         return self.root.joinpath("meltano.yml")
 
     @property
-    def dotenv(self):
+    def dotenv(self) -> Path:
         """Get the path to this project's .env file.
 
         Returns:
             the path to this project's .env file
         """
         return self.root.joinpath(".env")
 
     @cached_property
-    def dotenv_env(self):
+    def dotenv_env(self) -> dict[str, str | None]:
         """Get values from this project's .env file.
 
         Returns:
             values found in this project's .env file
         """
         return dotenv_values(self.dotenv)
 
@@ -413,159 +419,201 @@
         if self.readonly:
             raise ProjectReadonly
 
         yield self.dotenv
         self.refresh()
 
     @makedirs
-    def meltano_dir(self, *joinpaths):
+    def meltano_dir(self, *joinpaths: StrPath, make_dirs: bool = True) -> Path:  # noqa: ARG002
         """Path to the project `.meltano` directory.
 
         Args:
             joinpaths: Paths to join to the `.meltano` directory.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Resolved path to `.meltano` dir optionally joined to given paths.
         """
         return self.sys_dir_root.joinpath(*joinpaths)
 
     @makedirs
-    def analyze_dir(self, *joinpaths):
+    def analyze_dir(self, *joinpaths: StrPath, make_dirs: bool = True) -> Path:  # noqa: ARG002
         """Path to the project `analyze` directory.
 
         Args:
             joinpaths: Paths to join to the `analyze` directory.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Resolved path to `analyze` dir optionally joined to given paths.
         """
         return self.root_dir("analyze", *joinpaths)
 
     @makedirs
-    def extract_dir(self, *joinpaths):
+    def extract_dir(self, *joinpaths: StrPath, make_dirs: bool = True) -> Path:  # noqa: ARG002
         """Path to the project `extract` directory.
 
         Args:
             joinpaths: Paths to join to the `extract` directory.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Resolved path to `extract` dir optionally joined to given paths.
         """
         return self.root_dir("extract", *joinpaths)
 
     @makedirs
-    def venvs_dir(self, *prefixes):
+    def venvs_dir(self, *prefixes: StrPath, make_dirs: bool = True) -> Path:
         """Path to a `venv` directory in `.meltano`.
 
         Args:
             prefixes: Paths to prepend to the `venv` directory in `.meltano`.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Resolved path to `venv` dir optionally prepended with given prefixes.
         """
-        return self.meltano_dir(*prefixes, "venv")
+        return self.meltano_dir(*prefixes, "venv", make_dirs=make_dirs)
 
     @makedirs
-    def run_dir(self, *joinpaths):
+    def run_dir(self, *joinpaths: StrPath, make_dirs: bool = True) -> Path:
         """Path to the `run` directory in `.meltano`.
 
         Args:
             joinpaths: Paths to join to the `run` directory in `.meltano`.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Resolved path to `run` dir optionally joined to given paths.
         """
-        return self.meltano_dir("run", *joinpaths)
+        return self.meltano_dir("run", *joinpaths, make_dirs=make_dirs)
 
     @makedirs
-    def logs_dir(self, *joinpaths):
+    def logs_dir(self, *joinpaths: StrPath, make_dirs: bool = True) -> Path:
         """Path to the `logs` directory in `.meltano`.
 
         Args:
             joinpaths: Paths to join to the `logs` directory in `.meltano`.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Resolved path to `logs` dir optionally joined to given paths.
         """
-        return self.meltano_dir("logs", *joinpaths)
+        return self.meltano_dir("logs", *joinpaths, make_dirs=make_dirs)
 
     @makedirs
-    def job_dir(self, state_id, *joinpaths):
+    def job_dir(self, state_id, *joinpaths: StrPath, make_dirs: bool = True) -> Path:
         """Path to the `elt` directory in `.meltano/run`.
 
         Args:
             state_id: State ID of `run` dir.
             joinpaths: Paths to join to the `elt` directory in `.meltano`.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Resolved path to `elt` dir optionally joined to given paths.
         """
-        return self.run_dir("elt", sanitize_filename(state_id), *joinpaths)
+        return self.run_dir(
+            "elt",
+            sanitize_filename(state_id),
+            *joinpaths,
+            make_dirs=make_dirs,
+        )
 
     @makedirs
-    def job_logs_dir(self, state_id, *joinpaths):
+    def job_logs_dir(
+        self,
+        state_id,
+        *joinpaths: StrPath,
+        make_dirs: bool = True,
+    ) -> Path:
         """Path to the `elt` directory in `.meltano/logs`.
 
         Args:
             state_id: State ID of `logs` dir.
             joinpaths: Paths to join to the `elt` directory in `.meltano/logs`.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Resolved path to `elt` dir optionally joined to given paths.
         """
-        return self.logs_dir("elt", sanitize_filename(state_id), *joinpaths)
+        return self.logs_dir(
+            "elt",
+            sanitize_filename(state_id),
+            *joinpaths,
+            make_dirs=make_dirs,
+        )
 
     @makedirs
-    def plugin_dir(self, plugin: PluginRef, *joinpaths):
+    def plugin_dir(
+        self,
+        plugin: PluginRef,
+        *joinpaths: StrPath,
+        make_dirs: bool = True,
+    ) -> Path:
         """Path to the plugin installation directory in `.meltano`.
 
         Args:
             plugin: Plugin to retrieve or create directory for.
             joinpaths: Paths to join to the plugin installation directory in `.meltano`.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Resolved path to plugin installation dir optionally joined to given paths.
         """
-        return self.meltano_dir(plugin.type, plugin.name, *joinpaths)
+        return self.meltano_dir(
+            plugin.type,
+            plugin.name,
+            *joinpaths,
+            make_dirs=make_dirs,
+        )
 
     @makedirs
-    def root_plugins_dir(self, *joinpaths: str):
+    def root_plugins_dir(self, *joinpaths: StrPath, make_dirs: bool = True) -> Path:  # noqa: ARG002
         """Path to the project `plugins` directory.
 
         Args:
             joinpaths: Paths to join with the project `plugins` directory.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Path to the project `plugins` directory.
         """
         return self.root_dir("plugins", *joinpaths)
 
     @makedirs
     def plugin_lock_path(
         self,
         plugin_type: str,
         plugin_name: str,
+        *,
         variant_name: str | None = None,
+        make_dirs: bool = True,  # noqa: ARG002
     ):
         """Path to the project lock file.
 
         Args:
             plugin_type: The plugin type.
             plugin_name: The plugin name.
             variant_name: The plugin variant name.
+            make_dirs: Whether to create the directory hierarchy if it doesn't exist.
 
         Returns:
             Path to the plugin lock file.
         """
         filename = f"{plugin_name}"
 
         if variant_name:
             filename = f"{filename}--{variant_name}"
 
-        return self.root_plugins_dir(plugin_type, f"{filename}.lock")
+        return self.root_plugins_dir(
+            plugin_type,
+            f"{filename}.lock",
+            make_dirs=make_dirs,
+        )
 
     def __eq__(self, other):
         """Project equivalence check.
 
         Args:
             other: The other Project instance to check against.
```

### Comparing `meltano-3.3.2/src/meltano/core/project_add_service.py` & `meltano-3.4.0a1/src/meltano/core/project_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/project_files.py` & `meltano-3.4.0a1/src/meltano/core/project_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         Args:
             file_path: The path to check.
 
         Raises:
             InvalidIncludePathError: If the included path is not a valid file.
         """
         if not (file_path.is_file() and file_path.exists()):
-            raise InvalidIncludePathError(f"Included path '{file_path}' not found.")
+            raise InvalidIncludePathError(f"Included path '{file_path}' not found.")  # noqa: EM102
 
     def _resolve_include_paths(self, include_path_patterns: list[str]) -> list[Path]:
         """Return a list of paths from a list of glob pattern strings.
 
         Not including `meltano.yml` (even if it is matched by a pattern).
 
         Args:
@@ -178,17 +178,17 @@
         if key in self._plugin_file_map:
             key_path_string = ":".join(key)
             existing_key_file_path = self._plugin_file_map.get(key)
             logger.critical(
                 f'Plugin with path "{key_path_string}" already added in '  # noqa: G004
                 f"file {existing_key_file_path}.",
             )
-            raise Exception("Duplicate plugin name found.")
-        else:
-            self._plugin_file_map.update({key: str(include_path)})
+            raise Exception("Duplicate plugin name found.")  # noqa: EM101
+
+        self._plugin_file_map.update({key: str(include_path)})
 
     def _index_file(  # noqa: WPS210
         self,
         include_file_path: Path,
         include_file_contents: CommentedMap,
     ) -> None:
         """Populate map of plugins/schedules to their respective files.
```

### Comparing `meltano-3.3.2/src/meltano/core/project_init_service.py` & `meltano-3.4.0a1/src/meltano/core/project_init_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,19 +64,19 @@
                 msg = (
                     "A `meltano.yml` file already exists in the target directory. "
                     "Use `--force` to overwrite it."
                 )
                 raise ProjectInitServiceError(msg) from ex
         except PermissionError as ex:
             raise ProjectInitServiceError(
-                f"Permission denied to create '{self.project_directory}'.",
+                f"Permission denied to create '{self.project_directory}'.",  # noqa: EM102
             ) from ex
         except Exception as ex:
             raise ProjectInitServiceError(
-                f"Could not create directory '{self.project_directory}'. {ex}",
+                f"Could not create directory '{self.project_directory}'. {ex}",  # noqa: EM102
             ) from ex
 
         project = Project(self.project_directory)
 
         self.create_dot_meltano_dir(project)
         self.create_files(project)
```

### Comparing `meltano-3.3.2/src/meltano/core/project_plugins_service.py` & `meltano-3.4.0a1/src/meltano/core/project_plugins_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Project plugin service."""
 
-
 from __future__ import annotations
 
 import enum
 import typing as t
 from contextlib import contextmanager, suppress
 from functools import cached_property
 
@@ -239,25 +238,26 @@
                 )
                 and (
                     configurable is None
                     or self.ensure_parent(plugin).is_configurable() == configurable
                 )
             ):
                 return self.ensure_parent(plugin)
-            elif plugin.type == PluginType.MAPPERS:
+
+            if plugin.type == PluginType.MAPPERS:
                 mapping = self._find_mapping(plugin_name, plugin)
                 if mapping:
                     return mapping
         raise PluginNotFoundError(
             PluginRef(plugin_type, plugin_name) if plugin_type else plugin_name,
         )
 
     def _find_mapping(self, plugin_name: str, plugin: ProjectPlugin) -> ProjectPlugin:
         mapping_name = plugin.extra_config.get("_mapping_name")
-        if mapping_name == plugin_name:
+        if mapping_name == plugin_name:  # noqa: RET503
             all_mappings = self.find_plugins_by_mapping_name(mapping_name)
             if len(all_mappings) > 1:
                 raise AmbiguousMappingName(mapping_name)
             return self.ensure_parent(plugin)
 
     def find_plugin_by_namespace(
         self,
@@ -533,15 +533,15 @@
         """
         parent, source = self.find_parent(plugin)
 
         logger.debug(
             "Found plugin parent",
             plugin=plugin.name,
             parent=parent.name,
-            source=source,
+            source=source.name,
         )
         return parent
 
     def ensure_parent(self, plugin: ProjectPlugin) -> ProjectPlugin:
         """Ensure that plugin has a parent set.
 
         Args:
@@ -565,15 +565,15 @@
             First available transformer plugin.
         """
         if transformer := next(
             iter(self.get_plugins_of_type(plugin_type=PluginType.TRANSFORMERS)),
             None,
         ):
             return transformer
-        raise PluginNotFoundError("No Plugin of type Transformer found.")
+        raise PluginNotFoundError("No Plugin of type Transformer found.")  # noqa: EM101
 
     @contextmanager
     def use_preferred_source(self, source: DefinitionSource) -> None:
         """Prefer a source of definition.
 
         Args:
             source: The source to prefer.
```

### Comparing `meltano-3.3.2/src/meltano/core/project_settings_service.py` & `meltano-3.4.0a1/src/meltano/core/project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/runner/dbt.py` & `meltano-3.4.0a1/src/meltano/core/runner/dbt.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             handle = await dbt.invoke_async(
                 *args,
                 **kwargs,
                 stdout=asyncio.subprocess.PIPE,
                 stderr=asyncio.subprocess.PIPE,
             )
         except Exception as err:
-            raise RunnerError(f"Cannot start dbt: {err}") from err
+            raise RunnerError(f"Cannot start dbt: {err}") from err  # noqa: EM102
 
         await asyncio.wait(
             [
                 asyncio.create_task(coro)
                 for coro in (
                     capture_subprocess_output(handle.stdout, log),
                     capture_subprocess_output(handle.stderr, log),
@@ -51,15 +51,15 @@
             ],
             return_when=asyncio.ALL_COMPLETED,
         )
 
         if exitcode := handle.returncode:
             command = kwargs["command"] or args[0]
             raise RunnerError(
-                f"`dbt {command}` failed",
+                f"`dbt {command}` failed",  # noqa: EM102
                 {PluginType.TRANSFORMERS: exitcode},
             )
 
     async def run(self, log=None):
         dbt = self.context.transformer_invoker()
 
         async with dbt.prepared(self.context.session):
```

### Comparing `meltano-3.3.2/src/meltano/core/runner/singer.py` & `meltano-3.4.0a1/src/meltano/core/runner/singer.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,26 +54,26 @@
         try:
             p_tap = await tap.invoke_async(
                 limit=line_length_limit,
                 stdout=asyncio.subprocess.PIPE,  # Singer messages
                 stderr=asyncio.subprocess.PIPE,  # Log
             )
         except Exception as err:
-            raise RunnerError(f"Cannot start extractor: {err}") from err
+            raise RunnerError(f"Cannot start extractor: {err}") from err  # noqa: EM102
 
         # Start target
         try:
             p_target = await target.invoke_async(
                 limit=line_length_limit,
                 stdin=asyncio.subprocess.PIPE,  # Singer messages
                 stdout=asyncio.subprocess.PIPE,  # Singer state
                 stderr=asyncio.subprocess.PIPE,  # Log
             )
         except Exception as err:
-            raise RunnerError(f"Cannot start loader: {err}") from err
+            raise RunnerError(f"Cannot start loader: {err}") from err  # noqa: EM102
 
         # Process tap output
         tap_outputs = [p_target.stdin]
         if extractor_out:
             tap_outputs.insert(0, extractor_out)
 
         tap_stdout_future = asyncio.ensure_future(
@@ -138,22 +138,22 @@
                         tap_stdout_future.exception(),
                         line_length_limit=line_length_limit,
                         stream_buffer_size=stream_buffer_size,
                     )
 
                 failed_future = output_futures_failed.pop()
                 raise failed_future.exception()  # noqa: RSE102
-            else:
-                # If all of the output handlers completed without raising an
-                # exception, we still need to wait for the tap or target to
-                # complete.
-                done, _ = await asyncio.wait(
-                    [tap_process_future, target_process_future],
-                    return_when=asyncio.FIRST_COMPLETED,
-                )
+
+            # If all of the output handlers completed without raising an
+            # exception, we still need to wait for the tap or target to
+            # complete.
+            done, _ = await asyncio.wait(
+                [tap_process_future, target_process_future],
+                return_when=asyncio.FIRST_COMPLETED,
+            )
 
         if target_process_future in done:
             target_code = target_process_future.result()
 
             if tap_process_future in done:
                 tap_code = tap_process_future.result()
             else:
@@ -188,21 +188,21 @@
             await asyncio.wait([target_stdout_future, target_stderr_future])
 
             # Wait for target to complete
             target_code = await target_process_future
 
         if tap_code and target_code:
             raise RunnerError(
-                "Extractor and loader failed",
+                "Extractor and loader failed",  # noqa: EM101
                 {PluginType.EXTRACTORS: tap_code, PluginType.LOADERS: target_code},
             )
-        elif tap_code:
-            raise RunnerError("Extractor failed", {PluginType.EXTRACTORS: tap_code})
-        elif target_code:
-            raise RunnerError("Loader failed", {PluginType.LOADERS: target_code})
+        if tap_code:
+            raise RunnerError("Extractor failed", {PluginType.EXTRACTORS: tap_code})  # noqa: EM101
+        if target_code:
+            raise RunnerError("Loader failed", {PluginType.LOADERS: target_code})  # noqa: EM101
 
     def dry_run(self, tap: PluginInvoker, target: PluginInvoker):
         logging.info("Dry run:")
         logging.info(f"\textractor: {tap.plugin.name} at '{tap.exec_path()}'")  # noqa: G004
         logging.info(f"\tloader: {target.plugin.name} at '{target.exec_path()}'")  # noqa: G004
 
     async def run(
@@ -217,15 +217,15 @@
 
         if self.context.dry_run:
             return self.dry_run(tap, target)
 
         async with tap.prepared(self.context.session), target.prepared(
             self.context.session,
         ):
-            await self.invoke(
+            await self.invoke(  # noqa: RET503
                 tap,
                 target,
                 extractor_log=extractor_log,
                 loader_log=loader_log,
                 extractor_out=extractor_out,
                 loader_out=loader_out,
             )
@@ -255,8 +255,8 @@
             "setting to at least double the size of the largest expected "
             "message, and try again.",
         )
         logging.error(
             "To learn more, visit "
             "https://docs.meltano.com/reference/settings#eltbuffer_size",
         )
-        raise RunnerError("Output line length limit exceeded") from exception
+        raise RunnerError("Output line length limit exceeded") from exception  # noqa: EM101
```

### Comparing `meltano-3.3.2/src/meltano/core/schedule.py` & `meltano-3.4.0a1/src/meltano/core/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,10 +125,10 @@
             The last successful run for this schedule.
 
         Raises:
             NotImplementedError: If the schedule is a job.
         """
         if self.job:
             raise NotImplementedError(
-                "Can't obtain last successful State(Job) for schedule job.",
+                "Can't obtain last successful State(Job) for schedule job.",  # noqa: EM101
             )
         return StateJobFinder(self.name).latest_success(session)
```

### Comparing `meltano-3.3.2/src/meltano/core/schedule_service.py` & `meltano-3.4.0a1/src/meltano/core/schedule_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/select_service.py` & `meltano-3.4.0a1/src/meltano/core/select_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     async def list_all(self, session) -> ListSelectedExecutor:
         """List all select."""
         try:
             catalog = await self.load_catalog(session)
         except FileNotFoundError as err:
             raise PluginExecutionError(
-                "Could not find catalog. Verify that the tap supports discovery "
+                "Could not find catalog. Verify that the tap supports discovery "  # noqa: EM101
                 "mode and advertises the `discover` capability as well as either "
                 "`catalog` or `properties`",
             ) from err
 
         list_all = ListSelectedExecutor()
         list_all.visit(catalog)
```

### Comparing `meltano-3.3.2/src/meltano/core/setting.py` & `meltano-3.4.0a1/src/meltano/core/setting.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/setting_definition.py` & `meltano-3.4.0a1/src/meltano/core/setting_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,17 +447,17 @@
             ValueError: If value is not of the expected type.
         """
         value = value.isoformat() if isinstance(value, (date, datetime)) else value
 
         if isinstance(value, str):
             if self.kind == SettingKind.BOOLEAN:
                 return utils.truthy(value)
-            elif self.kind == SettingKind.INTEGER:
+            if self.kind == SettingKind.INTEGER:
                 return int(value)
-            elif self.kind == SettingKind.OBJECT:
+            if self.kind == SettingKind.OBJECT:
                 value = dict(
                     self._parse_value(value, "object", Mapping),  # type: ignore
                 )
             elif self.kind == SettingKind.ARRAY:
                 value = list(
                     self._parse_value(value, "array", Sequence),  # type: ignore
                 )
```

### Comparing `meltano-3.3.2/src/meltano/core/settings_service.py` & `meltano-3.4.0a1/src/meltano/core/settings_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     @abstractmethod
     def setting_definitions(self) -> list[SettingDefinition]:
         """Return definitions of supported settings."""
 
     @property
     def inherited_settings_service(self):
         """Return settings service to inherit configuration from."""
-        return None  # noqa: DAR201
+        return None  # noqa: DAR201, RET501
 
     @property
     @abstractmethod
     def meltano_yml_config(self) -> dict:
         """Return current configuration in `meltano.yml`."""
 
     @abstractmethod
@@ -619,15 +619,15 @@
                 setting
                 for setting in self.definitions()
                 if setting.name == name or name in setting.aliases
             )
         except StopIteration as err:
             raise SettingMissingError(name) from err
 
-    # TODO: The `for_writing` parameter is unsued, but referenced elsewhere.
+    # TODO: The `for_writing` parameter is unused, but referenced elsewhere.
     # Callers should be updated to not use it, and then it should be removed.
     def setting_env_vars(
         self,
         setting_def,
         for_writing=False,  # noqa: ARG002
     ):
         """Get environment variables for the given setting definition.
```

### Comparing `meltano-3.3.2/src/meltano/core/settings_store.py` & `meltano-3.4.0a1/src/meltano/core/settings_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Storage Managers for Meltano Configuration."""
 
-
 from __future__ import annotations
 
 import logging
 import typing as t
 from abc import ABC, abstractmethod
 from contextlib import contextmanager, suppress
 from copy import deepcopy
@@ -80,24 +79,24 @@
 
 
 def cast_setting_value(
     value: t.Any,
     metadata: dict[str, t.Any],
     setting_def: SettingDefinition | None,
 ) -> tuple[t.Any, dict[str, t.Any]]:
-    """Cast a setting value according to its setting defition.
+    """Cast a setting value according to its setting definition.
 
     Args:
         value: The setting value to be cast.
         metadata: The metadata of the setting value.
-        setting_def: The setting defition.
+        setting_def: The setting definition.
 
     Returns:
         A tuple with the setting value, and its metadata. If the
-        setting defition was `None`, or the value was not changed by
+        setting definition was `None`, or the value was not changed by
         the cast, the pair returned is the same `value` and `metadata`
         objects provided. Otherwise, the cast value is returned along
         with a new dictionary which is a shallow copy of the provided
         metadata with the "uncast_value" key-value pair added.
     """
     if setting_def is not None:
         cast_value = setting_def.cast_value(value)
@@ -105,18 +104,18 @@
             return cast_value, {**metadata, "uncast_value": value}
     return value, metadata
 
 
 class SettingValueStore(str, Enum):
     """Setting Value Store.
 
-    Note: The declaration order of stores determins store precedence when using
+    Note: The declaration order of stores determines store precedence when using
         the Auto store manager. This is because the `.readables()` and
         `.writables()` methods return ordered lists that the Auto store manager
-        iterates over when retrieveing setting values.
+        iterates over when retrieving setting values.
     """
 
     CONFIG_OVERRIDE = "config_override"
     ENV = "env"
     DOTENV = "dotenv"
     MELTANO_ENV = "meltano_environment"
     MELTANO_YML = "meltano_yml"
@@ -839,15 +838,15 @@
         Raises:
             StoreNotSupportedError: if the project is read-only or no
                 environment is active.
         """
         super().ensure_supported(method)
         if not self.settings_service.supports_environments:
             raise StoreNotSupportedError(
-                "Project config cannot be stored in an Environment.",
+                "Project config cannot be stored in an Environment.",  # noqa: EM101
             )
         if self.settings_service.project.environment is None:
             raise StoreNotSupportedError(NoActiveEnvironment())
 
     @contextmanager
     def update_config(self) -> None:
         """Update Meltano Environment configuration.
@@ -909,15 +908,15 @@
         Args:
             method: Unused. Included to match parent class method signature.
 
         Raises:
             StoreNotSupportedError: if database session is not provided.
         """
         if not self.session:
-            raise StoreNotSupportedError("No database session provided")
+            raise StoreNotSupportedError("No database session provided")  # noqa: EM101
 
     def get(
         self,
         name: str,
         setting_def: SettingDefinition | None = None,  # noqa: ARG002
         cast_value: bool = False,  # noqa: ARG002
     ) -> tuple[str, dict]:
@@ -1087,18 +1086,18 @@
         Returns:
             A tuple containing the got value and accompanying metadata dictionary.
 
         Raises:
             StoreNotSupportedError: if no setting_def is passed.
         """
         if not setting_def:
-            raise StoreNotSupportedError("Setting is missing")
+            raise StoreNotSupportedError("Setting is missing")  # noqa: EM101
 
         if not self.inherited_settings_service:
-            raise StoreNotSupportedError("Inherited settings service is missing")
+            raise StoreNotSupportedError("Inherited settings service is missing")  # noqa: EM101
 
         value, metadata = self.get_with_metadata(setting_def.name)
         if value is None or metadata["source"] is SettingValueStore.DEFAULT:
             return None, {}
 
         self.log(f"Read key '{name}' from inherited: {value!r}")
         return value, {
@@ -1271,15 +1270,15 @@
                 return SettingValueStore.DB
             return None
 
         # value is a secret
         if setting_def and setting_def.is_redacted:
             if self.ensure_supported(store=SettingValueStore.DOTENV):
                 return SettingValueStore.DOTENV
-            elif self.ensure_supported(store=SettingValueStore.DB):
+            if self.ensure_supported(store=SettingValueStore.DB):
                 return SettingValueStore.DB
             # ensure secrets don't leak into other stores
             return None
 
         # value is env-specific
         if (
             setting_def
@@ -1290,33 +1289,33 @@
 
         # no active meltano environment
         if not self.project.environment:
             # return root `meltano.yml`
             if self.ensure_supported(store=SettingValueStore.MELTANO_YML):
                 return SettingValueStore.MELTANO_YML
             # fall back to dotenv
-            elif self.ensure_supported(store=SettingValueStore.DOTENV):
+            if self.ensure_supported(store=SettingValueStore.DOTENV):
                 return SettingValueStore.DOTENV
             # fall back to meltano system db
-            elif self.ensure_supported(store=SettingValueStore.DB):
+            if self.ensure_supported(store=SettingValueStore.DB):
                 return SettingValueStore.DB
             return None
 
         # any remaining config routed to meltano environment
         if self.ensure_supported(store=SettingValueStore.MELTANO_ENV):
             return SettingValueStore.MELTANO_ENV
         # Fall back to root `meltano.yml`. This is required for Meltano
         # settings, which cannot be stored in an Environment
         if self.ensure_supported(store=SettingValueStore.MELTANO_YML):
             return SettingValueStore.MELTANO_YML
         # fall back to dotenv
-        elif self.ensure_supported(store=SettingValueStore.DOTENV):
+        if self.ensure_supported(store=SettingValueStore.DOTENV):
             return SettingValueStore.DOTENV
         # fall back to meltano system db
-        elif self.ensure_supported(store=SettingValueStore.DB):
+        if self.ensure_supported(store=SettingValueStore.DB):
             return SettingValueStore.DB
         return None
 
     def get(
         self,
         name: str,
         setting_def: SettingDefinition | None = None,
@@ -1326,15 +1325,15 @@
         """Get a Setting value by name and SettingDefinition.
 
         Args:
             name: Setting name.
             setting_def: SettingDefinition. If none is passed, one will be
                 discovered using `self.find_setting(name)`.
             cast_value: Whether to cast the value according to `setting_def`.
-            kwargs: Additional keword arguments to pass to `manager.get()`.
+            kwargs: Additional keyword arguments to pass to `manager.get()`.
 
         Returns:
             A tuple containing the got value and accompanying metadata dictionary.
         """
         setting_def = setting_def or self.find_setting(name)
 
         metadata = {}
@@ -1391,15 +1390,15 @@
             StoreNotSupportedError: exception encountered when attempting to
                 write to store.
         """
         setting_def = setting_def or self.find_setting(name)
         store = self.auto_store(name, setting_def=setting_def)
         logger.debug(f"AutoStoreManager returned store '{store}'")  # noqa: G004
         if store is None:
-            raise StoreNotSupportedError("No storage method available")
+            raise StoreNotSupportedError("No storage method available")  # noqa: EM101
 
         # May raise StoreNotSupportedError, but that's good.
         manager = self.manager_for(store)
         metadata = manager.set(name, path, value, setting_def=setting_def)
         metadata["store"] = store
         return metadata
```

### Comparing `meltano-3.3.2/src/meltano/core/sqlalchemy.py` & `meltano-3.4.0a1/src/meltano/core/sqlalchemy.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             return dialect.type_descriptor(UUID())
         type_descriptor_length = 32
         return dialect.type_descriptor(CHAR(type_descriptor_length))
 
     def process_bind_param(self, value, dialect):
         if value is None:
             return value
-        elif dialect.name == "postgresql":
+        if dialect.name == "postgresql":
             return str(value)
         if not isinstance(value, uuid.UUID):
             value = uuid.UUID(value)
         return value.hex
 
     def process_result_value(  # noqa: D102
         self,
```

### Comparing `meltano-3.3.2/src/meltano/core/state_service.py` & `meltano-3.4.0a1/src/meltano/core/state_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Manager for state that persists across runs of a BlockSet.
 
 'State' in this module refers to _Singer_ state, which is held in a Job's
 'payload' field. This is not to be confused with the Job's 'state' field,
 which refers to a given job run's status, e.g. 'RUNNING' or 'FAILED'.
 """
+
 from __future__ import annotations
 
 import datetime
 import json
 import typing as t
 
 import structlog
@@ -74,17 +75,17 @@
             now = datetime.datetime.now(datetime.timezone.utc)
             return Job(
                 job_name=job,
                 state=State.STATE_EDIT,
                 started_at=now,
                 ended_at=now,
             )
-        elif isinstance(job, Job):
+        if isinstance(job, Job):
             return job
-        raise TypeError("job must be of type Job or of type str")
+        raise TypeError("job must be of type Job or of type str")  # noqa: EM101
 
     @property
     def state_store_manager(self):
         """Initialize and return the correct StateStoreManager.
 
         Returns:
             StateStoreManager instance.
@@ -104,15 +105,15 @@
             state: the state to validate
 
         Raises:
             InvalidJobStateError: if supplied state is not valid singer state
         """
         if SINGER_STATE_KEY not in state:
             raise InvalidJobStateError(
-                f"{SINGER_STATE_KEY} not found in top level of provided state",
+                f"{SINGER_STATE_KEY} not found in top level of provided state",  # noqa: EM102
             )
 
     def add_state(
         self,
         job: Job | str,
         new_state: str,
         payload_flags: Payload = Payload.STATE,
```

### Comparing `meltano-3.3.2/src/meltano/core/state_store/__init__.py` & `meltano-3.4.0a1/src/meltano/core/state_store/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """State backends."""
+
 from __future__ import annotations
 
 import platform
 import typing as t
 from enum import Enum
 from urllib.parse import urlparse
```

### Comparing `meltano-3.3.2/src/meltano/core/state_store/azure.py` & `meltano-3.4.0a1/src/meltano/core/state_store/azure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """StateStoreManager for Azure Blob storage backend."""
+
 from __future__ import annotations
 
 import typing as t
 from contextlib import contextmanager
 from functools import cached_property
 
 from meltano.core.error import MeltanoError
@@ -71,15 +72,15 @@
         """
         super().__init__(**kwargs)
         self.connection_string = connection_string
         self.storage_account_url = storage_account_url
 
         if not self.parsed.hostname:
             raise MeltanoError(
-                f"Azure state backend URI must include a container name: {self.uri}",
+                f"Azure state backend URI must include a container name: {self.uri}",  # noqa: EM102
                 "Verify state backend URI. Must be in the form of azure://<container>/<prefix>",  # noqa: E501
             )
 
         self.container_name = self.parsed.hostname
         self.prefix = prefix or self.parsed.path
 
     @staticmethod
@@ -119,15 +120,15 @@
                     credential=default_credential,
                 )
 
             if self.connection_string:
                 return BlobServiceClient.from_connection_string(self.connection_string)
 
             raise MeltanoError(
-                "Azure state backend requires a connection string "
+                "Azure state backend requires a connection string "  # noqa: EM101
                 "or an account URL to use host credentials",
                 "Read https://learn.microsoft.com/en-us/azure/storage/common/storage-configure-connection-string for more information.",  # noqa: E501
             )
 
     def delete(self, file_path: str):
         """Delete the file/blob at the given path.
```

### Comparing `meltano-3.3.2/src/meltano/core/state_store/base.py` & `meltano-3.4.0a1/src/meltano/core/state_store/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Storage managers for job state."""
+
 from __future__ import annotations
 
 import typing as t
 from abc import ABC, abstractmethod, abstractproperty
 
 if t.TYPE_CHECKING:
     from meltano.core.job_state import JobState
```

### Comparing `meltano-3.3.2/src/meltano/core/state_store/db.py` & `meltano-3.4.0a1/src/meltano/core/state_store/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """StateStoreManager for systemdb state backend."""
+
 from __future__ import annotations
 
 import typing as t
 
 from sqlalchemy import select
 
 from meltano.core.job_state import JobState
@@ -110,19 +111,19 @@
 
         For DBStateStoreManager, the db manages transactions.
         This does nothing.
 
         Args:
             state_id: the state_id to lock
         """
-        ...  # noqa: WPS428
+        # noqa: WPS428
 
     def release_lock(self, state_id):
         """Release the lock for the given job's state.
 
         For DBStateStoreManager, the db manages transactions.
         This does nothing.
 
         Args:
             state_id: the state_id to unlock
         """
-        ...  # noqa: WPS428
+        # noqa: WPS428
```

### Comparing `meltano-3.3.2/src/meltano/core/state_store/filesystem.py` & `meltano-3.4.0a1/src/meltano/core/state_store/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """StateStoreManagers for filesystems."""
+
 from __future__ import annotations
 
 import glob
 import logging
 import os
 import re
 import shutil
@@ -231,15 +232,14 @@
 
         Does nothing, but not @abstractmethod because many state backends
         will automatically create prefixes when files/blobs are created.
 
         Args:
             state_id: the state_id to create the dir/prefix for
         """
-        ...
 
     @contextmanager
     def acquire_lock(self, state_id: str, retry_seconds: int = 1) -> Iterator[None]:
         """Context manager for locking state_id during reads and writes.
 
         Args:
             state_id: the state_id to lock.
@@ -373,15 +373,15 @@
     @property
     def client(self):
         """Get a client for performing fs operations.
 
         Returns:
             None
         """
-        return None
+        return None  # noqa: RET501
 
     @property
     def state_dir(self) -> str:
         """Get the path that state should be stored at.
 
         Returns:
             The relevant path
```

### Comparing `meltano-3.3.2/src/meltano/core/state_store/google.py` & `meltano-3.4.0a1/src/meltano/core/state_store/google.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """StateStoreManager for Google Cloud storage backend."""
+
 from __future__ import annotations
 
 import typing as t
 from contextlib import contextmanager
 from functools import cached_property
 
 from meltano.core.state_store.filesystem import CloudStateStoreManager
```

### Comparing `meltano-3.3.2/src/meltano/core/state_store/s3.py` & `meltano-3.4.0a1/src/meltano/core/state_store/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """StateStoreManager for S3 cloud storage backend."""
+
 from __future__ import annotations
 
 import typing as t
 from contextlib import contextmanager
 from functools import cached_property
 
 from meltano.core.state_store.filesystem import (
@@ -107,21 +108,21 @@
         with requires_boto3():
             if self.aws_secret_access_key and self.aws_access_key_id:
                 session = boto3.Session(
                     aws_access_key_id=self.aws_access_key_id,
                     aws_secret_access_key=self.aws_secret_access_key,
                 )
                 return session.client("s3", endpoint_url=self.endpoint_url)
-            elif self.aws_secret_access_key:
+            if self.aws_secret_access_key:
                 raise InvalidStateBackendConfigurationException(
-                    "AWS secret access key configured, but not AWS access key ID.",
+                    "AWS secret access key configured, but not AWS access key ID.",  # noqa: EM101
                 )
-            elif self.aws_access_key_id:
+            if self.aws_access_key_id:
                 raise InvalidStateBackendConfigurationException(
-                    "AWS access key ID configured, but no AWS secret access key.",
+                    "AWS access key ID configured, but no AWS secret access key.",  # noqa: EM101
                 )
             session = boto3.Session()
             return session.client("s3")
 
     def delete(self, file_path: str):
         """Delete the file/blob at the given path.
```

### Comparing `meltano-3.3.2/src/meltano/core/task_sets.py` & `meltano-3.4.0a1/src/meltano/core/task_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """meltano tasks/jobs (not state related jobs)."""
+
 from __future__ import annotations
 
 from collections.abc import Iterable
 
 import structlog
 import yaml
 from jsonschema import validate
```

### Comparing `meltano-3.3.2/src/meltano/core/task_sets_service.py` & `meltano-3.4.0a1/src/meltano/core/task_sets_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Service for managing task sets (aka jobs)."""
+
 from __future__ import annotations
 
 import typing as t
 
 import structlog
 
 if t.TYPE_CHECKING:
```

### Comparing `meltano-3.3.2/src/meltano/core/tracking/README.md` & `meltano-3.4.0a1/src/meltano/core/tracking/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/contexts/cli.py` & `meltano-3.4.0a1/src/meltano/core/tracking/contexts/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Meltano telemetry contexts for the CLI events."""
+
 from __future__ import annotations
 
 import typing as t
 from enum import Enum, auto
 
 from snowplow_tracker import SelfDescribingJson
```

### Comparing `meltano-3.3.2/src/meltano/core/tracking/contexts/environment.py` & `meltano-3.4.0a1/src/meltano/core/tracking/contexts/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/contexts/exception.py` & `meltano-3.4.0a1/src/meltano/core/tracking/contexts/exception.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/contexts/plugins.py` & `meltano-3.4.0a1/src/meltano/core/tracking/contexts/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                 for plugin_block in blk.blocks
             ]
 
             return cls(plugins)
         if isinstance(blk, PluginCommandBlock):
             return cls([(blk.context.plugin, blk.command)])
         raise TypeError(
-            "Parameter 'blk' must be an instance of 'BlockSet' or "
+            "Parameter 'blk' must be an instance of 'BlockSet' or "  # noqa: EM102
             f"'PluginCommandBlock', not {type(blk)!r}",
         )
 
     @classmethod
     def from_blocks(
         cls,
         parsed_blocks: list[BlockSet | PluginCommandBlock],
```

### Comparing `meltano-3.3.2/src/meltano/core/tracking/contexts/project.py` & `meltano-3.4.0a1/src/meltano/core/tracking/contexts/project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0` & `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/micro.conf` & `meltano-3.4.0a1/src/meltano/core/tracking/micro.conf`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/schemas.py` & `meltano-3.4.0a1/src/meltano/core/tracking/schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/tracking/tracker.py` & `meltano-3.4.0a1/src/meltano/core/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/transform_add_service.py` & `meltano-3.4.0a1/src/meltano/core/transform_add_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         if not os.path.exists(self.packages_file):
             self.packages_file.touch()
 
         package_yaml = yaml.load(self.packages_file) or {"packages": []}
 
         git_repo = plugin.pip_url
         if not git_repo:
-            raise ValueError(f"Missing pip_url for transform plugin '{plugin.name}'")
+            raise ValueError(f"Missing pip_url for transform plugin '{plugin.name}'")  # noqa: EM102
 
         revision: str | None = None
         if len(git_repo.split("@")) == 2:
             git_repo, revision = git_repo.split("@")
         for package in package_yaml["packages"]:
             same_ref = (
                 package.get("git", "") == git_repo
```

### Comparing `meltano-3.3.2/src/meltano/core/upgrade_service.py` & `meltano-3.4.0a1/src/meltano/core/upgrade_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         run = subprocess.run(
             [sys.executable, "-m", "pip", "install", "--upgrade", pip_url],
             stderr=subprocess.PIPE,
             text=True,
         )
 
         if run.returncode != 0:
-            raise UpgradeError("Failed to upgrade `meltano`.", run)
+            raise UpgradeError("Failed to upgrade `meltano`.", run)  # noqa: EM101
 
         return True
 
     def upgrade_package(self, pip_url: str | None = None, force: bool = False) -> bool:
         """Upgrade the Meltano package.
 
         Args:
@@ -137,15 +137,15 @@
 
         success = install_plugins(
             self.project,
             file_plugins,
             reason=PluginInstallReason.UPGRADE,
         )
         if not success:
-            raise MeltanoError("Failed to upgrade plugin(s)")
+            raise MeltanoError("Failed to upgrade plugin(s)")  # noqa: EM101
 
     def migrate_database(self):
         """Migrate the Meltano database.
 
         Raises:
             UpgradeError: The migration failed.
         """
```

### Comparing `meltano-3.3.2/src/meltano/core/utils/__init__.py` & `meltano-3.4.0a1/src/meltano/core/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Defines helpers for the core codebase."""
 
-
 from __future__ import annotations
 
 import asyncio
 import collections
 import functools
 import hashlib
 import logging
@@ -256,15 +255,15 @@
     """
     return "_".join(re.sub("[^A-Za-z0-9]", "_", x).upper() for x in xs if x)
 
 
 def flatten(d: dict, reducer: str | t.Callable = "tuple", **kwargs):
     """Flatten a dictionary with `dot` and `env_var` reducers.
 
-    Wrapper arround `flatten_dict.flatten`.
+    Wrapper around `flatten_dict.flatten`.
 
     Args:
         d: the dict to flatten
         reducer: the reducer to flatten with
         **kwargs: additional kwargs to pass to flatten_dict.flatten
 
     Returns:
@@ -304,26 +303,23 @@
 
 
 def truthy(val: str) -> bool:
     return str(val).lower() in TRUTHY
 
 
 @t.overload
-def coerce_datetime(d: None) -> None:
-    ...  # noqa: WPS428
+def coerce_datetime(d: None) -> None: ...  # noqa: WPS428
 
 
 @t.overload
-def coerce_datetime(d: datetime) -> datetime:
-    ...  # noqa: WPS428
+def coerce_datetime(d: datetime) -> datetime: ...  # noqa: WPS428
 
 
 @t.overload
-def coerce_datetime(d: date) -> datetime:
-    ...  # noqa: WPS428
+def coerce_datetime(d: date) -> datetime: ...  # noqa: WPS428
 
 
 def coerce_datetime(d):
     """Add a `time` component to `d` if it is missing.
 
     Args:
         d: the date or datetime to add the time to
@@ -334,21 +330,19 @@
     if d is None:
         return None
 
     return d if isinstance(d, datetime) else datetime.combine(d, time())
 
 
 @t.overload
-def iso8601_datetime(d: None) -> None:
-    ...  # noqa: WPS428
+def iso8601_datetime(d: None) -> None: ...  # noqa: WPS428
 
 
 @t.overload
-def iso8601_datetime(d: str) -> datetime:
-    ...  # noqa: WPS428
+def iso8601_datetime(d: str) -> datetime: ...  # noqa: WPS428
 
 
 def iso8601_datetime(d):
     if d is None:
         return None
 
     isoformats = [
@@ -357,20 +351,19 @@
         "%Y-%m-%d %H:%M:%S",  # noqa: WPS323
         "%Y-%m-%d",  # noqa: WPS323
     ]
 
     for format_string in isoformats:
         with suppress(ValueError):
             return coerce_datetime(datetime.strptime(d, format_string))
-    raise ValueError(f"{d} is not a valid UTC date.")
+    raise ValueError(f"{d} is not a valid UTC date.")  # noqa: EM102
 
 
 class _GetItemProtocol(t.Protocol):
-    def __getitem__(self, key: str) -> str:
-        ...  # noqa: WPS428
+    def __getitem__(self, key: str) -> str: ...  # noqa: WPS428
 
 
 _G = t.TypeVar("_G", bound=_GetItemProtocol)
 
 
 def find_named(xs: t.Iterable[_G], name: str, obj_type: type | None = None) -> _G:
     """Find an object by its 'name' key.
@@ -393,15 +386,15 @@
 
 
 def makedirs(func):
     @functools.wraps(func)
     def decorate(*args, **kwargs):
         enabled = kwargs.pop("make_dirs", True)
 
-        path = func(*args, **kwargs)
+        path = func(*args, **kwargs, make_dirs=enabled)
 
         if not enabled:
             return path
 
         # if there is an extension, only create the base dir
         _, ext = os.path.splitext(path)
         os.makedirs(os.path.dirname(path) if ext else path, exist_ok=True)
@@ -538,15 +531,15 @@
             val = str(env[var])
         except KeyError as ex:
             logger.debug(
                 f"Variable '${var}' is not set in the provided env dictionary.",  # noqa: G004
             )
             if if_missing == EnvVarMissingBehavior.raise_exception:
                 raise EnvironmentVariableNotSetError(var) from ex
-            elif if_missing == EnvVarMissingBehavior.ignore:
+            if if_missing == EnvVarMissingBehavior.ignore:
                 return f"${{{var}}}"
             return ""
         if not val:
             logger.debug(f"Variable '${var}' is empty.")  # noqa: G004
         return val
 
     return _expand_env_vars(raw_value, replacer, flat)
@@ -628,15 +621,15 @@
     Returns:
         The hashed value of the given string.
 
     Raises:
         ValueError: If we are blindly passed a value that is None.
     """
     if value is None:
-        raise ValueError("Cannot hash None.")
+        raise ValueError("Cannot hash None.")  # noqa: EM101
     if isinstance(value, str):
         value = value.encode()
     return hashlib.sha256(value).hexdigest()
 
 
 def format_exception(exception: BaseException) -> str:
     """Get the exception with its traceback formatted as it would have been printed.
@@ -691,18 +684,18 @@
 
     Raises:
         ValueError: If the string is not a valid representation of a boolean.
     """
     val = val.lower()
     if val in {"y", "yes", "t", "true", "on", "1"}:
         return True
-    elif val in {"n", "no", "f", "false", "off", "0"}:
+    if val in {"n", "no", "f", "false", "off", "0"}:
         return False
 
-    raise ValueError(f"invalid truth value {val!r}")
+    raise ValueError(f"invalid truth value {val!r}")  # noqa: EM102
 
 
 def get_boolean_env_var(env_var: str, default: bool = False) -> bool:
     """Get the value of an environment variable as a boolean.
 
     Args:
         env_var: The name of the environment variable.
@@ -830,15 +823,15 @@
         suffix: the suffix to remove
 
     Returns:
         The changed string
     """
     if sys.version_info >= (3, 9):
         return string.removesuffix(suffix)
-    elif string.endswith(suffix):
+    if string.endswith(suffix):
         return string[: -len(suffix)]
     return string
 
 
 _filename_restriction_pattern = re.compile(r"[^\w.-]")
 _reserved_windows_filenames = frozenset(
     (
@@ -881,15 +874,15 @@
 def sanitize_filename(filename: str) -> str:
     """Sanitize `filename` in a consistent cross-platform way.
 
     Args:
         filename: The name of the file to sanitize - not the full path.
 
     Returns:
-        The provided filename after a series of santitization steps. It will
+        The provided filename after a series of sanitization steps. It will
         only contain ASCII characters. If necessary on Windows, the filename
         will be prefixed by an underscore to avoid conflict with reserved
         Windows file names.
     """
     return functools.reduce(
         lambda x, y: y(x),  # noqa: WPS442
         _sanitize_filename_transformations,
```

### Comparing `meltano-3.3.2/src/meltano/core/utils/pidfile.py` & `meltano-3.4.0a1/src/meltano/core/utils/pidfile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/core/validation_service.py` & `meltano-3.4.0a1/src/meltano/core/validation_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         Raises:
             KeyError: If plugin test is not defined.
         """
         try:
             self.tests_selection[name] = True
         except KeyError as exc:
             raise KeyError(
-                f"Plugin {self.plugin_name} does not have a test named '{name}'",
+                f"Plugin {self.plugin_name} does not have a test named '{name}'",  # noqa: EM102
             ) from exc
 
     def select_all(self) -> None:
         """Mark all plugin validators as selected."""
         for name in self.tests_selection:
             self.tests_selection[name] = True
```

### Comparing `meltano-3.3.2/src/meltano/core/venv_service.py` & `meltano-3.4.0a1/src/meltano/core/venv_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,39 +49,39 @@
                 $PATH. Defaults to the Python executable running Meltano.
 
         Raises:
             MeltanoError: The current system is not supported.
         """
         self._system = platform.system()
         if self._system not in self._SUPPORTED_PLATFORMS:
-            raise MeltanoError(f"Platform {self._system!r} not supported.")
+            raise MeltanoError(f"Platform {self._system!r} not supported.")  # noqa: EM102
         self.root = root.resolve()
         self.python_path = self._resolve_python_path(python)
 
     @staticmethod
     def _resolve_python_path(python: Path | str | None) -> str:
         python_path: str | None = None
 
         if python is None:
             python_path = sys.executable
         elif isinstance(python, Path):
             python_path = str(python.resolve())
         elif isinstance(python, Number):
             raise MeltanoError(
-                "Python must be specified as an executable name or path, "
+                "Python must be specified as an executable name or path, "  # noqa: EM102
                 f"not the number {python!r}",
             )
         else:
             python_path = python if os.path.exists(python) else shutil.which(python)
 
         if python_path is None:
-            raise MeltanoError(f"Python executable {python!r} was not found")
+            raise MeltanoError(f"Python executable {python!r} was not found")  # noqa: EM102
 
         if not os.access(python_path, os.X_OK):
-            raise MeltanoError(f"{python_path!r} is not executable")
+            raise MeltanoError(f"{python_path!r} is not executable")  # noqa: EM102
 
         return python_path
 
     @cached_property
     def lib_dir(self) -> Path:
         """Return the lib directory of the virtual environment.
 
@@ -89,33 +89,33 @@
             MeltanoError: The current system is not supported.
 
         Returns:
             The lib directory of the virtual environment.
         """
         if self._system in {"Linux", "Darwin"}:
             return self.root / "lib"
-        elif self._system == "Windows":
+        if self._system == "Windows":
             return self.root / "Lib"
-        raise MeltanoError(f"Platform {self._system!r} not supported.")
+        raise MeltanoError(f"Platform {self._system!r} not supported.")  # noqa: EM102
 
     @cached_property
     def bin_dir(self) -> Path:
         """Return the bin directory of the virtual environment.
 
         Raises:
             MeltanoError: The current system is not supported.
 
         Returns:
             The bin directory of the virtual environment.
         """
         if self._system in {"Linux", "Darwin"}:
             return self.root / "bin"
-        elif self._system == "Windows":
+        if self._system == "Windows":
             return self.root / "Scripts"
-        raise MeltanoError(f"Platform {self._system!r} not supported.")
+        raise MeltanoError(f"Platform {self._system!r} not supported.")  # noqa: EM102
 
     @cached_property
     def site_packages_dir(self) -> Path:
         """Return the site-packages directory of the virtual environment.
 
         Raises:
             MeltanoError: The current system is not supported.
@@ -125,17 +125,17 @@
         """
         if self._system in {"Linux", "Darwin"}:
             return (
                 self.lib_dir
                 / f"python{'.'.join(str(x) for x in self.python_version_tuple[:2])}"
                 / "site-packages"
             )
-        elif self._system == "Windows":
+        if self._system == "Windows":
             return self.lib_dir / "site-packages"
-        raise MeltanoError(f"Platform {self._system!r} not supported.")
+        raise MeltanoError(f"Platform {self._system!r} not supported.")  # noqa: EM102
 
     @cached_property
     def python_version_tuple(self) -> tuple[int, int, int]:
         """Return the Python version tuple of the virtual environment.
 
         Returns:
             The Python version tuple of the virtual environment.
@@ -183,15 +183,15 @@
         stderr=subprocess.STDOUT,
         **kwargs,
     )
     await run.wait()
 
     if run.returncode != 0:
         raise AsyncSubprocessError(
-            "Command failed",
+            "Command failed",  # noqa: EM101
             process=run,
             stderr=await extract_stderr(run),
         )
 
     return run
 
 
@@ -232,15 +232,15 @@
             namespace: The namespace for the venv, e.g. a Plugin type.
             name: The name of the venv, e.g. a Plugin name.
         """
         self.project = project
         self.namespace = namespace
         self.name = name
         self.venv = VirtualEnv(
-            self.project.venvs_dir(namespace, name),
+            self.project.venvs_dir(namespace, name, make_dirs=False),
             python or project.settings.get("python"),
         )
         self.plugin_fingerprint_path = self.venv.root / ".meltano_plugin_fingerprint"
         self.pip_log_path = self.project.logs_dir(
             "pip",
             self.namespace,
             self.name,
@@ -336,15 +336,15 @@
                 "--python",
                 self.venv.python_path,
                 str(self.venv.root),
                 extract_stderr=extract_stderr,
             )
         except AsyncSubprocessError as err:
             raise AsyncSubprocessError(
-                f"Could not create the virtualenv for '{self.namespace}/{self.name}'",
+                f"Could not create the virtualenv for '{self.namespace}/{self.name}'",  # noqa: EM102
                 process=err.process,
                 stderr=await err.stderr,
             ) from err
 
     async def upgrade_pip(self) -> Process:
         """Upgrade the `pip` package to the latest version in the virtual environment.
 
@@ -355,15 +355,15 @@
             The process running `pip install --upgrade ...`.
         """
         logger.debug(f"Upgrading pip for '{self.namespace}/{self.name}'")  # noqa: G004
         try:
             return await self._pip_install(("--upgrade", "pip"))
         except AsyncSubprocessError as err:
             raise AsyncSubprocessError(
-                "Failed to upgrade pip to the latest version.",
+                "Failed to upgrade pip to the latest version.",  # noqa: EM101
                 err.process,
             ) from err
 
     def read_fingerprint(self) -> str | None:
         """Get the fingerprint of the existing virtual environment.
 
         Returns:
@@ -457,11 +457,11 @@
             )
         except AsyncSubprocessError as err:
             logger.info(
                 "Logged pip install output to %s",  # noqa: WPS323
                 self.pip_log_path,
             )
             raise AsyncSubprocessError(
-                f"Failed to install plugin '{self.name}'.",
+                f"Failed to install plugin '{self.name}'.",  # noqa: EM102
                 err.process,
                 stderr=await err.stderr,
             ) from err
```

### Comparing `meltano-3.3.2/src/meltano/core/yaml.py` & `meltano-3.4.0a1/src/meltano/core/yaml.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/env.py` & `meltano-3.4.0a1/src/meltano/migrations/env.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/utils/dialect_typing.py` & `meltano-3.4.0a1/src/meltano/migrations/utils/dialect_typing.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/6ef30ab7b8e5_.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/6ef30ab7b8e5_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/b4c05e463b53_.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/b4c05e463b53_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py` & `meltano-3.4.0a1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/src/meltano/schemas/meltano.schema.json` & `meltano-3.4.0a1/src/meltano/schemas/meltano.schema.json`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/conftest.py` & `meltano-3.4.0a1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 elif PYTEST_BACKEND == "postgresql":
     pytest_plugins.append("fixtures.db.postgresql")
 elif PYTEST_BACKEND == "postgresql_psycopg3":
     pytest_plugins.append("fixtures.db.postgresql_psycopg3")
 elif PYTEST_BACKEND == "mssql":
     pytest_plugins.append("fixtures.db.mssql")
 else:
-    raise Exception(f"Unsuported backend: {PYTEST_BACKEND}.")
+    raise Exception(f"Unsuported backend: {PYTEST_BACKEND}.")  # noqa: EM102
 
 BACKEND = ["sqlite", "postgresql", "mssql", "mysql"]
 
 
 def pytest_runtest_setup(item):
     backend_marker = item.get_closest_marker("backend")
 
@@ -126,17 +126,17 @@
                         "repo": plugin.get("repo"),
                         "pip_url": plugin.get("pip_url"),
                     }
 
                     if "dialect" in plugin:
                         hub[plugin_key]["dialect"] = plugin["dialect"]
 
-                hub[index_key][plugin_name][
-                    "logo_url"
-                ] = f"https://mock.meltano.com/{plugin_name}.png"
+                hub[index_key][plugin_name]["logo_url"] = (
+                    f"https://mock.meltano.com/{plugin_name}.png"
+                )
                 hub[index_key][plugin_name]["default_variant"] = default_variant
 
         return hub
 
     def __init__(self, api_url: str, discovery: dict) -> None:
         """Create a mock HTTP adapter for the Hub.
```

### Comparing `meltano-3.3.2/tests/fixtures/cli.py` & `meltano-3.4.0a1/tests/fixtures/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/core.py` & `meltano-3.4.0a1/tests/fixtures/core.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/db/__init__.py` & `meltano-3.4.0a1/tests/fixtures/db/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/db/mssql.py` & `meltano-3.4.0a1/tests/fixtures/db/mssql.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/db/postgresql.py` & `meltano-3.4.0a1/tests/fixtures/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/db/postgresql_psycopg3.py` & `meltano-3.4.0a1/tests/fixtures/db/postgresql_psycopg3.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/docker/__init__.py` & `meltano-3.4.0a1/tests/fixtures/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/docker/snowplow.py` & `meltano-3.4.0a1/tests/fixtures/docker/snowplow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/fs.py` & `meltano-3.4.0a1/tests/fixtures/fs.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/large_config_project/meltano.yml` & `meltano-3.4.0a1/tests/fixtures/large_config_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/large_config_project/schedule.yml` & `meltano-3.4.0a1/tests/fixtures/large_config_project/schedule.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/multifile_project/meltano.yml` & `meltano-3.4.0a1/tests/fixtures/multifile_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/plugins/extractors/tap-custom/test.yml` & `meltano-3.4.0a1/tests/fixtures/plugins/extractors/tap-custom/test.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/fixtures/utils.py` & `meltano-3.4.0a1/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_add.py` & `meltano-3.4.0a1/tests/meltano/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_cli.py` & `meltano-3.4.0a1/tests/meltano/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_compile.py` & `meltano-3.4.0a1/tests/meltano/cli/test_compile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_config.py` & `meltano-3.4.0a1/tests/meltano/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_elt.py` & `meltano-3.4.0a1/tests/meltano/cli/test_elt.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
         Args:
             lines: the log lines to check against
 
         Returns:
             True if a matching log line is found, else False
         """
-        for line in lines:
+        for line in lines:  # noqa: RET503
             matches = (
                 line.get("name") == self.name
                 and line.get("cmd_type") == self.cmd_type
                 and line.get("event").startswith(self.event)
                 and line.get("level") == self.level
             )
 
@@ -200,15 +200,15 @@
         cli_runner,
         tap,
         target,
     ):
         args = ["elt", tap.name, target.name]
         result = cli_runner.invoke(cli, args)
         assert result.exit_code == 1
-        # Didn't use `exception_logged()` as `result.stderr` doensn't contain
+        # Didn't use `exception_logged()` as `result.stderr` doesn't contain
         # the error for some reason
         assert (
             "ELT command not supported on Windows. Please use the run command "
             "as documented here: "
             "https://docs.meltano.com/reference/command-line-interface#run"
         ) in str(result.exception)
 
@@ -723,15 +723,15 @@
         args = [command, "--state-id", state_id, tap.name, target.name]
 
         # Raise a `ValueError` wrapping a `LimitOverrunError`, like
         # `StreamReader.readline` does:
         # https://github.com/python/cpython/blob/v3.8.7/Lib/asyncio/streams.py#L549
         try:  # noqa: WPS328
             raise asyncio.LimitOverrunError(
-                "Separator is not found, and chunk exceed the limit",
+                "Separator is not found, and chunk exceed the limit",  # noqa: EM101
                 0,
             )
         except asyncio.LimitOverrunError as err:
             try:  # noqa: WPS328, WPS505
                 # `ValueError` needs to be raised from inside the except block
                 # for `LimitOverrunError` so that `__context__` is set.
                 raise ValueError(str(err))
```

### Comparing `meltano-3.3.2/tests/meltano/cli/test_hub.py` & `meltano-3.4.0a1/tests/meltano/cli/test_hub.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_initialize.py` & `meltano-3.4.0a1/tests/meltano/cli/test_initialize.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_install.py` & `meltano-3.4.0a1/tests/meltano/cli/test_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,28 @@
                 project,
                 [tap, tap_gitlab, target, dbt],
                 parallelism=None,
                 clean=False,
                 force=False,
             )
 
+        with mock.patch("meltano.cli.install.install_plugins") as install_plugin_mock:
+            install_plugin_mock.return_value = True
+
+            result = cli_runner.invoke(cli, ["install", "-"])
+            assert_cli_runner(result)
+
+            install_plugin_mock.assert_called_once_with(
+                project,
+                [tap, tap_gitlab, target, dbt],
+                parallelism=None,
+                clean=False,
+                force=False,
+            )
+
     @pytest.mark.usefixtures("dbt")
     def test_install_type(
         self,
         project,
         tap,
         tap_gitlab,
         target,
@@ -160,14 +174,33 @@
                 project,
                 [tap, tap_gitlab],
                 parallelism=None,
                 clean=False,
                 force=False,
             )
 
+    @pytest.mark.usefixtures("dbt")
+    def test_install_multiple_any_type(self, project, tap, target, dbt, cli_runner):
+        with mock.patch("meltano.cli.install.install_plugins") as install_plugin_mock:
+            install_plugin_mock.return_value = True
+
+            result = cli_runner.invoke(
+                cli,
+                ["install", "-", tap.name, target.name, dbt.name],
+            )
+            assert_cli_runner(result)
+
+            install_plugin_mock.assert_called_once_with(
+                project,
+                [tap, target, dbt],
+                parallelism=None,
+                clean=False,
+                force=False,
+            )
+
     def test_install_parallel(
         self,
         project,
         tap,
         tap_gitlab,
         target,
         dbt,
```

### Comparing `meltano-3.3.2/tests/meltano/cli/test_invoke.py` & `meltano-3.4.0a1/tests/meltano/cli/test_invoke.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_job_cmd.py` & `meltano-3.4.0a1/tests/meltano/cli/test_job_cmd.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_lock.py` & `meltano-3.4.0a1/tests/meltano/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_remove.py` & `meltano-3.4.0a1/tests/meltano/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_run.py` & `meltano-3.4.0a1/tests/meltano/cli/test_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
         Args:
             event: the event to search for.
 
         Returns:
             True if the event was found, False otherwise.
         """
-        for line in self.seen_events:
+        for line in self.seen_events:  # noqa: RET503
             matches = line["event"] == event
             if matches:
                 return True
 
     def find_by_event(self, event: str) -> list[dict] | None:
         """Return the first matching event, that matches the given event.
 
@@ -932,15 +932,15 @@
         args = ["run", tap.name, target.name]
 
         # Raise a `ValueError` wrapping a `LimitOverrunError`, like
         # `StreamReader.readline` does:
         # https://github.com/python/cpython/blob/v3.8.7/Lib/asyncio/streams.py#L549
         try:  # noqa: WPS328
             raise asyncio.LimitOverrunError(
-                "Separator is not found, and chunk exceed the limit",
+                "Separator is not found, and chunk exceed the limit",  # noqa: EM101
                 0,
             )
         except asyncio.LimitOverrunError as err:
             try:  # noqa: WPS328, WPS505
                 # `ValueError` needs to be raised from inside the except block
                 # for `LimitOverrunError` so that `__context__` is set.
                 raise ValueError(str(err))
```

### Comparing `meltano-3.3.2/tests/meltano/cli/test_schedule.py` & `meltano-3.4.0a1/tests/meltano/cli/test_schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_select.py` & `meltano-3.4.0a1/tests/meltano/cli/test_select.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_state.py` & `meltano-3.4.0a1/tests/meltano/cli/test_state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/cli/test_upgrade.py` & `meltano-3.4.0a1/tests/meltano/cli/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/behavior/test_canonical.py` & `meltano-3.4.0a1/tests/meltano/core/behavior/test_canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/behavior/test_hookable.py` & `meltano-3.4.0a1/tests/meltano/core/behavior/test_hookable.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/block/test_extract_load.py` & `meltano-3.4.0a1/tests/meltano/core/block/test_extract_load.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/block/test_plugin_command.py` & `meltano-3.4.0a1/tests/meltano/core/block/test_plugin_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/block/test_singer.py` & `meltano-3.4.0a1/tests/meltano/core/block/test_singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/container/test_container_spec.py` & `meltano-3.4.0a1/tests/meltano/core/container/test_container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/hub/test_meltano_hub_service.py` & `meltano-3.4.0a1/tests/meltano/core/hub/test_meltano_hub_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/job/test_finder.py` & `meltano-3.4.0a1/tests/meltano/core/job/test_finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/job/test_job.py` & `meltano-3.4.0a1/tests/meltano/core/job/test_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def test_save(self, session):
         subject = self.sample_job().save(session)
 
         assert subject.id > 0
 
     def test_load(self, session):
-        for key in range(0, 10):
+        for key in range(10):
             session.add(self.sample_job({"key": key}))
 
         subjects = session.query(Job).filter_by(job_name="meltano:sample-elt")
 
         assert len(subjects.all()) == 10
         session.rollback()
```

### Comparing `meltano-3.3.2/tests/meltano/core/job/test_stale_job_failer.py` & `meltano-3.4.0a1/tests/meltano/core/job/test_stale_job_failer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/logging/test_formatters.py` & `meltano-3.4.0a1/tests/meltano/core/logging/test_formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 
 
 class FakeTraceback:  # pragma: no cover
     """A fake traceback that can be used to test log formatters."""
 
     def __init__(self, frames, line_nums):
         if len(frames) != len(line_nums):
-            raise ValueError("Ya messed up!")
+            raise ValueError("Ya messed up!")  # noqa: EM101
         self._frames = frames
         self._line_nums = line_nums
         self.tb_frame = frames[0]
         self.tb_lineno = line_nums[0]
 
     @property
     def tb_next(self):
-        if len(self._frames) > 1:
+        if len(self._frames) > 1:  # noqa: RET503
             return FakeTraceback(self._frames[1:], self._line_nums[1:])
 
 
 class TestLogFormatters:
     @pytest.fixture()
     def record(self):
         return logging.LogRecord(
```

### Comparing `meltano-3.3.2/tests/meltano/core/logging/test_logging_utils.py` & `meltano-3.4.0a1/tests/meltano/core/logging/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/logging/test_output_logger.py` & `meltano-3.4.0a1/tests/meltano/core/logging/test_output_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         stdout_out = subject.out("stdout")
         stderr_out = subject.out("stderr")
 
         async with stdout_out.redirect_stdout():
             sys.stdout.write("STD")
             sys.stdout.write("OUT\n")
-            print("STDOUT 2")  # noqa: WPS421
+            print("STDOUT 2")  # noqa: T201, WPS421
 
         assert_lines(
             log_output.entries,
             {
                 "name": "stdout",
                 "event": "STDOUT",
                 "log_level": "info",
@@ -84,15 +84,15 @@
                 "log_level": "info",
             },
         )
 
         async with stderr_out.redirect_stderr():
             sys.stderr.write("STD")
             sys.stderr.write("ERR\n")
-            print("STDERR 2", file=sys.stderr)  # noqa: WPS421
+            print("STDERR 2", file=sys.stderr)  # noqa: T201, WPS421
 
         assert_lines(
             log_output.entries,
             {
                 "name": "stderr",
                 "event": "STDERR",
                 "log_level": "info",
```

### Comparing `meltano-3.3.2/tests/meltano/core/plugin/singer/test_catalog.py` & `meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_catalog.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/plugin/singer/test_mapper.py` & `meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_mapper.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/plugin/singer/test_tap.py` & `meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_tap.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/plugin/singer/test_target.py` & `meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_target.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/plugin/test_airflow.py` & `meltano-3.4.0a1/tests/meltano/core/plugin/test_airflow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/plugin/test_command.py` & `meltano-3.4.0a1/tests/meltano/core/plugin/test_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/plugin/test_plugin.py` & `meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/plugin/test_plugin_settings.py` & `meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin_settings.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/plugin/test_superset.py` & `meltano-3.4.0a1/tests/meltano/core/plugin/test_superset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/runner/test_runner.py` & `meltano-3.4.0a1/tests/meltano/core/runner/test_runner.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/state_store/test_db.py` & `meltano-3.4.0a1/tests/meltano/core/state_store/test_db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/state_store/test_filesystem.py` & `meltano-3.4.0a1/tests/meltano/core/state_store/test_filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import pytest
 from azure.core.exceptions import ResourceNotFoundError
 from azure.storage.blob._models import BlobProperties  # noqa: WPS436
 from boto3 import client
 from botocore.stub import Stubber
 from dateutil.tz import tzutc
-from google.api_core.exceptions import NotFound as GCSNotFound
 from google.cloud.storage import Blob, Bucket
 
 from meltano.core.job_state import JobState
 from meltano.core.state_store import (
     AZStorageStateStoreManager,
     GCSStateStoreManager,
     LocalFilesystemStateStoreManager,
@@ -520,18 +519,16 @@
 
     @pytest.mark.usefixtures("mock_client")
     def test_is_file_not_found_error_true(
         self,
         subject: GCSStateStoreManager,
     ):
         got_reader = False
-        mock_blob = MagicMock()
-        mock_blob.open.side_effect = GCSNotFound("No such object: nonexistent")
         mock_bucket = MagicMock()
-        mock_bucket.blob.return_value = mock_blob
+        mock_bucket.get_blob.return_value = None
         subject.client.bucket.return_value = mock_bucket
         try:
             with subject.get_reader("nonexistent"):
                 got_reader = True
         except Exception as e:
             assert subject.is_file_not_found_error(e)  # noqa: PT017
         assert not got_reader
```

### Comparing `meltano-3.3.2/tests/meltano/core/state_store/test_state_store.py` & `meltano-3.4.0a1/tests/meltano/core/state_store/test_state_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_db_compat.py` & `meltano-3.4.0a1/tests/meltano/core/test_db_compat.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_db_connection.py` & `meltano-3.4.0a1/tests/meltano/core/test_db_connection.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_elt_context.py` & `meltano-3.4.0a1/tests/meltano/core/test_elt_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_environment_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_environment_variables.py` & `meltano-3.4.0a1/tests/meltano/core/test_environment_variables.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_locked_definition_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_locked_definition_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             "tap_locked",
             variant="meltano",
             foo="bar",
         )
         path = subject.project.plugin_lock_path(
             definition.plugin_type,
             definition.name,
-            definition.variant,
+            variant_name=definition.variant,
         )
         with path.open("w") as file:
             json.dump(definition.canonical(), file)
         yield definition
 
         path.unlink()
```

### Comparing `meltano-3.3.2/tests/meltano/core/test_meltano_file.py` & `meltano-3.4.0a1/tests/meltano/core/test_meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_meltano_invoker.py` & `meltano-3.4.0a1/tests/meltano/core/test_meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_plugin_install_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_plugin_install_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_plugin_invoker.py` & `meltano-3.4.0a1/tests/meltano/core/test_plugin_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_plugin_lock_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_plugin_lock_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_plugin_remove_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_plugin_remove_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,20 +54,20 @@
         os.makedirs(target_csv_installation, exist_ok=True)
 
     @pytest.fixture()
     def lock(self, subject: PluginRemoveService):
         tap_gitlab_lockfile = subject.project.plugin_lock_path(
             "extractors",
             "tap-gitlab",
-            "meltanolabs",
+            variant_name="meltanolabs",
         )
         target_csv_lockfile = subject.project.plugin_lock_path(
             "loaders",
             "target-csv",
-            "hotgluexyz",
+            variant_name="hotgluexyz",
         )
         tap_gitlab_lockfile.touch()
         target_csv_lockfile.touch()
 
     def test_default_init_should_not_fail(self, subject):
         assert subject
```

### Comparing `meltano-3.3.2/tests/meltano/core/test_plugin_test_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_plugin_test_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_project.py` & `meltano-3.4.0a1/tests/meltano/core/test_project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_project_add_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_project_add_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         )
         assert parent_path.stem == "tap-mock--meltano"
         assert parent_path.exists()
 
         child_path = subject.project.plugin_lock_path(
             child.type,
             child.name,
-            child.variant,
+            variant_name=child.variant,
         )
         assert child_path.stem == "tap-mock-inherited-new--meltano"
         assert not child_path.exists()
 
         grandchild = subject.add(
             PluginType.EXTRACTORS,
             "tap-mock-inherited-new-2",
@@ -157,15 +157,15 @@
         assert isinstance(grandchild.parent, ProjectPlugin)
         assert grandchild.parent.name == "tap-mock-inherited-new"
         assert grandchild.parent.parent.name == "tap-mock"
 
         grandchild_path = subject.project.plugin_lock_path(
             grandchild.type,
             grandchild.name,
-            grandchild.variant,
+            variant_name=grandchild.variant,
         )
         assert grandchild_path.stem == "tap-mock-inherited-new-2--meltano"
         assert not grandchild_path.exists()
 
         matches = list(parent_path.parent.glob("tap-mock-inherited-new*"))
         assert not matches
```

### Comparing `meltano-3.3.2/tests/meltano/core/test_project_files.py` & `meltano-3.4.0a1/tests/meltano/core/test_project_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,20 +225,20 @@
         read_result = project_files.load()
         assert read_result == expected_result
 
     @pytest.mark.order(6)
     def test_update(self, project_files):
         meltano_config = project_files.load()
         meltano_config["version"] = 2
-        meltano_config["plugins"]["extractors"][1][
-            "name"
-        ] = "modified-tap-subconfig-2-yml"
-        meltano_config["plugins"]["loaders"][2][
-            "name"
-        ] = "modified-target-subconfig-1-yml"
+        meltano_config["plugins"]["extractors"][1]["name"] = (
+            "modified-tap-subconfig-2-yml"
+        )
+        meltano_config["plugins"]["loaders"][2]["name"] = (
+            "modified-target-subconfig-1-yml"
+        )
         meltano_config["schedules"][0]["name"] = "modified-test-meltano-yml"
 
         project_files.update(meltano_config)
         expected_result = {
             "default_environment": "test-meltano-environment",
             "database_uri": "sqlite:///.meltano/meltano.db",
             "include_paths": [
```

### Comparing `meltano-3.3.2/tests/meltano/core/test_project_init_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_project_init_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_project_plugins_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_project_plugins_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_project_settings_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_schedule_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_schedule_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_setting_definition.py` & `meltano-3.4.0a1/tests/meltano/core/test_setting_definition.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_settings_store.py` & `meltano-3.4.0a1/tests/meltano/core/test_settings_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_state_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_state_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_task_sets.py` & `meltano-3.4.0a1/tests/meltano/core/test_task_sets.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_task_sets_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_task_sets_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_utils.py` & `meltano-3.4.0a1/tests/meltano/core/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pytest  # noqa: F401
 
 from meltano.core.utils import (
     EnvVarMissingBehavior,
     expand_env_vars,
     flatten,
+    makedirs,
     nest,
     pop_at_path,
     remove_suffix,
     set_at_path,
 )
 
 
@@ -218,7 +219,26 @@
     assert expand_env_vars(input_array, env) == expected_output
 
 
 def test_remove_suffix():
     assert remove_suffix("a_string", "ing") == "a_str"
     assert remove_suffix("a_string", "in") == "a_string"
     assert remove_suffix("a_string", "gni") == "a_string"
+
+
+def test_makedirs_decorator(tmp_path):
+    def root(*paths):
+        return tmp_path.joinpath(*paths)
+
+    @makedirs
+    def hierarchy(*ranks, make_dirs: bool = True):  # noqa: ARG001
+        return root(*ranks)
+
+    @makedirs
+    def species(genus_name, species_name, make_dirs: bool = True):  # noqa: ARG001
+        return hierarchy(genus_name, species_name, make_dirs=make_dirs)
+
+    cat = species("felis", "catus")
+    assert cat.exists()
+
+    wolf = species("canis", "lupus", make_dirs=False)
+    assert not wolf.exists()
```

### Comparing `meltano-3.3.2/tests/meltano/core/test_validation_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_validation_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/test_venv_service.py` & `meltano-3.4.0a1/tests/meltano/core/test_venv_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/tracking/test_environment_context.py` & `meltano-3.4.0a1/tests/meltano/core/tracking/test_environment_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/tracking/test_exception.py` & `meltano-3.4.0a1/tests/meltano/core/tracking/test_exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         try:
             line_nums.append(1 + inspect.currentframe().f_lineno)
             Path("/tmp/fake/path/will/not/resolve").resolve(strict=True)  # noqa: S108
         except Exception as ex:
             nonlocal file_not_found_error
             file_not_found_error = ex
             line_nums.append(1 + inspect.currentframe().f_lineno)
-            raise ValueError("that path was a bad value") from ex
+            raise ValueError("that path was a bad value") from ex  # noqa: EM101
 
     try:
         try:  # noqa: WPS505
             line_nums.append(1 + inspect.currentframe().f_lineno)
             _function_to_deepen_traceback()
         except Exception:
             line_nums.append(1 + inspect.currentframe().f_lineno)
```

### Comparing `meltano-3.3.2/tests/meltano/core/tracking/test_plugins.py` & `meltano-3.4.0a1/tests/meltano/core/tracking/test_plugins.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/tracking/test_project_context.py` & `meltano-3.4.0a1/tests/meltano/core/tracking/test_project_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/tracking/test_schemas.py` & `meltano-3.4.0a1/tests/meltano/core/tracking/test_schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/tests/meltano/core/tracking/test_tracker.py` & `meltano-3.4.0a1/tests/meltano/core/tracking/test_tracker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.3.2/PKG-INFO` & `meltano-3.4.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltano
-Version: 3.3.2
+Version: 3.4.0a1
 Summary: Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love.
 Home-page: https://meltano.com
 License: MIT
 Keywords: Meltano,ELT,Data integration,singer-io,dbt
 Author: Meltano
 Author-email: hello@meltano.com
 Requires-Python: >=3.8,<3.13
@@ -24,49 +24,49 @@
 Provides-Extra: postgres
 Provides-Extra: psycopg2
 Provides-Extra: s3
 Requires-Dist: aiodocker (>=0.21.0,<0.22.0)
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: atomicwrites (>=1.2.1,<2.0.0)
 Requires-Dist: azure-common (>=1.1.28,<2.0.0) ; extra == "azure"
-Requires-Dist: azure-core (>=1.30.0,<2.0.0) ; extra == "azure"
+Requires-Dist: azure-core (>=1.30.1,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0) ; extra == "azure"
-Requires-Dist: azure-storage-blob (>=12.19.0,<13.0.0) ; extra == "azure"
-Requires-Dist: boto3 (>=1.34.49,<2.0.0) ; extra == "s3"
-Requires-Dist: check-jsonschema (>=0.28.0,<0.29.0)
+Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0) ; extra == "azure"
+Requires-Dist: boto3 (>=1.34.74,<2.0.0) ; extra == "s3"
+Requires-Dist: check-jsonschema (>=0.28.1,<0.29.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: click-default-group (>=1.2.4,<2.0.0)
-Requires-Dist: click-didyoumean (>=0.3.0,<0.4.0)
-Requires-Dist: croniter (>=2.0.1,<3.0.0)
+Requires-Dist: click-didyoumean (>=0.3.1,<0.4.0)
+Requires-Dist: croniter (>=2.0.3,<3.0.0)
 Requires-Dist: fasteners (>=0.19,<0.20)
 Requires-Dist: flatten-dict (>=0,<1)
 Requires-Dist: google-cloud-storage (>=1.31.0) ; extra == "gcs"
-Requires-Dist: importlib-resources (>=6.1.2,<7.0.0)
+Requires-Dist: importlib-resources (>=6.4.0,<7.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: jsonschema (>=4.21,<5.0)
-Requires-Dist: packaging (>=23.2,<24.0)
+Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) ; extra == "psycopg2"
 Requires-Dist: psycopg[binary] (>=3.1.18,<4.0.0) ; extra == "postgres"
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: pymssql (>=2.2.11,<3.0.0) ; extra == "mssql"
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-slugify (>=8.0.4,<9.0.0)
 Requires-Dist: python-ulid (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
-Requires-Dist: ruamel.yaml (>=0.18.5,<0.19.0)
-Requires-Dist: setuptools (>=69.1.1,<70.0.0) ; python_version >= "3.12"
-Requires-Dist: smart-open (>=7.0.1,<8.0.0)
-Requires-Dist: snowplow-tracker (>=1.0.1,<2.0.0)
-Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: ruamel.yaml (>=0.18.6,<0.19.0)
+Requires-Dist: setuptools (>=69.2.0,<70.0.0) ; python_version >= "3.12"
+Requires-Dist: smart-open (>=7.0.4,<8.0.0)
+Requires-Dist: snowplow-tracker (>=1.0.2,<2.0.0)
+Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Requires-Dist: tzlocal (>=5.2,<6.0)
 Requires-Dist: urllib3 (<2)
 Requires-Dist: virtualenv (>=20.25.1,<21.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
```

