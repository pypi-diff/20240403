# Comparing `tmp/pythagoras-0.10.33.tar.gz` & `tmp/pythagoras-0.10.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythagoras-0.10.33.tar", last modified: Wed Apr  3 03:10:13 2024, max compression
+gzip compressed data, was "pythagoras-0.10.34.tar", last modified: Wed Apr  3 05:54:11 2024, max compression
```

## Comparing `pythagoras-0.10.33.tar` & `pythagoras-0.10.34.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.425131 pythagoras-0.10.33/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1114 2023-12-24 04:46:00.000000 pythagoras-0.10.33/LICENSE
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-03 03:10:13.424397 pythagoras-0.10.33/PKG-INFO
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2195 2024-03-24 05:25:36.000000 pythagoras-0.10.33/README.md
--rw-r--r--   0 Pythagoras   (504) staff       (20)       80 2023-12-24 04:46:00.000000 pythagoras-0.10.33/pyproject.toml
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.390045 pythagoras-0.10.33/pythagoras/
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.394261 pythagoras-0.10.33/pythagoras/_01_foundational_objects/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      792 2024-03-23 20:14:41.000000 pythagoras-0.10.33/pythagoras/_01_foundational_objects/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1239 2024-02-22 05:34:39.000000 pythagoras-0.10.33/pythagoras/_01_foundational_objects/base_16_32_convertors.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3341 2024-03-17 06:20:02.000000 pythagoras-0.10.33/pythagoras/_01_foundational_objects/hash_addresses.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1510 2024-03-10 05:40:41.000000 pythagoras-0.10.33/pythagoras/_01_foundational_objects/hash_and_random_signatures.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      720 2024-03-10 19:35:01.000000 pythagoras-0.10.33/pythagoras/_01_foundational_objects/multipersidict.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2611 2024-03-17 06:40:19.000000 pythagoras-0.10.33/pythagoras/_01_foundational_objects/value_addresses.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.398446 pythagoras-0.10.33/pythagoras/_02_ordinary_functions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      908 2024-03-17 06:16:19.000000 pythagoras-0.10.33/pythagoras/_02_ordinary_functions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1894 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_02_ordinary_functions/assert_ordinarity.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      815 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_02_ordinary_functions/check_n_positional_args.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      723 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_02_ordinary_functions/code_normalizer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     4595 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      400 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_02_ordinary_functions/function_name.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      288 2024-03-16 20:40:58.000000 pythagoras-0.10.33/pythagoras/_02_ordinary_functions/ordinary_decorator.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1469 2024-03-17 05:40:33.000000 pythagoras-0.10.33/pythagoras/_02_ordinary_functions/ordinary_funcs.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.403190 pythagoras-0.10.33/pythagoras/_03_autonomous_functions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2518 2024-03-23 20:14:41.000000 pythagoras-0.10.33/pythagoras/_03_autonomous_functions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      978 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_03_autonomous_functions/autonomicity_checks.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     4986 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_03_autonomous_functions/autonomous_decorators.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     9725 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_03_autonomous_functions/autonomous_funcs.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3575 2024-03-17 06:16:19.000000 pythagoras-0.10.33/pythagoras/_03_autonomous_functions/call_graph_explorer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     8286 2024-03-17 06:16:19.000000 pythagoras-0.10.33/pythagoras/_03_autonomous_functions/names_usage_analyzer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      404 2024-03-16 05:00:28.000000 pythagoras-0.10.33/pythagoras/_03_autonomous_functions/pth_available_names_retriever.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.409990 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2385 2024-03-23 20:14:41.000000 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      936 2024-02-27 05:38:18.000000 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      200 2024-03-16 20:57:07.000000 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/idempotency_checks.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      824 2024-03-16 20:57:07.000000 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/idempotent_decorator.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)    23549 2024-03-24 03:13:32.000000 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2266 2024-03-17 06:20:02.000000 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/kw_args.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     4280 2024-03-19 06:32:05.000000 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/output_capturer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      569 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/persidict_to_timeline.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1398 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_04_idempotent_functions/process_augmented_func_src.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.415213 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      192 2024-03-09 06:54:01.000000 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      411 2024-03-01 23:23:38.000000 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/current_date_gmt_str.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2691 2024-03-16 20:59:15.000000 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/event_posters.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1748 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/execution_environment_summary.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1800 2024-03-17 06:16:39.000000 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/find_in_callstack.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1051 2024-03-16 05:20:24.000000 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/global_event_loggers.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      540 2024-03-02 05:43:58.000000 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/notebook_checker.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1066 2024-03-17 06:18:06.000000 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/type_retrievers.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2132 2024-03-08 04:41:55.000000 pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.417647 pythagoras-0.10.33/pythagoras/_06_swarming/
--rw-r--r--   0 Pythagoras   (504) staff       (20)       87 2024-03-13 04:53:14.000000 pythagoras-0.10.33/pythagoras/_06_swarming/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2664 2024-03-17 06:12:34.000000 pythagoras-0.10.33/pythagoras/_06_swarming/background_workers.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      626 2024-03-10 22:12:16.000000 pythagoras-0.10.33/pythagoras/_06_swarming/output_suppressor.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.420265 pythagoras-0.10.33/pythagoras/_07_mission_control/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      352 2024-03-10 21:01:51.000000 pythagoras-0.10.33/pythagoras/_07_mission_control/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     9436 2024-03-18 02:05:58.000000 pythagoras-0.10.33/pythagoras/_07_mission_control/global_state_management.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1595 2024-04-02 20:44:54.000000 pythagoras-0.10.33/pythagoras/_07_mission_control/summary.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.423459 pythagoras-0.10.33/pythagoras/_99_misc_utils/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      175 2024-03-10 05:49:40.000000 pythagoras-0.10.33/pythagoras/_99_misc_utils/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      451 2024-03-16 04:14:22.000000 pythagoras-0.10.33/pythagoras/_99_misc_utils/id_examiner.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      650 2024-02-22 18:42:45.000000 pythagoras-0.10.33/pythagoras/_99_misc_utils/long_infoname.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1116 2024-02-27 01:25:58.000000 pythagoras-0.10.33/pythagoras/_99_misc_utils/package_manager.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1648 2024-03-23 20:14:41.000000 pythagoras-0.10.33/pythagoras/__init__.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 03:10:13.391452 pythagoras-0.10.33/pythagoras.egg-info/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-03 03:10:13.000000 pythagoras-0.10.33/pythagoras.egg-info/PKG-INFO
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2929 2024-04-03 03:10:13.000000 pythagoras-0.10.33/pythagoras.egg-info/SOURCES.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)        1 2024-04-03 03:10:13.000000 pythagoras-0.10.33/pythagoras.egg-info/dependency_links.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)      121 2024-04-03 03:10:13.000000 pythagoras-0.10.33/pythagoras.egg-info/requires.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)       11 2024-04-03 03:10:13.000000 pythagoras-0.10.33/pythagoras.egg-info/top_level.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)       38 2024-04-03 03:10:13.425319 pythagoras-0.10.33/setup.cfg
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1964 2024-04-03 03:08:11.000000 pythagoras-0.10.33/setup.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.880807 pythagoras-0.10.34/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1114 2023-12-24 04:46:00.000000 pythagoras-0.10.34/LICENSE
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-03 05:54:11.880242 pythagoras-0.10.34/PKG-INFO
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2195 2024-03-24 05:25:36.000000 pythagoras-0.10.34/README.md
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       80 2023-12-24 04:46:00.000000 pythagoras-0.10.34/pyproject.toml
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.843810 pythagoras-0.10.34/pythagoras/
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.848518 pythagoras-0.10.34/pythagoras/_01_foundational_objects/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      792 2024-03-23 20:14:41.000000 pythagoras-0.10.34/pythagoras/_01_foundational_objects/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1239 2024-02-22 05:34:39.000000 pythagoras-0.10.34/pythagoras/_01_foundational_objects/base_16_32_convertors.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3341 2024-03-17 06:20:02.000000 pythagoras-0.10.34/pythagoras/_01_foundational_objects/hash_addresses.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1510 2024-03-10 05:40:41.000000 pythagoras-0.10.34/pythagoras/_01_foundational_objects/hash_and_random_signatures.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      720 2024-03-10 19:35:01.000000 pythagoras-0.10.34/pythagoras/_01_foundational_objects/multipersidict.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2611 2024-03-17 06:40:19.000000 pythagoras-0.10.34/pythagoras/_01_foundational_objects/value_addresses.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.853222 pythagoras-0.10.34/pythagoras/_02_ordinary_functions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      908 2024-03-17 06:16:19.000000 pythagoras-0.10.34/pythagoras/_02_ordinary_functions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1894 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_02_ordinary_functions/assert_ordinarity.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      815 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_02_ordinary_functions/check_n_positional_args.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      723 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_02_ordinary_functions/code_normalizer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     4595 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      400 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_02_ordinary_functions/function_name.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      288 2024-03-16 20:40:58.000000 pythagoras-0.10.34/pythagoras/_02_ordinary_functions/ordinary_decorator.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1469 2024-03-17 05:40:33.000000 pythagoras-0.10.34/pythagoras/_02_ordinary_functions/ordinary_funcs.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.859353 pythagoras-0.10.34/pythagoras/_03_autonomous_functions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2518 2024-03-23 20:14:41.000000 pythagoras-0.10.34/pythagoras/_03_autonomous_functions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      978 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_03_autonomous_functions/autonomicity_checks.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     4986 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_03_autonomous_functions/autonomous_decorators.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     9725 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_03_autonomous_functions/autonomous_funcs.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3575 2024-03-17 06:16:19.000000 pythagoras-0.10.34/pythagoras/_03_autonomous_functions/call_graph_explorer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     8286 2024-03-17 06:16:19.000000 pythagoras-0.10.34/pythagoras/_03_autonomous_functions/names_usage_analyzer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      404 2024-03-16 05:00:28.000000 pythagoras-0.10.34/pythagoras/_03_autonomous_functions/pth_available_names_retriever.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.866240 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2385 2024-03-23 20:14:41.000000 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      936 2024-02-27 05:38:18.000000 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      200 2024-03-16 20:57:07.000000 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/idempotency_checks.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      824 2024-03-16 20:57:07.000000 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/idempotent_decorator.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)    23549 2024-03-24 03:13:32.000000 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2266 2024-03-17 06:20:02.000000 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/kw_args.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     4280 2024-03-19 06:32:05.000000 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/output_capturer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      569 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/persidict_to_timeline.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1398 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_04_idempotent_functions/process_augmented_func_src.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.871912 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      192 2024-03-09 06:54:01.000000 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      411 2024-03-01 23:23:38.000000 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/current_date_gmt_str.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2691 2024-03-16 20:59:15.000000 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/event_posters.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1748 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/execution_environment_summary.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1800 2024-03-17 06:16:39.000000 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/find_in_callstack.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1051 2024-03-16 05:20:24.000000 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/global_event_loggers.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      540 2024-03-02 05:43:58.000000 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/notebook_checker.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1066 2024-03-17 06:18:06.000000 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/type_retrievers.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2132 2024-03-08 04:41:55.000000 pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.874117 pythagoras-0.10.34/pythagoras/_06_swarming/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       87 2024-03-13 04:53:14.000000 pythagoras-0.10.34/pythagoras/_06_swarming/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2664 2024-03-17 06:12:34.000000 pythagoras-0.10.34/pythagoras/_06_swarming/background_workers.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      626 2024-03-10 22:12:16.000000 pythagoras-0.10.34/pythagoras/_06_swarming/output_suppressor.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.876578 pythagoras-0.10.34/pythagoras/_07_mission_control/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      352 2024-03-10 21:01:51.000000 pythagoras-0.10.34/pythagoras/_07_mission_control/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     9436 2024-03-18 02:05:58.000000 pythagoras-0.10.34/pythagoras/_07_mission_control/global_state_management.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2195 2024-04-03 05:51:17.000000 pythagoras-0.10.34/pythagoras/_07_mission_control/summary.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.879175 pythagoras-0.10.34/pythagoras/_99_misc_utils/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      175 2024-03-10 05:49:40.000000 pythagoras-0.10.34/pythagoras/_99_misc_utils/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      451 2024-03-16 04:14:22.000000 pythagoras-0.10.34/pythagoras/_99_misc_utils/id_examiner.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      650 2024-02-22 18:42:45.000000 pythagoras-0.10.34/pythagoras/_99_misc_utils/long_infoname.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1116 2024-02-27 01:25:58.000000 pythagoras-0.10.34/pythagoras/_99_misc_utils/package_manager.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1648 2024-03-23 20:14:41.000000 pythagoras-0.10.34/pythagoras/__init__.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 05:54:11.845325 pythagoras-0.10.34/pythagoras.egg-info/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-03 05:54:11.000000 pythagoras-0.10.34/pythagoras.egg-info/PKG-INFO
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2929 2024-04-03 05:54:11.000000 pythagoras-0.10.34/pythagoras.egg-info/SOURCES.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)        1 2024-04-03 05:54:11.000000 pythagoras-0.10.34/pythagoras.egg-info/dependency_links.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      121 2024-04-03 05:54:11.000000 pythagoras-0.10.34/pythagoras.egg-info/requires.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       11 2024-04-03 05:54:11.000000 pythagoras-0.10.34/pythagoras.egg-info/top_level.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       38 2024-04-03 05:54:11.880962 pythagoras-0.10.34/setup.cfg
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1964 2024-04-03 05:53:34.000000 pythagoras-0.10.34/setup.py
```

### Comparing `pythagoras-0.10.33/LICENSE` & `pythagoras-0.10.34/LICENSE`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/PKG-INFO` & `pythagoras-0.10.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythagoras
-Version: 0.10.33
+Version: 0.10.34
 Summary: Simple framework for planet-scale idempotent computations in Python.
 Home-page: https://github.com/vladlpavlov/pythagoras
 Author: Volodymyr (Vlad) Pavlov
 Author-email: vlpavlov@ieee.org
 Keywords: cloud,ML,AI,serverless,distributed,parallel,machine-learning,deep-learning,pythagoras
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pythagoras-0.10.33/README.md` & `pythagoras-0.10.34/README.md`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_01_foundational_objects/__init__.py` & `pythagoras-0.10.34/pythagoras/_01_foundational_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_01_foundational_objects/base_16_32_convertors.py` & `pythagoras-0.10.34/pythagoras/_01_foundational_objects/base_16_32_convertors.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_01_foundational_objects/hash_addresses.py` & `pythagoras-0.10.34/pythagoras/_01_foundational_objects/hash_addresses.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_01_foundational_objects/hash_and_random_signatures.py` & `pythagoras-0.10.34/pythagoras/_01_foundational_objects/hash_and_random_signatures.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_01_foundational_objects/multipersidict.py` & `pythagoras-0.10.34/pythagoras/_01_foundational_objects/multipersidict.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_01_foundational_objects/value_addresses.py` & `pythagoras-0.10.34/pythagoras/_01_foundational_objects/value_addresses.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_02_ordinary_functions/__init__.py` & `pythagoras-0.10.34/pythagoras/_02_ordinary_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_02_ordinary_functions/assert_ordinarity.py` & `pythagoras-0.10.34/pythagoras/_02_ordinary_functions/assert_ordinarity.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_02_ordinary_functions/check_n_positional_args.py` & `pythagoras-0.10.34/pythagoras/_02_ordinary_functions/check_n_positional_args.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_02_ordinary_functions/code_normalizer.py` & `pythagoras-0.10.34/pythagoras/_02_ordinary_functions/code_normalizer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py` & `pythagoras-0.10.34/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_02_ordinary_functions/ordinary_funcs.py` & `pythagoras-0.10.34/pythagoras/_02_ordinary_functions/ordinary_funcs.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_03_autonomous_functions/__init__.py` & `pythagoras-0.10.34/pythagoras/_03_autonomous_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_03_autonomous_functions/autonomicity_checks.py` & `pythagoras-0.10.34/pythagoras/_03_autonomous_functions/autonomicity_checks.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_03_autonomous_functions/autonomous_decorators.py` & `pythagoras-0.10.34/pythagoras/_03_autonomous_functions/autonomous_decorators.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_03_autonomous_functions/autonomous_funcs.py` & `pythagoras-0.10.34/pythagoras/_03_autonomous_functions/autonomous_funcs.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_03_autonomous_functions/call_graph_explorer.py` & `pythagoras-0.10.34/pythagoras/_03_autonomous_functions/call_graph_explorer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_03_autonomous_functions/names_usage_analyzer.py` & `pythagoras-0.10.34/pythagoras/_03_autonomous_functions/names_usage_analyzer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_04_idempotent_functions/__init__.py` & `pythagoras-0.10.34/pythagoras/_04_idempotent_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py` & `pythagoras-0.10.34/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_04_idempotent_functions/idempotent_decorator.py` & `pythagoras-0.10.34/pythagoras/_04_idempotent_functions/idempotent_decorator.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py` & `pythagoras-0.10.34/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_04_idempotent_functions/kw_args.py` & `pythagoras-0.10.34/pythagoras/_04_idempotent_functions/kw_args.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_04_idempotent_functions/output_capturer.py` & `pythagoras-0.10.34/pythagoras/_04_idempotent_functions/output_capturer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_04_idempotent_functions/persidict_to_timeline.py` & `pythagoras-0.10.34/pythagoras/_04_idempotent_functions/persidict_to_timeline.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_04_idempotent_functions/process_augmented_func_src.py` & `pythagoras-0.10.34/pythagoras/_04_idempotent_functions/process_augmented_func_src.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/event_posters.py` & `pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/event_posters.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/execution_environment_summary.py` & `pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/execution_environment_summary.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/find_in_callstack.py` & `pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/find_in_callstack.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/global_event_loggers.py` & `pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/global_event_loggers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/notebook_checker.py` & `pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/notebook_checker.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/type_retrievers.py` & `pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/type_retrievers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py` & `pythagoras-0.10.34/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_06_swarming/background_workers.py` & `pythagoras-0.10.34/pythagoras/_06_swarming/background_workers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_06_swarming/output_suppressor.py` & `pythagoras-0.10.34/pythagoras/_06_swarming/output_suppressor.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_07_mission_control/global_state_management.py` & `pythagoras-0.10.34/pythagoras/_07_mission_control/global_state_management.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_99_misc_utils/long_infoname.py` & `pythagoras-0.10.34/pythagoras/_99_misc_utils/long_infoname.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/_99_misc_utils/package_manager.py` & `pythagoras-0.10.34/pythagoras/_99_misc_utils/package_manager.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras/__init__.py` & `pythagoras-0.10.34/pythagoras/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/pythagoras.egg-info/PKG-INFO` & `pythagoras-0.10.34/pythagoras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythagoras
-Version: 0.10.33
+Version: 0.10.34
 Summary: Simple framework for planet-scale idempotent computations in Python.
 Home-page: https://github.com/vladlpavlov/pythagoras
 Author: Volodymyr (Vlad) Pavlov
 Author-email: vlpavlov@ieee.org
 Keywords: cloud,ML,AI,serverless,distributed,parallel,machine-learning,deep-learning,pythagoras
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pythagoras-0.10.33/pythagoras.egg-info/SOURCES.txt` & `pythagoras-0.10.34/pythagoras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.33/setup.py` & `pythagoras-0.10.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pythagoras"
-    ,version="0.10.33"
+    ,version="0.10.34"
     ,author="Volodymyr (Vlad) Pavlov"
     ,author_email="vlpavlov@ieee.org"
     ,description= "Simple framework for planet-scale "
                   + "idempotent computations in Python."
     ,long_description=long_description
     ,long_description_content_type="text/markdown"
     ,url="https://github.com/vladlpavlov/pythagoras"
```

