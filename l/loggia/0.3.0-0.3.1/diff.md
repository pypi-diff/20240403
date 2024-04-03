# Comparing `tmp/loggia-0.3.0.tar.gz` & `tmp/loggia-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggia-0.3.0.tar", last modified: Mon Jan 22 16:05:17 2024, max compression
+gzip compressed data, was "loggia-0.3.1.tar", last modified: Wed Apr  3 10:52:32 2024, max compression
```

## Comparing `loggia-0.3.0.tar` & `loggia-0.3.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0      742 2024-01-22 16:05:04.020053 loggia-0.3.0/LICENSE
--rw-r--r--   0        0        0     3737 2024-01-22 16:05:04.020053 loggia-0.3.0/README.md
--rw-r--r--   0        0        0       69 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/__init__.py
--rw-r--r--   0        0        0        0 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/_internal/__init__.py
--rw-r--r--   0        0        0     2240 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/_internal/bootstrap_logger.py
--rw-r--r--   0        0        0     2657 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/_internal/conf.py
--rw-r--r--   0        0        0      531 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/_internal/env_parsers.py
--rw-r--r--   0        0        0     3917 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/_internal/loguru_stuff.py
--rw-r--r--   0        0        0     7729 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/_internal/presets.py
--rw-r--r--   0        0        0       27 2024-01-22 16:05:17.436118 loggia-0.3.0/loggia/_version.py
--rw-r--r--   0        0        0       49 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/auto.py
--rw-r--r--   0        0        0     2410 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/base_preset.py
--rw-r--r--   0        0        0    11976 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/conf.py
--rw-r--r--   0        0        0     3412 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/constants.py
--rw-r--r--   0        0        0        0 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/filters/__init__.py
--rw-r--r--   0        0        0      642 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/filters/extra_allow.py
--rw-r--r--   0        0        0     3781 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/logger.py
--rw-r--r--   0        0        0     1281 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/loguru_sink.py
--rw-r--r--   0        0        0        0 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/presets/__init__.py
--rw-r--r--   0        0        0     3478 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/presets/datadog_normalisation.py
--rw-r--r--   0        0        0     1339 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/presets/dev.py
--rw-r--r--   0        0        0      232 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/presets/gunicorn.py
--rw-r--r--   0        0        0      234 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/presets/hypercorn.py
--rw-r--r--   0        0        0      334 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/presets/null_preset.py
--rw-r--r--   0        0        0     1415 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/presets/prod.py
--rw-r--r--   0        0        0        0 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/py.typed
--rw-r--r--   0        0        0       43 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/stdlib_formatters/__init__.py
--rw-r--r--   0        0        0     6736 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/stdlib_formatters/json_formatter.py
--rw-r--r--   0        0        0     2752 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/stdlib_formatters/pretty_formatter.py
--rw-r--r--   0        0        0        0 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/structlog_utils/__init__.py
--rw-r--r--   0        0        0     2454 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/structlog_utils/gunicorn_logger.py
--rw-r--r--   0        0        0     2611 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/structlog_utils/hypercorn_logger.py
--rw-r--r--   0        0        0      529 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/types.py
--rw-r--r--   0        0        0       57 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/utils/__init__.py
--rw-r--r--   0        0        0      862 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/utils/colorsutils.py
--rw-r--r--   0        0        0     2656 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/utils/dictutils.py
--rw-r--r--   0        0        0      242 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/utils/envutils.py
--rw-r--r--   0        0        0     4253 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/utils/loaderutils.py
--rw-r--r--   0        0        0     1238 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/utils/logrecordutils.py
--rw-r--r--   0        0        0      215 2024-01-22 16:05:04.020053 loggia-0.3.0/loggia/utils/strutils.py
--rw-r--r--   0        0        0     6278 2024-01-22 16:05:17.444119 loggia-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     5620 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1014 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_basics/test_propagate.py
--rw-r--r--   0        0        0        0 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_filters/__init__.py
--rw-r--r--   0        0        0     1114 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_filters/test_extra_allow.py
--rw-r--r--   0        0        0      704 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_hooks/excepthook_test_1.py
--rw-r--r--   0        0        0      676 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_hooks/excepthook_test_2.py
--rw-r--r--   0        0        0     1884 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_hooks/test_hooks.py
--rw-r--r--   0        0        0      815 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_hooks/threadinghook_test_1.py
--rw-r--r--   0        0        0     1054 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_hooks/threadinghook_test_2.py
--rw-r--r--   0        0        0      824 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_hooks/unraisablehook_test_1.py
--rw-r--r--   0        0        0     1081 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_hooks/unraisablehook_test_2.py
--rw-r--r--   0        0        0     1881 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_logging_utils/test_logger.py
--rw-r--r--   0        0        0     1091 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_logging_utils/test_logging_dictconfig.py
--rw-r--r--   0        0        0     3350 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_logging_utils/test_loguru.py
--rw-r--r--   0        0        0        0 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_logging_utils/test_loguru_sink.py
--rw-r--r--   0        0        0      647 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_logging_utils/test_structlog_pretty_console_renderer.py
--rw-r--r--   0        0        0     9878 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_logging_utils/test_structlog_processors.py.disabled
--rw-r--r--   0        0        0      330 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_preset.py
--rw-r--r--   0        0        0     1224 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_presets/test_basic_slots.py
--rw-r--r--   0        0        0     2133 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_presets/test_dynamic_import.py
--rw-r--r--   0        0        0     4459 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_presets/test_requirements.py
--rw-r--r--   0        0        0      952 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_usage_docs/test_usage.py
--rw-r--r--   0        0        0     1415 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_usage_docs/test_usage_api_trace.py
--rw-r--r--   0        0        0      637 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_usage_docs/test_usage_basic.py
--rw-r--r--   0        0        0      994 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_usage_docs/test_usage_custom_config.py
--rw-r--r--   0        0        0      633 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_usage_docs/test_usage_preset_env.py
--rw-r--r--   0        0        0      737 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_usage_docs/test_usage_std_trace.py
--rw-r--r--   0        0        0      866 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_usage_docs/test_usage_with_loguru.py
--rw-r--r--   0        0        0     1885 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_util/test_dictutils.py
--rw-r--r--   0        0        0      937 2024-01-22 16:05:04.024053 loggia-0.3.0/tests/test_util/test_jsonencoder.py
--rw-r--r--   0        0        0     6091 1970-01-01 00:00:00.000000 loggia-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      742 2024-04-03 10:52:18.779058 loggia-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3752 2024-04-03 10:52:18.779058 loggia-0.3.1/README.md
+-rw-r--r--   0        0        0       69 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/_internal/__init__.py
+-rw-r--r--   0        0        0     2240 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/_internal/bootstrap_logger.py
+-rw-r--r--   0        0        0     2657 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/_internal/conf.py
+-rw-r--r--   0        0        0      531 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/_internal/env_parsers.py
+-rw-r--r--   0        0        0     3917 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/_internal/loguru_stuff.py
+-rw-r--r--   0        0        0     7729 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/_internal/presets.py
+-rw-r--r--   0        0        0       27 2024-04-03 10:52:32.158966 loggia-0.3.1/loggia/_version.py
+-rw-r--r--   0        0        0       49 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/auto.py
+-rw-r--r--   0        0        0     2410 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/base_preset.py
+-rw-r--r--   0        0        0    11875 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/conf.py
+-rw-r--r--   0        0        0     3412 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/constants.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/filters/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/filters/extra_allow.py
+-rw-r--r--   0        0        0     3757 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/logger.py
+-rw-r--r--   0        0        0     1281 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/loguru_sink.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/presets/__init__.py
+-rw-r--r--   0        0        0     3898 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/presets/datadog_normalisation.py
+-rw-r--r--   0        0        0     1339 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/presets/dev.py
+-rw-r--r--   0        0        0      232 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/presets/gunicorn.py
+-rw-r--r--   0        0        0      234 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/presets/hypercorn.py
+-rw-r--r--   0        0        0      334 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/presets/null_preset.py
+-rw-r--r--   0        0        0     1415 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/presets/prod.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/py.typed
+-rw-r--r--   0        0        0       43 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/stdlib_formatters/__init__.py
+-rw-r--r--   0        0        0     6813 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/stdlib_formatters/json_formatter.py
+-rw-r--r--   0        0        0     2752 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/stdlib_formatters/pretty_formatter.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:52:18.779058 loggia-0.3.1/loggia/structlog_utils/__init__.py
+-rw-r--r--   0        0        0     2454 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/structlog_utils/gunicorn_logger.py
+-rw-r--r--   0        0        0     2611 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/structlog_utils/hypercorn_logger.py
+-rw-r--r--   0        0        0      529 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/types.py
+-rw-r--r--   0        0        0       57 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/utils/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/utils/colorsutils.py
+-rw-r--r--   0        0        0     2656 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/utils/dictutils.py
+-rw-r--r--   0        0        0      242 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/utils/envutils.py
+-rw-r--r--   0        0        0     4253 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/utils/loaderutils.py
+-rw-r--r--   0        0        0     1238 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/utils/logrecordutils.py
+-rw-r--r--   0        0        0      406 2024-04-03 10:52:18.783058 loggia-0.3.1/loggia/utils/strutils.py
+-rw-r--r--   0        0        0     6281 2024-04-03 10:52:32.170966 loggia-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     5806 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1751 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_basics/test_propagate.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_filters/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_filters/test_extra_allow.py
+-rw-r--r--   0        0        0      704 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_hooks/excepthook_test_1.py
+-rw-r--r--   0        0        0      676 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_hooks/excepthook_test_2.py
+-rw-r--r--   0        0        0     1884 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_hooks/test_hooks.py
+-rw-r--r--   0        0        0      815 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_hooks/threadinghook_test_1.py
+-rw-r--r--   0        0        0     1054 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_hooks/threadinghook_test_2.py
+-rw-r--r--   0        0        0      824 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_hooks/unraisablehook_test_1.py
+-rw-r--r--   0        0        0     1081 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_hooks/unraisablehook_test_2.py
+-rw-r--r--   0        0        0     1881 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_logging_utils/test_logger.py
+-rw-r--r--   0        0        0     1091 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_logging_utils/test_logging_dictconfig.py
+-rw-r--r--   0        0        0     3350 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_logging_utils/test_loguru.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_logging_utils/test_loguru_sink.py
+-rw-r--r--   0        0        0      647 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_logging_utils/test_structlog_pretty_console_renderer.py
+-rw-r--r--   0        0        0     9878 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_logging_utils/test_structlog_processors.py.disabled
+-rw-r--r--   0        0        0      330 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_preset.py
+-rw-r--r--   0        0        0     1224 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_presets/test_basic_slots.py
+-rw-r--r--   0        0        0     2133 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_presets/test_dynamic_import.py
+-rw-r--r--   0        0        0     4459 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_presets/test_requirements.py
+-rw-r--r--   0        0        0      952 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_usage_docs/test_usage.py
+-rw-r--r--   0        0        0     1415 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_usage_docs/test_usage_api_trace.py
+-rw-r--r--   0        0        0      637 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_usage_docs/test_usage_basic.py
+-rw-r--r--   0        0        0      994 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_usage_docs/test_usage_custom_config.py
+-rw-r--r--   0        0        0      633 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_usage_docs/test_usage_preset_env.py
+-rw-r--r--   0        0        0      737 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_usage_docs/test_usage_std_trace.py
+-rw-r--r--   0        0        0      866 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_usage_docs/test_usage_with_loguru.py
+-rw-r--r--   0        0        0     1922 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_util/test_dictutils.py
+-rw-r--r--   0        0        0      983 2024-04-03 10:52:18.783058 loggia-0.3.1/tests/test_util/test_jsonencoder.py
+-rw-r--r--   0        0        0     6245 1970-01-01 00:00:00.000000 loggia-0.3.1/PKG-INFO
```

### Comparing `loggia-0.3.0/LICENSE` & `loggia-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/README.md` & `loggia-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Loggia
 
-![PyPI - Version](https://img.shields.io/pypi/v/loggia) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loggia) ![PyPI - License](https://img.shields.io/pypi/l/loggia) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
+[![PyPI - Version](https://img.shields.io/pypi/v/loggia)](https://pypi.org/project/loggia/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loggia)](https://pypi.org/project/loggia/) [![PyPI - License](https://img.shields.io/pypi/l/loggia)](https://github.com/ManoManoTech/loggia/blob/main/LICENSE) [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/astral-sh/ruff)
 
 > **The documentation is available on Github Pages**
 >
 > [Read it online](https://manomanotech.github.io/loggia/)
 
 ## Objective
```

### Comparing `loggia-0.3.0/loggia/_internal/bootstrap_logger.py` & `loggia-0.3.1/loggia/_internal/bootstrap_logger.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/_internal/conf.py` & `loggia-0.3.1/loggia/_internal/conf.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/_internal/env_parsers.py` & `loggia-0.3.1/loggia/_internal/env_parsers.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/_internal/loguru_stuff.py` & `loggia-0.3.1/loggia/_internal/loguru_stuff.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/_internal/presets.py` & `loggia-0.3.1/loggia/_internal/presets.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/base_preset.py` & `loggia-0.3.1/loggia/base_preset.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/conf.py` & `loggia-0.3.1/loggia/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import loggia._internal.env_parsers as ep
 from loggia._internal.conf import EnvironmentLoader, is_falsy_string, is_truthy_string
 from loggia._internal.presets import Presets
 from loggia.constants import BASE_DICTCONFIG
 from loggia.types import SupportsFilter, UserDefinedObject
 from loggia.utils.dictutils import get_in
+from loggia.utils.strutils import clean_log_level
 
 if TYPE_CHECKING:
     from json import JSONEncoder
 
     from loggia.types import UserDefinedFilter
 
 
@@ -85,44 +86,39 @@
     @env.register("LOGGIA_LEVEL")
     def set_general_level(self, level: int | str) -> None:
         """Set the general/root, or default, log level.
 
         Can be either a level name string or a level numder int.
         """
         assert "loggers" in self._dictconfig  # noqa: S101
-        if isinstance(level, str):
-            level = level.upper()
-            if level.isdigit():
-                level = int(level)
+        level = clean_log_level(level)
         self._dictconfig["loggers"][""]["level"] = level
 
     @property
     def log_level(self) -> int:
         root_level = self._dictconfig["loggers"][""]["level"]
+        root_level = clean_log_level(root_level)
+        if isinstance(root_level, int):
+            return root_level
         if isinstance(root_level, str):
-            if root_level.isdigit():
-                return int(root_level)
-            root_level = root_level.upper()
             root_level_nb = logging.getLevelName(root_level)
             if not isinstance(root_level_nb, int):
                 raise RuntimeError(f"Unexpected root level name {root_level}")
             return root_level_nb
-        if isinstance(root_level, int):
-            return root_level
         raise RuntimeError(f"Unexpected root level type str or int, got: {type(root_level)}")
 
     @env.register("LOGGIA_SUB_LEVEL", parser=ep.comma_colon)
     def set_logger_level(self, logger_name: str, level: int | str) -> None:
         """Set a specific log level for a specific logger.
 
         This allows you to fine tune verbosity according to your needs.
         """
         assert "loggers" in self._dictconfig  # noqa: S101
         self._enforce_logger(logger_name)
-        self._dictconfig["loggers"][logger_name]["level"] = level
+        self._dictconfig["loggers"][logger_name]["level"] = clean_log_level(level)
 
     @env.register("LOGGIA_SUB_PROPAGATION", parser=ep.comma_colon)
     def set_logger_propagation(self, logger_name: str, does_propagate: str) -> None:
         """Set a specific logger's propagation."""
         assert "loggers" in self._dictconfig  # noqa: S101
         self._enforce_logger(logger_name)
         self._dictconfig["loggers"][logger_name]["propagate"] = is_truthy_string(does_propagate)
```

### Comparing `loggia-0.3.0/loggia/constants.py` & `loggia-0.3.1/loggia/constants.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/filters/extra_allow.py` & `loggia-0.3.1/loggia/filters/extra_allow.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/logger.py` & `loggia-0.3.1/loggia/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
     Sanity check for existing levels is left as an exercise to the user.
     XXX(dugab): Some of these statements may be redundant.
     """
     # pylint: disable=protected-access
     # ruff: noqa: SLF001
     level_name_upper = level_name.upper()
-    level_name.lower()
     logging.addLevelName(level_number, level_name_upper)
 
 
 def _bootstrap_config(
     conf: LoggerConfiguration | dict[str, str] | None = None,
     presets: str | list[str] | None = None,
 ) -> LoggerConfiguration:
@@ -69,15 +68,14 @@
             _patch_to_add_level(25, "SUCCESS")
             configure_loguru(conf)
         except ModuleNotFoundError as e:
             if conf.capture_loguru == FlexibleFlag.ENABLED:
                 bootstrap_logger.error("Failed to configure loguru! Is is installed?", e)
 
     # XXX Check that logger levels exists
-
     # BIM BAM BADABEEM BADABOOM, LOGGIA MAGICA!
     logging.config.dictConfig(conf._dictconfig)
 
 
 def _set_excepthook(logger: logging.Logger) -> None:
     def _excepthook(exc_type: type[BaseException], exc_value: BaseException, exc_traceback: TracebackType | None) -> None:
         logger.critical("Unhandled exception", exc_info=(exc_type, exc_value, exc_traceback))
```

### Comparing `loggia-0.3.0/loggia/loguru_sink.py` & `loggia-0.3.1/loggia/loguru_sink.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/presets/datadog_normalisation.py` & `loggia-0.3.1/loggia/presets/datadog_normalisation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Remap anything to Datadog standard and common attributes."""
 from __future__ import annotations
 
+import os
 import sys
 import traceback
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Final
 
+from loggia._internal.bootstrap_logger import bootstrap_logger
+from loggia._internal.conf import is_truthy_string
 from loggia.base_preset import BasePreset
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     pass
 
@@ -18,19 +21,22 @@
 
     from typing_extensions import TypeAlias
 
     from loggia.conf import LoggerConfiguration
 
 ExcInfo: TypeAlias = "tuple[type[BaseException], BaseException, None | TracebackType]"
 
-
-try:
-    import ddtrace
-except ImportError:
-    ddtrace = None  # type: ignore[assignment]
+# XXX(GabDug): cleanup ddtrace import
+DD_TRACE_ENABLED: Final[bool | None] = is_truthy_string(os.environ.get("DD_TRACE_ENABLED", False))
+if DD_TRACE_ENABLED:
+    try:
+        import ddtrace
+    except ImportError:
+        bootstrap_logger.error("DD_TRACE_ENABLED environment variable is set but ddtrace package cannot be loaded")
+        ddtrace = None  # type: ignore[assignment]
 
 try:
     from loggia._version import __version__
 except ImportError:
     __version__ = "unknown"
 
 loggia_version_str = f"loggia/{__version__}"
```

### Comparing `loggia-0.3.0/loggia/presets/dev.py` & `loggia-0.3.1/loggia/presets/dev.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/presets/prod.py` & `loggia-0.3.1/loggia/presets/prod.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/stdlib_formatters/json_formatter.py` & `loggia-0.3.1/loggia/stdlib_formatters/json_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 from socket import socket
 from typing import TYPE_CHECKING, Any, Final, Protocol, runtime_checkable
 from uuid import UUID
 
 from pythonjsonlogger.jsonlogger import RESERVED_ATTRS, JsonEncoder, JsonFormatter
 
 from loggia._internal.bootstrap_logger import bootstrap_logger
+from loggia._internal.conf import is_truthy_string
 from loggia.constants import SAFE_HEADER_ATTRIBUTES
 from loggia.utils.dictutils import del_if_possible, del_many_if_possible, mv_attr
 
 if TYPE_CHECKING:
     import logging
 
 GUNICORN_KEY_RE = re.compile("{([^}]+)}")
-DD_TRACE_ENABLED: Final[str | None] = os.environ.get("DD_TRACE_ENABLED")
+DD_TRACE_ENABLED: Final[bool | None] = is_truthy_string(os.environ.get("DD_TRACE_ENABLED", False))
 if DD_TRACE_ENABLED:
     try:
         from ddtrace import tracer
     except ImportError:
         bootstrap_logger.error("DD_TRACE_ENABLED environment variable is set but ddtrace package cannot be loaded")
         tracer = None  # type: ignore[assignment]
```

### Comparing `loggia-0.3.0/loggia/stdlib_formatters/pretty_formatter.py` & `loggia-0.3.1/loggia/stdlib_formatters/pretty_formatter.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/structlog_utils/gunicorn_logger.py` & `loggia-0.3.1/loggia/structlog_utils/gunicorn_logger.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/structlog_utils/hypercorn_logger.py` & `loggia-0.3.1/loggia/structlog_utils/hypercorn_logger.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/types.py` & `loggia-0.3.1/loggia/types.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/utils/colorsutils.py` & `loggia-0.3.1/loggia/utils/colorsutils.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/utils/dictutils.py` & `loggia-0.3.1/loggia/utils/dictutils.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/utils/loaderutils.py` & `loggia-0.3.1/loggia/utils/loaderutils.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/loggia/utils/logrecordutils.py` & `loggia-0.3.1/loggia/utils/logrecordutils.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/pyproject.toml` & `loggia-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -33,21 +33,23 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Logging",
     "Topic :: Utilities",
     "Operating System :: OS Independent",
     "Environment :: Console",
     "Environment :: Web Environment",
 ]
-version = "0.3.0"
+version = "0.3.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
-Homepage = "https://git.manomano.tech/component-python/pkgs/loggia/"
+Repository = "https://github.com/ManoManoTech/loggia"
+Documentation = "https://manomanotech.github.io/loggia/latest/"
+Changelog = "https://manomanotech.github.io/loggia/latest/CHANGELOG/"
 
 [project.optional-dependencies]
 loguru = [
     "loguru>=0.7.0",
 ]
 rich = [
     "rich>=13.3.4",
@@ -86,27 +88,27 @@
     "lint-ruff",
     "lint-pylint",
     "lint-mypy",
 ]
 help = "Run all linters (ruff, pylint, mypy)."
 
 [tool.pdm.scripts.fmt-black]
-cmd = "black ."
-help = "Run black formatter"
+cmd = "ruff format ."
+help = "Run ruff black-like formatter"
 
 [tool.pdm.scripts.fmt-ruff]
 cmd = "ruff . --fix --select I001"
 help = "Run isort-like import sorting with ruff"
 
 [tool.pdm.scripts.fmt]
 composite = [
     "fmt-black",
     "fmt-ruff",
 ]
-help = "Run all formatters (black, isort-like ruff)"
+help = "Run all formatters (black-like ruff, isort-like ruff)"
 
 [tool.pdm.scripts.test]
 cmd = "pytest"
 help = "Run the tests"
 
 [tool.pdm.scripts.test-cov]
 cmd = "pytest --junitxml=pytest-report.xml --cov --cov-report xml:pytest-coverage.xml --cov-fail-under=0 --cov-report html"
@@ -118,15 +120,14 @@
 
 [tool.pdm.scripts.docs-build]
 cmd = "mkdocs build --strict"
 help = "Build the docs"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=22.12.0",
     "mypy>=1.4",
     "pylint>=3.0.3",
     "pytest-cov>=4.0.0",
     "yamllint>=1.28.0",
     "ipdb>=0.13.13",
     "rich>=13.3.4",
     "gunicorn>=20.1.0",
@@ -150,22 +151,14 @@
     "mdx-truly-sane-lists>=1.3",
     "mike>=1.1.2",
 ]
 debug = [
     "check-wheel-contents>=0.4.0",
 ]
 
-[[tool.pdm.source]]
-url = "https://pypi.org/simple"
-verify_ssl = true
-name = "pypi"
-include_packages = [
-    "*",
-]
-
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-ra -q --pdbcls=IPython.terminal.debugger:Pdb"
 testpaths = [
     "tests",
 ]
 pythonpath = [
@@ -173,15 +166,14 @@
 ]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
     "tests/*",
-    "__pypackages__/*",
     ".venv/*",
 ]
 source = [
     "loggia",
 ]
 
 [tool.coverage.report]
@@ -192,20 +184,14 @@
     "raise AssertionError",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
     "class .*\\bProtocol\\):",
     "@(abc\\.)?abstractmethod]",
 ]
 
-[tool.black]
-line-length = 140
-target-version = [
-    "py39",
-]
-
 [tool.pylint.main]
 py-version = "3.9"
 disable = [
     "C",
     "R0903",
     "R1735",
     "W0511",
@@ -215,14 +201,16 @@
 ]
 
 [tool.pylint.format]
 max-line-length = 180
 
 [tool.ruff]
 line-length = 140
+
+[tool.ruff.lint]
 ignore = [
     "E501",
     "ANN101",
     "ANN102",
     "ANN401",
     "ARG002",
     "ARG005",
@@ -239,54 +227,56 @@
     "SIM105",
     "EM101",
     "TRY",
     "FIX003",
     "N817",
     "N813",
     "ICN003",
+    "COM812",
+    "ISC001",
 ]
 select = [
     "ALL",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.flake8-annotations]
+[tool.ruff.lint.flake8-annotations]
 allow-star-arg-any = true
 mypy-init-return = true
 suppress-dummy-args = true
 suppress-none-returning = true
 
-[tool.ruff.flake8-unused-arguments]
+[tool.ruff.lint.flake8-unused-arguments]
 ignore-variadic-names = true
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.flake8-errmsg]
+[tool.ruff.lint.flake8-errmsg]
 max-string-length = 20
 
-[tool.ruff.flake8-import-conventions]
+[tool.ruff.lint.flake8-import-conventions]
 banned-from = [
     "datetime",
     "os",
     "sys",
     "logging",
     "time",
     "re",
 ]
 
-[tool.ruff.flake8-builtins]
+[tool.ruff.lint.flake8-builtins]
 builtins-ignorelist = [
     "filter",
     "format",
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**/*.py" = [
     "S101",
     "D",
     "ANN",
     "B018",
     "TRY",
     "EM",
```

### Comparing `loggia-0.3.0/tests/conftest.py` & `loggia-0.3.1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from importlib import reload
 from typing import TYPE_CHECKING, Any
 
 import pytest
 from _pytest.capture import SysCapture
 
 if TYPE_CHECKING:
-    from collections.abc import Callable
+    from collections.abc import Callable, Generator
 
     from _pytest.capture import CaptureManager
     from _pytest.fixtures import SubRequest
 
     from loggia._internal.bootstrap_logger import BootstrapLogger
 
 os.environ["ENV"] = "test"
@@ -29,15 +29,15 @@
     original_excepthook = sys.excepthook
 
     try:
         import loguru
 
         import loggia._internal.loguru_stuff
     except ImportError:
-        loguru = None
+        loguru = None  # type: ignore[assignment]
 
     import loggia._internal
     import loggia._internal.bootstrap_logger
     import loggia._internal.presets
     import loggia.logger
     import loggia.loguru_sink
 
@@ -79,30 +79,30 @@
     os.environ.clear()
     yield
     os.environ.clear()
     os.environ.update(original_environ)
 
 
 class ErrlinesCaptureFixture(pytest.CaptureFixture[str]):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self._lines: list[str] | None = None
+        self._lines: list[str] = []
 
     @property
-    def lines(self):
+    def lines(self) -> list[str]:
         if self._lines:
             return self._lines
 
         captured = self.readouterr()
         err_lines = captured.err.split("\n")
         err_lines.remove("")  # ignore blank lines
         self._lines = err_lines
         return self._lines
 
-    def strip_ansi_codes(self):
+    def strip_ansi_codes(self) -> None:
         def strip(text: str):
             return re.sub(r"\x1B\[[0-?]*[ -/]*[@-~]", "", text)
 
         self._lines = [strip(line) for line in self._lines]
 
     @property
     def line(self):
@@ -112,28 +112,28 @@
         return any(fn(line) for line in self._lines)
 
     def has_line_containing(self, substring: str):
         return any(substring in line for line in self._lines)
 
 
 @pytest.fixture()
-def caperrlines(request: SubRequest):
+def caperrlines(request: SubRequest) -> Generator[ErrlinesCaptureFixture, None, None]:
     """Convenience helper around capsys that only exposes non empty split stderr lines"""
     # most code lifted from upstreams capsys fixture
     capman: CaptureManager = request.config.pluginmanager.getplugin("capturemanager")
     capture_fixture = ErrlinesCaptureFixture(SysCapture, request, _ispytest=True)
     capman.set_fixture(capture_fixture)
     capture_fixture._start()
     yield capture_fixture
     capture_fixture.close()
     capman.unset_fixture()
 
 
 class JsonStderrCaptureFixture(ErrlinesCaptureFixture):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._records: list[Any] | None = None
 
     @property
     def records(self):
         if self._records:
             return self._records
@@ -162,15 +162,15 @@
 class BootstrapLoggerFixture:
     def __init__(self, logger: BootstrapLogger):
         self.logger = logger
 
     def __len__(self):
         return len(self.logger.buf)
 
-    def assert_one_message(self):
+    def assert_one_message(self) -> None:
         assert len(self) == 1, self.messages
 
     @property
     def first_entry(self):
         return self.logger.buf[0]
 
     @property
@@ -191,10 +191,10 @@
 def _nologgingerror():
     import logging
 
     def fixturedHandler(*args, **kwargs):
         raise RuntimeError("An error log was emitted during testing! That's a fail.")
 
     previous_error_handler = logging.Handler.handleError
-    logging.Handler.handleError = fixturedHandler
+    logging.Handler.handleError = fixturedHandler  # type: ignore[method-assign]
     yield
-    logging.Handler.handleError = previous_error_handler
+    logging.Handler.handleError = previous_error_handler  # type: ignore[method-assign]
```

### Comparing `loggia-0.3.0/tests/test_basics/test_propagate.py` & `loggia-0.3.1/tests/test_filters/test_extra_allow.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 from __future__ import annotations
 
 import logging
 import logging.config
 from typing import TYPE_CHECKING
 
 from loggia.conf import LoggerConfiguration
+from loggia.filters.extra_allow import ExtraAllow
 from loggia.logger import initialize
 
 if TYPE_CHECKING:
     from tests.conftest import JsonStderrCaptureFixture
 
 
-def test_child_high_root_low(capjson: JsonStderrCaptureFixture):
-    conf = LoggerConfiguration()
-    conf.set_general_level = "INFO"
-    conf.set_logger_level("test", "WARN")
-    initialize(conf)
-
+def test_basic_logger_filtering(capjson: JsonStderrCaptureFixture):
+    logging_config = LoggerConfiguration()
+    logging_config.add_log_filter("test", ExtraAllow(allow_list=["toto"]))
+    initialize(logging_config)
     logger = logging.getLogger("test")
-    logger.warning("should go through")
-    logger.info("should not go through")
-
-    assert len(capjson.records) == 1
+    logger.info("test", extra={"toto": "oui", "tata": "non"})
+    assert "toto" in capjson.record
+    assert "tata" not in capjson.record
 
 
-def test_child_low_root_high(capjson: JsonStderrCaptureFixture):
-    conf = LoggerConfiguration()
-    conf.set_general_level = "ERROR"
-    conf.set_logger_level("test", "INFO")
-    initialize(conf)
-
+def test_propagated_logger_filtering(capjson: JsonStderrCaptureFixture):
+    logging_config = LoggerConfiguration()
+    logging_config.add_default_handler_filter(ExtraAllow(allow_list=["toto"]))
+    initialize(logging_config)
     logger = logging.getLogger("test")
-    logger.error("should go through")
-    logger.warning("should go through")
-    logger.info("should go through")
-
-    assert len(capjson.records) == 3
+    logger.info("test", extra={"toto": "oui", "tata": "non"})
+    assert "toto" in capjson.record
+    assert "tata" not in capjson.record
```

### Comparing `loggia-0.3.0/tests/test_hooks/excepthook_test_1.py` & `loggia-0.3.1/tests/test_hooks/excepthook_test_1.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_hooks/excepthook_test_2.py` & `loggia-0.3.1/tests/test_hooks/excepthook_test_2.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_hooks/test_hooks.py` & `loggia-0.3.1/tests/test_hooks/test_hooks.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_hooks/threadinghook_test_1.py` & `loggia-0.3.1/tests/test_hooks/threadinghook_test_1.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_hooks/threadinghook_test_2.py` & `loggia-0.3.1/tests/test_hooks/threadinghook_test_2.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_hooks/unraisablehook_test_1.py` & `loggia-0.3.1/tests/test_hooks/unraisablehook_test_1.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_hooks/unraisablehook_test_2.py` & `loggia-0.3.1/tests/test_hooks/unraisablehook_test_2.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_logging_utils/test_logger.py` & `loggia-0.3.1/tests/test_logging_utils/test_logger.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_logging_utils/test_logging_dictconfig.py` & `loggia-0.3.1/tests/test_logging_utils/test_logging_dictconfig.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_logging_utils/test_loguru.py` & `loggia-0.3.1/tests/test_logging_utils/test_loguru.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_logging_utils/test_structlog_pretty_console_renderer.py` & `loggia-0.3.1/tests/test_logging_utils/test_structlog_pretty_console_renderer.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_logging_utils/test_structlog_processors.py.disabled` & `loggia-0.3.1/tests/test_logging_utils/test_structlog_processors.py.disabled`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_presets/test_basic_slots.py` & `loggia-0.3.1/tests/test_presets/test_basic_slots.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_presets/test_dynamic_import.py` & `loggia-0.3.1/tests/test_presets/test_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_presets/test_requirements.py` & `loggia-0.3.1/tests/test_presets/test_requirements.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_usage_docs/test_usage.py` & `loggia-0.3.1/tests/test_usage_docs/test_usage.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_usage_docs/test_usage_api_trace.py` & `loggia-0.3.1/tests/test_usage_docs/test_usage_api_trace.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_usage_docs/test_usage_basic.py` & `loggia-0.3.1/tests/test_usage_docs/test_usage_basic.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_usage_docs/test_usage_custom_config.py` & `loggia-0.3.1/tests/test_usage_docs/test_usage_custom_config.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_usage_docs/test_usage_preset_env.py` & `loggia-0.3.1/tests/test_usage_docs/test_usage_preset_env.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_usage_docs/test_usage_std_trace.py` & `loggia-0.3.1/tests/test_usage_docs/test_usage_std_trace.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_usage_docs/test_usage_with_loguru.py` & `loggia-0.3.1/tests/test_usage_docs/test_usage_with_loguru.py`

 * *Files identical despite different names*

### Comparing `loggia-0.3.0/tests/test_util/test_dictutils.py` & `loggia-0.3.1/tests/test_util/test_dictutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,19 @@
     # Test setup
     dict_cfg: logging.config._DictConfigArgs = {
         "disable_existing_loggers": False,
         "version": 1,
         "handlers": {"console": {"class": "logging.StreamHandler", "formatter": "simple"}},
     }
 
-    opt_dict_cfg: logging.config._OptionalDictConfigArgs = {"handlers": {"console": {"level": "INFO"}}, "root": {"handlers": ["console"]}}
+    opt_dict_cfg: logging.config._DictConfigArgs = {
+        "version": 1,
+        "handlers": {"console": {"level": "INFO"}},
+        "root": {"handlers": ["console"]},
+    }
 
     # Expected result
     expected: logging.config._DictConfigArgs = {
         "disable_existing_loggers": False,
         "version": 1,
         "handlers": {"console": {"class": "logging.StreamHandler", "formatter": "simple", "level": "INFO"}},
         "root": {"handlers": ["console"]},
```

### Comparing `loggia-0.3.0/tests/test_util/test_jsonencoder.py` & `loggia-0.3.1/tests/test_util/test_jsonencoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     output = json.dumps(JsonEncodable(), cls=CustomJsonEncoder)
     assert output == "ok"
 
 
 # We skip this because it's ahead of its time. We could revisit with
 # either homegrown checking, or better support from standard library.
 #
-# python/3.11.3/lib/python3.11/typing.py:2223
-# Warning: this will check only the presence of the required methods,
-# not their type signatures!
+# python/3.11.3/lib/python3.11/typing.py:2223 (runtime_checkable)
+# > Warning: this will check only the presence of the required methods,
+# > not their type signatures!
 @pytest.mark.skip("ahead of its time")
 def test_json_dunder_ko_type():
     class JsonEncodable:
         def __json__(self) -> int:
             return 1
 
     if isinstance(JsonEncodable(), JsonSerializable):
-        raise RuntimeError("Z")
+        raise RuntimeError("This should not be true")
     output = json.dumps(JsonEncodable(), cls=CustomJsonEncoder)
     assert output == "ok"
```

### Comparing `loggia-0.3.0/PKG-INFO` & `loggia-0.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggia
-Version: 0.3.0
+Version: 0.3.1
 Summary: A convenient logging configuration manager for Python's standard logging library and Loguru.
 Author-Email: Gabriel Dugny <gabriel.dugny@manomano.com>, Elie Bleton <elie.bleton@manomano.com>, Jonathan Gallon <jonathan.gallon@manomano.com>
 License: Copyright (c) 2021 - 2024 ManoMano Colibri SAS
         
         Permission to use, copy, modify, and distribute this software for any purpose
         with or without fee is hereby granted, provided that the above copyright notice
         and this permission notice appear in all copies.
@@ -28,29 +28,31 @@
 Classifier: Typing :: Typed
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Utilities
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
-Project-URL: Homepage, https://git.manomano.tech/component-python/pkgs/loggia/
+Project-URL: Repository, https://github.com/ManoManoTech/loggia
+Project-URL: Documentation, https://manomanotech.github.io/loggia/latest/
+Project-URL: Changelog, https://manomanotech.github.io/loggia/latest/CHANGELOG/
 Requires-Python: >=3.9
 Requires-Dist: python-json-logger>=2.0.7
 Requires-Dist: typing-extensions>=4.7.1; python_version < "3.10"
 Requires-Dist: loguru>=0.7.0; extra == "loguru"
 Requires-Dist: rich>=13.3.4; extra == "rich"
 Requires-Dist: ddtrace>=1.18.0; extra == "ddtrace"
 Provides-Extra: loguru
 Provides-Extra: rich
 Provides-Extra: ddtrace
 Description-Content-Type: text/markdown
 
 # Loggia
 
-![PyPI - Version](https://img.shields.io/pypi/v/loggia) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loggia) ![PyPI - License](https://img.shields.io/pypi/l/loggia) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
+[![PyPI - Version](https://img.shields.io/pypi/v/loggia)](https://pypi.org/project/loggia/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loggia)](https://pypi.org/project/loggia/) [![PyPI - License](https://img.shields.io/pypi/l/loggia)](https://github.com/ManoManoTech/loggia/blob/main/LICENSE) [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/astral-sh/ruff)
 
 > **The documentation is available on Github Pages**
 >
 > [Read it online](https://manomanotech.github.io/loggia/)
 
 ## Objective
```

